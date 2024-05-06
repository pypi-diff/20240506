# Comparing `tmp/HdRezkaApi-7.0.0.tar.gz` & `tmp/HdRezkaApi-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HdRezkaApi-7.0.0.tar", last modified: Wed Feb  7 21:45:13 2024, max compression
+gzip compressed data, was "HdRezkaApi-7.0.1.tar", last modified: Mon May  6 16:16:09 2024, max compression
```

## Comparing `HdRezkaApi-7.0.0.tar` & `HdRezkaApi-7.0.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 21:45:13.404112 HdRezkaApi-7.0.0/
-drwxrwxrwx   0        0        0        0 2024-02-07 21:45:13.372743 HdRezkaApi-7.0.0/HdRezkaApi/
--rw-rw-rw-   0        0        0     9119 2024-02-07 21:29:02.000000 HdRezkaApi-7.0.0/HdRezkaApi/HdRezkaApi.py
-drwxrwxrwx   0        0        0        0 2024-02-07 21:45:13.404112 HdRezkaApi-7.0.0/HdRezkaApi/utils/
--rw-rw-rw-   0        0        0     2004 2024-02-07 21:17:28.000000 HdRezkaApi-7.0.0/HdRezkaApi/utils/stream.py
--rw-rw-rw-   0        0        0     1039 2023-08-31 12:26:52.000000 HdRezkaApi-7.0.0/HdRezkaApi/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-02-07 21:45:13.404112 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/
--rw-rw-rw-   0        0        0     4243 2024-02-07 21:45:13.000000 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-02-07 21:45:13.000000 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 21:45:13.000000 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-02-07 21:45:13.000000 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-07 21:45:13.000000 HdRezkaApi-7.0.0/HdRezkaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2024-02-07 21:45:12.000000 HdRezkaApi-7.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4243 2024-02-07 21:45:13.404112 HdRezkaApi-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3856 2024-02-07 21:37:55.000000 HdRezkaApi-7.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-07 21:45:13.404112 HdRezkaApi-7.0.0/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-02-07 21:45:12.000000 HdRezkaApi-7.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.069477 HdRezkaApi-7.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.012651 HdRezkaApi-7.0.1/HdRezkaApi/
+-rw-rw-rw-   0        0        0     9119 2024-02-07 21:31:39.000000 HdRezkaApi-7.0.1/HdRezkaApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.066971 HdRezkaApi-7.0.1/HdRezkaApi/utils/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.069477 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/
+-rw-rw-rw-   0        0        0     5034 2024-02-07 21:20:07.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/stream.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3806 2024-02-07 21:04:17.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/__pycache__/types.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2004 2024-02-07 21:17:28.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/stream.py
+-rw-rw-rw-   0        0        0     1039 2023-08-31 12:26:52.000000 HdRezkaApi-7.0.1/HdRezkaApi/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:16:09.046401 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/
+-rw-rw-rw-   0        0        0     4361 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 16:16:08.000000 HdRezkaApi-7.0.1/HdRezkaApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2024-05-06 16:16:07.000000 HdRezkaApi-7.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4361 2024-05-06 16:16:09.070803 HdRezkaApi-7.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3829 2024-05-06 16:14:47.000000 HdRezkaApi-7.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 16:16:09.071904 HdRezkaApi-7.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-05-06 16:16:07.000000 HdRezkaApi-7.0.1/setup.py
```

### Comparing `HdRezkaApi-7.0.0/HdRezkaApi/HdRezkaApi.py` & `HdRezkaApi-7.0.1/HdRezkaApi/__init__.py`

 * *Files identical despite different names*

### Comparing `HdRezkaApi-7.0.0/HdRezkaApi/utils/stream.py` & `HdRezkaApi-7.0.1/HdRezkaApi/utils/stream.py`

 * *Files identical despite different names*

### Comparing `HdRezkaApi-7.0.0/HdRezkaApi/utils/types.py` & `HdRezkaApi-7.0.1/HdRezkaApi/utils/types.py`

 * *Files identical despite different names*

### Comparing `HdRezkaApi-7.0.0/HdRezkaApi.egg-info/PKG-INFO` & `HdRezkaApi-7.0.1/HdRezkaApi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HdRezkaApi
-Version: 7.0.0
+Version: 7.0.1
 Home-page: https://github.com/SuperZombi/HdRezkaApi
 Author: Super_Zombi
 Author-email: super.zombi.yt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -144,7 +144,14 @@
 ```
 
 <br>
 
 # HdRezkaRating:
 #### `self.value` - rating value (`float`)
 #### `self.votes` - votes amount (`int`)
+
+<hr>
+
+### Proxy usage example:
+```python
+rezka = HdRezkaApi(url, proxy={'http': 'http://192.168.0.1:80'})
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.0 Home-page: https://
+Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.1 Home-page: https://
 github.com/SuperZombi/HdRezkaApi Author: Super_Zombi Author-email:
 super.zombi.yt@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown # HdRezkaApi [https://shields.io/badge/version-v7.0-blue]### Install:
 ``` pip install HdRezkaApi ``` ### Usage: ```python from HdRezkaApi import *
 url = "https://hdrezka.ag/ __YOUR_URL__ .html" rezka = HdRezkaApi(url) print
@@ -53,7 +53,10 @@
 rezka.getStream(1, 5) print( stream.subtitles.keys ) # ['en', 'ru'] print
 ( stream.subtitles.subtitles ) # { 'en': {'title': 'English', 'link': 'https:/
 '}, ... } print( stream.subtitles('en') ) # 'https:/' print( stream.subtitles
 ('English') ) # 'https:/' print( stream.subtitles(0) ) # 'https:/' # ^ index
 ```
 # HdRezkaRating: #### `self.value` - rating value (`float`) #### `self.votes` -
 votes amount (`int`)
+===============================================================================
+### Proxy usage example: ```python rezka = HdRezkaApi(url, proxy={'http':
+'http://192.168.0.1:80'}) ```
```

### Comparing `HdRezkaApi-7.0.0/PKG-INFO` & `HdRezkaApi-7.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HdRezkaApi
-Version: 7.0.0
+Version: 7.0.1
 Home-page: https://github.com/SuperZombi/HdRezkaApi
 Author: Super_Zombi
 Author-email: super.zombi.yt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -144,7 +144,14 @@
 ```
 
 <br>
 
 # HdRezkaRating:
 #### `self.value` - rating value (`float`)
 #### `self.votes` - votes amount (`int`)
+
+<hr>
+
+### Proxy usage example:
+```python
+rezka = HdRezkaApi(url, proxy={'http': 'http://192.168.0.1:80'})
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.0 Home-page: https://
+Metadata-Version: 2.1 Name: HdRezkaApi Version: 7.0.1 Home-page: https://
 github.com/SuperZombi/HdRezkaApi Author: Super_Zombi Author-email:
 super.zombi.yt@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown # HdRezkaApi [https://shields.io/badge/version-v7.0-blue]### Install:
 ``` pip install HdRezkaApi ``` ### Usage: ```python from HdRezkaApi import *
 url = "https://hdrezka.ag/ __YOUR_URL__ .html" rezka = HdRezkaApi(url) print
@@ -53,7 +53,10 @@
 rezka.getStream(1, 5) print( stream.subtitles.keys ) # ['en', 'ru'] print
 ( stream.subtitles.subtitles ) # { 'en': {'title': 'English', 'link': 'https:/
 '}, ... } print( stream.subtitles('en') ) # 'https:/' print( stream.subtitles
 ('English') ) # 'https:/' print( stream.subtitles(0) ) # 'https:/' # ^ index
 ```
 # HdRezkaRating: #### `self.value` - rating value (`float`) #### `self.votes` -
 votes amount (`int`)
+===============================================================================
+### Proxy usage example: ```python rezka = HdRezkaApi(url, proxy={'http':
+'http://192.168.0.1:80'}) ```
```

### Comparing `HdRezkaApi-7.0.0/README.md` & `HdRezkaApi-7.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,241 +1,240 @@
-00000000: 2320 4864 5265 7a6b 6141 7069 0d0a 0d0a  # HdRezkaApi....
-00000010: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000020: 2f2f 7368 6965 6c64 732e 696f 2f62 6164  //shields.io/bad
-00000030: 6765 2f76 6572 7369 6f6e 2d76 372e 302d  ge/version-v7.0-
-00000040: 626c 7565 223e 0d0a 0d0a 2323 2320 496e  blue">....### In
-00000050: 7374 616c 6c3a 0d0a 6060 600d 0a70 6970  stall:..```..pip
-00000060: 2069 6e73 7461 6c6c 2048 6452 657a 6b61   install HdRezka
-00000070: 4170 690d 0a60 6060 0d0a 0d0a 2323 2320  Api..```....### 
-00000080: 5573 6167 653a 0d0a 0d0a 6060 6070 7974  Usage:....```pyt
-00000090: 686f 6e0d 0a66 726f 6d20 4864 5265 7a6b  hon..from HdRezk
-000000a0: 6141 7069 2069 6d70 6f72 7420 2a0d 0a0d  aApi import *...
-000000b0: 0a75 726c 203d 2022 6874 7470 733a 2f2f  .url = "https://
-000000c0: 6864 7265 7a6b 612e 6167 2f20 2020 5f5f  hdrezka.ag/   __
-000000d0: 594f 5552 5f55 524c 5f5f 2020 202e 6874  YOUR_URL__   .ht
-000000e0: 6d6c 220d 0a0d 0a72 657a 6b61 203d 2048  ml"....rezka = H
-000000f0: 6452 657a 6b61 4170 6928 7572 6c29 0d0a  dRezkaApi(url)..
-00000100: 7072 696e 7428 7265 7a6b 612e 6e61 6d65  print(rezka.name
-00000110: 290d 0a70 7269 6e74 2872 657a 6b61 2e74  )..print(rezka.t
-00000120: 6875 6d62 6e61 696c 290d 0a70 7269 6e74  humbnail)..print
-00000130: 2820 7265 7a6b 612e 7261 7469 6e67 2e76  ( rezka.rating.v
-00000140: 616c 7565 2029 0d0a 7072 696e 7428 2072  alue )..print( r
-00000150: 657a 6b61 2e72 6174 696e 672e 766f 7465  ezka.rating.vote
-00000160: 7320 290d 0a70 7269 6e74 2820 7265 7a6b  s )..print( rezk
-00000170: 612e 7472 616e 736c 6174 6f72 7320 290d  a.translators ).
-00000180: 0a70 7269 6e74 2820 7265 7a6b 612e 6f74  .print( rezka.ot
-00000190: 6865 7250 6172 7473 2029 0d0a 7072 696e  herParts )..prin
-000001a0: 7428 2072 657a 6b61 2e73 6572 6965 7349  t( rezka.seriesI
-000001b0: 6e66 6f20 290d 0a0d 0a70 7269 6e74 2872  nfo )....print(r
-000001c0: 657a 6b61 2e74 7970 6529 0d0a 7072 696e  ezka.type)..prin
-000001d0: 7428 7265 7a6b 612e 7479 7065 203d 3d20  t(rezka.type == 
-000001e0: 4864 5265 7a6b 6154 5653 6572 6965 7320  HdRezkaTVSeries 
-000001f0: 3d3d 2048 6452 657a 6b61 5456 5365 7269  == HdRezkaTVSeri
-00000200: 6573 2829 203d 3d20 2274 765f 7365 7269  es() == "tv_seri
-00000210: 6573 2229 0d0a 0d0a 7072 696e 7428 2072  es")....print( r
-00000220: 657a 6b61 2e67 6574 5374 7265 616d 2829  ezka.getStream()
-00000230: 2827 3732 3070 2729 2029 2023 2069 6620  ('720p') ) # if 
-00000240: 6d6f 7669 650d 0a70 7269 6e74 2820 7265  movie..print( re
-00000250: 7a6b 612e 6765 7453 7472 6561 6d28 2731  zka.getStream('1
-00000260: 272c 2027 3127 2928 2737 3230 7027 2920  ', '1')('720p') 
-00000270: 290d 0a70 7269 6e74 2820 6469 6374 2872  )..print( dict(r
-00000280: 657a 6b61 2e67 6574 5365 6173 6f6e 5374  ezka.getSeasonSt
-00000290: 7265 616d 7328 2731 2729 2920 290d 0a60  reams('1')) )..`
-000002a0: 6060 0d0a 0d0a 2323 2323 2060 7365 6c66  ``....#### `self
-000002b0: 2e69 6460 202d 2046 696c 6d20 6964 2028  .id` - Film id (
-000002c0: 6070 6f73 745f 6964 6029 0d0a 2323 2323  `post_id`)..####
-000002d0: 2060 7365 6c66 2e6e 616d 6560 202d 2046   `self.name` - F
-000002e0: 696c 6d20 6e61 6d65 2028 6070 6f73 745f  ilm name (`post_
-000002f0: 5f74 6974 6c65 6029 0d0a 2323 2323 2060  _title`)..#### `
-00000300: 7365 6c66 2e74 7970 6560 202d 2060 4864  self.type` - `Hd
-00000310: 5265 7a6b 6154 5653 6572 6965 7360 206f  RezkaTVSeries` o
-00000320: 7220 6048 6452 657a 6b61 4d6f 7669 6560  r `HdRezkaMovie`
-00000330: 0d0a 2323 2323 2060 7365 6c66 2e74 6875  ..#### `self.thu
-00000340: 6d62 6e61 696c 6020 2d20 4669 6c6d 2074  mbnail` - Film t
-00000350: 6875 6d62 6e61 696c 2075 726c 0d0a 2323  humbnail url..##
-00000360: 2323 2060 7365 6c66 2e72 6174 696e 6760  ## `self.rating`
-00000370: 202d 2046 696c 6d20 7261 7469 6e67 2028   - Film rating (
-00000380: 3c61 2068 7265 663d 2223 6864 7265 7a6b  <a href="#hdrezk
-00000390: 6172 6174 696e 6722 3e48 6472 657a 6b61  arating">Hdrezka
-000003a0: 2052 6174 696e 673c 2f61 3e29 0d0a 2323   Rating</a>)..##
-000003b0: 2323 2060 7365 6c66 2e74 7261 6e73 6c61  ## `self.transla
-000003c0: 746f 7273 6020 2d20 5472 616e 736c 6174  tors` - Translat
-000003d0: 6f72 7320 6172 7261 790d 0a23 2323 2320  ors array..#### 
-000003e0: 6073 656c 662e 7365 7269 6573 496e 666f  `self.seriesInfo
-000003f0: 6020 2d20 5365 6173 6f6e 7320 616e 6420  ` - Seasons and 
-00000400: 4570 6973 6f64 6573 2061 7272 6179 0d0a  Episodes array..
-00000410: 2323 2323 2060 7365 6c66 2e6f 7468 6572  #### `self.other
-00000420: 5061 7274 7360 202d 204f 7468 6572 2070  Parts` - Other p
-00000430: 6172 7473 206f 6620 7468 6973 2066 696c  arts of this fil
-00000440: 6d0d 0a0d 0a3c 6872 3e0d 0a0d 0a23 2323  m....<hr>....###
-00000450: 2067 6574 5374 7265 616d 2860 7365 6173   getStream(`seas
-00000460: 6f6e 602c 2060 6570 6973 6f64 6560 2c20  on`, `episode`, 
-00000470: 6074 7261 6e73 6c61 7469 6f6e 3d4e 6f6e  `translation=Non
-00000480: 6560 2c20 6069 6e64 6578 3d30 6029 0d0a  e`, `index=0`)..
-00000490: 6060 600d 0a67 6574 5374 7265 616d 280d  ```..getStream(.
-000004a0: 0a20 2020 2074 7261 6e73 6c61 7469 6f6e  .    translation
-000004b0: 3d27 d094 d183 d0b1 d0bb d18f d0b6 2720  ='............' 
-000004c0: 6f72 2074 7261 6e73 6c61 7469 6f6e 3d27  or translation='
-000004d0: 3536 2720 6f72 2069 6e64 6578 3d30 0d0a  56' or index=0..
-000004e0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 5e20 7468 6973 2069 7320 696e 6465 7820  ^ this is index 
-00000520: 696e 2074 7261 6e73 6c61 746f 7273 2061  in translators a
-00000530: 7272 6179 0d0a 6060 600d 0a49 6620 7479  rray..```..If ty
-00000540: 7065 203d 3d20 6d6f 7669 6520 7468 656e  pe == movie then
-00000550: 2074 6865 7265 2069 7320 6e6f 206e 6565   there is no nee
-00000560: 6420 746f 2073 7065 6369 6679 2073 6561  d to specify sea
-00000570: 736f 6e20 616e 6420 6570 6973 6f64 652e  son and episode.
-00000580: 0d0a 6060 6070 7974 686f 6e0d 0a73 7472  ..```python..str
-00000590: 6561 6d20 3d20 7265 7a6b 612e 6765 7453  eam = rezka.getS
-000005a0: 7472 6561 6d28 2920 2320 6966 206d 6f76  tream() # if mov
-000005b0: 6965 0d0a 6060 600d 0a3c 6872 3e0d 0a0d  ie..```..<hr>...
-000005c0: 0a23 2323 2067 6574 5365 6173 6f6e 5374  .### getSeasonSt
-000005d0: 7265 616d 7328 6073 6561 736f 6e60 2c20  reams(`season`, 
-000005e0: 6074 7261 6e73 6c61 7469 6f6e 3d4e 6f6e  `translation=Non
-000005f0: 6560 2c20 6069 6e64 6578 3d30 602c 2060  e`, `index=0`, `
-00000600: 6967 6e6f 7265 3d46 616c 7365 602c 2060  ignore=False`, `
-00000610: 7072 6f67 7265 7373 3d4e 6f6e 6560 290d  progress=None`).
-00000620: 0a60 6060 0d0a 6765 7453 6561 736f 6e53  .```..getSeasonS
-00000630: 7472 6561 6d73 280d 0a20 2020 2074 7261  treams(..    tra
-00000640: 6e73 6c61 7469 6f6e 3d27 d094 d183 d0b1  nslation='......
-00000650: d0bb d18f d0b6 2720 6f72 2074 7261 6e73  ......' or trans
-00000660: 6c61 7469 6f6e 3d27 3536 2720 6f72 2069  lation='56' or i
-00000670: 6e64 6578 3d30 0d0a 2920 2020 2020 2020  ndex=0..)       
-00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2020 5e20 7468 6973 2069          ^ this i
-000006b0: 7320 696e 6465 7820 696e 2074 7261 6e73  s index in trans
-000006c0: 6c61 746f 7273 2061 7272 6179 0d0a 6060  lators array..``
-000006d0: 600d 0a0d 0a23 2323 2320 6069 676e 6f72  `....#### `ignor
-000006e0: 6560 202d 2069 676e 6f72 6520 6572 726f  e` - ignore erro
-000006f0: 7273 0d0a 2323 2323 2060 7072 6f67 7265  rs..#### `progre
-00000700: 7373 6020 2d20 6361 6c6c 6261 636b 2066  ss` - callback f
-00000710: 756e 6374 696f 6e0d 0a0d 0a60 6060 7079  unction....```py
-00000720: 7468 6f6e 0d0a 6465 6620 7072 6f67 7265  thon..def progre
-00000730: 7373 2863 7572 7265 6e74 2c20 616c 6c29  ss(current, all)
-00000740: 3a0d 0a20 2020 2070 6572 6365 6e74 203d  :..    percent =
-00000750: 2072 6f75 6e64 2863 7572 7265 6e74 202a   round(current *
-00000760: 2031 3030 202f 2061 6c6c 290d 0a20 2020   100 / all)..   
-00000770: 2070 7269 6e74 2866 227b 7065 7263 656e   print(f"{percen
-00000780: 747d 253a 207b 6375 7272 656e 747d 2f7b  t}%: {current}/{
-00000790: 616c 6c7d 222c 2065 6e64 3d22 5c72 2229  all}", end="\r")
-000007a0: 0d0a 0d0a 7072 696e 7428 2064 6963 7428  ....print( dict(
-000007b0: 7265 7a6b 612e 6765 7453 6561 736f 6e53  rezka.getSeasonS
-000007c0: 7472 6561 6d73 2831 2c20 6967 6e6f 7265  treams(1, ignore
-000007d0: 3d54 7275 652c 2070 726f 6772 6573 733d  =True, progress=
-000007e0: 7072 6f67 7265 7373 2929 2029 0d0a 6060  progress)) )..``
-000007f0: 600d 0a0d 0a4f 7574 7075 7420 6578 616d  `....Output exam
-00000800: 706c 653a 0d0a 6060 600d 0a7b 2731 273a  ple:..```..{'1':
-00000810: 203c 4864 5265 7a6b 6153 7472 6561 6d28   <HdRezkaStream(
-00000820: 7365 6173 6f6e 3a31 2c20 6570 6973 6f64  season:1, episod
-00000830: 653a 3129 3e2c 2027 3227 3a20 3c48 6452  e:1)>, '2': <HdR
-00000840: 657a 6b61 5374 7265 616d 2873 6561 736f  ezkaStream(seaso
-00000850: 6e3a 312c 2065 7069 736f 6465 3a32 293e  n:1, episode:2)>
-00000860: 2c20 2e2e 2e7d 0d0a 6060 600d 0a0d 0a49  , ...}..```....I
-00000870: 6620 616e 2065 7272 6f72 206f 6363 7572  f an error occur
-00000880: 732c 2061 6e20 6174 7465 6d70 7420 7769  s, an attempt wi
-00000890: 6c6c 2062 6520 6d61 6465 2074 6f20 7265  ll be made to re
-000008a0: 7065 6174 2074 6865 2072 6571 7565 7374  peat the request
-000008b0: 2061 6761 696e 2e3c 6272 3e0d 0a42 7574   again.<br>..But
-000008c0: 2069 6620 7468 6520 6572 726f 7220 6f63   if the error oc
-000008d0: 6375 7273 2061 6761 696e 2c20 7468 656e  curs again, then
-000008e0: 2060 4e6f 6e65 6020 7769 6c6c 2062 6520   `None` will be 
-000008f0: 6164 6465 6420 746f 2074 6865 2066 696e  added to the fin
-00000900: 616c 2064 6963 742e 3c62 723e 0d0a 546f  al dict.<br>..To
-00000910: 2069 676e 6f72 6520 6572 726f 7273 2061   ignore errors a
-00000920: 6e64 2072 6574 7279 2072 6571 7565 7374  nd retry request
-00000930: 7320 756e 7469 6c20 6120 7265 7370 6f6e  s until a respon
-00000940: 7365 2069 7320 7265 6365 6976 6564 2c20  se is received, 
-00000950: 7370 6563 6966 7920 7468 6520 6069 676e  specify the `ign
-00000960: 6f72 653d 5472 7565 6020 6f70 7469 6f6e  ore=True` option
-00000970: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-00000980: 666f 7220 692c 2073 7472 6561 6d20 696e  for i, stream in
-00000990: 2072 657a 6b61 2e67 6574 5365 6173 6f6e   rezka.getSeason
-000009a0: 5374 7265 616d 7328 2731 2729 3a0d 0a20  Streams('1'):.. 
-000009b0: 2020 2070 7269 6e74 2873 7472 6561 6d29     print(stream)
-000009c0: 0d0a 6060 600d 0a0d 0a3c 6872 3e0d 0a3c  ..```....<hr>..<
-000009d0: 6272 3e0d 0a0d 0a23 2048 6452 657a 6b61  br>....# HdRezka
-000009e0: 5374 7265 616d 3a0d 0a23 2323 2320 6073  Stream:..#### `s
-000009f0: 656c 662e 7669 6465 6f73 6020 2d20 6469  elf.videos` - di
-00000a00: 6374 206f 6620 7669 6465 6f73 2c20 7768  ct of videos, wh
-00000a10: 6572 6520 6b65 7920 6973 2072 6573 6f6c  ere key is resol
-00000a20: 7574 696f 6e20 616e 6420 7661 6c75 6520  ution and value 
-00000a30: 6973 2075 726c 0d0a 2323 2323 2060 7365  is url..#### `se
-00000a40: 6c66 2e6e 616d 6560 0d0a 2323 2323 2060  lf.name`..#### `
-00000a50: 7365 6c66 2e74 7261 6e73 6c61 746f 725f  self.translator_
-00000a60: 6964 600d 0a23 2323 2320 6073 656c 662e  id`..#### `self.
-00000a70: 7365 6173 6f6e 6020 2d20 2860 4e6f 6e65  season` - (`None
-00000a80: 6020 6966 2066 696c 6d29 0d0a 2323 2323  ` if film)..####
-00000a90: 2060 7365 6c66 2e65 7069 736f 6465 6020   `self.episode` 
-00000aa0: 2d20 2860 4e6f 6e65 6020 6966 2066 696c  - (`None` if fil
-00000ab0: 6d29 0d0a 2323 2323 2060 7365 6c66 2e73  m)..#### `self.s
-00000ac0: 7562 7469 746c 6573 6020 2d20 3c61 2068  ubtitles` - <a h
-00000ad0: 7265 663d 2223 6864 7265 7a6b 6173 7472  ref="#hdrezkastr
-00000ae0: 6561 6d73 7562 7469 746c 6573 2220 3e48  eamsubtitles" >H
-00000af0: 6452 657a 6b61 5374 7265 616d 5375 6274  dRezkaStreamSubt
-00000b00: 6974 6c65 733c 2f61 3e0d 0a23 2323 2320  itles</a>..#### 
-00000b10: 6048 6452 657a 6b61 5374 7265 616d 2872  `HdRezkaStream(r
-00000b20: 6573 6f6c 7574 696e 2960 202d 2063 616c  esolutin)` - cal
-00000b30: 6c20 6f62 6a65 6374 2077 6974 6820 6172  l object with ar
-00000b40: 6775 6d65 6e74 2074 6f20 6765 7420 7572  gument to get ur
-00000b50: 6c20 6f66 2076 6964 656f 0d0a 0d0a 2323  l of video....##
-00000b60: 2320 5573 6167 6520 6578 616d 706c 6573  # Usage examples
-00000b70: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
-00000b80: 7374 7265 616d 203d 2072 657a 6b61 2e67  stream = rezka.g
-00000b90: 6574 5374 7265 616d 2831 2c20 3529 0d0a  etStream(1, 5)..
-00000ba0: 0d0a 7072 696e 7428 2073 7472 6561 6d28  ..print( stream(
-00000bb0: 2737 3230 7027 2920 290d 0a70 7269 6e74  '720p') )..print
-00000bc0: 2820 7374 7265 616d 2827 3732 3027 2920  ( stream('720') 
-00000bd0: 290d 0a70 7269 6e74 2820 7374 7265 616d  )..print( stream
-00000be0: 2831 3038 3029 2029 0d0a 7072 696e 7428  (1080) )..print(
-00000bf0: 2073 7472 6561 6d28 2755 6c74 7261 2729   stream('Ultra')
-00000c00: 2029 0d0a 7072 696e 7428 2073 7472 6561   )..print( strea
-00000c10: 6d28 2731 3038 3070 2055 6c74 7261 2729  m('1080p Ultra')
-00000c20: 2029 0d0a 7072 696e 7428 2073 7472 6561   )..print( strea
-00000c30: 6d2e 7669 6465 6f73 2029 0d0a 6060 600d  m.videos )..```.
-00000c40: 0a0d 0a3c 6272 3e0d 0a0d 0a23 2048 6452  ...<br>....# HdR
-00000c50: 657a 6b61 5374 7265 616d 5375 6274 6974  ezkaStreamSubtit
-00000c60: 6c65 733a 0d0a 2323 2323 2060 7365 6c66  les:..#### `self
-00000c70: 2e73 7562 7469 746c 6573 6020 2d20 6469  .subtitles` - di
-00000c80: 6374 206f 6620 7375 6274 6974 6c65 730d  ct of subtitles.
-00000c90: 0a23 2323 2320 6073 656c 662e 6b65 7973  .#### `self.keys
-00000ca0: 6020 2d20 6c69 7374 206f 6620 7375 6274  ` - list of subt
-00000cb0: 6974 6c65 7320 636f 6465 730d 0a23 2323  itles codes..###
-00000cc0: 2320 6073 656c 6628 6964 2960 202d 2063  # `self(id)` - c
-00000cd0: 616c 6c20 6f62 6a65 6374 2077 6974 6820  all object with 
-00000ce0: 6172 6775 6d65 6e74 2074 6f20 6765 7420  argument to get 
-00000cf0: 7572 6c20 6f66 2073 7562 7469 746c 6573  url of subtitles
-00000d00: 0d0a 0d0a 2323 2320 5573 6167 6520 6578  ....### Usage ex
-00000d10: 616d 706c 6573 3a0d 0a0d 0a60 6060 7079  amples:....```py
-00000d20: 7468 6f6e 0d0a 7374 7265 616d 203d 2072  thon..stream = r
-00000d30: 657a 6b61 2e67 6574 5374 7265 616d 2831  ezka.getStream(1
-00000d40: 2c20 3529 0d0a 0d0a 7072 696e 7428 2073  , 5)....print( s
-00000d50: 7472 6561 6d2e 7375 6274 6974 6c65 732e  tream.subtitles.
-00000d60: 6b65 7973 2029 2020 2020 2020 2020 2320  keys )        # 
-00000d70: 5b27 656e 272c 2027 7275 275d 0d0a 7072  ['en', 'ru']..pr
-00000d80: 696e 7428 2073 7472 6561 6d2e 7375 6274  int( stream.subt
-00000d90: 6974 6c65 732e 7375 6274 6974 6c65 7320  itles.subtitles 
-00000da0: 2920 2020 2320 7b20 2765 6e27 3a20 7b27  )   # { 'en': {'
-00000db0: 7469 746c 6527 3a20 2745 6e67 6c69 7368  title': 'English
-00000dc0: 272c 2027 6c69 6e6b 273a 2027 6874 7470  ', 'link': 'http
-00000dd0: 733a 2f27 7d2c 202e 2e2e 2020 7d0d 0a70  s:/'}, ...  }..p
-00000de0: 7269 6e74 2820 7374 7265 616d 2e73 7562  rint( stream.sub
-00000df0: 7469 746c 6573 2827 656e 2729 2029 2020  titles('en') )  
-00000e00: 2020 2020 2023 2027 6874 7470 733a 2f27       # 'https:/'
-00000e10: 0d0a 7072 696e 7428 2073 7472 6561 6d2e  ..print( stream.
-00000e20: 7375 6274 6974 6c65 7328 2745 6e67 6c69  subtitles('Engli
-00000e30: 7368 2729 2029 2020 2320 2768 7474 7073  sh') )  # 'https
-00000e40: 3a2f 270d 0a70 7269 6e74 2820 7374 7265  :/'..print( stre
-00000e50: 616d 2e73 7562 7469 746c 6573 2830 2920  am.subtitles(0) 
-00000e60: 2920 2020 2020 2020 2020 2023 2027 6874  )          # 'ht
-00000e70: 7470 733a 2f27 0d0a 2320 2020 2020 2020  tps:/'..#       
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 5e20 696e 6465 780d 0a60 6060 0d0a 0d0a  ^ index..```....
-00000ea0: 3c62 723e 0d0a 0d0a 2320 4864 5265 7a6b  <br>....# HdRezk
-00000eb0: 6152 6174 696e 673a 0d0a 2323 2323 2060  aRating:..#### `
-00000ec0: 7365 6c66 2e76 616c 7565 6020 2d20 7261  self.value` - ra
-00000ed0: 7469 6e67 2076 616c 7565 2028 6066 6c6f  ting value (`flo
-00000ee0: 6174 6029 0d0a 2323 2323 2060 7365 6c66  at`)..#### `self
-00000ef0: 2e76 6f74 6573 6020 2d20 766f 7465 7320  .votes` - votes 
-00000f00: 616d 6f75 6e74 2028 6069 6e74 6029 0d0a  amount (`int`)..
+00000000: 2320 4864 5265 7a6b 6141 7069 0a0a 3c69  # HdRezkaApi..<i
+00000010: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000020: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000030: 2f76 6572 7369 6f6e 2d76 372e 302d 626c  /version-v7.0-bl
+00000040: 7565 223e 0a0a 2323 2320 496e 7374 616c  ue">..### Instal
+00000050: 6c3a 0a60 6060 0a70 6970 2069 6e73 7461  l:.```.pip insta
+00000060: 6c6c 2048 6452 657a 6b61 4170 690a 6060  ll HdRezkaApi.``
+00000070: 600a 0a23 2323 2055 7361 6765 3a0a 0a60  `..### Usage:..`
+00000080: 6060 7079 7468 6f6e 0a66 726f 6d20 4864  ``python.from Hd
+00000090: 5265 7a6b 6141 7069 2069 6d70 6f72 7420  RezkaApi import 
+000000a0: 2a0a 0a75 726c 203d 2022 6874 7470 733a  *..url = "https:
+000000b0: 2f2f 6864 7265 7a6b 612e 6167 2f20 2020  //hdrezka.ag/   
+000000c0: 5f5f 594f 5552 5f55 524c 5f5f 2020 202e  __YOUR_URL__   .
+000000d0: 6874 6d6c 220a 0a72 657a 6b61 203d 2048  html"..rezka = H
+000000e0: 6452 657a 6b61 4170 6928 7572 6c29 0a70  dRezkaApi(url).p
+000000f0: 7269 6e74 2872 657a 6b61 2e6e 616d 6529  rint(rezka.name)
+00000100: 0a70 7269 6e74 2872 657a 6b61 2e74 6875  .print(rezka.thu
+00000110: 6d62 6e61 696c 290a 7072 696e 7428 2072  mbnail).print( r
+00000120: 657a 6b61 2e72 6174 696e 672e 7661 6c75  ezka.rating.valu
+00000130: 6520 290a 7072 696e 7428 2072 657a 6b61  e ).print( rezka
+00000140: 2e72 6174 696e 672e 766f 7465 7320 290a  .rating.votes ).
+00000150: 7072 696e 7428 2072 657a 6b61 2e74 7261  print( rezka.tra
+00000160: 6e73 6c61 746f 7273 2029 0a70 7269 6e74  nslators ).print
+00000170: 2820 7265 7a6b 612e 6f74 6865 7250 6172  ( rezka.otherPar
+00000180: 7473 2029 0a70 7269 6e74 2820 7265 7a6b  ts ).print( rezk
+00000190: 612e 7365 7269 6573 496e 666f 2029 0a0a  a.seriesInfo )..
+000001a0: 7072 696e 7428 7265 7a6b 612e 7479 7065  print(rezka.type
+000001b0: 290a 7072 696e 7428 7265 7a6b 612e 7479  ).print(rezka.ty
+000001c0: 7065 203d 3d20 4864 5265 7a6b 6154 5653  pe == HdRezkaTVS
+000001d0: 6572 6965 7320 3d3d 2048 6452 657a 6b61  eries == HdRezka
+000001e0: 5456 5365 7269 6573 2829 203d 3d20 2274  TVSeries() == "t
+000001f0: 765f 7365 7269 6573 2229 0a0a 7072 696e  v_series")..prin
+00000200: 7428 2072 657a 6b61 2e67 6574 5374 7265  t( rezka.getStre
+00000210: 616d 2829 2827 3732 3070 2729 2029 2023  am()('720p') ) #
+00000220: 2069 6620 6d6f 7669 650a 7072 696e 7428   if movie.print(
+00000230: 2072 657a 6b61 2e67 6574 5374 7265 616d   rezka.getStream
+00000240: 2827 3127 2c20 2731 2729 2827 3732 3070  ('1', '1')('720p
+00000250: 2729 2029 0a70 7269 6e74 2820 6469 6374  ') ).print( dict
+00000260: 2872 657a 6b61 2e67 6574 5365 6173 6f6e  (rezka.getSeason
+00000270: 5374 7265 616d 7328 2731 2729 2920 290a  Streams('1')) ).
+00000280: 6060 600a 0a23 2323 2320 6073 656c 662e  ```..#### `self.
+00000290: 6964 6020 2d20 4669 6c6d 2069 6420 2860  id` - Film id (`
+000002a0: 706f 7374 5f69 6460 290a 2323 2323 2060  post_id`).#### `
+000002b0: 7365 6c66 2e6e 616d 6560 202d 2046 696c  self.name` - Fil
+000002c0: 6d20 6e61 6d65 2028 6070 6f73 745f 5f74  m name (`post__t
+000002d0: 6974 6c65 6029 0a23 2323 2320 6073 656c  itle`).#### `sel
+000002e0: 662e 7479 7065 6020 2d20 6048 6452 657a  f.type` - `HdRez
+000002f0: 6b61 5456 5365 7269 6573 6020 6f72 2060  kaTVSeries` or `
+00000300: 4864 5265 7a6b 614d 6f76 6965 600a 2323  HdRezkaMovie`.##
+00000310: 2323 2060 7365 6c66 2e74 6875 6d62 6e61  ## `self.thumbna
+00000320: 696c 6020 2d20 4669 6c6d 2074 6875 6d62  il` - Film thumb
+00000330: 6e61 696c 2075 726c 0a23 2323 2320 6073  nail url.#### `s
+00000340: 656c 662e 7261 7469 6e67 6020 2d20 4669  elf.rating` - Fi
+00000350: 6c6d 2072 6174 696e 6720 283c 6120 6872  lm rating (<a hr
+00000360: 6566 3d22 2368 6472 657a 6b61 7261 7469  ef="#hdrezkarati
+00000370: 6e67 223e 4864 7265 7a6b 6120 5261 7469  ng">Hdrezka Rati
+00000380: 6e67 3c2f 613e 290a 2323 2323 2060 7365  ng</a>).#### `se
+00000390: 6c66 2e74 7261 6e73 6c61 746f 7273 6020  lf.translators` 
+000003a0: 2d20 5472 616e 736c 6174 6f72 7320 6172  - Translators ar
+000003b0: 7261 790a 2323 2323 2060 7365 6c66 2e73  ray.#### `self.s
+000003c0: 6572 6965 7349 6e66 6f60 202d 2053 6561  eriesInfo` - Sea
+000003d0: 736f 6e73 2061 6e64 2045 7069 736f 6465  sons and Episode
+000003e0: 7320 6172 7261 790a 2323 2323 2060 7365  s array.#### `se
+000003f0: 6c66 2e6f 7468 6572 5061 7274 7360 202d  lf.otherParts` -
+00000400: 204f 7468 6572 2070 6172 7473 206f 6620   Other parts of 
+00000410: 7468 6973 2066 696c 6d0a 0a3c 6872 3e0a  this film..<hr>.
+00000420: 0a23 2323 2067 6574 5374 7265 616d 2860  .### getStream(`
+00000430: 7365 6173 6f6e 602c 2060 6570 6973 6f64  season`, `episod
+00000440: 6560 2c20 6074 7261 6e73 6c61 7469 6f6e  e`, `translation
+00000450: 3d4e 6f6e 6560 2c20 6069 6e64 6578 3d30  =None`, `index=0
+00000460: 6029 0a60 6060 0a67 6574 5374 7265 616d  `).```.getStream
+00000470: 280a 2020 2020 7472 616e 736c 6174 696f  (.    translatio
+00000480: 6e3d 27d0 94d1 83d0 b1d0 bbd1 8fd0 b627  n='............'
+00000490: 206f 7220 7472 616e 736c 6174 696f 6e3d   or translation=
+000004a0: 2735 3627 206f 7220 696e 6465 783d 300a  '56' or index=0.
+000004b0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000004c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 5e20 7468 6973 2069 7320 696e 6465 7820  ^ this is index 
+000004f0: 696e 2074 7261 6e73 6c61 746f 7273 2061  in translators a
+00000500: 7272 6179 0a60 6060 0a49 6620 7479 7065  rray.```.If type
+00000510: 203d 3d20 6d6f 7669 6520 7468 656e 2074   == movie then t
+00000520: 6865 7265 2069 7320 6e6f 206e 6565 6420  here is no need 
+00000530: 746f 2073 7065 6369 6679 2073 6561 736f  to specify seaso
+00000540: 6e20 616e 6420 6570 6973 6f64 652e 0a60  n and episode..`
+00000550: 6060 7079 7468 6f6e 0a73 7472 6561 6d20  ``python.stream 
+00000560: 3d20 7265 7a6b 612e 6765 7453 7472 6561  = rezka.getStrea
+00000570: 6d28 2920 2320 6966 206d 6f76 6965 0a60  m() # if movie.`
+00000580: 6060 0a3c 6872 3e0a 0a23 2323 2067 6574  ``.<hr>..### get
+00000590: 5365 6173 6f6e 5374 7265 616d 7328 6073  SeasonStreams(`s
+000005a0: 6561 736f 6e60 2c20 6074 7261 6e73 6c61  eason`, `transla
+000005b0: 7469 6f6e 3d4e 6f6e 6560 2c20 6069 6e64  tion=None`, `ind
+000005c0: 6578 3d30 602c 2060 6967 6e6f 7265 3d46  ex=0`, `ignore=F
+000005d0: 616c 7365 602c 2060 7072 6f67 7265 7373  alse`, `progress
+000005e0: 3d4e 6f6e 6560 290a 6060 600a 6765 7453  =None`).```.getS
+000005f0: 6561 736f 6e53 7472 6561 6d73 280a 2020  easonStreams(.  
+00000600: 2020 7472 616e 736c 6174 696f 6e3d 27d0    translation='.
+00000610: 94d1 83d0 b1d0 bbd1 8fd0 b627 206f 7220  ...........' or 
+00000620: 7472 616e 736c 6174 696f 6e3d 2735 3627  translation='56'
+00000630: 206f 7220 696e 6465 783d 300a 2920 2020   or index=0.)   
+00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2020 2020 2020 5e20 7468              ^ th
+00000670: 6973 2069 7320 696e 6465 7820 696e 2074  is is index in t
+00000680: 7261 6e73 6c61 746f 7273 2061 7272 6179  ranslators array
+00000690: 0a60 6060 0a0a 2323 2323 2060 6967 6e6f  .```..#### `igno
+000006a0: 7265 6020 2d20 6967 6e6f 7265 2065 7272  re` - ignore err
+000006b0: 6f72 730a 2323 2323 2060 7072 6f67 7265  ors.#### `progre
+000006c0: 7373 6020 2d20 6361 6c6c 6261 636b 2066  ss` - callback f
+000006d0: 756e 6374 696f 6e0a 0a60 6060 7079 7468  unction..```pyth
+000006e0: 6f6e 0a64 6566 2070 726f 6772 6573 7328  on.def progress(
+000006f0: 6375 7272 656e 742c 2061 6c6c 293a 0a20  current, all):. 
+00000700: 2020 2070 6572 6365 6e74 203d 2072 6f75     percent = rou
+00000710: 6e64 2863 7572 7265 6e74 202a 2031 3030  nd(current * 100
+00000720: 202f 2061 6c6c 290a 2020 2020 7072 696e   / all).    prin
+00000730: 7428 6622 7b70 6572 6365 6e74 7d25 3a20  t(f"{percent}%: 
+00000740: 7b63 7572 7265 6e74 7d2f 7b61 6c6c 7d22  {current}/{all}"
+00000750: 2c20 656e 643d 225c 7222 290a 0a70 7269  , end="\r")..pri
+00000760: 6e74 2820 6469 6374 2872 657a 6b61 2e67  nt( dict(rezka.g
+00000770: 6574 5365 6173 6f6e 5374 7265 616d 7328  etSeasonStreams(
+00000780: 312c 2069 676e 6f72 653d 5472 7565 2c20  1, ignore=True, 
+00000790: 7072 6f67 7265 7373 3d70 726f 6772 6573  progress=progres
+000007a0: 7329 2920 290a 6060 600a 0a4f 7574 7075  s)) ).```..Outpu
+000007b0: 7420 6578 616d 706c 653a 0a60 6060 0a7b  t example:.```.{
+000007c0: 2731 273a 203c 4864 5265 7a6b 6153 7472  '1': <HdRezkaStr
+000007d0: 6561 6d28 7365 6173 6f6e 3a31 2c20 6570  eam(season:1, ep
+000007e0: 6973 6f64 653a 3129 3e2c 2027 3227 3a20  isode:1)>, '2': 
+000007f0: 3c48 6452 657a 6b61 5374 7265 616d 2873  <HdRezkaStream(s
+00000800: 6561 736f 6e3a 312c 2065 7069 736f 6465  eason:1, episode
+00000810: 3a32 293e 2c20 2e2e 2e7d 0a60 6060 0a0a  :2)>, ...}.```..
+00000820: 4966 2061 6e20 6572 726f 7220 6f63 6375  If an error occu
+00000830: 7273 2c20 616e 2061 7474 656d 7074 2077  rs, an attempt w
+00000840: 696c 6c20 6265 206d 6164 6520 746f 2072  ill be made to r
+00000850: 6570 6561 7420 7468 6520 7265 7175 6573  epeat the reques
+00000860: 7420 6167 6169 6e2e 3c62 723e 0a42 7574  t again.<br>.But
+00000870: 2069 6620 7468 6520 6572 726f 7220 6f63   if the error oc
+00000880: 6375 7273 2061 6761 696e 2c20 7468 656e  curs again, then
+00000890: 2060 4e6f 6e65 6020 7769 6c6c 2062 6520   `None` will be 
+000008a0: 6164 6465 6420 746f 2074 6865 2066 696e  added to the fin
+000008b0: 616c 2064 6963 742e 3c62 723e 0a54 6f20  al dict.<br>.To 
+000008c0: 6967 6e6f 7265 2065 7272 6f72 7320 616e  ignore errors an
+000008d0: 6420 7265 7472 7920 7265 7175 6573 7473  d retry requests
+000008e0: 2075 6e74 696c 2061 2072 6573 706f 6e73   until a respons
+000008f0: 6520 6973 2072 6563 6569 7665 642c 2073  e is received, s
+00000900: 7065 6369 6679 2074 6865 2060 6967 6e6f  pecify the `igno
+00000910: 7265 3d54 7275 6560 206f 7074 696f 6e2e  re=True` option.
+00000920: 0a0a 6060 6070 7974 686f 6e0a 666f 7220  ..```python.for 
+00000930: 692c 2073 7472 6561 6d20 696e 2072 657a  i, stream in rez
+00000940: 6b61 2e67 6574 5365 6173 6f6e 5374 7265  ka.getSeasonStre
+00000950: 616d 7328 2731 2729 3a0a 2020 2020 7072  ams('1'):.    pr
+00000960: 696e 7428 7374 7265 616d 290a 6060 600a  int(stream).```.
+00000970: 0a3c 6872 3e0a 3c62 723e 0a0a 2320 4864  .<hr>.<br>..# Hd
+00000980: 5265 7a6b 6153 7472 6561 6d3a 0a23 2323  RezkaStream:.###
+00000990: 2320 6073 656c 662e 7669 6465 6f73 6020  # `self.videos` 
+000009a0: 2d20 6469 6374 206f 6620 7669 6465 6f73  - dict of videos
+000009b0: 2c20 7768 6572 6520 6b65 7920 6973 2072  , where key is r
+000009c0: 6573 6f6c 7574 696f 6e20 616e 6420 7661  esolution and va
+000009d0: 6c75 6520 6973 2075 726c 0a23 2323 2320  lue is url.#### 
+000009e0: 6073 656c 662e 6e61 6d65 600a 2323 2323  `self.name`.####
+000009f0: 2060 7365 6c66 2e74 7261 6e73 6c61 746f   `self.translato
+00000a00: 725f 6964 600a 2323 2323 2060 7365 6c66  r_id`.#### `self
+00000a10: 2e73 6561 736f 6e60 202d 2028 604e 6f6e  .season` - (`Non
+00000a20: 6560 2069 6620 6669 6c6d 290a 2323 2323  e` if film).####
+00000a30: 2060 7365 6c66 2e65 7069 736f 6465 6020   `self.episode` 
+00000a40: 2d20 2860 4e6f 6e65 6020 6966 2066 696c  - (`None` if fil
+00000a50: 6d29 0a23 2323 2320 6073 656c 662e 7375  m).#### `self.su
+00000a60: 6274 6974 6c65 7360 202d 203c 6120 6872  btitles` - <a hr
+00000a70: 6566 3d22 2368 6472 657a 6b61 7374 7265  ef="#hdrezkastre
+00000a80: 616d 7375 6274 6974 6c65 7322 203e 4864  amsubtitles" >Hd
+00000a90: 5265 7a6b 6153 7472 6561 6d53 7562 7469  RezkaStreamSubti
+00000aa0: 746c 6573 3c2f 613e 0a23 2323 2320 6048  tles</a>.#### `H
+00000ab0: 6452 657a 6b61 5374 7265 616d 2872 6573  dRezkaStream(res
+00000ac0: 6f6c 7574 696e 2960 202d 2063 616c 6c20  olutin)` - call 
+00000ad0: 6f62 6a65 6374 2077 6974 6820 6172 6775  object with argu
+00000ae0: 6d65 6e74 2074 6f20 6765 7420 7572 6c20  ment to get url 
+00000af0: 6f66 2076 6964 656f 0a0a 2323 2320 5573  of video..### Us
+00000b00: 6167 6520 6578 616d 706c 6573 3a0a 0a60  age examples:..`
+00000b10: 6060 7079 7468 6f6e 0a73 7472 6561 6d20  ``python.stream 
+00000b20: 3d20 7265 7a6b 612e 6765 7453 7472 6561  = rezka.getStrea
+00000b30: 6d28 312c 2035 290a 0a70 7269 6e74 2820  m(1, 5)..print( 
+00000b40: 7374 7265 616d 2827 3732 3070 2729 2029  stream('720p') )
+00000b50: 0a70 7269 6e74 2820 7374 7265 616d 2827  .print( stream('
+00000b60: 3732 3027 2920 290a 7072 696e 7428 2073  720') ).print( s
+00000b70: 7472 6561 6d28 3130 3830 2920 290a 7072  tream(1080) ).pr
+00000b80: 696e 7428 2073 7472 6561 6d28 2755 6c74  int( stream('Ult
+00000b90: 7261 2729 2029 0a70 7269 6e74 2820 7374  ra') ).print( st
+00000ba0: 7265 616d 2827 3130 3830 7020 556c 7472  ream('1080p Ultr
+00000bb0: 6127 2920 290a 7072 696e 7428 2073 7472  a') ).print( str
+00000bc0: 6561 6d2e 7669 6465 6f73 2029 0a60 6060  eam.videos ).```
+00000bd0: 0a0a 3c62 723e 0a0a 2320 4864 5265 7a6b  ..<br>..# HdRezk
+00000be0: 6153 7472 6561 6d53 7562 7469 746c 6573  aStreamSubtitles
+00000bf0: 3a0a 2323 2323 2060 7365 6c66 2e73 7562  :.#### `self.sub
+00000c00: 7469 746c 6573 6020 2d20 6469 6374 206f  titles` - dict o
+00000c10: 6620 7375 6274 6974 6c65 730a 2323 2323  f subtitles.####
+00000c20: 2060 7365 6c66 2e6b 6579 7360 202d 206c   `self.keys` - l
+00000c30: 6973 7420 6f66 2073 7562 7469 746c 6573  ist of subtitles
+00000c40: 2063 6f64 6573 0a23 2323 2320 6073 656c   codes.#### `sel
+00000c50: 6628 6964 2960 202d 2063 616c 6c20 6f62  f(id)` - call ob
+00000c60: 6a65 6374 2077 6974 6820 6172 6775 6d65  ject with argume
+00000c70: 6e74 2074 6f20 6765 7420 7572 6c20 6f66  nt to get url of
+00000c80: 2073 7562 7469 746c 6573 0a0a 2323 2320   subtitles..### 
+00000c90: 5573 6167 6520 6578 616d 706c 6573 3a0a  Usage examples:.
+00000ca0: 0a60 6060 7079 7468 6f6e 0a73 7472 6561  .```python.strea
+00000cb0: 6d20 3d20 7265 7a6b 612e 6765 7453 7472  m = rezka.getStr
+00000cc0: 6561 6d28 312c 2035 290a 0a70 7269 6e74  eam(1, 5)..print
+00000cd0: 2820 7374 7265 616d 2e73 7562 7469 746c  ( stream.subtitl
+00000ce0: 6573 2e6b 6579 7320 2920 2020 2020 2020  es.keys )       
+00000cf0: 2023 205b 2765 6e27 2c20 2772 7527 5d0a   # ['en', 'ru'].
+00000d00: 7072 696e 7428 2073 7472 6561 6d2e 7375  print( stream.su
+00000d10: 6274 6974 6c65 732e 7375 6274 6974 6c65  btitles.subtitle
+00000d20: 7320 2920 2020 2320 7b20 2765 6e27 3a20  s )   # { 'en': 
+00000d30: 7b27 7469 746c 6527 3a20 2745 6e67 6c69  {'title': 'Engli
+00000d40: 7368 272c 2027 6c69 6e6b 273a 2027 6874  sh', 'link': 'ht
+00000d50: 7470 733a 2f27 7d2c 202e 2e2e 2020 7d0a  tps:/'}, ...  }.
+00000d60: 7072 696e 7428 2073 7472 6561 6d2e 7375  print( stream.su
+00000d70: 6274 6974 6c65 7328 2765 6e27 2920 2920  btitles('en') ) 
+00000d80: 2020 2020 2020 2320 2768 7474 7073 3a2f        # 'https:/
+00000d90: 270a 7072 696e 7428 2073 7472 6561 6d2e  '.print( stream.
+00000da0: 7375 6274 6974 6c65 7328 2745 6e67 6c69  subtitles('Engli
+00000db0: 7368 2729 2029 2020 2320 2768 7474 7073  sh') )  # 'https
+00000dc0: 3a2f 270a 7072 696e 7428 2073 7472 6561  :/'.print( strea
+00000dd0: 6d2e 7375 6274 6974 6c65 7328 3029 2029  m.subtitles(0) )
+00000de0: 2020 2020 2020 2020 2020 2320 2768 7474            # 'htt
+00000df0: 7073 3a2f 270a 2320 2020 2020 2020 2020  ps:/'.#         
+00000e00: 2020 2020 2020 2020 2020 2020 2020 5e20                ^ 
+00000e10: 696e 6465 780a 6060 600a 0a3c 6272 3e0a  index.```..<br>.
+00000e20: 0a23 2048 6452 657a 6b61 5261 7469 6e67  .# HdRezkaRating
+00000e30: 3a0a 2323 2323 2060 7365 6c66 2e76 616c  :.#### `self.val
+00000e40: 7565 6020 2d20 7261 7469 6e67 2076 616c  ue` - rating val
+00000e50: 7565 2028 6066 6c6f 6174 6029 0a23 2323  ue (`float`).###
+00000e60: 2320 6073 656c 662e 766f 7465 7360 202d  # `self.votes` -
+00000e70: 2076 6f74 6573 2061 6d6f 756e 7420 2860   votes amount (`
+00000e80: 696e 7460 290a 0a3c 6872 3e0a 0a23 2323  int`)..<hr>..###
+00000e90: 2050 726f 7879 2075 7361 6765 2065 7861   Proxy usage exa
+00000ea0: 6d70 6c65 3a0a 6060 6070 7974 686f 6e0a  mple:.```python.
+00000eb0: 7265 7a6b 6120 3d20 4864 5265 7a6b 6141  rezka = HdRezkaA
+00000ec0: 7069 2875 726c 2c20 7072 6f78 793d 7b27  pi(url, proxy={'
+00000ed0: 6874 7470 273a 2027 6874 7470 3a2f 2f31  http': 'http://1
+00000ee0: 3932 2e31 3638 2e30 2e31 3a38 3027 7d29  92.168.0.1:80'})
+00000ef0: 0a60 6060 0a                             .```.
```

### Comparing `HdRezkaApi-7.0.0/setup.py` & `HdRezkaApi-7.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\Users\rost\Downloads\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='HdRezkaApi',
-	version='7.0.0',
+	version='7.0.1',
 	author='Super_Zombi',
 	author_email='super.zombi.yt@gmail.com',
 	description='',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/SuperZombi/HdRezkaApi',
 	packages=['HdRezkaApi'],
```

