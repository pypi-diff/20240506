# Comparing `tmp/maya_umbrella-0.4.1.tar.gz` & `tmp/maya_umbrella-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.4.1.tar", max compression
+gzip compressed data, was "maya_umbrella-0.5.0.tar", max compression
```

## Comparing `maya_umbrella-0.4.1.tar` & `maya_umbrella-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1060 2024-05-05 17:37:22.477592 maya_umbrella-0.4.1/LICENSE
--rw-r--r--   0        0        0     5659 2024-05-05 17:37:22.477592 maya_umbrella-0.4.1/README.md
--rw-r--r--   0        0        0      106 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/__version__.py
--rw-r--r--   0        0        0      130 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/constants.py
--rw-r--r--   0        0        0     4112 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/core.py
--rw-r--r--   0        0        0     4125 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      734 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1246 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      546 2024-05-05 17:37:22.501592 maya_umbrella-0.4.1/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      457 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     1338 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/log.py
--rw-r--r--   0        0        0     7033 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      430 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2526 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3053 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     3849 2024-05-05 17:37:22.505591 maya_umbrella-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6710 1970-01-01 00:00:00.000000 maya_umbrella-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-06 17:49:28.275867 maya_umbrella-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6202 2024-05-06 17:49:28.275867 maya_umbrella-0.5.0/README.md
+-rw-r--r--   0        0        0      106 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0      408 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     4223 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/core.py
+-rw-r--r--   0        0        0     5293 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1281 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      556 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      484 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     1338 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/log.py
+-rw-r--r--   0        0        0      951 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/maya_funs.py
+-rw-r--r--   0        0        0     8699 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      450 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2151 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     2869 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     5202 2024-05-06 17:49:28.299867 maya_umbrella-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7253 1970-01-01 00:00:00.000000 maya_umbrella-0.5.0/PKG-INFO
```

### Comparing `maya_umbrella-0.4.1/LICENSE` & `maya_umbrella-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.1/README.md` & `maya_umbrella-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,338 +17,372 @@
 00000100: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
 00000110: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
 00000120: 2f76 2f6d 6179 612d 756d 6272 656c 6c61  /v/maya-umbrella
 00000130: 3f63 6f6c 6f72 3d67 7265 656e 295d 2868  ?color=green)](h
 00000140: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
 00000150: 7072 6f6a 6563 742f 6d61 7961 2d75 6d62  project/maya-umb
 00000160: 7265 6c6c 612f 290a 5b21 5b44 6f77 6e6c  rella/).[![Downl
-00000170: 6f61 6473 2053 7461 7475 735d 2868 7474  oads Status](htt
-00000180: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000190: 2e69 6f2f 7079 7069 2f64 772f 6d61 7961  .io/pypi/dw/maya
-000001a0: 2d75 6d62 7265 6c6c 6129 5d28 6874 7470  -umbrella)](http
-000001b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000001c0: 6a65 6374 2f6d 6179 612d 756d 6272 656c  ject/maya-umbrel
-000001d0: 6c61 2f29 0a5b 215b 446f 776e 6c6f 6164  la/).[![Download
-000001e0: 735d 2868 7474 7073 3a2f 2f70 6570 792e  s](https://pepy.
+00000170: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
+00000180: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
+00000190: 6164 6765 2f6d 6179 612d 756d 6272 656c  adge/maya-umbrel
+000001a0: 6c61 295d 2868 7474 7073 3a2f 2f70 6570  la)](https://pep
+000001b0: 792e 7465 6368 2f70 726f 6a65 6374 2f6d  y.tech/project/m
+000001c0: 6179 612d 756d 6272 656c 6c61 290a 5b21  aya-umbrella).[!
+000001d0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+000001e0: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
 000001f0: 7465 6368 2f62 6164 6765 2f6d 6179 612d  tech/badge/maya-
-00000200: 756d 6272 656c 6c61 295d 2868 7474 7073  umbrella)](https
-00000210: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00000220: 6a65 6374 2f6d 6179 612d 756d 6272 656c  ject/maya-umbrel
-00000230: 6c61 290a 5b21 5b4c 6963 656e 7365 5d28  la).[![License](
-00000240: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000250: 6c64 732e 696f 2f70 7970 692f 6c2f 6d61  lds.io/pypi/l/ma
-00000260: 7961 2d75 6d62 7265 6c6c 6129 5d28 6874  ya-umbrella)](ht
-00000270: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00000280: 726f 6a65 6374 2f6d 6179 612d 756d 6272  roject/maya-umbr
-00000290: 656c 6c61 2f29 0a5b 215b 5079 5049 2046  ella/).[![PyPI F
-000002a0: 6f72 6d61 745d 2868 7474 7073 3a2f 2f69  ormat](https://i
-000002b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000002c0: 7069 2f66 6f72 6d61 742f 6d61 7961 2d75  pi/format/maya-u
-000002d0: 6d62 7265 6c6c 6129 5d28 6874 7470 733a  mbrella)](https:
-000002e0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000002f0: 6374 2f6d 6179 612d 756d 6272 656c 6c61  ct/maya-umbrella
-00000300: 2f29 0a5b 215b 4d61 696e 7465 6e61 6e63  /).[![Maintenanc
-00000310: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000320: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000330: 4d61 696e 7461 696e 6564 2533 462d 7965  Maintained%3F-ye
-00000340: 732d 6772 6565 6e2e 7376 6729 5d28 6874  s-green.svg)](ht
-00000350: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000360: 2f6c 6f6f 6e67 6861 6f2f 6d61 7961 2d75  /loonghao/maya-u
-00000370: 6d62 7265 6c6c 612f 6772 6170 6873 2f63  mbrella/graphs/c
-00000380: 6f6d 6d69 742d 6163 7469 7669 7479 290a  ommit-activity).
-00000390: 5b21 5b6d 6179 612d 3230 3234 5d28 6874  [![maya-2024](ht
-000003a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000003b0: 732e 696f 2f62 6164 6765 2f6d 6179 612d  s.io/badge/maya-
-000003c0: 3230 3234 2d67 7265 656e 295d 2868 7474  2024-green)](htt
-000003d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000003e0: 2e69 6f2f 6261 6467 652f 6d61 7961 2d32  .io/badge/maya-2
-000003f0: 3032 342d 6772 6565 6e29 0a5b 215b 6d61  024-green).[![ma
-00000400: 7961 2d32 3032 335d 2868 7474 7073 3a2f  ya-2023](https:/
-00000410: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000420: 6261 6467 652f 6d61 7961 2d32 3032 332d  badge/maya-2023-
-00000430: 6772 6565 6e29 5d28 6874 7470 733a 2f2f  green)](https://
-00000440: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000450: 6164 6765 2f6d 6179 612d 3230 3233 2d67  adge/maya-2023-g
-00000460: 7265 656e 290a 5b21 5b6d 6179 612d 3230  reen).[![maya-20
-00000470: 3232 5d28 6874 7470 733a 2f2f 696d 672e  22](https://img.
-00000480: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000490: 2f6d 6179 612d 3230 3232 2d67 7265 656e  /maya-2022-green
-000004a0: 295d 2868 7474 7073 3a2f 2f69 6d67 2e73  )](https://img.s
-000004b0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000004c0: 6d61 7961 2d32 3032 322d 6772 6565 6e29  maya-2022-green)
-000004d0: 0a5b 215b 6d61 7961 2d32 3032 315d 2868  .[![maya-2021](h
-000004e0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004f0: 6473 2e69 6f2f 6261 6467 652f 6d61 7961  ds.io/badge/maya
-00000500: 2d32 3032 312d 6772 6565 6e29 5d28 6874  -2021-green)](ht
-00000510: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000520: 732e 696f 2f62 6164 6765 2f6d 6179 612d  s.io/badge/maya-
-00000530: 3230 3231 2d67 7265 656e 290a 5b21 5b6d  2021-green).[![m
-00000540: 6179 612d 3230 3230 5d28 6874 7470 733a  aya-2020](https:
-00000550: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000560: 2f62 6164 6765 2f6d 6179 612d 3230 3230  /badge/maya-2020
-00000570: 2d67 7265 656e 295d 2868 7474 7073 3a2f  -green)](https:/
-00000580: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000590: 6261 6467 652f 6d61 7961 2d32 3032 302d  badge/maya-2020-
-000005a0: 6772 6565 6e29 0a5b 215b 6d61 7961 2d32  green).[![maya-2
-000005b0: 3031 395d 2868 7474 7073 3a2f 2f69 6d67  019](https://img
-000005c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000005d0: 652f 6d61 7961 2d32 3031 392d 6772 6565  e/maya-2019-gree
-000005e0: 6e29 5d28 6874 7470 733a 2f2f 696d 672e  n)](https://img.
-000005f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000600: 2f6d 6179 612d 3230 3139 2d67 7265 656e  /maya-2019-green
-00000610: 290a 5b21 5b6d 6179 612d 3230 3138 5d28  ).[![maya-2018](
-00000620: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000630: 6c64 732e 696f 2f62 6164 6765 2f6d 6179  lds.io/badge/may
-00000640: 612d 3230 3138 2d67 7265 656e 295d 2868  a-2018-green)](h
-00000650: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000660: 6473 2e69 6f2f 6261 6467 652f 6d61 7961  ds.io/badge/maya
-00000670: 2d32 3031 382d 6772 6565 6e29 0a0a 3c21  -2018-green)..<!
-00000680: 2d2d 2041 4c4c 2d43 4f4e 5452 4942 5554  -- ALL-CONTRIBUT
-00000690: 4f52 532d 4241 4447 453a 5354 4152 5420  ORS-BADGE:START 
-000006a0: 2d20 446f 206e 6f74 2072 656d 6f76 6520  - Do not remove 
-000006b0: 6f72 206d 6f64 6966 7920 7468 6973 2073  or modify this s
-000006c0: 6563 7469 6f6e 202d 2d3e 0a5b 215b 416c  ection -->.[![Al
-000006d0: 6c20 436f 6e74 7269 6275 746f 7273 5d28  l Contributors](
-000006e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000006f0: 6c64 732e 696f 2f62 6164 6765 2f61 6c6c  lds.io/badge/all
-00000700: 5f63 6f6e 7472 6962 7574 6f72 732d 342d  _contributors-4-
-00000710: 6f72 616e 6765 2e73 7667 3f73 7479 6c65  orange.svg?style
-00000720: 3d66 6c61 742d 7371 7561 7265 295d 2823  =flat-square)](#
-00000730: 636f 6e74 7269 6275 746f 7273 2d29 0a3c  contributors-).<
-00000740: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
-00000750: 544f 5253 2d42 4144 4745 3a45 4e44 202d  TORS-BADGE:END -
-00000760: 2d3e 0a0a 4368 6563 6b20 616e 6420 6669  ->..Check and fi
-00000770: 7820 6d61 7961 2076 6972 7573 2e0a 0a0a  x maya virus....
-00000780: 2320 e58f 91e5 bc80 e78e afe5 a283 e8ae  # ..............
-00000790: bee7 bdae 0a0a e980 9ae8 bf87 e899 9ae6  ................
-000007a0: 8b9f e78e afe5 a283 e58e bbe8 aebe e7bd  ................
-000007b0: aee5 bc80 e58f 91e7 8eaf e5a2 832c 20e6  ............., .
-000007c0: 8ea8 e88d 9070 7974 686f 6e2d 332e 38e4  .....python-3.8.
-000007d0: bba5 e4b8 8ae7 9a84 e789 88e6 9cac 0a0a  ................
-000007e0: 6060 6073 6865 6c6c 0a70 6970 2069 6e73  ```shell.pip ins
-000007f0: 7461 6c6c 206e 6f78 2070 6f65 7472 790a  tall nox poetry.
-00000800: 6060 600a 0a23 20e5 bc80 e58f 91e8 b083  ```..# .........
-00000810: e8af 950a 0a60 6060 7368 656c 6c0a 6e6f  .....```shell.no
-00000820: 7820 2d73 206d 6179 612d 3230 3230 0a60  x -s maya-2020.`
-00000830: 6060 0a0a 2323 20e5 9ca8 6d61 7961 e4b8  ``..## ...maya..
-00000840: ade6 b58b e8af 950a 0ae9 809a e8bf 8760  ...............`
-00000850: 6e6f 7820 2d73 206d 6179 612d 7878 7860  nox -s maya-xxx`
-00000860: 2c20 e590 afe5 8aa8 6d61 7961 2e0a 6e6f  , ......maya..no
-00000870: 78e4 bc9a e58a a8e6 8081 e6a0 b9e6 8dae  x...............
-00000880: e4bd a0e6 9cac e59c b0e5 ae89 e8a3 85e5  ................
-00000890: be97 6d61 7961 e58e bbe6 b3a8 e586 8c6e  ..maya.........n
-000008a0: 6f78 2073 6573 7369 6f6e 2c20 e6af 94e5  ox session, ....
-000008b0: a682 e4bd a0e6 9cac e59c b0e5 ae89 e8a3  ................
-000008c0: 85e4 ba86 606d 6179 612d 3230 3230 60ef  ....`maya-2020`.
-000008d0: bc8c e982 a3e4 b988 e980 9ae8 bf87 606e  ..............`n
-000008e0: 6f78 202d 7320 6d61 7961 2d32 3031 3860  ox -s maya-2018`
-000008f0: 0a0a e590 afe5 8aa8 6d61 7961 e590 8ee5  ........maya....
-00000900: 9ca8 e884 9ae6 9cac e7bc 96e8 be91 e599  ................
-00000910: a8e4 b8ad e689 a7e8 a18c e4b8 8be9 9da2  ................
-00000920: e5be 97e4 bba3 e7a0 81ef bc8c e5b0 b1e4  ................
-00000930: bc9a e58a a8e6 8081 e79a 84e4 bb8e 603c  ..............`<
-00000940: 7265 706f 3e2f 7465 7374 732f 7669 7275  repo>/tests/viru
-00000950: 732f 60e9 878c e99d a2e5 8ebb 6f70 656e  s/`.........open
-00000960: 206d 61e6 9687 e4bb b6e5 8ebb e8bf 9be8   ma.............
-00000970: a18c e6b5 8be8 af95 2e0a 0a60 6060 7079  ...........```py
-00000980: 7468 6f6e 0a69 6d70 6f72 7420 6d61 6e75  thon.import manu
-00000990: 616c 5f74 6573 745f 696e 5f6d 6179 610a  al_test_in_maya.
-000009a0: 0a6d 616e 7561 6c5f 7465 7374 5f69 6e5f  .manual_test_in_
-000009b0: 6d61 7961 2e73 7461 7274 2829 0a60 6060  maya.start().```
-000009c0: 0a0a 2323 20e5 a29e e58a a0e6 96b0 e79a  ..## ...........
-000009d0: 84e7 96ab e88b 970a 0ae5 9ca8 603c 7265  ............`<re
-000009e0: 706f 3e2f 6d61 7961 5f75 6d62 7265 6c6c  po>/maya_umbrell
-000009f0: 612f 7661 6363 696e 6573 2f60 20e6 96b0  a/vaccines/` ...
-00000a00: e5bb bae4 b880 e4b8 aa70 792c 20e5 9ba0  .........py, ...
-00000a10: e4b8 bae6 9c89 e5be 88e5 a49a e797 85e6  ................
-00000a20: af92 e6b2 a1e6 9c89 e585 b7e4 bd93 e79a  ................
-00000a30: 84e5 908d e5ad 97e4 bba3 e58f b7ef bc8c  ................
-00000a40: e688 91e4 bbac e7bb 9fe4 b880 e4bb a560  ...............`
-00000a50: 7661 6363 696e 653c 6964 3e2e 7079 600a  vaccine<id>.py`.
-00000a60: e7bb a7e6 89bf 6066 726f 6d20 6d61 7961  ......`from maya
-00000a70: 5f75 6d62 7265 6c6c 612e 7661 6363 696e  _umbrella.vaccin
-00000a80: 6520 696d 706f 7274 2041 6273 7472 6163  e import Abstrac
-00000a90: 7456 6163 6369 6e65 60e5 b9b6 e4b8 9463  tVaccine`......c
-00000aa0: 6c61 7373 e590 8de5 ad97 e58f ab60 5661  lass.........`Va
-00000ab0: 6363 696e 6560 e58d b3e5 8faf 2c20 e784  ccine`......, ..
-00000ac0: b6e5 908e e58e bbe5 8699 e585 b7e4 bd93  ................
-00000ad0: e79a 84e6 94b6 e99b 86e7 9785 e6af 92e9  ................
-00000ae0: 80bb e8be 910a 0a23 2320 e4bb a3e7 a081  .......## ......
-00000af0: e6a3 80e6 9fa5 0a0a e688 91e4 bbac e58f  ................
-00000b00: afe4 bba5 e588 a9e7 94a8 e5b0 81e8 a385  ................
-00000b10: e5a5 bde7 9a84 606e 6f78 60e5 91bd e4bb  ......`nox`.....
-00000b20: a4e5 8ebb e689 a7e8 a18c e8bf 9be8 a18c  ................
-00000b30: e4bb a3e7 a081 e6a3 80e6 9fa5 0a0a 6060  ..............``
-00000b40: 6073 6865 6c6c 0a6e 6f78 202d 7320 7275  `shell.nox -s ru
-00000b50: 6666 5f63 6865 636b 0a60 6060 0a0a 2320  ff_check.```..# 
-00000b60: e78e afe5 a283 e58f 98e9 878f 0a0a e688  ................
-00000b70: 91e4 bbac e58f afe4 bba5 e980 9ae8 bf87  ................
-00000b80: e4b8 8be5 8897 e78e afe5 a283 e58f 98e9  ................
-00000b90: 878f e58e bbe4 bfae e694 b96d 6179 615f  ...........maya_
-00000ba0: 756d 6272 656c 6c61 e79a 84e4 b880 e4ba  umbrella........
-00000bb0: 9be8 aebe e7bd aeef bc8c e696 b9e4 bebf  ................
-00000bc0: e69c 8970 6970 656c 696e 65e7 9a84 e585  ...pipeline.....
-00000bd0: ace5 8fb8 e58f afe4 bba5 e69b b4e5 a5bd  ................
-00000be0: e79a 84e9 9b86 e688 900a 0ae4 bfae e694  ................
-00000bf0: b96d 6179 6120 756d 6272 656c 6c61 e79a  .maya umbrella..
-00000c00: 84e6 97a5 e5bf 97e4 bf9d e5ad 98e7 9bae  ................
-00000c10: e5bd 95ef bc8c e9bb 98e8 aea4 e698 af77  ...............w
-00000c20: 696e 646f 7773 2074 656d 70e7 9bae e5bd  indows temp.....
-00000c30: 950a 0a60 6060 7368 656c 6c0a 4d41 5941  ...```shell.MAYA
-00000c40: 5f55 4d42 5245 4c4c 415f 4c4f 475f 524f  _UMBRELLA_LOG_RO
-00000c50: 4f54 0a60 6060 0a0a e4bf aee6 94b9 6d61  OT.```........ma
-00000c60: 7961 2075 6d62 7265 6c6c 61e7 9a84 e697  ya umbrella.....
-00000c70: a5e5 bf97 e696 87e4 bbb6 e590 8de7 a7b0  ................
-00000c80: 2c20 e9bb 98e8 aea4 e698 af60 6d61 7961  , .........`maya
-00000c90: 5f75 6d62 7265 6c6c 6160 0a0a 6060 6073  _umbrella`..```s
-00000ca0: 6865 6c6c 0a4d 4159 415f 554d 4252 454c  hell.MAYA_UMBREL
-00000cb0: 4c41 5f4c 4f47 5f4e 414d 450a 6060 600a  LA_LOG_NAME.```.
-00000cc0: 0ae8 aebe e7bd aee6 97a5 e5bf 97e7 baa7  ................
-00000cd0: e588 abef bc8c e9bb 98e8 aea4 e698 af69  ...............i
-00000ce0: 6e66 6f2c 20e5 8faf e4bb a5e6 98af 6465  nfo, .........de
-00000cf0: 6275 67e5 8faf e4bb a5e7 9c8b e588 b0e6  bug.............
-00000d00: 9bb4 e5a4 9ae7 9a84 e697 a5e5 bf97 e4bf  ................
-00000d10: a1e6 81af 0a0a 6060 6073 6865 6c6c 0a4d  ......```shell.M
-00000d20: 4159 415f 554d 4252 454c 4c41 5f4c 4f47  AYA_UMBRELLA_LOG
-00000d30: 5f4c 4556 454c 0a60 6060 0a0a 2323 2043  _LEVEL.```..## C
-00000d40: 6f6e 7472 6962 7574 6f72 7320 e29c a80a  ontributors ....
-00000d50: 0a54 6861 6e6b 7320 676f 6573 2074 6f20  .Thanks goes to 
-00000d60: 7468 6573 6520 776f 6e64 6572 6675 6c20  these wonderful 
-00000d70: 7065 6f70 6c65 2028 5b65 6d6f 6a69 206b  people ([emoji k
-00000d80: 6579 5d28 6874 7470 733a 2f2f 616c 6c63  ey](https://allc
-00000d90: 6f6e 7472 6962 7574 6f72 732e 6f72 672f  ontributors.org/
-00000da0: 646f 6373 2f65 6e2f 656d 6f6a 692d 6b65  docs/en/emoji-ke
-00000db0: 7929 293a 0a0a 3c21 2d2d 2041 4c4c 2d43  y)):..<!-- ALL-C
-00000dc0: 4f4e 5452 4942 5554 4f52 532d 4c49 5354  ONTRIBUTORS-LIST
-00000dd0: 3a53 5441 5254 202d 2044 6f20 6e6f 7420  :START - Do not 
-00000de0: 7265 6d6f 7665 206f 7220 6d6f 6469 6679  remove or modify
-00000df0: 2074 6869 7320 7365 6374 696f 6e20 2d2d   this section --
-00000e00: 3e0a 3c21 2d2d 2070 7265 7474 6965 722d  >.<!-- prettier-
-00000e10: 6967 6e6f 7265 2d73 7461 7274 202d 2d3e  ignore-start -->
-00000e20: 0a3c 212d 2d20 6d61 726b 646f 776e 6c69  .<!-- markdownli
-00000e30: 6e74 2d64 6973 6162 6c65 202d 2d3e 0a3c  nt-disable -->.<
-00000e40: 7461 626c 653e 0a20 203c 7462 6f64 793e  table>.  <tbody>
-00000e50: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
-00000e60: 3c74 6420 616c 6967 6e3d 2263 656e 7465  <td align="cente
-00000e70: 7222 2076 616c 6967 6e3d 2274 6f70 2220  r" valign="top" 
-00000e80: 7769 6474 683d 2231 342e 3238 2522 3e3c  width="14.28%"><
-00000e90: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000ea0: 6769 7468 7562 2e63 6f6d 2f6c 6f6f 6e67  github.com/loong
-00000eb0: 6861 6f22 3e3c 696d 6720 7372 633d 2268  hao"><img src="h
-00000ec0: 7474 7073 3a2f 2f61 7661 7461 7273 312e  ttps://avatars1.
-00000ed0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000ee0: 742e 636f 6d2f 752f 3133 3131 3137 3435  t.com/u/13111745
-00000ef0: 3f76 3d34 3f73 3d31 3030 2220 7769 6474  ?v=4?s=100" widt
-00000f00: 683d 2231 3030 7078 3b22 2061 6c74 3d22  h="100px;" alt="
-00000f10: 4861 6c22 2f3e 3c62 7220 2f3e 3c73 7562  Hal"/><br /><sub
-00000f20: 3e3c 623e 4861 6c3c 2f62 3e3c 2f73 7562  ><b>Hal</b></sub
-00000f30: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
-00000f40: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000f50: 7562 2e63 6f6d 2f6c 6f6f 6e67 6861 6f2f  ub.com/loonghao/
-00000f60: 6d61 7961 5f75 6d62 7265 6c6c 612f 636f  maya_umbrella/co
-00000f70: 6d6d 6974 733f 6175 7468 6f72 3d6c 6f6f  mmits?author=loo
-00000f80: 6e67 6861 6f22 2074 6974 6c65 3d22 436f  nghao" title="Co
-00000f90: 6465 223e f09f 92bb 3c2f 613e 203c 6120  de">....</a> <a 
-00000fa0: 6872 6566 3d22 2369 6e66 7261 2d6c 6f6f  href="#infra-loo
-00000fb0: 6e67 6861 6f22 2074 6974 6c65 3d22 496e  nghao" title="In
-00000fc0: 6672 6173 7472 7563 7475 7265 2028 486f  frastructure (Ho
-00000fd0: 7374 696e 672c 2042 7569 6c64 2d54 6f6f  sting, Build-Too
-00000fe0: 6c73 2c20 6574 6329 223e f09f 9a87 3c2f  ls, etc)">....</
-00000ff0: 613e 203c 6120 6872 6566 3d22 6874 7470  a> <a href="http
-00001000: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00001010: 6f6f 6e67 6861 6f2f 6d61 7961 5f75 6d62  oonghao/maya_umb
-00001020: 7265 6c6c 612f 636f 6d6d 6974 733f 6175  rella/commits?au
-00001030: 7468 6f72 3d6c 6f6f 6e67 6861 6f22 2074  thor=loonghao" t
-00001040: 6974 6c65 3d22 5465 7374 7322 3ee2 9aa0  itle="Tests">...
-00001050: efb8 8f3c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
-00001060: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
-00001070: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
-00001080: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
-00001090: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
-000010a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 686f  ://github.com/ho
-000010b0: 7477 696e 7465 7230 223e 3c69 6d67 2073  twinter0"><img s
-000010c0: 7263 3d22 6874 7470 733a 2f2f 6176 6174  rc="https://avat
-000010d0: 6172 732e 6769 7468 7562 7573 6572 636f  ars.githubuserco
-000010e0: 6e74 656e 742e 636f 6d2f 752f 3130 3632  ntent.com/u/1062
-000010f0: 3337 3330 353f 763d 343f 733d 3130 3022  37305?v=4?s=100"
-00001100: 2077 6964 7468 3d22 3130 3070 783b 2220   width="100px;" 
-00001110: 616c 743d 2268 6f74 7769 6e74 6572 3022  alt="hotwinter0"
-00001120: 2f3e 3c62 7220 2f3e 3c73 7562 3e3c 623e  /><br /><sub><b>
-00001130: 686f 7477 696e 7465 7230 3c2f 623e 3c2f  hotwinter0</b></
-00001140: 7375 623e 3c2f 613e 3c62 7220 2f3e 3c61  sub></a><br /><a
-00001150: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00001160: 6974 6875 622e 636f 6d2f 6c6f 6f6e 6768  ithub.com/loongh
-00001170: 616f 2f6d 6179 615f 756d 6272 656c 6c61  ao/maya_umbrella
-00001180: 2f63 6f6d 6d69 7473 3f61 7574 686f 723d  /commits?author=
-00001190: 686f 7477 696e 7465 7230 2220 7469 746c  hotwinter0" titl
-000011a0: 653d 2254 6573 7473 223e e29a a0ef b88f  e="Tests">......
-000011b0: 3c2f 613e 203c 6120 6872 6566 3d22 6874  </a> <a href="ht
-000011c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000011d0: 2f6c 6f6f 6e67 6861 6f2f 6d61 7961 5f75  /loonghao/maya_u
-000011e0: 6d62 7265 6c6c 612f 636f 6d6d 6974 733f  mbrella/commits?
-000011f0: 6175 7468 6f72 3d68 6f74 7769 6e74 6572  author=hotwinter
-00001200: 3022 2074 6974 6c65 3d22 436f 6465 223e  0" title="Code">
-00001210: f09f 92bb 3c2f 613e 3c2f 7464 3e0a 2020  ....</a></td>.  
-00001220: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
-00001230: 656e 7465 7222 2076 616c 6967 6e3d 2274  enter" valign="t
-00001240: 6f70 2220 7769 6474 683d 2231 342e 3238  op" width="14.28
-00001250: 2522 3e3c 6120 6872 6566 3d22 6874 7470  %"><a href="http
-00001260: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00001270: 696e 6779 756e 6678 223e 3c69 6d67 2073  ingyunfx"><img s
-00001280: 7263 3d22 6874 7470 733a 2f2f 6176 6174  rc="https://avat
-00001290: 6172 732e 6769 7468 7562 7573 6572 636f  ars.githubuserco
-000012a0: 6e74 656e 742e 636f 6d2f 752f 3733 3636  ntent.com/u/7366
-000012b0: 3636 3239 3f76 3d34 3f73 3d31 3030 2220  6629?v=4?s=100" 
-000012c0: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
-000012d0: 6c74 3d22 6c69 6e67 7975 6e66 7822 2f3e  lt="lingyunfx"/>
-000012e0: 3c62 7220 2f3e 3c73 7562 3e3c 623e 6c69  <br /><sub><b>li
-000012f0: 6e67 7975 6e66 783c 2f62 3e3c 2f73 7562  ngyunfx</b></sub
-00001300: 3e3c 2f61 3e3c 6272 202f 3e3c 6120 6872  ></a><br /><a hr
-00001310: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001320: 7562 2e63 6f6d 2f6c 6f6f 6e67 6861 6f2f  ub.com/loonghao/
-00001330: 6d61 7961 5f75 6d62 7265 6c6c 612f 636f  maya_umbrella/co
-00001340: 6d6d 6974 733f 6175 7468 6f72 3d6c 696e  mmits?author=lin
-00001350: 6779 756e 6678 2220 7469 746c 653d 2254  gyunfx" title="T
-00001360: 6573 7473 223e e29a a0ef b88f 3c2f 613e  ests">......</a>
-00001370: 3c2f 7464 3e0a 2020 2020 2020 3c74 6420  </td>.      <td 
-00001380: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
-00001390: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
-000013a0: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
-000013b0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000013c0: 7562 2e63 6f6d 2f79 6a6a 6a6a 223e 3c69  ub.com/yjjjj"><i
-000013d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000013e0: 6176 6174 6172 732e 6769 7468 7562 7573  avatars.githubus
-000013f0: 6572 636f 6e74 656e 742e 636f 6d2f 752f  ercontent.com/u/
-00001400: 3132 3734 3137 3335 3f76 3d34 3f73 3d31  12741735?v=4?s=1
-00001410: 3030 2220 7769 6474 683d 2231 3030 7078  00" width="100px
-00001420: 3b22 2061 6c74 3d22 796a 6a6a 6a22 2f3e  ;" alt="yjjjj"/>
-00001430: 3c62 7220 2f3e 3c73 7562 3e3c 623e 796a  <br /><sub><b>yj
-00001440: 6a6a 6a3c 2f62 3e3c 2f73 7562 3e3c 2f61  jjj</b></sub></a
-00001450: 3e3c 6272 202f 3e3c 6120 6872 6566 3d22  ><br /><a href="
-00001460: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001470: 6f6d 2f6c 6f6f 6e67 6861 6f2f 6d61 7961  om/loonghao/maya
-00001480: 5f75 6d62 7265 6c6c 612f 636f 6d6d 6974  _umbrella/commit
-00001490: 733f 6175 7468 6f72 3d79 6a6a 6a6a 2220  s?author=yjjjj" 
-000014a0: 7469 746c 653d 2254 6573 7473 223e e29a  title="Tests">..
-000014b0: a0ef b88f 3c2f 613e 203c 6120 6872 6566  ....</a> <a href
-000014c0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-000014d0: 2e63 6f6d 2f6c 6f6f 6e67 6861 6f2f 6d61  .com/loonghao/ma
-000014e0: 7961 5f75 6d62 7265 6c6c 612f 636f 6d6d  ya_umbrella/comm
-000014f0: 6974 733f 6175 7468 6f72 3d79 6a6a 6a6a  its?author=yjjjj
-00001500: 2220 7469 746c 653d 2243 6f64 6522 3ef0  " title="Code">.
-00001510: 9f92 bb3c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
-00001520: 203c 2f74 723e 0a20 203c 2f74 626f 6479   </tr>.  </tbody
-00001530: 3e0a 3c2f 7461 626c 653e 0a0a 3c21 2d2d  >.</table>..<!--
-00001540: 206d 6172 6b64 6f77 6e6c 696e 742d 7265   markdownlint-re
-00001550: 7374 6f72 6520 2d2d 3e0a 3c21 2d2d 2070  store -->.<!-- p
-00001560: 7265 7474 6965 722d 6967 6e6f 7265 2d65  rettier-ignore-e
-00001570: 6e64 202d 2d3e 0a0a 3c21 2d2d 2041 4c4c  nd -->..<!-- ALL
-00001580: 2d43 4f4e 5452 4942 5554 4f52 532d 4c49  -CONTRIBUTORS-LI
-00001590: 5354 3a45 4e44 202d 2d3e 0a0a 5468 6973  ST:END -->..This
-000015a0: 2070 726f 6a65 6374 2066 6f6c 6c6f 7773   project follows
-000015b0: 2074 6865 205b 616c 6c2d 636f 6e74 7269   the [all-contri
-000015c0: 6275 746f 7273 5d28 6874 7470 733a 2f2f  butors](https://
-000015d0: 616c 6c63 6f6e 7472 6962 7574 6f72 732e  allcontributors.
-000015e0: 6f72 6729 2073 7065 6369 6669 6361 7469  org) specificati
-000015f0: 6f6e 2e0a 436f 6e74 7269 6275 7469 6f6e  on..Contribution
-00001600: 7320 6f66 2061 6e79 206b 696e 6420 6172  s of any kind ar
-00001610: 6520 7765 6c63 6f6d 6521 0a              e welcome!.
+00000200: 756d 6272 656c 6c61 2f6d 6f6e 7468 295d  umbrella/month)]
+00000210: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
+00000220: 6368 2f70 726f 6a65 6374 2f6d 6179 612d  ch/project/maya-
+00000230: 756d 6272 656c 6c61 290a 5b21 5b44 6f77  umbrella).[![Dow
+00000240: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00000250: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+00000260: 2f62 6164 6765 2f6d 6179 612d 756d 6272  /badge/maya-umbr
+00000270: 656c 6c61 2f77 6565 6b29 5d28 6874 7470  ella/week)](http
+00000280: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+00000290: 6f6a 6563 742f 6d61 7961 2d75 6d62 7265  oject/maya-umbre
+000002a0: 6c6c 6129 0a5b 215b 4c69 6365 6e73 655d  lla).[![License]
+000002b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000002c0: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f6d  elds.io/pypi/l/m
+000002d0: 6179 612d 756d 6272 656c 6c61 295d 2868  aya-umbrella)](h
+000002e0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000002f0: 7072 6f6a 6563 742f 6d61 7961 2d75 6d62  project/maya-umb
+00000300: 7265 6c6c 612f 290a 5b21 5b50 7950 4920  rella/).[![PyPI 
+00000310: 466f 726d 6174 5d28 6874 7470 733a 2f2f  Format](https://
+00000320: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000330: 7970 692f 666f 726d 6174 2f6d 6179 612d  ypi/format/maya-
+00000340: 756d 6272 656c 6c61 295d 2868 7474 7073  umbrella)](https
+00000350: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000360: 6563 742f 6d61 7961 2d75 6d62 7265 6c6c  ect/maya-umbrell
+00000370: 612f 290a 5b21 5b4d 6169 6e74 656e 616e  a/).[![Maintenan
+00000380: 6365 5d28 6874 7470 733a 2f2f 696d 672e  ce](https://img.
+00000390: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000003a0: 2f4d 6169 6e74 6169 6e65 6425 3346 2d79  /Maintained%3F-y
+000003b0: 6573 2d67 7265 656e 2e73 7667 295d 2868  es-green.svg)](h
+000003c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003d0: 6d2f 6c6f 6f6e 6768 616f 2f6d 6179 612d  m/loonghao/maya-
+000003e0: 756d 6272 656c 6c61 2f67 7261 7068 732f  umbrella/graphs/
+000003f0: 636f 6d6d 6974 2d61 6374 6976 6974 7929  commit-activity)
+00000400: 0a5b 215b 6d61 7961 2d32 3032 345d 2868  .[![maya-2024](h
+00000410: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000420: 6473 2e69 6f2f 6261 6467 652f 6d61 7961  ds.io/badge/maya
+00000430: 2d32 3032 342d 6772 6565 6e29 5d28 6874  -2024-green)](ht
+00000440: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000450: 732e 696f 2f62 6164 6765 2f6d 6179 612d  s.io/badge/maya-
+00000460: 3230 3234 2d67 7265 656e 290a 5b21 5b6d  2024-green).[![m
+00000470: 6179 612d 3230 3233 5d28 6874 7470 733a  aya-2023](https:
+00000480: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000490: 2f62 6164 6765 2f6d 6179 612d 3230 3233  /badge/maya-2023
+000004a0: 2d67 7265 656e 295d 2868 7474 7073 3a2f  -green)](https:/
+000004b0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000004c0: 6261 6467 652f 6d61 7961 2d32 3032 332d  badge/maya-2023-
+000004d0: 6772 6565 6e29 0a5b 215b 6d61 7961 2d32  green).[![maya-2
+000004e0: 3032 325d 2868 7474 7073 3a2f 2f69 6d67  022](https://img
+000004f0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000500: 652f 6d61 7961 2d32 3032 322d 6772 6565  e/maya-2022-gree
+00000510: 6e29 5d28 6874 7470 733a 2f2f 696d 672e  n)](https://img.
+00000520: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000530: 2f6d 6179 612d 3230 3232 2d67 7265 656e  /maya-2022-green
+00000540: 290a 5b21 5b6d 6179 612d 3230 3231 5d28  ).[![maya-2021](
+00000550: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000560: 6c64 732e 696f 2f62 6164 6765 2f6d 6179  lds.io/badge/may
+00000570: 612d 3230 3231 2d67 7265 656e 295d 2868  a-2021-green)](h
+00000580: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000590: 6473 2e69 6f2f 6261 6467 652f 6d61 7961  ds.io/badge/maya
+000005a0: 2d32 3032 312d 6772 6565 6e29 0a5b 215b  -2021-green).[![
+000005b0: 6d61 7961 2d32 3032 305d 2868 7474 7073  maya-2020](https
+000005c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000005d0: 6f2f 6261 6467 652f 6d61 7961 2d32 3032  o/badge/maya-202
+000005e0: 302d 6772 6565 6e29 5d28 6874 7470 733a  0-green)](https:
+000005f0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000600: 2f62 6164 6765 2f6d 6179 612d 3230 3230  /badge/maya-2020
+00000610: 2d67 7265 656e 290a 5b21 5b6d 6179 612d  -green).[![maya-
+00000620: 3230 3139 5d28 6874 7470 733a 2f2f 696d  2019](https://im
+00000630: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000640: 6765 2f6d 6179 612d 3230 3139 2d67 7265  ge/maya-2019-gre
+00000650: 656e 295d 2868 7474 7073 3a2f 2f69 6d67  en)](https://img
+00000660: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000670: 652f 6d61 7961 2d32 3031 392d 6772 6565  e/maya-2019-gree
+00000680: 6e29 0a5b 215b 6d61 7961 2d32 3031 385d  n).[![maya-2018]
+00000690: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000006a0: 656c 6473 2e69 6f2f 6261 6467 652f 6d61  elds.io/badge/ma
+000006b0: 7961 2d32 3031 382d 6772 6565 6e29 5d28  ya-2018-green)](
+000006c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000006d0: 6c64 732e 696f 2f62 6164 6765 2f6d 6179  lds.io/badge/may
+000006e0: 612d 3230 3138 2d67 7265 656e 290a 0a3c  a-2018-green)..<
+000006f0: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00000700: 544f 5253 2d42 4144 4745 3a53 5441 5254  TORS-BADGE:START
+00000710: 202d 2044 6f20 6e6f 7420 7265 6d6f 7665   - Do not remove
+00000720: 206f 7220 6d6f 6469 6679 2074 6869 7320   or modify this 
+00000730: 7365 6374 696f 6e20 2d2d 3e0a 5b21 5b41  section -->.[![A
+00000740: 6c6c 2043 6f6e 7472 6962 7574 6f72 735d  ll Contributors]
+00000750: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000760: 656c 6473 2e69 6f2f 6261 6467 652f 616c  elds.io/badge/al
+00000770: 6c5f 636f 6e74 7269 6275 746f 7273 2d34  l_contributors-4
+00000780: 2d6f 7261 6e67 652e 7376 673f 7374 796c  -orange.svg?styl
+00000790: 653d 666c 6174 2d73 7175 6172 6529 5d28  e=flat-square)](
+000007a0: 2363 6f6e 7472 6962 7574 6f72 732d 290a  #contributors-).
+000007b0: 3c21 2d2d 2041 4c4c 2d43 4f4e 5452 4942  <!-- ALL-CONTRIB
+000007c0: 5554 4f52 532d 4241 4447 453a 454e 4420  UTORS-BADGE:END 
+000007d0: 2d2d 3e0a 0a54 6869 7320 746f 6f6c 2069  -->..This tool i
+000007e0: 7320 6465 7369 676e 6564 2074 6f20 7072  s designed to pr
+000007f0: 6f76 6964 6520 6120 726f 6275 7374 2073  ovide a robust s
+00000800: 6f6c 7574 696f 6e20 666f 7220 6964 656e  olution for iden
+00000810: 7469 6679 696e 6720 616e 6420 7265 736f  tifying and reso
+00000820: 6c76 696e 6720 616e 7920 706f 7465 6e74  lving any potent
+00000830: 6961 6c20 7669 7275 7365 7320 7769 7468  ial viruses with
+00000840: 696e 2041 7574 6f64 6573 6b20 4d61 7961  in Autodesk Maya
+00000850: 2e20 0a49 7420 656e 7375 7265 7320 6120  . .It ensures a 
+00000860: 7365 6375 7265 2061 6e64 2073 6561 6d6c  secure and seaml
+00000870: 6573 7320 7573 6572 2065 7870 6572 6965  ess user experie
+00000880: 6e63 6520 6279 2070 726f 6163 7469 7665  nce by proactive
+00000890: 6c79 2073 6361 6e6e 696e 6720 666f 7220  ly scanning for 
+000008a0: 7468 7265 6174 7320 616e 6420 6566 6665  threats and effe
+000008b0: 6374 6976 656c 7920 6e65 7574 7261 6c69  ctively neutrali
+000008c0: 7a69 6e67 2074 6865 6d2e 0a0a 4974 2063  zing them...It c
+000008d0: 616e 2062 6520 7072 6f76 6964 6564 2061  an be provided a
+000008e0: 7320 616e 2041 5049 2066 6f72 2073 6561  s an API for sea
+000008f0: 6d6c 6573 7320 696e 7465 6772 6174 696f  mless integratio
+00000900: 6e20 696e 746f 2079 6f75 7220 6578 6973  n into your exis
+00000910: 7469 6e67 2070 6970 656c 696e 652e 0a0a  ting pipeline...
+00000920: 0a23 20e5 bc80 e58f 91e7 8eaf e5a2 83e8  .# .............
+00000930: aebe e7bd ae0a 0a53 6574 2075 7020 7468  .......Set up th
+00000940: 6520 6465 7665 6c6f 706d 656e 7420 656e  e development en
+00000950: 7669 726f 6e6d 656e 7420 7573 696e 6720  vironment using 
+00000960: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
+00000970: 6e6d 656e 742c 200a 616e 6420 6974 2069  nment, .and it i
+00000980: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
+00000990: 2075 7365 2050 7974 686f 6e20 332e 3820   use Python 3.8 
+000009a0: 6f72 2068 6967 6865 7220 7665 7273 696f  or higher versio
+000009b0: 6e73 2e0a 0ae9 809a e8bf 87e8 999a e68b  ns..............
+000009c0: 9fe7 8eaf e5a2 83e5 8ebb e8ae bee7 bdae  ................
+000009d0: e5bc 80e5 8f91 e78e afe5 a283 2c20 e68e  ............, ..
+000009e0: a8e8 8d90 7079 7468 6f6e 2d33 2e38 e4bb  ....python-3.8..
+000009f0: a5e4 b88a e79a 84e7 8988 e69c ac0a 0a60  ...............`
+00000a00: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+00000a10: 616c 6c20 6e6f 7820 706f 6574 7279 0a60  all nox poetry.`
+00000a20: 6060 0a0a 2320 e5bc 80e5 8f91 e8b0 83e8  ``..# ..........
+00000a30: af95 0a0a 6060 6073 6865 6c6c 0a6e 6f78  ....```shell.nox
+00000a40: 202d 7320 6d61 7961 2d32 3032 300a 6060   -s maya-2020.``
+00000a50: 600a 0a23 2320 e59c a86d 6179 61e4 b8ad  `..## ...maya...
+00000a60: e6b5 8be8 af95 0a0a e980 9ae8 bf87 606e  ..............`n
+00000a70: 6f78 202d 7320 6d61 7961 2d78 7878 602c  ox -s maya-xxx`,
+00000a80: 20e5 90af e58a a86d 6179 612e 0a6e 6f78   ......maya..nox
+00000a90: e4bc 9ae5 8aa8 e680 81e6 a0b9 e68d aee4  ................
+00000aa0: bda0 e69c ace5 9cb0 e5ae 89e8 a385 e5be  ................
+00000ab0: 976d 6179 61e5 8ebb e6b3 a8e5 868c 6e6f  .maya.........no
+00000ac0: 7820 7365 7373 696f 6e2c 20e6 af94 e5a6  x session, .....
+00000ad0: 82e4 bda0 e69c ace5 9cb0 e5ae 89e8 a385  ................
+00000ae0: e4ba 8660 6d61 7961 2d32 3032 3060 efbc  ...`maya-2020`..
+00000af0: 8ce9 82a3 e4b9 88e9 809a e8bf 8760 6e6f  .............`no
+00000b00: 7820 2d73 206d 6179 612d 3230 3138 600a  x -s maya-2018`.
+00000b10: 0ae5 90af e58a a86d 6179 61e5 908e e59c  .......maya.....
+00000b20: a8e8 849a e69c ace7 bc96 e8be 91e5 99a8  ................
+00000b30: e4b8 ade6 89a7 e8a1 8ce4 b88b e99d a2e5  ................
+00000b40: be97 e4bb a3e7 a081 efbc 8ce5 b0b1 e4bc  ................
+00000b50: 9ae5 8aa8 e680 81e7 9a84 e4bb 8e60 3c72  .............`<r
+00000b60: 6570 6f3e 2f74 6573 7473 2f76 6972 7573  epo>/tests/virus
+00000b70: 2f60 e987 8ce9 9da2 e58e bb6f 7065 6e20  /`.........open 
+00000b80: 6d61 e696 87e4 bbb6 e58e bbe8 bf9b e8a1  ma..............
+00000b90: 8ce6 b58b e8af 952e 0a0a 6060 6070 7974  ..........```pyt
+00000ba0: 686f 6e0a 696d 706f 7274 206d 616e 7561  hon.import manua
+00000bb0: 6c5f 7465 7374 5f69 6e5f 6d61 7961 0a0a  l_test_in_maya..
+00000bc0: 6d61 6e75 616c 5f74 6573 745f 696e 5f6d  manual_test_in_m
+00000bd0: 6179 612e 7374 6172 7428 290a 6060 600a  aya.start().```.
+00000be0: 0a23 2320 e5a2 9ee5 8aa0 e696 b0e7 9a84  .## ............
+00000bf0: e796 abe8 8b97 0a0a e59c a860 3c72 6570  ...........`<rep
+00000c00: 6f3e 2f6d 6179 615f 756d 6272 656c 6c61  o>/maya_umbrella
+00000c10: 2f76 6163 6369 6e65 732f 6020 e696 b0e5  /vaccines/` ....
+00000c20: bbba e4b8 80e4 b8aa 7079 2c20 e59b a0e4  ........py, ....
+00000c30: b8ba e69c 89e5 be88 e5a4 9ae7 9785 e6af  ................
+00000c40: 92e6 b2a1 e69c 89e5 85b7 e4bd 93e7 9a84  ................
+00000c50: e590 8de5 ad97 e4bb a3e5 8fb7 efbc 8ce6  ................
+00000c60: 8891 e4bb ace7 bb9f e4b8 80e4 bba5 6076  ..............`v
+00000c70: 6163 6369 6e65 3c69 643e 2e70 7960 0ae7  accine<id>.py`..
+00000c80: bba7 e689 bf60 6672 6f6d 206d 6179 615f  .....`from maya_
+00000c90: 756d 6272 656c 6c61 2e76 6163 6369 6e65  umbrella.vaccine
+00000ca0: 2069 6d70 6f72 7420 4162 7374 7261 6374   import Abstract
+00000cb0: 5661 6363 696e 6560 e5b9 b6e4 b894 636c  Vaccine`......cl
+00000cc0: 6173 73e5 908d e5ad 97e5 8fab 6056 6163  ass.........`Vac
+00000cd0: 6369 6e65 60e5 8db3 e58f af2c 20e7 84b6  cine`......, ...
+00000ce0: e590 8ee5 8ebb e586 99e5 85b7 e4bd 93e7  ................
+00000cf0: 9a84 e694 b6e9 9b86 e797 85e6 af92 e980  ................
+00000d00: bbe8 be91 0a0a 2323 20e4 bba3 e7a0 81e6  ......## .......
+00000d10: a380 e69f a50a 0ae6 8891 e4bb ace5 8faf  ................
+00000d20: e4bb a5e5 88a9 e794 a8e5 b081 e8a3 85e5  ................
+00000d30: a5bd e79a 8460 6e6f 7860 e591 bde4 bba4  .....`nox`......
+00000d40: e58e bbe6 89a7 e8a1 8ce8 bf9b e8a1 8ce4  ................
+00000d50: bba3 e7a0 81e6 a380 e69f a50a 0a60 6060  .............```
+00000d60: 7368 656c 6c0a 6e6f 7820 2d73 2072 7566  shell.nox -s ruf
+00000d70: 665f 6368 6563 6b0a 6060 600a 0a23 20e7  f_check.```..# .
+00000d80: 8eaf e5a2 83e5 8f98 e987 8f0a 0ae6 8891  ................
+00000d90: e4bb ace5 8faf e4bb a5e9 809a e8bf 87e4  ................
+00000da0: b88b e588 97e7 8eaf e5a2 83e5 8f98 e987  ................
+00000db0: 8fe5 8ebb e4bf aee6 94b9 6d61 7961 5f75  ..........maya_u
+00000dc0: 6d62 7265 6c6c 61e7 9a84 e4b8 80e4 ba9b  mbrella.........
+00000dd0: e8ae bee7 bdae efbc 8ce6 96b9 e4be bfe6  ................
+00000de0: 9c89 7069 7065 6c69 6e65 e79a 84e5 85ac  ..pipeline......
+00000df0: e58f b8e5 8faf e4bb a5e6 9bb4 e5a5 bde7  ................
+00000e00: 9a84 e99b 86e6 8890 0a0a e4bf aee6 94b9  ................
+00000e10: 6d61 7961 2075 6d62 7265 6c6c 61e7 9a84  maya umbrella...
+00000e20: e697 a5e5 bf97 e4bf 9de5 ad98 e79b aee5  ................
+00000e30: bd95 efbc 8ce9 bb98 e8ae a4e6 98af 7769  ..............wi
+00000e40: 6e64 6f77 7320 7465 6d70 e79b aee5 bd95  ndows temp......
+00000e50: 0a0a 6060 6073 6865 6c6c 0a4d 4159 415f  ..```shell.MAYA_
+00000e60: 554d 4252 454c 4c41 5f4c 4f47 5f52 4f4f  UMBRELLA_LOG_ROO
+00000e70: 540a 6060 600a 0ae4 bfae e694 b96d 6179  T.```........may
+00000e80: 6120 756d 6272 656c 6c61 e79a 84e6 97a5  a umbrella......
+00000e90: e5bf 97e6 9687 e4bb b6e5 908d e7a7 b02c  ...............,
+00000ea0: 20e9 bb98 e8ae a4e6 98af 606d 6179 615f   .........`maya_
+00000eb0: 756d 6272 656c 6c61 600a 0a60 6060 7368  umbrella`..```sh
+00000ec0: 656c 6c0a 4d41 5941 5f55 4d42 5245 4c4c  ell.MAYA_UMBRELL
+00000ed0: 415f 4c4f 475f 4e41 4d45 0a60 6060 0a0a  A_LOG_NAME.```..
+00000ee0: e8ae bee7 bdae e697 a5e5 bf97 e7ba a7e5  ................
+00000ef0: 88ab efbc 8ce9 bb98 e8ae a4e6 98af 696e  ..............in
+00000f00: 666f 2c20 e58f afe4 bba5 e698 af64 6562  fo, .........deb
+00000f10: 7567 e58f afe4 bba5 e79c 8be5 88b0 e69b  ug..............
+00000f20: b4e5 a49a e79a 84e6 97a5 e5bf 97e4 bfa1  ................
+00000f30: e681 af0a 0a60 6060 7368 656c 6c0a 4d41  .....```shell.MA
+00000f40: 5941 5f55 4d42 5245 4c4c 415f 4c4f 475f  YA_UMBRELLA_LOG_
+00000f50: 4c45 5645 4c0a 6060 600a 0a23 2320 436f  LEVEL.```..## Co
+00000f60: 6e74 7269 6275 746f 7273 20e2 9ca8 0a0a  ntributors .....
+00000f70: 5468 616e 6b73 2067 6f65 7320 746f 2074  Thanks goes to t
+00000f80: 6865 7365 2077 6f6e 6465 7266 756c 2070  hese wonderful p
+00000f90: 656f 706c 6520 285b 656d 6f6a 6920 6b65  eople ([emoji ke
+00000fa0: 795d 2868 7474 7073 3a2f 2f61 6c6c 636f  y](https://allco
+00000fb0: 6e74 7269 6275 746f 7273 2e6f 7267 2f64  ntributors.org/d
+00000fc0: 6f63 732f 656e 2f65 6d6f 6a69 2d6b 6579  ocs/en/emoji-key
+00000fd0: 2929 3a0a 0a3c 212d 2d20 414c 4c2d 434f  )):..<!-- ALL-CO
+00000fe0: 4e54 5249 4255 544f 5253 2d4c 4953 543a  NTRIBUTORS-LIST:
+00000ff0: 5354 4152 5420 2d20 446f 206e 6f74 2072  START - Do not r
+00001000: 656d 6f76 6520 6f72 206d 6f64 6966 7920  emove or modify 
+00001010: 7468 6973 2073 6563 7469 6f6e 202d 2d3e  this section -->
+00001020: 0a3c 212d 2d20 7072 6574 7469 6572 2d69  .<!-- prettier-i
+00001030: 676e 6f72 652d 7374 6172 7420 2d2d 3e0a  gnore-start -->.
+00001040: 3c21 2d2d 206d 6172 6b64 6f77 6e6c 696e  <!-- markdownlin
+00001050: 742d 6469 7361 626c 6520 2d2d 3e0a 3c74  t-disable -->.<t
+00001060: 6162 6c65 3e0a 2020 3c74 626f 6479 3e0a  able>.  <tbody>.
+00001070: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+00001080: 7464 2061 6c69 676e 3d22 6365 6e74 6572  td align="center
+00001090: 2220 7661 6c69 676e 3d22 746f 7022 2077  " valign="top" w
+000010a0: 6964 7468 3d22 3134 2e32 3825 223e 3c61  idth="14.28%"><a
+000010b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000010c0: 6974 6875 622e 636f 6d2f 6c6f 6f6e 6768  ithub.com/loongh
+000010d0: 616f 223e 3c69 6d67 2073 7263 3d22 6874  ao"><img src="ht
+000010e0: 7470 733a 2f2f 6176 6174 6172 7331 2e67  tps://avatars1.g
+000010f0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001100: 2e63 6f6d 2f75 2f31 3331 3131 3734 353f  .com/u/13111745?
+00001110: 763d 343f 733d 3130 3022 2077 6964 7468  v=4?s=100" width
+00001120: 3d22 3130 3070 783b 2220 616c 743d 2248  ="100px;" alt="H
+00001130: 616c 222f 3e3c 6272 202f 3e3c 7375 623e  al"/><br /><sub>
+00001140: 3c62 3e48 616c 3c2f 623e 3c2f 7375 623e  <b>Hal</b></sub>
+00001150: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
+00001160: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001170: 622e 636f 6d2f 6c6f 6f6e 6768 616f 2f6d  b.com/loonghao/m
+00001180: 6179 615f 756d 6272 656c 6c61 2f63 6f6d  aya_umbrella/com
+00001190: 6d69 7473 3f61 7574 686f 723d 6c6f 6f6e  mits?author=loon
+000011a0: 6768 616f 2220 7469 746c 653d 2243 6f64  ghao" title="Cod
+000011b0: 6522 3ef0 9f92 bb3c 2f61 3e20 3c61 2068  e">....</a> <a h
+000011c0: 7265 663d 2223 696e 6672 612d 6c6f 6f6e  ref="#infra-loon
+000011d0: 6768 616f 2220 7469 746c 653d 2249 6e66  ghao" title="Inf
+000011e0: 7261 7374 7275 6374 7572 6520 2848 6f73  rastructure (Hos
+000011f0: 7469 6e67 2c20 4275 696c 642d 546f 6f6c  ting, Build-Tool
+00001200: 732c 2065 7463 2922 3ef0 9f9a 873c 2f61  s, etc)">....</a
+00001210: 3e20 3c61 2068 7265 663d 2268 7474 7073  > <a href="https
+00001220: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c6f  ://github.com/lo
+00001230: 6f6e 6768 616f 2f6d 6179 615f 756d 6272  onghao/maya_umbr
+00001240: 656c 6c61 2f63 6f6d 6d69 7473 3f61 7574  ella/commits?aut
+00001250: 686f 723d 6c6f 6f6e 6768 616f 2220 7469  hor=loonghao" ti
+00001260: 746c 653d 2254 6573 7473 223e e29a a0ef  tle="Tests">....
+00001270: b88f 3c2f 613e 3c2f 7464 3e0a 2020 2020  ..</a></td>.    
+00001280: 2020 3c74 6420 616c 6967 6e3d 2263 656e    <td align="cen
+00001290: 7465 7222 2076 616c 6967 6e3d 2274 6f70  ter" valign="top
+000012a0: 2220 7769 6474 683d 2231 342e 3238 2522  " width="14.28%"
+000012b0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+000012c0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6f74  //github.com/hot
+000012d0: 7769 6e74 6572 3022 3e3c 696d 6720 7372  winter0"><img sr
+000012e0: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
+000012f0: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
+00001300: 7465 6e74 2e63 6f6d 2f75 2f31 3036 3233  tent.com/u/10623
+00001310: 3733 3035 3f76 3d34 3f73 3d31 3030 2220  7305?v=4?s=100" 
+00001320: 7769 6474 683d 2231 3030 7078 3b22 2061  width="100px;" a
+00001330: 6c74 3d22 686f 7477 696e 7465 7230 222f  lt="hotwinter0"/
+00001340: 3e3c 6272 202f 3e3c 7375 623e 3c62 3e68  ><br /><sub><b>h
+00001350: 6f74 7769 6e74 6572 303c 2f62 3e3c 2f73  otwinter0</b></s
+00001360: 7562 3e3c 2f61 3e3c 6272 202f 3e3c 6120  ub></a><br /><a 
+00001370: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001380: 7468 7562 2e63 6f6d 2f6c 6f6f 6e67 6861  thub.com/loongha
+00001390: 6f2f 6d61 7961 5f75 6d62 7265 6c6c 612f  o/maya_umbrella/
+000013a0: 636f 6d6d 6974 733f 6175 7468 6f72 3d68  commits?author=h
+000013b0: 6f74 7769 6e74 6572 3022 2074 6974 6c65  otwinter0" title
+000013c0: 3d22 5465 7374 7322 3ee2 9aa0 efb8 8f3c  ="Tests">......<
+000013d0: 2f61 3e20 3c61 2068 7265 663d 2268 7474  /a> <a href="htt
+000013e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013f0: 6c6f 6f6e 6768 616f 2f6d 6179 615f 756d  loonghao/maya_um
+00001400: 6272 656c 6c61 2f63 6f6d 6d69 7473 3f61  brella/commits?a
+00001410: 7574 686f 723d 686f 7477 696e 7465 7230  uthor=hotwinter0
+00001420: 2220 7469 746c 653d 2243 6f64 6522 3ef0  " title="Code">.
+00001430: 9f92 bb3c 2f61 3e3c 2f74 643e 0a20 2020  ...</a></td>.   
+00001440: 2020 203c 7464 2061 6c69 676e 3d22 6365     <td align="ce
+00001450: 6e74 6572 2220 7661 6c69 676e 3d22 746f  nter" valign="to
+00001460: 7022 2077 6964 7468 3d22 3134 2e32 3825  p" width="14.28%
+00001470: 223e 3c61 2068 7265 663d 2268 7474 7073  "><a href="https
+00001480: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c69  ://github.com/li
+00001490: 6e67 7975 6e66 7822 3e3c 696d 6720 7372  ngyunfx"><img sr
+000014a0: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
+000014b0: 7273 2e67 6974 6875 6275 7365 7263 6f6e  rs.githubusercon
+000014c0: 7465 6e74 2e63 6f6d 2f75 2f37 3336 3636  tent.com/u/73666
+000014d0: 3632 393f 763d 343f 733d 3130 3022 2077  629?v=4?s=100" w
+000014e0: 6964 7468 3d22 3130 3070 783b 2220 616c  idth="100px;" al
+000014f0: 743d 226c 696e 6779 756e 6678 222f 3e3c  t="lingyunfx"/><
+00001500: 6272 202f 3e3c 7375 623e 3c62 3e6c 696e  br /><sub><b>lin
+00001510: 6779 756e 6678 3c2f 623e 3c2f 7375 623e  gyunfx</b></sub>
+00001520: 3c2f 613e 3c62 7220 2f3e 3c61 2068 7265  </a><br /><a hre
+00001530: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001540: 622e 636f 6d2f 6c6f 6f6e 6768 616f 2f6d  b.com/loonghao/m
+00001550: 6179 615f 756d 6272 656c 6c61 2f63 6f6d  aya_umbrella/com
+00001560: 6d69 7473 3f61 7574 686f 723d 6c69 6e67  mits?author=ling
+00001570: 7975 6e66 7822 2074 6974 6c65 3d22 5465  yunfx" title="Te
+00001580: 7374 7322 3ee2 9aa0 efb8 8f3c 2f61 3e3c  sts">......</a><
+00001590: 2f74 643e 0a20 2020 2020 203c 7464 2061  /td>.      <td a
+000015a0: 6c69 676e 3d22 6365 6e74 6572 2220 7661  lign="center" va
+000015b0: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
+000015c0: 3d22 3134 2e32 3825 223e 3c61 2068 7265  ="14.28%"><a hre
+000015d0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000015e0: 622e 636f 6d2f 796a 6a6a 6a22 3e3c 696d  b.com/yjjjj"><im
+000015f0: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
+00001600: 7661 7461 7273 2e67 6974 6875 6275 7365  vatars.githubuse
+00001610: 7263 6f6e 7465 6e74 2e63 6f6d 2f75 2f31  rcontent.com/u/1
+00001620: 3237 3431 3733 353f 763d 343f 733d 3130  2741735?v=4?s=10
+00001630: 3022 2077 6964 7468 3d22 3130 3070 783b  0" width="100px;
+00001640: 2220 616c 743d 2279 6a6a 6a6a 222f 3e3c  " alt="yjjjj"/><
+00001650: 6272 202f 3e3c 7375 623e 3c62 3e79 6a6a  br /><sub><b>yjj
+00001660: 6a6a 3c2f 623e 3c2f 7375 623e 3c2f 613e  jj</b></sub></a>
+00001670: 3c62 7220 2f3e 3c61 2068 7265 663d 2268  <br /><a href="h
+00001680: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001690: 6d2f 6c6f 6f6e 6768 616f 2f6d 6179 615f  m/loonghao/maya_
+000016a0: 756d 6272 656c 6c61 2f63 6f6d 6d69 7473  umbrella/commits
+000016b0: 3f61 7574 686f 723d 796a 6a6a 6a22 2074  ?author=yjjjj" t
+000016c0: 6974 6c65 3d22 5465 7374 7322 3ee2 9aa0  itle="Tests">...
+000016d0: efb8 8f3c 2f61 3e20 3c61 2068 7265 663d  ...</a> <a href=
+000016e0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000016f0: 636f 6d2f 6c6f 6f6e 6768 616f 2f6d 6179  com/loonghao/may
+00001700: 615f 756d 6272 656c 6c61 2f63 6f6d 6d69  a_umbrella/commi
+00001710: 7473 3f61 7574 686f 723d 796a 6a6a 6a22  ts?author=yjjjj"
+00001720: 2074 6974 6c65 3d22 436f 6465 223e f09f   title="Code">..
+00001730: 92bb 3c2f 613e 3c2f 7464 3e0a 2020 2020  ..</a></td>.    
+00001740: 3c2f 7472 3e0a 2020 3c2f 7462 6f64 793e  </tr>.  </tbody>
+00001750: 0a3c 2f74 6162 6c65 3e0a 0a3c 212d 2d20  .</table>..<!-- 
+00001760: 6d61 726b 646f 776e 6c69 6e74 2d72 6573  markdownlint-res
+00001770: 746f 7265 202d 2d3e 0a3c 212d 2d20 7072  tore -->.<!-- pr
+00001780: 6574 7469 6572 2d69 676e 6f72 652d 656e  ettier-ignore-en
+00001790: 6420 2d2d 3e0a 0a3c 212d 2d20 414c 4c2d  d -->..<!-- ALL-
+000017a0: 434f 4e54 5249 4255 544f 5253 2d4c 4953  CONTRIBUTORS-LIS
+000017b0: 543a 454e 4420 2d2d 3e0a 0a54 6869 7320  T:END -->..This 
+000017c0: 7072 6f6a 6563 7420 666f 6c6c 6f77 7320  project follows 
+000017d0: 7468 6520 5b61 6c6c 2d63 6f6e 7472 6962  the [all-contrib
+000017e0: 7574 6f72 735d 2868 7474 7073 3a2f 2f61  utors](https://a
+000017f0: 6c6c 636f 6e74 7269 6275 746f 7273 2e6f  llcontributors.o
+00001800: 7267 2920 7370 6563 6966 6963 6174 696f  rg) specificatio
+00001810: 6e2e 0a43 6f6e 7472 6962 7574 696f 6e73  n..Contributions
+00001820: 206f 6620 616e 7920 6b69 6e64 2061 7265   of any kind are
+00001830: 2077 656c 636f 6d65 210a                  welcome!.
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/core.py` & `maya_umbrella-0.5.0/maya_umbrella/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Import built-in modules
 import logging
 
-# Import third-party modules
-import maya.api.OpenMaya as om
-import maya.cmds as cmds
-
 # Import local modules
 from maya_umbrella.filesystem import get_hooks
 from maya_umbrella.filesystem import get_vaccines
 from maya_umbrella.filesystem import load_hook
 from maya_umbrella.log import setup_logger
+from maya_umbrella.maya_funs import is_maya_standalone
+from maya_umbrella.maya_funs import om
 from maya_umbrella.vaccine import MayaVirusCleaner
 
 
 class MayaVirusDefender(object):
     callback_ids = []
     remove_callbacks = []
     _bad_files = []
@@ -59,34 +57,38 @@
         Returns:
             list: A list of loaded vaccines.
         """
         return self._vaccines
 
     def run_hooks(self):
         """Run all hooks, only works in non-batch mode."""
-        if not cmds.about(batch=True):
+        if not is_maya_standalone():
             for hook_file in get_hooks():
                 self.logger.debug("run_hook: %s", hook_file)
                 try:
                     load_hook(hook_file).hook(virus_cleaner=self.virus_cleaner)
                 except Exception as e:
                     self.logger.error("Error running hook: %s", e)
 
     def collect(self):
         """Collect all issues related to the Maya virus."""
         for vaccine in self.vaccines:
             vaccine.collect_issues()
 
+    def reset(self):
+        """Reset internal buffer."""
+        self.virus_cleaner.reset_all_issues()
+
     def fix(self):
         """Fix all issues related to the Maya virus."""
         self.virus_cleaner.fix_all_issues()
 
     def report(self):
         """Report all issues related to the Maya virus."""
-        self.virus_cleaner.reset_all_issues()
+        self.reset()
         self.collect()
         self.virus_cleaner.report_all_issues()
 
     def setup(self):
         """Set up the MayaVirusDefender."""
         self.virus_cleaner.setup_default_callbacks()
         for name, callbacks in self.virus_cleaner.registered_callbacks.items():
@@ -102,14 +104,15 @@
         """Callback function for MayaVirusDefender.
 
         Args:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
         """
         if self.auto_fix:
+            self.reset()
             self.collect()
             self.fix()
             self.run_hooks()
         else:
             self.report()
 
     def start(self):
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.5.0/maya_umbrella/hooks/delete_turtle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Import third-party modules
-import maya.cmds as cmds
-import maya.mel as mel
+# Import local modules
+from maya_umbrella.maya_funs import cmds
+from maya_umbrella.maya_funs import mel
 
 
 def hook(virus_cleaner):
     for plugin in ["Turtle.mll", "mayatomr.mll"]:
         if cmds.pluginInfo(plugin, q=1, loaded=1):
             cmds.unloadPlugin(plugin, f=1)
     turtle_nodes = [
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.5.0/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Import third-party modules
-import maya.cmds as cmds
+# Import local modules
+from maya_umbrella.maya_funs import cmds
 
 
 def hook(virus_cleaner):
     unknown_node = cmds.ls(type="unknown")
     unknown_plugin = cmds.unknownPlugin(query=True, l=True)
     if unknown_node:
         for nodeObj in unknown_node:
@@ -12,15 +12,16 @@
                     virus_cleaner.logger.warning("Node from reference, skip. {}".format(nodeObj))
                     continue
                 if cmds.lockNode(nodeObj, query=True)[0]:
                     try:
                         cmds.lockNode(nodeObj, lock=False)
                     except Exception:
                         virus_cleaner.logger.warning(
-                            "The node is locked and cannot be unlocked. skip {}".format(nodeObj))
+                            "The node is locked and cannot be unlocked. skip {}".format(nodeObj)
+                        )
                         continue
                 try:
                     cmds.delete(nodeObj)
                     virus_cleaner.logger.warning("Delete node: {}".format(nodeObj))
                 except Exception:
                     pass
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.5.0/maya_umbrella/hooks/fix_model_panel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Import third-party modules
-import maya.cmds as cmds
+# Import local modules
+from maya_umbrella.maya_funs import cmds
 
 
 def hook(virus_cleaner):
     for model_panel in cmds.getPanel(typ="modelPanel"):
         # Get callback of the model editor
         callback = cmds.modelEditor(model_panel, query=True, editorChanged=True)
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/log.py` & `maya_umbrella-0.5.0/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.4.1/maya_umbrella/vaccine.py` & `maya_umbrella-0.5.0/maya_umbrella/vaccine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Import built-in modules
 from collections import defaultdict
 import glob
 import logging
 import os
-
-# Import third-party modules
-import maya.cmds as cmds
+import re
 
 # Import local modules
+from maya_umbrella.constants import FILE_VIRUS_SIGNATURES
+from maya_umbrella.filesystem import remove_virus_file_by_signature
 from maya_umbrella.filesystem import safe_remove_file
 from maya_umbrella.filesystem import safe_rmtree
+from maya_umbrella.maya_funs import check_reference_node_exists
+from maya_umbrella.maya_funs import cmds
 
 
 class MayaVirusCleaner(object):
     _bad_files = []
+    _infected_files = []
     _bad_nodes = []
     _bad_script_nodes = []
     _bad_script_jobs = []
     _registered_callbacks = defaultdict(list)
     _fix_funcs = []
 
     def __init__(self, logger=None, auto_fix=True):
@@ -28,15 +31,15 @@
     def user_app_dir(self):
         """Return the user application directory."""
         return cmds.internalVar(userAppDir=True)
 
     @property
     def maya_file(self):
         """Return the current Maya file."""
-        return cmds.file(q=True, sn=True)
+        return cmds.file(query=True, sceneName=True, shortName=True) or "empty/scene"
 
     @property
     def maya_install_root(self):
         """Return the Maya installation root directory."""
         return os.environ["MAYA_LOCATION"]
 
     @property
@@ -65,25 +68,34 @@
         return list(set(self._bad_script_nodes))
 
     @property
     def bad_script_jobs(self):
         """Return a list of bad script jobs."""
         return list(set(self._bad_script_jobs))
 
+    @property
+    def infected_files(self):
+        return self._infected_files
+
     def callback_remove_rename_temp_files(self, *args, **kwargs):
-        """
-        Remove temporary files in the local script path.
-        """
+        """Remove temporary files in the local script path."""
         self.logger.info("Removing temporary files in %s", self.local_script_path)
-        [safe_remove_file(temp_file) for temp_file in glob.glob(os.path.join(self.local_script_path, "._*"))]
+        for temp_file in glob.glob(os.path.join(self.local_script_path, "._*")):
+            safe_remove_file(temp_file)
 
     @property
     def registered_callbacks(self):
         return self._registered_callbacks
 
+    def add_infected_files(self, files):
+        self._infected_files.extend(files)
+
+    def add_infected_file(self, file):
+        self._infected_files.append(file)
+
     def add_bad_files(self, files):
         self._bad_files.extend(files)
 
     def add_bad_file(self, file):
         self._bad_files.append(file)
 
     def add_bad_nodes(self, nodes):
@@ -141,19 +153,17 @@
     def setup_default_callbacks(self):
         self.add_maya_initialized_callback(self.callback_remove_rename_temp_files)
         self.add_maya_exiting_callback(self.callback_remove_rename_temp_files)
 
     def add_fix_function(self, func):
         self._fix_funcs.append(func)
 
-    # fix
-
     def fix_script_jobs(self):
         for script_job in self.bad_script_jobs:
-            script_num = int(script_job.split(":", 1)[0])
+            script_num = int(re.findall(r"^(\d+):", script_job)[0])
             self.logger.info("Kill script job %s", script_job)
             cmds.scriptJob(kill=script_num, force=True)
             self._bad_script_jobs.remove(script_job)
 
     def fix_bad_files(self):
         for file_ in self.bad_files:
             if os.path.exists(file_):
@@ -165,44 +175,65 @@
                     self.logger.info("Removing folder %s", file_)
                     safe_rmtree(file_)
                     self._bad_files.remove(file_)
 
     def fix_bad_nodes(self):
         for node in self.bad_nodes:
             self.logger.info("Deleting %s", node)
-            try:
-                cmds.lockNode(node, lock=False)
-            except ValueError:
-                pass
-            try:
-                cmds.delete(node)
-            except ValueError:
-                pass
-            self._bad_nodes.remove(node)
+            is_referenced = check_reference_node_exists(node)
+            if is_referenced:
+                try:
+                    cmds.setAttr("{node}.before".format(node=node), "", type="string")
+                    cmds.setAttr("{node}.after".format(node=node), "", type="string")
+                    cmds.setAttr("{node}.scriptType".format(node=node), 0)
+                    self._bad_nodes.remove(node)
+                except Exception as e:
+                    self.logger.debug(e)
+            else:
+                try:
+                    cmds.lockNode(node, lock=False)
+                except ValueError:
+                    pass
+                try:
+                    cmds.delete(node)
+                except ValueError:
+                    pass
+                self._bad_nodes.remove(node)
+
+    def fix_infected_files(self):
+        for file_path in self.infected_files:
+            self.logger.info("Removing infected file: %s", file_path)
+            remove_virus_file_by_signature(file_path, FILE_VIRUS_SIGNATURES)
+            self._infected_files.remove(file_path)
 
     def fix_all_issues(self):
         """Fix all issues related to the Maya virus."""
+        self.logger.info("Starting Fixing all issues related to the Maya virus from %s.", self.maya_file)
         self.fix_bad_files()
+        self.fix_infected_files()
         self.fix_bad_nodes()
         self.fix_script_jobs()
         for func in self._fix_funcs:
             func()
+        self.logger.info("Finished Fixing all issues related to the Maya virus from %s.", self.maya_file)
 
     def report_all_issues(self):
         """Report all issues related to the Maya virus."""
         self.logger.info("Bad files: %s", self.bad_files)
         self.logger.info("Bad nodes: %s", self.bad_nodes)
         self.logger.info("Bad script jobs: %s", self.bad_script_jobs)
+        self.logger.info("Infected files: %s", self.infected_files)
 
     def reset_all_issues(self):
         """Reset all issues related to the Maya virus."""
         self._bad_files = []
         self._bad_nodes = []
         self._bad_script_nodes = []
         self._bad_script_jobs = []
+        self._infected_files = []
 
 
 class AbstractVaccine(object):
     virus_name = None
 
     def __init__(self, api, logger):
         """Abstract class for Vaccine.
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Import built-in modules
 import os.path
 
-# Import third-party modules
-import maya.cmds as cmds
-
 # Import local modules
-from maya_umbrella.filesystem import read_file
-from maya_umbrella.filesystem import rename
+from maya_umbrella.constants import JOB_SCRIPTS_VIRUS_SIGNATURES
+from maya_umbrella.filesystem import check_virus_by_signature
+from maya_umbrella.filesystem import check_virus_file_by_signature
+from maya_umbrella.maya_funs import check_reference_node_exists
+from maya_umbrella.maya_funs import cmds
 from maya_umbrella.vaccine import AbstractVaccine
 
 
 class Vaccine(AbstractVaccine):
+    """A class for handling the ZeiJianKang virus."""
+
     virus_name = "zei jian kang"
 
     def collect_bad_nodes(self):
         """Collect all bad nodes related to the virus."""
         for script_node in cmds.ls(type="script"):
-            if cmds.referenceQuery(script_node, isNodeReferenced=True):
+            if check_reference_node_exists(script_node):
                 continue
             script_before_string = cmds.getAttr("{}.before".format(script_node))
             script_after_string = cmds.getAttr("{}.after".format(script_node))
             for script_string in [script_before_string, script_after_string]:
                 if not script_string:
                     continue
-                if "internalVar" in script_string or "userSetup" in script_string or "fuckVirus" in script_string:
+                if check_virus_by_signature(script_string, JOB_SCRIPTS_VIRUS_SIGNATURES):
                     self.report_issue(script_node)
                     self.api.add_bad_node(script_node)
 
     def collect_issues(self):
         """Collect all issues related to the virus."""
         self.api.add_bad_files(
             [
@@ -37,24 +39,14 @@
         )
         self.collect_bad_usersetup_py()
         self.collect_bad_nodes()
 
     def collect_bad_usersetup_py(self):
         """Collect all bad userSetup.py files related to the virus."""
         for usersetup_py in [
-            os.path.join(self.api.local_script_path, "vaccine.py"),
-            os.path.join(self.api.user_script_path, "vaccine.py"),
             os.path.join(self.api.local_script_path, "userSetup.py"),
             os.path.join(self.api.user_script_path, "userSetup.py"),
         ]:
             if os.path.exists(usersetup_py):
-                data = read_file(usersetup_py)
-                if "petri_dish_path = cmds.internalVar(userAppDir=True) + 'scripts/userSetup.py" in data:
-                    self.report_issue("vaccine.py")
-                    self.api.add_bad_file(rename(usersetup_py))
-
-                if (
-                    "cmds.evalDeferred('leukocyte = vaccine.phage()')" in data
-                    and "cmds.evalDeferred('leukocyte.occupation()')" in data
-                ):
-                    self.report_issue("userSetup.py")
-                    self.api.add_bad_file(rename(usersetup_py))
+                if check_virus_file_by_signature(usersetup_py):
+                    self.report_issue(usersetup_py)
+                    self.api.add_infected_file(usersetup_py)
```

### Comparing `maya_umbrella-0.4.1/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.5.0/maya_umbrella/vaccines/vaccine3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,72 @@
 # Import built-in modules
 import glob
 import os.path
-import re
-
-# Import third-party modules
-import maya.cmds as cmds
 
 # Import local modules
-from maya_umbrella.filesystem import read_file
-from maya_umbrella.filesystem import rename
+from maya_umbrella.filesystem import check_virus_file_by_signature
+from maya_umbrella.maya_funs import cmds
+from maya_umbrella.maya_funs import is_maya_standalone
 from maya_umbrella.vaccine import AbstractVaccine
 
 
 class Vaccine(AbstractVaccine):
+    """A class for handling the virus2024429 virus."""
+
     virus_name = "virus2024429"
-    hik_regex = r"python\(\"import base64;\s*pyCode\s*=\s*base64\.urlsafe_b64decode\([\'\"].*?[\"\']\);\s*exec\s*\(\s*pyCode\s*\)\"\)\s*;"
 
     def collect_bad_nodes(self):
         """Collect all bad nodes related to the virus."""
         for script_node in cmds.ls(type="script"):
             if cmds.referenceQuery(script_node, isNodeReferenced=True):
                 continue
             # check uifiguration
             if cmds.objExists("{}.KGMScriptProtector".format(script_node)):
+                self.report_issue(script_node)
                 self.api.add_bad_node(script_node)
             # check vaccine
             if "_gene" in script_node:
+                self.report_issue(script_node)
                 self.api.add_bad_node(script_node)
 
     def collect_bad_mel_files(self):
         """Collect all bad MEL files related to the virus."""
         # check usersetup.mel
         # C:/Users/hallong/Documents/maya/scripts/usersetup.mel
         # C:/Users/hallong/Documents/maya/xxxx/scripts/usersetup.mel
         for usersetup_mel in [
             os.path.join(self.api.local_script_path, "usersetup.mel"),
             os.path.join(self.api.user_script_path, "usersetup.mel"),
         ]:
             if os.path.exists(usersetup_mel):
-                data = read_file(usersetup_mel)
-                if "import base64; pyCode = base64.urlsafe_b64decode" in data:
-                    self.api.add_bad_file(rename(usersetup_mel))
+                if check_virus_file_by_signature(usersetup_mel):
+                    self.report_issue(usersetup_mel)
+                    self.api.add_infected_file(usersetup_mel)
 
     def collect_script_jobs(self):
         """Collect all script jobs related to the virus."""
         virus_gene = [
             "leukocyte",
             "execute",
         ]
-
         for script_job in cmds.scriptJob(listJobs=True):
             for virus in virus_gene:
                 if virus in script_job:
-                    self.api.add_bad_script_jobs(script_job)
+                    self.api.add_bad_script_job(script_job)
 
     def fix_bad_hik_files(self):
         """Fix all bad HIK files related to the virus."""
         pattern = os.path.join(self.api.maya_install_root, "resources/l10n/*/plug-ins/mayaHIK.pres.mel")
         for hik_mel in glob.glob(pattern):
-            with open(hik_mel, "rb") as f:
-                data = f.read()
-            try:
-                check = re.findall(self.hik_regex, data)
-            except TypeError:
-                check = []
-            if len(check) > 0:
+            if check_virus_file_by_signature(hik_mel):
                 self.report_issue(hik_mel)
-                with open(hik_mel, "wb") as f:
-                    f.write(re.sub(self.hik_regex, "", data))
-                self.logger.info("Remove virus code from %s", hik_mel)
+                self.api.add_infected_file(hik_mel)
 
     def collect_issues(self):
         """Collect all issues related to the virus."""
         self.api.add_bad_file(os.path.join(os.getenv("APPDATA"), "syssst"))
         self.collect_bad_mel_files()
         self.collect_bad_nodes()
+        # This only works for Maya Gui model.
+        if not is_maya_standalone():
+            self.collect_script_jobs()
         self.api.add_fix_function(self.fix_bad_hik_files)
```

### Comparing `maya_umbrella-0.4.1/PKG-INFO` & `maya_umbrella-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_umbrella
-Version: 0.4.1
+Version: 0.5.0
 Summary: Check and fix maya virus.
 Home-page: https://github.com/loonghao/maya_umbrella
 License: MIT
 Keywords: notifiers,python,Maya,dcc
 Author: longhao
 Author-email: hal.long@outlook.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
@@ -24,16 +24,17 @@
 Description-Content-Type: text/markdown
 
 # maya-umbrella
 
 [![Python Version](https://img.shields.io/pypi/pyversions/maya-umbrella)](https://img.shields.io/pypi/pyversions/maya-umbrella)
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 [![PyPI Version](https://img.shields.io/pypi/v/maya-umbrella?color=green)](https://pypi.org/project/maya-umbrella/)
-[![Downloads Status](https://img.shields.io/pypi/dw/maya-umbrella)](https://pypi.org/project/maya-umbrella/)
-[![Downloads](https://pepy.tech/badge/maya-umbrella)](https://pepy.tech/project/maya-umbrella)
+[![Downloads](https://static.pepy.tech/badge/maya-umbrella)](https://pepy.tech/project/maya-umbrella)
+[![Downloads](https://static.pepy.tech/badge/maya-umbrella/month)](https://pepy.tech/project/maya-umbrella)
+[![Downloads](https://static.pepy.tech/badge/maya-umbrella/week)](https://pepy.tech/project/maya-umbrella)
 [![License](https://img.shields.io/pypi/l/maya-umbrella)](https://pypi.org/project/maya-umbrella/)
 [![PyPI Format](https://img.shields.io/pypi/format/maya-umbrella)](https://pypi.org/project/maya-umbrella/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/loonghao/maya-umbrella/graphs/commit-activity)
 [![maya-2024](https://img.shields.io/badge/maya-2024-green)](https://img.shields.io/badge/maya-2024-green)
 [![maya-2023](https://img.shields.io/badge/maya-2023-green)](https://img.shields.io/badge/maya-2023-green)
 [![maya-2022](https://img.shields.io/badge/maya-2022-green)](https://img.shields.io/badge/maya-2022-green)
 [![maya-2021](https://img.shields.io/badge/maya-2021-green)](https://img.shields.io/badge/maya-2021-green)
@@ -41,18 +42,24 @@
 [![maya-2019](https://img.shields.io/badge/maya-2019-green)](https://img.shields.io/badge/maya-2019-green)
 [![maya-2018](https://img.shields.io/badge/maya-2018-green)](https://img.shields.io/badge/maya-2018-green)
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
-Check and fix maya virus.
+This tool is designed to provide a robust solution for identifying and resolving any potential viruses within Autodesk Maya. 
+It ensures a secure and seamless user experience by proactively scanning for threats and effectively neutralizing them.
 
+It can be provided as an API for seamless integration into your existing pipeline.
 
-# 发开环境设置
+
+# 开发环境设置
+
+Set up the development environment using a virtual environment, 
+and it is recommended to use Python 3.8 or higher versions.
 
 通过虚拟环境去设置开发环境, 推荐python-3.8以上的版本
 
 ```shell
 pip install nox poetry
 ```
```

