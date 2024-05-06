# Comparing `tmp/eth_typing-4.2.2.tar.gz` & `tmp/eth_typing-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_typing-4.2.2.tar", last modified: Mon Apr 29 17:23:02 2024, max compression
+gzip compressed data, was "eth_typing-4.2.3.tar", last modified: Mon May  6 18:16:42 2024, max compression
```

## Comparing `eth_typing-4.2.2.tar` & `eth_typing-4.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-29 17:23:02.873035 eth_typing-4.2.2/
--rw-r--r--   0 reedsa     (501) staff       (20)     1095 2023-09-28 17:35:29.000000 eth_typing-4.2.2/LICENSE
--rw-r--r--   0 reedsa     (501) staff       (20)      168 2023-08-18 16:16:13.000000 eth_typing-4.2.2/MANIFEST.in
--rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-04-29 17:23:02.872078 eth_typing-4.2.2/PKG-INFO
--rw-r--r--   0 reedsa     (501) staff       (20)     3285 2024-04-08 18:59:39.000000 eth_typing-4.2.2/README.md
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-29 17:23:02.853032 eth_typing-4.2.2/eth_typing/
--rw-r--r--   0 reedsa     (501) staff       (20)     1480 2024-04-17 16:11:12.000000 eth_typing-4.2.2/eth_typing/__init__.py
--rw-r--r--   0 reedsa     (501) staff       (20)     4639 2024-04-29 17:18:54.000000 eth_typing-4.2.2/eth_typing/abi.py
--rw-r--r--   0 reedsa     (501) staff       (20)      191 2023-09-28 17:31:13.000000 eth_typing-4.2.2/eth_typing/bls.py
--rw-r--r--   0 reedsa     (501) staff       (20)       71 2024-04-09 21:54:01.000000 eth_typing-4.2.2/eth_typing/discovery.py
--rw-r--r--   0 reedsa     (501) staff       (20)      117 2023-09-28 17:31:13.000000 eth_typing-4.2.2/eth_typing/encoding.py
--rw-r--r--   0 reedsa     (501) staff       (20)      458 2023-09-28 17:31:13.000000 eth_typing-4.2.2/eth_typing/enums.py
--rw-r--r--   0 reedsa     (501) staff       (20)      173 2024-04-17 20:31:08.000000 eth_typing-4.2.2/eth_typing/ethpm.py
--rw-r--r--   0 reedsa     (501) staff       (20)      546 2024-04-16 21:57:08.000000 eth_typing-4.2.2/eth_typing/evm.py
--rw-r--r--   0 reedsa     (501) staff       (20)      320 2024-04-15 20:26:59.000000 eth_typing-4.2.2/eth_typing/exceptions.py
--rw-r--r--   0 reedsa     (501) staff       (20)    28684 2024-04-29 17:18:54.000000 eth_typing-4.2.2/eth_typing/networks.py
--rw-r--r--   0 reedsa     (501) staff       (20)        0 2023-09-28 17:31:13.000000 eth_typing-4.2.2/eth_typing/py.typed
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-29 17:23:02.865572 eth_typing-4.2.2/eth_typing.egg-info/
--rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-04-29 17:23:02.000000 eth_typing-4.2.2/eth_typing.egg-info/PKG-INFO
--rw-r--r--   0 reedsa     (501) staff       (20)      525 2024-04-29 17:23:02.000000 eth_typing-4.2.2/eth_typing.egg-info/SOURCES.txt
--rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-04-29 17:23:02.000000 eth_typing-4.2.2/eth_typing.egg-info/dependency_links.txt
--rw-r--r--   0 reedsa     (501) staff       (20)        1 2023-10-19 21:43:55.000000 eth_typing-4.2.2/eth_typing.egg-info/not-zip-safe
--rw-r--r--   0 reedsa     (501) staff       (20)      284 2024-04-29 17:23:02.000000 eth_typing-4.2.2/eth_typing.egg-info/requires.txt
--rw-r--r--   0 reedsa     (501) staff       (20)       11 2024-04-29 17:23:02.000000 eth_typing-4.2.2/eth_typing.egg-info/top_level.txt
--rw-r--r--   0 reedsa     (501) staff       (20)     3459 2024-04-08 18:59:39.000000 eth_typing-4.2.2/pyproject.toml
--rw-r--r--   0 reedsa     (501) staff       (20)       38 2024-04-29 17:23:02.873219 eth_typing-4.2.2/setup.cfg
--rw-r--r--   0 reedsa     (501) staff       (20)     1944 2024-04-29 17:22:51.000000 eth_typing-4.2.2/setup.py
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-29 17:23:02.679268 eth_typing-4.2.2/tests/
-drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-29 17:23:02.864556 eth_typing-4.2.2/tests/core/
--rw-r--r--   0 reedsa     (501) staff       (20)      105 2024-04-08 18:59:39.000000 eth_typing-4.2.2/tests/core/test_import_and_version.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:16:42.206704 eth_typing-4.2.3/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1095 2023-09-28 17:35:29.000000 eth_typing-4.2.3/LICENSE
+-rw-r--r--   0 reedsa     (501) staff       (20)      168 2023-08-18 16:16:13.000000 eth_typing-4.2.3/MANIFEST.in
+-rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-05-06 18:16:42.205185 eth_typing-4.2.3/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)     3285 2024-04-08 18:59:39.000000 eth_typing-4.2.3/README.md
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:16:42.184343 eth_typing-4.2.3/eth_typing/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1480 2024-04-17 16:11:12.000000 eth_typing-4.2.3/eth_typing/__init__.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     4639 2024-04-29 17:18:54.000000 eth_typing-4.2.3/eth_typing/abi.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      191 2023-09-28 17:31:13.000000 eth_typing-4.2.3/eth_typing/bls.py
+-rw-r--r--   0 reedsa     (501) staff       (20)       71 2024-04-09 21:54:01.000000 eth_typing-4.2.3/eth_typing/discovery.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      117 2023-09-28 17:31:13.000000 eth_typing-4.2.3/eth_typing/encoding.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      458 2023-09-28 17:31:13.000000 eth_typing-4.2.3/eth_typing/enums.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      173 2024-04-17 20:31:08.000000 eth_typing-4.2.3/eth_typing/ethpm.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      546 2024-04-16 21:57:08.000000 eth_typing-4.2.3/eth_typing/evm.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      320 2024-04-15 20:26:59.000000 eth_typing-4.2.3/eth_typing/exceptions.py
+-rw-r--r--   0 reedsa     (501) staff       (20)    29365 2024-05-06 15:30:34.000000 eth_typing-4.2.3/eth_typing/networks.py
+-rw-r--r--   0 reedsa     (501) staff       (20)        0 2023-09-28 17:31:13.000000 eth_typing-4.2.3/eth_typing/py.typed
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:16:42.195478 eth_typing-4.2.3/eth_typing.egg-info/
+-rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-05-06 18:16:41.000000 eth_typing-4.2.3/eth_typing.egg-info/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)      525 2024-05-06 18:16:42.000000 eth_typing-4.2.3/eth_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-05-06 18:16:41.000000 eth_typing-4.2.3/eth_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2023-10-19 21:43:55.000000 eth_typing-4.2.3/eth_typing.egg-info/not-zip-safe
+-rw-r--r--   0 reedsa     (501) staff       (20)      284 2024-05-06 18:16:41.000000 eth_typing-4.2.3/eth_typing.egg-info/requires.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)       11 2024-05-06 18:16:41.000000 eth_typing-4.2.3/eth_typing.egg-info/top_level.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)     3459 2024-04-08 18:59:39.000000 eth_typing-4.2.3/pyproject.toml
+-rw-r--r--   0 reedsa     (501) staff       (20)       38 2024-05-06 18:16:42.206833 eth_typing-4.2.3/setup.cfg
+-rw-r--r--   0 reedsa     (501) staff       (20)     1944 2024-05-06 18:16:32.000000 eth_typing-4.2.3/setup.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:16:42.167045 eth_typing-4.2.3/tests/
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-05-06 18:16:42.193033 eth_typing-4.2.3/tests/core/
+-rw-r--r--   0 reedsa     (501) staff       (20)      105 2024-04-08 18:59:39.000000 eth_typing-4.2.3/tests/core/test_import_and_version.py
```

### Comparing `eth_typing-4.2.2/LICENSE` & `eth_typing-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/PKG-INFO` & `eth_typing-4.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.2.2
+Version: 4.2.3
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth_typing-4.2.2/README.md` & `eth_typing-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/eth_typing/__init__.py` & `eth_typing-4.2.3/eth_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/eth_typing/abi.py` & `eth_typing-4.2.3/eth_typing/abi.py`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/eth_typing/evm.py` & `eth_typing-4.2.3/eth_typing/evm.py`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/eth_typing/networks.py` & `eth_typing-4.2.3/eth_typing/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     DWU = 124
     OYCHAINTESTNET = 125
     OYCHAINMAINNET = 126
     FETH = 127
     HECO = 128
     INNOVATOR = 129
     TGRAM = 131
+    HSKT = 133
     RLC = 134
     ALYXTESTNET = 135
     DEAM = 136
     MATIC = 137
     DFIO_META_MAIN = 138
     WOOP = 139
     OPTEST = 141
@@ -155,14 +156,15 @@
     PUPPYNET = 157
     RBA = 158
     RBAT = 159
     EVA = 160
     WALL_E = 161
     TPHT = 162
     PHT = 163
+    OMNI_TESTNET_164 = 164
     OMNI_TESTNET = 165
     OMNI = 166
     ATOSHI = 167
     AIOZ = 168
     MANTA = 169
     HOOSMARTCHAIN = 170
     RESIL = 172
@@ -193,14 +195,15 @@
     SO1_OLD = 218
     SEPSCAL = 220
     ASK = 222
     B2_MAINNET = 223
     VRD_TESTNET = 224
     LA = 225
     TLA = 226
+    FHE = 228
     SDX = 230
     PROTOJUMBO = 234
     DEAMTEST = 236
     BLAST = 238
     PLGCHAIN = 242
     EWT = 246
     OAS = 248
@@ -213,14 +216,15 @@
     SUR = 262
     NEURA = 266
     TNEURA = 267
     DNEURA = 268
     HPB = 269
     EGONM = 271
     LACHAIN = 274
+    FAI = 278
     BPX = 279
     ZKSYNC_GOERLI = 280
     ZKTCRO = 282
     BOBA = 288
     ORDERLY = 291
     HEDERA_MAINNET = 295
     HEDERA_TESTNET = 296
@@ -313,14 +317,15 @@
     KALICHAINMAINNET = 654
     ULTRONSMARTCHAIN = 662
     PIXIE_CHAIN_TESTNET = 666
     LAOS = 667
     JUNCA = 668
     JUNCAT = 669
     KAR = 686
+    REDSTONE = 690
     SNS = 700
     BCS = 707
     TBCS = 708
     FURY = 710
     VRC = 713
     SHIBARIUM = 719
     LYC = 721
@@ -375,14 +380,15 @@
     MUNODE = 956
     LYRA = 957
     BTC20 = 963
     CCN = 970
     HUYGENS = 971
     ASCRAEUS = 972
     YETI = 977
+    SEXYTESTNET = 979
     TOP_EVM = 980
     MEMOCHAIN = 985
     TOP = 989
     ELM = 990
     _5IRE = 997
     LN = 998
     TWAN = 999
@@ -390,14 +396,15 @@
     BAOBAB = 1001
     TET = 1003
     T_EKTA = 1004
     TNEW = 1007
     EUN = 1008
     JUMBOSCAN = 1009
     EVC = 1010
+    REBUS = 1011
     NEW = 1012
     SKU = 1022
     TCLV = 1023
     CLV = 1024
     TBTT = 1028
     CFX = 1030
     PRX = 1031
@@ -422,14 +429,15 @@
     TCORE = 1115
     CORE = 1116
     DOGSM = 1117
     B2_TESTNET = 1123
     DFI = 1130
     DFI_T = 1131
     CHANGI = 1133
+    LISK = 1135
     ASART = 1138
     MATH = 1139
     TMATH = 1140
     PLEXCHAIN = 1149
     AUOC = 1170
     SHT = 1177
     MOS = 1188
@@ -543,14 +551,15 @@
     KYOTO_TESTNET = 1998
     DC = 2000
     MILKADA = 2001
     MILKALGO = 2002
     CLOUDWALK_TESTNET = 2008
     CLOUDWALK_MAINNET = 2009
     NETZ = 2016
+    TEL = 2017
     PMINT_DEV = 2018
     PMINT_TEST = 2019
     PMINT = 2020
     EDG = 2021
     EDGT = 2022
     TAYCAN_TESTNET = 2023
     SWAN = 2024
@@ -575,14 +584,16 @@
     EXN = 2109
     CMCX = 2121
     METAD = 2122
     MEU = 2124
     BIGSB_TESTNET = 2136
     BIGSB = 2137
     DFIO_META_TEST = 2138
+    ONENESS = 2140
+    ONENESS_TESTNET = 2141
     BOA = 2151
     FRA = 2152
     FINDORA_TESTNET = 2153
     FINDORA_FORGE = 2154
     MSN = 2199
     ABNM = 2202
     BTC = 2203
@@ -635,25 +646,27 @@
     XENON = 2941
     BTY = 2999
     CENNZ_R = 3000
     CENNZ_N = 3001
     CAU = 3003
     _3ULL = 3011
     ORL = 3031
+    REBUS_TESTNET = 3033
     BFC = 3068
+    MOVE = 3073
     IMMU3 = 3100
     VFI = 3102
     SAVM = 3109
     TSAVM = 3110
     FILECOIN_HYPERSPACE = 3141
     DUBX = 3269
     TESTDUBX = 3270
     DEBOUNCE_DEVNET = 3306
     ZCRBEACH = 3331
-    W3Q_T = 3333
+    ES_T = 3333
     W3Q_G = 3334
     PRB = 3400
     EVOM = 3424
     SCAIT = 3434
     PRBTESTNET = 3500
     JFIN = 3501
     PANDO_MAINNET = 3601
@@ -680,14 +693,15 @@
     TDYNO = 3967
     APEXSEP = 3993
     YCC = 3999
     OZO = 4000
     PERIUM = 4001
     TFTM = 4002
     X1_FASTNET = 4003
+    GANTESTNET = 4048
     BOBAOPERATESTNET = 4051
     NAHMII3MAINNET = 4061
     NAHMII3TESTNET = 4062
     MUSTER = 4078
     OASIS = 4090
     BNIT = 4096
     BNIM = 4099
@@ -799,14 +813,15 @@
     TADIL = 7575
     ADIL = 7576
     TRN_MAINNET = 7668
     TRN_PORCINI = 7672
     CANTO = 7700
     TESTNETCANTO = 7701
     TBITROCK = 7771
+    GDCC = 7775
     RISEOFTHEWARBOTSTESTNET = 7777
     ORE = 7778
     OEX = 7798
     MAAL_TEST = 7860
     TSCAS = 7878
     KINTOMAINNET = 7887
     ARD = 7895
@@ -953,15 +968,16 @@
     MTT = 16000
     MTTTEST = 16001
     GENESYS = 16507
     NYANCAT = 16688
     AIRDAO = 16718
     TIVAR = 16888
     HOLESKY = 17000
-    REDSTONE = 17001
+    REDSTONE_HOLESKY = 17001
+    GARNET = 17069
     G8CM = 17171
     ECLIPSE = 17172
     PCT = 17180
     KONET = 17217
     EOS = 17777
     ZKST = 18000
     STN = 18122
@@ -971,14 +987,15 @@
     UNREAL = 18233
     MXCZKEVM = 18686
     TITAN_TKX = 18888
     TITAN_TKX_TESTNET = 18889
     HMV = 19011
     DCSMS = 19224
     MGT = 19527
+    LBRY = 19600
     BTCIX = 19845
     CAMELARK = 20001
     CLOTESTNET = 20729
     P12 = 20736
     JONO11 = 20765
     C4EI = 21004
     AAH = 21133
@@ -1004,24 +1021,28 @@
     GOLDT = 25888
     BKCT = 25925
     FRM = 26026
     HTZ = 26600
     OAC = 26863
     KLAOSNOVA = 27181
     NANON_TESTNET = 27483
+    ZEROONEMAI = 27827
     VIZING_TESTNET = 28516
     VIZING = 28518
     OBGOR = 28528
     BOBASEPOLIA = 28882
     HYCHAIN_TESTNET = 29112
     TKEC = 29536
     MCHV = 29548
     PIECE = 30067
     MIYOU = 30088
     CERI = 30103
+    MOVELEG = 30730
+    MOVEDEV = 30731
+    MOVETEST = 30732
     ESN = 31102
     CLDTX = 31223
     CLD = 31224
     GOT = 31337
     TMTHN = 31414
     FILECOIN_WALLABY = 31415
     W3GAMEZ = 32001
@@ -1075,23 +1096,25 @@
     YVM = 50005
     YVT = 50006
     TGTON = 50021
     LUMOZ_TESTNET = 51178
     SRDXM = 51712
     ETN_MAINNET = 52014
     DOID = 53277
+    DODOCHAIN = 53457
     DFK = 53935
     ISLMT = 54211
     TORONETTESTNET = 54321
     PTON = 54555
     TETH = 55004
     REICHAIN = 55555
     TREI = 55556
     LAMBDA = 56026
     BOBABNB = 56288
+    TESTNETZER = 56400
     VELO = 56789
     DOIDTESTNET = 56797
     TSYS_ROLLUX = 57000
     SEPPGN = 58008
     LINEA_GOERLI = 59140
     LINEA_SEPOLIA = 59141
     LINEA = 59144
@@ -1169,14 +1192,15 @@
     NAUTTEST = 88002
     UNIT0_TESTNET = 88817
     UNIT0_STAGENET = 88819
     CHZ = 88880
     IVAR = 88888
     DHOBYGHAUT = 90001
     BVHL = 90210
+    CAMP = 90354
     NAUT = 91002
     METADAP = 91120
     COMBO_TESTNET = 91715
     LAMBDA_TESTNET = 92001
     TLILA = 93572
     MANTIS = 96970
     BOBABNBOLD = 97288
@@ -1195,14 +1219,15 @@
     VECHAIN = 100009
     VECHAIN_TESTNET = 100010
     CHI1 = 100100
     STABILITYPROTOCOL = 101010
     CTCTEST = 102031
     CRFI = 103090
     MASATEST = 103454
+    CAS = 104566
     STRATIS = 105105
     BRO = 108801
     QKC_D_R = 110000
     QKC_D_S0 = 110001
     QKC_D_S1 = 110002
     QKC_D_S2 = 110003
     QKC_D_S3 = 110004
@@ -1227,14 +1252,16 @@
     TAIKO_L2 = 167005
     TAIKO_L3 = 167006
     TKO_JOLNIR = 167007
     TKO_KATLA = 167008
     TKO_HEKLA = 167009
     BDCC = 188710
     CONDOR = 188881
+    FHET = 192940
+    FAIT = 200000
     MILKTADA = 200101
     MILKTALGO = 200202
     AKA = 200625
     BTRT = 200810
     BTR = 200901
     ALAYA = 201018
     ALAYADEV = 201030
@@ -1264,14 +1291,15 @@
     CMP_MAINNET = 256256
     GZ_TESTNET = 266256
     EGONT = 271271
     SOCHAIN = 281121
     ZILLSEP = 282828
     SAHARATEST = 313313
     FILECOIN_CALIBRATION = 314159
+    PAREX = 322202
     BGBC_TESTNET = 323213
     TC = 330844
     BGBC = 333313
     AVST = 333331
     N3_TEST = 333333
     OONETEST = 333666
     OONEDEV = 333777
@@ -1310,14 +1338,15 @@
     SCR_PREALPHA = 534354
     SHI = 534849
     BESC = 535037
     ECLIPSET = 555666
     HYP = 622277
     BRNKC = 641230
     ALL = 651940
+    XAI = 660279
     VPIONEER = 666666
     HELA_TESTNET = 666888
     WONCHAIN = 686868
     GALADRIEL_DEVNET = 696969
     TILTYARDMAINNET = 710420
     SEI_DEVNET = 713715
     HEMI_SEP = 743111
@@ -1340,14 +1369,15 @@
     RIA_DEV = 912559
     PSC_D_S0 = 920000
     PSC_D_S1 = 920001
     TFNCY = 923018
     JONO12 = 955081
     ELV = 955305
     ECROX = 988207
+    AMC = 999999
     NMTTEST = 1100789
     TILTYARD = 1127469
     AZKTN = 1261120
     ETHO = 1313114
     XERO = 1313500
     KINTSUGI = 1337702
     KILN = 1337802
@@ -1364,15 +1394,15 @@
     MANTATESTNET = 3441005
     MANTASEPOLIATESTNET = 3441006
     ALT_ZEROGAS = 4000003
     WORLDSCAL = 4281033
     MXCDISCONTINUED = 5167003
     MXC = 5167004
     ETN_TESTNET = 5201420
-    REACT = 5318008
+    KREACT = 5318008
     IMVERSED = 5555555
     IMVERSED_TESTNET = 5555558
     AZKYT = 6038361
     SAFEMAINNET = 6666665
     SAFETESTNET = 6666666
     SAAKURU = 7225878
     VSL = 7355310
@@ -1467,25 +1497,28 @@
     HMY_S1 = 1666600001
     HMY_S2 = 1666600002
     HMY_S3 = 1666600003
     HMY_B_S0 = 1666700000
     HMY_B_S1 = 1666700001
     HMY_PS_S0 = 1666900000
     HMY_PS_S1 = 1666900001
+    KKRT_SEPOLIA = 1802203764
     RARI_TESTNET = 1918988905
     HOP = 2021121117
     EUROPA = 2046399126
     A8OLD = 2863311531
     PIRL = 3125659152
     FRANKENSTEIN = 4216137055
     TPALM = 11297108099
     PALM = 11297108109
     GS_ETH = 28872323069
+    XAITESTNET = 37714555429
     ARB_BLUEBERRY = 88153591557
-    KKRT_SEPOLIA = 107107114116
+    KKRT_SEPOLIA_DEPRECATED = 107107114116
     ALPHABET = 111222333444
     NTT = 197710212030
     NTT_HARADEV = 197710212031
     ZENIQ = 383414847825
     IPDC = 666301171999
     MOLE = 6022140761023
     GW_TESTNET_V1_DEPRECATED = 868455272153094
+    DCHAINT = 2713017997578000
```

### Comparing `eth_typing-4.2.2/eth_typing.egg-info/PKG-INFO` & `eth_typing-4.2.3/eth_typing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.2.2
+Version: 4.2.3
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth_typing-4.2.2/eth_typing.egg-info/SOURCES.txt` & `eth_typing-4.2.3/eth_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/pyproject.toml` & `eth_typing-4.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth_typing-4.2.2/setup.py` & `eth_typing-4.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-typing",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="4.2.2",
+    version="4.2.3",
     description="""eth-typing: Common type annotations for ethereum python packages""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-typing",
     include_package_data=True,
```

