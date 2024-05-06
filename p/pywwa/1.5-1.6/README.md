# Comparing `tmp/pywwa-1.5.tar.gz` & `tmp/pywwa-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywwa-1.5.tar", last modified: Thu Mar  7 16:40:25 2024, max compression
+gzip compressed data, was "pywwa-1.6.tar", last modified: Mon May  6 11:18:59 2024, max compression
```

## Comparing `pywwa-1.5.tar` & `pywwa-1.6.tar`

### file list

```diff
@@ -1,378 +1,380 @@
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.423535 pywwa-1.5/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       58 2020-11-30 04:37:51.000000 pywwa-1.5/.coveragerc
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      154 2021-05-03 03:44:59.000000 pywwa-1.5/.deepsource.toml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       28 2020-11-23 22:37:16.000000 pywwa-1.5/.editorconfig
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.373535 pywwa-1.5/.github/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.376535 pywwa-1.5/.github/workflows/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3813 2024-03-07 16:39:12.000000 pywwa-1.5/.github/workflows/build.yml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      833 2023-09-05 13:08:56.000000 pywwa-1.5/.github/workflows/codeql.yml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      914 2022-06-30 13:37:49.000000 pywwa-1.5/.github/workflows/etchosts.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      240 2024-01-08 13:50:35.000000 pywwa-1.5/.gitignore
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      216 2024-03-07 16:39:12.000000 pywwa-1.5/.pre-commit-config.yaml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      616 2024-03-07 16:39:27.000000 pywwa-1.5/CHANGELOG.md
--rw-rw-r--   0 akrherz  (43306) domain-users   (101)     1065 2014-06-05 12:53:03.000000 pywwa-1.5/LICENSE
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      150 2024-01-07 18:54:00.000000 pywwa-1.5/MANIFEST.in
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2024-03-07 16:40:25.423535 pywwa-1.5/PKG-INFO
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4356 2024-01-15 17:56:23.000000 pywwa-1.5/README.md
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      665 2024-03-07 16:39:12.000000 pywwa-1.5/conftest.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      991 2024-03-07 16:39:12.000000 pywwa-1.5/environment.yml
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.394535 pywwa-1.5/examples/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      273 2020-11-24 02:23:22.000000 pywwa-1.5/examples/ADA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      163 2020-11-24 02:23:22.000000 pywwa-1.5/examples/ADM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4182 2020-11-24 02:23:22.000000 pywwa-1.5/examples/ADMNES.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4025 2024-02-05 20:09:37.000000 pywwa-1.5/examples/AFD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      847 2020-11-24 02:23:22.000000 pywwa-1.5/examples/AQA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      922 2020-11-24 02:23:22.000000 pywwa-1.5/examples/AQI.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1053 2020-11-24 02:23:22.000000 pywwa-1.5/examples/AVA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1794 2024-02-22 13:46:19.000000 pywwa-1.5/examples/AVG.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1035 2020-11-24 02:23:22.000000 pywwa-1.5/examples/AVW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      912 2020-11-24 02:23:22.000000 pywwa-1.5/examples/AWU.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      489 2022-09-10 12:59:09.000000 pywwa-1.5/examples/AWW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      221 2020-11-24 02:23:22.000000 pywwa-1.5/examples/BLU.txt
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.396535 pywwa-1.5/examples/BUFR/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      741 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISAB02_CWAO.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      609 2023-12-08 19:17:06.000000 pywwa-1.5/examples/BUFR/ISAE01_SKBO.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    81301 2023-12-06 21:16:59.000000 pywwa-1.5/examples/BUFR/ISAI01_SBBR.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     7181 2024-01-03 19:07:21.000000 pywwa-1.5/examples/BUFR/ISCI01_SABM.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      834 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISIA14_CWAO.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    20732 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISMA01_FNLU.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    21528 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISMA01_FNLU_badid.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    20335 2023-12-08 17:55:39.000000 pywwa-1.5/examples/BUFR/ISMA01_FNLU_badid2.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      723 2023-12-12 19:03:23.000000 pywwa-1.5/examples/BUFR/ISMD21_UAST.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      267 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISMI60_SBBR.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1374 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISND01_LEMM.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      996 2024-01-08 21:02:34.000000 pywwa-1.5/examples/BUFR/ISNN26_LFPW.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISXD03_EDZW.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    15190 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/ISXT14_EGRR.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1644 2023-12-06 15:36:24.000000 pywwa-1.5/examples/BUFR/IS_2023120401.bufr
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1472 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CAE.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      936 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CEM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6194 2020-11-25 19:12:07.000000 pywwa-1.5/examples/CF6.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1272 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CFW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      412 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CGR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5272 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CLI.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3486 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CLIANN.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8967 2020-12-30 03:14:45.000000 pywwa-1.5/examples/CLIHOU.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2995 2022-03-20 02:32:01.000000 pywwa-1.5/examples/CLM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      145 2023-05-15 19:05:41.000000 pywwa-1.5/examples/CORM6.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      258 2023-05-15 19:05:41.000000 pywwa-1.5/examples/CORM6_RTP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1130 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CRF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      231 2022-03-20 02:32:01.000000 pywwa-1.5/examples/CWA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8810 2020-11-24 02:23:22.000000 pywwa-1.5/examples/CWF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    23693 2020-11-24 02:23:22.000000 pywwa-1.5/examples/DGT.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3545 2020-11-24 02:23:22.000000 pywwa-1.5/examples/DSM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1054 2020-11-24 02:23:22.000000 pywwa-1.5/examples/EQI.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      959 2020-11-24 02:23:22.000000 pywwa-1.5/examples/EQR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    11107 2024-01-08 18:13:05.000000 pywwa-1.5/examples/ESF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      848 2020-11-24 02:23:22.000000 pywwa-1.5/examples/EVI.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1207 2020-11-24 02:23:22.000000 pywwa-1.5/examples/EWW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    13048 2023-03-09 13:15:00.000000 pywwa-1.5/examples/FD1US1.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2519 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FFA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3319 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FFGDMX.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1506 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FFS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1600 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FFW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1183 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FFWTWC_tilde.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      728 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FLS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1603 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FLW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      699 2022-04-06 02:46:23.000000 pywwa-1.5/examples/FRW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1099 2022-04-06 03:14:34.000000 pywwa-1.5/examples/FRWOUN.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      166 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FTM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      707 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FWA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    14157 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FWF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2290 2020-11-24 02:23:22.000000 pywwa-1.5/examples/FWS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3605 2020-11-24 02:23:22.000000 pywwa-1.5/examples/GLF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      657 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HCM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      834 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HLS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3551 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HMD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    51585 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HMLARX.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1361 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HWO.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6274 2020-11-24 02:23:22.000000 pywwa-1.5/examples/HYD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3654 2020-11-24 02:23:22.000000 pywwa-1.5/examples/ICE.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      553 2020-11-24 02:23:22.000000 pywwa-1.5/examples/LAE.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5239 2020-11-24 02:23:22.000000 pywwa-1.5/examples/LCO.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      549 2021-03-25 02:33:35.000000 pywwa-1.5/examples/LSR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    54358 2022-03-17 15:58:07.000000 pywwa-1.5/examples/LWGE86.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2160 2024-01-29 17:16:02.000000 pywwa-1.5/examples/MCD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1356 2020-11-24 02:23:22.000000 pywwa-1.5/examples/METAR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3968 2020-11-24 02:23:22.000000 pywwa-1.5/examples/METNC1.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4454 2020-11-24 02:23:22.000000 pywwa-1.5/examples/MIS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1428 2020-12-26 13:10:49.000000 pywwa-1.5/examples/MPD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1385 2020-11-24 02:23:22.000000 pywwa-1.5/examples/MWS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2277 2020-11-24 02:23:22.000000 pywwa-1.5/examples/MWW.txt
--rw-rw-r--   0 akrherz  (43306) domain-users   (101)    10245 2012-11-27 14:22:18.000000 pywwa-1.5/examples/NCR_20121127_1413
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8126 2020-05-19 20:07:00.000000 pywwa-1.5/examples/NCR_20200519_1950
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2386 2021-09-11 02:27:34.000000 pywwa-1.5/examples/NCR_20210911_0023
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2020-11-24 02:23:22.000000 pywwa-1.5/examples/NOW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      465 2024-01-09 11:42:08.000000 pywwa-1.5/examples/NOXX.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      534 2020-11-24 02:23:22.000000 pywwa-1.5/examples/NPW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3459 2020-11-24 02:23:22.000000 pywwa-1.5/examples/NSH.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2242 2020-11-24 02:23:22.000000 pywwa-1.5/examples/OAV.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      320 2020-11-24 02:23:22.000000 pywwa-1.5/examples/OMR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    14991 2020-11-24 02:23:22.000000 pywwa-1.5/examples/PFM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      746 2021-04-16 16:19:50.000000 pywwa-1.5/examples/PFWFD1.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      868 2021-04-16 16:20:04.000000 pywwa-1.5/examples/PFWFD2.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      321 2020-11-24 02:23:22.000000 pywwa-1.5/examples/PIREP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2212 2020-11-24 02:23:22.000000 pywwa-1.5/examples/PNS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2728 2023-07-27 14:51:31.000000 pywwa-1.5/examples/PNS_damage.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6053 2023-03-21 04:16:39.000000 pywwa-1.5/examples/PNS_damage_multi.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5210 2023-04-22 11:17:30.000000 pywwa-1.5/examples/PNS_damage_multi2.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5340 2020-11-24 02:23:22.000000 pywwa-1.5/examples/PSH.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2767 2020-11-24 02:23:22.000000 pywwa-1.5/examples/PTS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6765 2021-05-03 14:54:59.000000 pywwa-1.5/examples/PTSDY1.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2588 2021-04-16 16:19:20.000000 pywwa-1.5/examples/PTSDY2.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    14059 2020-11-24 02:23:22.000000 pywwa-1.5/examples/QPS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2477 2021-07-14 16:59:07.000000 pywwa-1.5/examples/RBG.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1445 2021-07-14 16:59:07.000000 pywwa-1.5/examples/RBG94E.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      805 2021-07-14 16:59:07.000000 pywwa-1.5/examples/RBG98E.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      654 2021-07-14 16:59:07.000000 pywwa-1.5/examples/RBG99E.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    24559 2020-11-24 02:23:22.000000 pywwa-1.5/examples/REC.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      338 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RER.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      564 2020-11-24 02:23:22.000000 pywwa-1.5/examples/REROKC.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      763 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RFD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2119 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RFW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      272 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RR3.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4094 2023-09-27 03:21:13.000000 pywwa-1.5/examples/RR7.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      603 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RRM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1283 2022-01-14 15:17:11.000000 pywwa-1.5/examples/RRSJAN.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5275 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RTP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3362 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RVA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1841 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RVD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1598 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RVF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      948 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RVS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1681 2020-11-24 02:23:22.000000 pywwa-1.5/examples/RWS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      541 2022-05-02 20:46:04.000000 pywwa-1.5/examples/SAW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      602 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SCPPR2.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2017 2022-05-02 20:46:04.000000 pywwa-1.5/examples/SEL.txt
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.397535 pywwa-1.5/examples/SHEF/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      273 2023-09-29 16:50:06.000000 pywwa-1.5/examples/SHEF/RR1.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       98 2023-09-26 20:12:35.000000 pywwa-1.5/examples/SHEF/RR7KRF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       64 2024-01-08 18:13:05.000000 pywwa-1.5/examples/SHEF/RR7ZOB.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     9530 2023-09-26 20:12:35.000000 pywwa-1.5/examples/SHEF/RR8KRF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      637 2023-10-28 04:01:18.000000 pywwa-1.5/examples/SHEF/RR8MSR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2023-10-28 04:01:18.000000 pywwa-1.5/examples/SHEF/RRSNMC.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      942 2021-07-23 18:27:50.000000 pywwa-1.5/examples/SHEF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      287 2020-11-30 13:25:40.000000 pywwa-1.5/examples/SIGC.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    14700 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SMF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1301 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SMW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1924 2020-11-30 04:37:51.000000 pywwa-1.5/examples/SPE.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      960 2021-03-14 03:44:33.000000 pywwa-1.5/examples/SPS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      952 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SPW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1890 2021-07-27 16:41:27.000000 pywwa-1.5/examples/SQW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2371 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SRF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4651 2020-11-24 02:23:22.000000 pywwa-1.5/examples/STF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1803 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SVR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      779 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SVS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1919 2020-11-24 02:23:22.000000 pywwa-1.5/examples/SWOMCD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      213 2021-03-23 02:10:30.000000 pywwa-1.5/examples/TAF.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1734 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TCD.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1431 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TCM.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2141 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TCP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1014 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TCU.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2206 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TIB.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1303 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TID.txt
--rw-rw-r--   0 akrherz  (43306) domain-users   (101)    57048 2017-08-15 13:00:42.000000 pywwa-1.5/examples/TIGH05
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      410 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TOE.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1526 2021-03-18 16:14:42.000000 pywwa-1.5/examples/TOR.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      268 2020-11-24 02:23:22.000000 pywwa-1.5/examples/TWO.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      355 2020-11-24 02:23:22.000000 pywwa-1.5/examples/VAA.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1131 2020-11-24 02:23:22.000000 pywwa-1.5/examples/WCN.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3232 2020-11-24 02:23:22.000000 pywwa-1.5/examples/WCNMEG.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      185 2020-11-24 02:23:22.000000 pywwa-1.5/examples/WRK.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      425 2020-11-24 02:23:22.000000 pywwa-1.5/examples/WSV.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      513 2020-11-24 02:23:22.000000 pywwa-1.5/examples/WSW.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1038 2022-05-02 20:46:04.000000 pywwa-1.5/examples/WWP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1026 2022-05-01 19:50:13.000000 pywwa-1.5/examples/WWP9.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3214 2022-12-28 17:27:33.000000 pywwa-1.5/examples/XTEUS.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    43582 2020-11-24 02:23:22.000000 pywwa-1.5/examples/ZFP.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      532 2024-01-10 17:11:57.000000 pywwa-1.5/examples/nldn.bin
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.398535 pywwa-1.5/goes/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3303 2024-03-07 16:39:12.000000 pywwa-1.5/goes/conus_composite.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      305 2024-03-07 16:39:12.000000 pywwa-1.5/goes/greys_cmap.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3716 2019-11-22 14:49:01.000000 pywwa-1.5/goes/greysramp.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1184 2024-03-07 16:39:12.000000 pywwa-1.5/goes/ir_cmap.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4226 2019-11-22 05:04:56.000000 pywwa-1.5/goes/irramp.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3118 2024-03-07 16:39:12.000000 pywwa-1.5/goes/make_ramp_legend.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6750 2024-03-07 16:39:12.000000 pywwa-1.5/goes/netcdf2png.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      168 2022-06-28 16:13:34.000000 pywwa-1.5/goes/run_goes.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      802 2024-03-07 16:39:12.000000 pywwa-1.5/goes/wv_cmap.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3965 2019-11-22 04:42:36.000000 pywwa-1.5/goes/wvramp.txt
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.403535 pywwa-1.5/parsers/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      100 2024-01-09 21:00:48.000000 pywwa-1.5/parsers/afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      130 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/aviation.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1652 2024-01-11 03:51:07.000000 pywwa-1.5/parsers/awos_ingest.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      148 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/bufr_surface.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      131 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/cf6_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      336 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/cli_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/cwa_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      158 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/dsm2afos.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      134 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/dsm_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/ero_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      136 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/fake_afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      129 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/fd_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       95 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/ffg_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/gairmet_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      122 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/generic_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      250 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/gini2gis.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      103 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/hml_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/lsr_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      145 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/mcd_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      319 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/metar_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      119 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/mos_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      161 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/nexrad3_attr.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       97 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/nldn_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      107 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/pirep_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      128 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/rr7.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      111 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/scp_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/shef_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      165 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/spammer.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/spc_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/spe_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      153 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/split_mav.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/sps_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      111 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/taf_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      526 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/vtec_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/watch_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.5/parsers/xteus_parser.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.404535 pywwa-1.5/pqact.d/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      647 2020-11-26 12:41:43.000000 pywwa-1.5/pqact.d/README.md
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2231 2024-02-22 13:46:19.000000 pywwa-1.5/pqact.d/pqact.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1802 2024-01-17 14:13:08.000000 pywwa-1.5/pqact.d/pqact_afos.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      187 2024-01-07 18:54:00.000000 pywwa-1.5/pqact.d/pqact_gini.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1309 2024-01-19 14:05:45.000000 pywwa-1.5/pqact.d/pqact_iemingest.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       94 2024-01-07 18:54:00.000000 pywwa-1.5/pqact.d/pqact_nexrad.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      926 2024-01-07 18:54:00.000000 pywwa-1.5/pqact.d/pqact_shef.conf
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      369 2024-03-07 16:39:12.000000 pywwa-1.5/pyproject.toml
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      352 2024-01-07 18:54:00.000000 pywwa-1.5/pywwa_settings.json-example
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2425 2024-03-07 16:40:25.423535 pywwa-1.5/setup.cfg
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      111 2024-03-07 16:39:12.000000 pywwa-1.5/setup.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.373535 pywwa-1.5/src/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.405535 pywwa-1.5/src/pywwa/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1713 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/__init__.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8164 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/common.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.409535 pywwa-1.5/src/pywwa/data/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)   136412 2024-01-07 18:54:00.000000 pywwa-1.5/src/pywwa/data/conus.shp
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      108 2024-01-07 18:54:00.000000 pywwa-1.5/src/pywwa/data/conus.shx
--rw-r--r--   0 akrherz  (43306) domain-users   (101)  1497650 2024-01-07 18:54:00.000000 pywwa-1.5/src/pywwa/data/faa_apt.tbl
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    16560 2024-01-07 18:54:00.000000 pywwa-1.5/src/pywwa/data/nexrad.stns
--rw-r--r--   0 akrherz  (43306) domain-users   (101)   514578 2024-01-22 17:02:54.000000 pywwa-1.5/src/pywwa/data/pirep_navaids.tbl
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    30715 2024-01-07 18:54:00.000000 pywwa-1.5/src/pywwa/data/vors.tbl
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3031 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/data/wmo2iso3166.tbl
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3526 2024-01-11 03:51:07.000000 pywwa-1.5/src/pywwa/database.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1923 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/ldm.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5248 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/ldmbridge.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      501 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/memclient.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      604 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/testing.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.414535 pywwa-1.5/src/pywwa/workflows/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)       30 2024-01-09 21:00:48.000000 pywwa-1.5/src/pywwa/workflows/__init__.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2688 2024-02-21 15:11:28.000000 pywwa-1.5/src/pywwa/workflows/afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2201 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/aviation.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    14929 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/bufr_surface.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      630 2024-01-09 21:49:01.000000 pywwa-1.5/src/pywwa/workflows/cf6.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1674 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/cli.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2367 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/cwa.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1491 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/dsm.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1083 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/dsm2afos.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      895 2024-01-11 03:51:07.000000 pywwa-1.5/src/pywwa/workflows/ero.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2671 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/fake_afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      639 2024-01-09 21:49:01.000000 pywwa-1.5/src/pywwa/workflows/fd.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      791 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/ffg.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      601 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/gairmet.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2192 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/generic.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8205 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/gini2gis.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      604 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/hml.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2526 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/lsr.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1411 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/mcd.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     5243 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/metar.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      663 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/mos.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     6122 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/nexrad3_attr.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/nldn.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3476 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/pirep.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      774 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/rr7.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      614 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/scp.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    20127 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/shef.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3840 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/spammer.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      898 2024-01-11 03:51:07.000000 pywwa-1.5/src/pywwa/workflows/spc.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1418 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/spe.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1691 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/split_mav.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1244 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/sps.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      797 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/taf.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2853 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/vtec.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2769 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/watch.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      596 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/workflows/xteus.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8002 2024-03-07 16:39:12.000000 pywwa-1.5/src/pywwa/xmpp.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.422535 pywwa-1.5/src/pywwa.egg-info/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/PKG-INFO
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     8096 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/SOURCES.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        1 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/dependency_links.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1673 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/entry_points.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      144 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/requires.txt
--rw-r--r--   0 akrherz  (43306) domain-users   (101)        6 2024-03-07 16:40:25.000000 pywwa-1.5/src/pywwa.egg-info/top_level.txt
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.414535 pywwa-1.5/tests/
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.414535 pywwa-1.5/tests/bin/
--rwxr-xr-x   0 akrherz  (43306) domain-users   (101)       26 2023-09-27 19:09:12.000000 pywwa-1.5/tests/bin/pqinsert
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      937 2024-01-11 03:51:07.000000 pywwa-1.5/tests/test_common.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      533 2024-03-07 16:39:12.000000 pywwa-1.5/tests/test_common_syslog.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      446 2024-01-09 21:00:48.000000 pywwa-1.5/tests/test_database.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      609 2024-03-07 16:39:12.000000 pywwa-1.5/tests/test_init.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      159 2024-03-07 16:39:12.000000 pywwa-1.5/tests/test_ldm.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      984 2024-03-07 16:39:12.000000 pywwa-1.5/tests/test_ldmbridge.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1269 2024-03-07 16:39:12.000000 pywwa-1.5/tests/test_workflow_main.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3151 2024-01-19 14:05:45.000000 pywwa-1.5/tests/test_xmpp.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.418535 pywwa-1.5/tests/workflows/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2093 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      913 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_aviation.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2506 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_bufr_surface.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      454 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_cf6_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1406 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_cli_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      433 2024-01-09 22:42:41.000000 pywwa-1.5/tests/workflows/test_cwa.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      223 2024-01-09 21:00:48.000000 pywwa-1.5/tests/workflows/test_dsm2afos.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      779 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_dsm_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      342 2024-01-20 14:02:58.000000 pywwa-1.5/tests/workflows/test_ero.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      771 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_fake_afos_dump.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_fd_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      554 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_generic_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      819 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_gini2gis.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      222 2024-01-09 21:00:48.000000 pywwa-1.5/tests/workflows/test_lsr_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      281 2024-01-29 17:16:02.000000 pywwa-1.5/tests/workflows/test_mcd.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1180 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_metar_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      275 2024-01-09 21:49:01.000000 pywwa-1.5/tests/workflows/test_mos.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1046 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_nexrad3_attr.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      948 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_nldn.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      503 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_pirep_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      330 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_rr7.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    10141 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_shef_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      990 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_spammer.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      409 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_spe_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      310 2024-03-07 16:39:12.000000 pywwa-1.5/tests/workflows/test_taf_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      276 2024-01-09 21:00:48.000000 pywwa-1.5/tests/workflows/test_vtec_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      523 2024-01-09 21:00:48.000000 pywwa-1.5/tests/workflows/test_watch_parser.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      329 2024-01-09 21:49:01.000000 pywwa-1.5/tests/workflows/test_xteus.py
-drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-03-07 16:40:25.422535 pywwa-1.5/util/
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2022-02-26 13:06:57.000000 pywwa-1.5/util/archive_noaaport.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      384 2022-08-16 15:33:18.000000 pywwa-1.5/util/archive_nwwsoi.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2080 2024-03-07 16:39:12.000000 pywwa-1.5/util/check_pireps_against_aviationwx.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1546 2024-03-07 16:39:12.000000 pywwa-1.5/util/compress_madis.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1586 2024-03-07 16:39:12.000000 pywwa-1.5/util/copy_iem_network.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1783 2024-03-07 16:39:12.000000 pywwa-1.5/util/feed_archived_ncr.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    19296 2024-03-07 16:39:12.000000 pywwa-1.5/util/gen_channels_html_table.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1135 2024-03-07 16:39:12.000000 pywwa-1.5/util/get_text_from_nwschat.py
--rwxr-xr-x   0 akrherz  (43306) domain-users   (101)      217 2022-02-26 13:06:57.000000 pywwa-1.5/util/gr.csh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      368 2024-03-07 16:39:12.000000 pywwa-1.5/util/make_text_noaaportish.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3011 2024-03-07 16:39:12.000000 pywwa-1.5/util/merge_hvtec_nwsli.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     4478 2024-01-09 21:00:48.000000 pywwa-1.5/util/nwws_oi_ingest.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      332 2024-03-07 16:39:12.000000 pywwa-1.5/util/prod_feeder_loop.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     3927 2024-03-07 16:39:12.000000 pywwa-1.5/util/ridge_processor.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      409 2024-03-07 16:39:12.000000 pywwa-1.5/util/ridge_runner.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1104 2024-03-07 16:39:12.000000 pywwa-1.5/util/rotate.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2456 2024-01-10 17:11:57.000000 pywwa-1.5/util/run_examples.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1604 2024-03-07 16:39:12.000000 pywwa-1.5/util/save_iowa_level3.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      426 2023-01-30 19:55:59.000000 pywwa-1.5/util/store_madis.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1461 2024-03-07 16:39:12.000000 pywwa-1.5/util/sync_stations.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      113 2023-09-19 15:39:59.000000 pywwa-1.5/util/touch.sh
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    10852 2024-03-07 16:39:12.000000 pywwa-1.5/util/ugcs_update.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     1178 2024-03-07 16:39:12.000000 pywwa-1.5/util/unzip.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      963 2024-03-07 16:39:12.000000 pywwa-1.5/util/watch_OP5R.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      481 2024-03-07 16:39:12.000000 pywwa-1.5/util/watch_feeder.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)    10436 2024-03-07 16:39:12.000000 pywwa-1.5/util/wpc_ero_geojson.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)     2174 2024-03-07 16:39:12.000000 pywwa-1.5/util/wpc_ero_ingest.py
--rw-r--r--   0 akrherz  (43306) domain-users   (101)      715 2024-03-07 16:39:12.000000 pywwa-1.5/util/xcheck_nwwsoi.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.563000 pywwa-1.6/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       58 2020-11-30 04:37:51.000000 pywwa-1.6/.coveragerc
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      154 2021-05-03 03:44:59.000000 pywwa-1.6/.deepsource.toml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       28 2020-11-23 22:37:16.000000 pywwa-1.6/.editorconfig
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.473999 pywwa-1.6/.github/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.477999 pywwa-1.6/.github/workflows/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3800 2024-03-07 20:26:50.000000 pywwa-1.6/.github/workflows/build.yml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      833 2023-09-05 13:08:56.000000 pywwa-1.6/.github/workflows/codeql.yml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      914 2022-06-30 13:37:49.000000 pywwa-1.6/.github/workflows/etchosts.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      240 2024-01-08 13:50:35.000000 pywwa-1.6/.gitignore
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      528 2024-05-04 11:56:22.000000 pywwa-1.6/.pre-commit-config.yaml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      975 2024-05-06 11:18:35.000000 pywwa-1.6/CHANGELOG.md
+-rw-rw-r--   0 akrherz  (43306) domain-users   (101)     1065 2014-06-05 12:53:03.000000 pywwa-1.6/LICENSE
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      170 2024-03-07 20:26:50.000000 pywwa-1.6/MANIFEST.in
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      949 2024-05-06 11:18:59.562000 pywwa-1.6/PKG-INFO
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4356 2024-01-15 17:56:23.000000 pywwa-1.6/README.md
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      665 2024-03-07 16:39:12.000000 pywwa-1.6/conftest.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1005 2024-03-07 20:26:50.000000 pywwa-1.6/environment.yml
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.504999 pywwa-1.6/examples/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      273 2020-11-24 02:23:22.000000 pywwa-1.6/examples/ADA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      163 2020-11-24 02:23:22.000000 pywwa-1.6/examples/ADM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4182 2020-11-24 02:23:22.000000 pywwa-1.6/examples/ADMNES.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4025 2024-02-05 20:09:37.000000 pywwa-1.6/examples/AFD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      847 2020-11-24 02:23:22.000000 pywwa-1.6/examples/AQA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      922 2020-11-24 02:23:22.000000 pywwa-1.6/examples/AQI.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1053 2020-11-24 02:23:22.000000 pywwa-1.6/examples/AVA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1794 2024-02-22 13:46:19.000000 pywwa-1.6/examples/AVG.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1035 2020-11-24 02:23:22.000000 pywwa-1.6/examples/AVW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      912 2020-11-24 02:23:22.000000 pywwa-1.6/examples/AWU.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      489 2022-09-10 12:59:09.000000 pywwa-1.6/examples/AWW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      221 2020-11-24 02:23:22.000000 pywwa-1.6/examples/BLU.txt
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.509999 pywwa-1.6/examples/BUFR/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      741 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISAB02_CWAO.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      609 2023-12-08 19:17:06.000000 pywwa-1.6/examples/BUFR/ISAE01_SKBO.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    81301 2023-12-06 21:16:59.000000 pywwa-1.6/examples/BUFR/ISAI01_SBBR.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6714 2024-04-05 14:18:20.000000 pywwa-1.6/examples/BUFR/ISCD01_OPKC.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     7181 2024-01-03 19:07:21.000000 pywwa-1.6/examples/BUFR/ISCI01_SABM.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      834 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISIA14_CWAO.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    20732 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISMA01_FNLU.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    21528 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISMA01_FNLU_badid.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    20335 2023-12-08 17:55:39.000000 pywwa-1.6/examples/BUFR/ISMA01_FNLU_badid2.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      723 2023-12-12 19:03:23.000000 pywwa-1.6/examples/BUFR/ISMD21_UAST.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      267 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISMI60_SBBR.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1374 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISND01_LEMM.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      996 2024-01-08 21:02:34.000000 pywwa-1.6/examples/BUFR/ISNN26_LFPW.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISXD03_EDZW.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    15190 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/ISXT14_EGRR.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1644 2023-12-06 15:36:24.000000 pywwa-1.6/examples/BUFR/IS_2023120401.bufr
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1472 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CAE.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      936 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CEM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6194 2020-11-25 19:12:07.000000 pywwa-1.6/examples/CF6.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1272 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CFW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      412 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CGR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5272 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CLI.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3486 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CLIANN.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8967 2020-12-30 03:14:45.000000 pywwa-1.6/examples/CLIHOU.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2995 2022-03-20 02:32:01.000000 pywwa-1.6/examples/CLM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      145 2023-05-15 19:05:41.000000 pywwa-1.6/examples/CORM6.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      258 2023-05-15 19:05:41.000000 pywwa-1.6/examples/CORM6_RTP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1130 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CRF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      231 2022-03-20 02:32:01.000000 pywwa-1.6/examples/CWA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8810 2020-11-24 02:23:22.000000 pywwa-1.6/examples/CWF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    23693 2020-11-24 02:23:22.000000 pywwa-1.6/examples/DGT.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3545 2020-11-24 02:23:22.000000 pywwa-1.6/examples/DSM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1054 2020-11-24 02:23:22.000000 pywwa-1.6/examples/EQI.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      959 2020-11-24 02:23:22.000000 pywwa-1.6/examples/EQR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    11107 2024-01-08 18:13:05.000000 pywwa-1.6/examples/ESF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      848 2020-11-24 02:23:22.000000 pywwa-1.6/examples/EVI.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1207 2020-11-24 02:23:22.000000 pywwa-1.6/examples/EWW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    13048 2023-03-09 13:15:00.000000 pywwa-1.6/examples/FD1US1.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2519 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FFA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3319 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FFGDMX.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1506 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FFS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1600 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FFW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1183 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FFWTWC_tilde.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      728 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FLS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1603 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FLW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      699 2022-04-06 02:46:23.000000 pywwa-1.6/examples/FRW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1099 2022-04-06 03:14:34.000000 pywwa-1.6/examples/FRWOUN.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      166 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FTM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      707 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FWA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    14157 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FWF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2290 2020-11-24 02:23:22.000000 pywwa-1.6/examples/FWS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3605 2020-11-24 02:23:22.000000 pywwa-1.6/examples/GLF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      657 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HCM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      834 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HLS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3551 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HMD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    51585 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HMLARX.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1361 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HWO.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6274 2020-11-24 02:23:22.000000 pywwa-1.6/examples/HYD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3654 2020-11-24 02:23:22.000000 pywwa-1.6/examples/ICE.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      553 2020-11-24 02:23:22.000000 pywwa-1.6/examples/LAE.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5239 2020-11-24 02:23:22.000000 pywwa-1.6/examples/LCO.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      549 2021-03-25 02:33:35.000000 pywwa-1.6/examples/LSR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    54358 2022-03-17 15:58:07.000000 pywwa-1.6/examples/LWGE86.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2160 2024-01-29 17:16:02.000000 pywwa-1.6/examples/MCD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1356 2020-11-24 02:23:22.000000 pywwa-1.6/examples/METAR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3968 2020-11-24 02:23:22.000000 pywwa-1.6/examples/METNC1.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4454 2020-11-24 02:23:22.000000 pywwa-1.6/examples/MIS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1428 2020-12-26 13:10:49.000000 pywwa-1.6/examples/MPD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1385 2020-11-24 02:23:22.000000 pywwa-1.6/examples/MWS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2277 2020-11-24 02:23:22.000000 pywwa-1.6/examples/MWW.txt
+-rw-rw-r--   0 akrherz  (43306) domain-users   (101)    10245 2012-11-27 14:22:18.000000 pywwa-1.6/examples/NCR_20121127_1413
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8126 2020-05-19 20:07:00.000000 pywwa-1.6/examples/NCR_20200519_1950
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2386 2021-09-11 02:27:34.000000 pywwa-1.6/examples/NCR_20210911_0023
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2020-11-24 02:23:22.000000 pywwa-1.6/examples/NOW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      465 2024-01-09 11:42:08.000000 pywwa-1.6/examples/NOXX.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      534 2020-11-24 02:23:22.000000 pywwa-1.6/examples/NPW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3459 2020-11-24 02:23:22.000000 pywwa-1.6/examples/NSH.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2242 2020-11-24 02:23:22.000000 pywwa-1.6/examples/OAV.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      320 2020-11-24 02:23:22.000000 pywwa-1.6/examples/OMR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    14991 2020-11-24 02:23:22.000000 pywwa-1.6/examples/PFM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      746 2021-04-16 16:19:50.000000 pywwa-1.6/examples/PFWFD1.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      868 2021-04-16 16:20:04.000000 pywwa-1.6/examples/PFWFD2.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      321 2020-11-24 02:23:22.000000 pywwa-1.6/examples/PIREP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2212 2020-11-24 02:23:22.000000 pywwa-1.6/examples/PNS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2728 2023-07-27 14:51:31.000000 pywwa-1.6/examples/PNS_damage.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6053 2023-03-21 04:16:39.000000 pywwa-1.6/examples/PNS_damage_multi.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5210 2023-04-22 11:17:30.000000 pywwa-1.6/examples/PNS_damage_multi2.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5340 2020-11-24 02:23:22.000000 pywwa-1.6/examples/PSH.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2767 2020-11-24 02:23:22.000000 pywwa-1.6/examples/PTS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6765 2021-05-03 14:54:59.000000 pywwa-1.6/examples/PTSDY1.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2588 2021-04-16 16:19:20.000000 pywwa-1.6/examples/PTSDY2.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    14059 2020-11-24 02:23:22.000000 pywwa-1.6/examples/QPS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2477 2021-07-14 16:59:07.000000 pywwa-1.6/examples/RBG.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1445 2021-07-14 16:59:07.000000 pywwa-1.6/examples/RBG94E.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      805 2021-07-14 16:59:07.000000 pywwa-1.6/examples/RBG98E.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      654 2021-07-14 16:59:07.000000 pywwa-1.6/examples/RBG99E.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    24559 2020-11-24 02:23:22.000000 pywwa-1.6/examples/REC.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      338 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RER.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      564 2020-11-24 02:23:22.000000 pywwa-1.6/examples/REROKC.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      763 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RFD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2119 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RFW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      272 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RR3.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4094 2023-09-27 03:21:13.000000 pywwa-1.6/examples/RR7.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      603 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RRM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1283 2022-01-14 15:17:11.000000 pywwa-1.6/examples/RRSJAN.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5275 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RTP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3362 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RVA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1841 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RVD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1598 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RVF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      948 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RVS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1681 2020-11-24 02:23:22.000000 pywwa-1.6/examples/RWS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      541 2022-05-02 20:46:04.000000 pywwa-1.6/examples/SAW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      602 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SCPPR2.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2017 2022-05-02 20:46:04.000000 pywwa-1.6/examples/SEL.txt
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.511999 pywwa-1.6/examples/SHEF/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      273 2023-09-29 16:50:06.000000 pywwa-1.6/examples/SHEF/RR1.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       98 2023-09-26 20:12:35.000000 pywwa-1.6/examples/SHEF/RR7KRF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       64 2024-01-08 18:13:05.000000 pywwa-1.6/examples/SHEF/RR7ZOB.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     9530 2023-09-26 20:12:35.000000 pywwa-1.6/examples/SHEF/RR8KRF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      637 2023-10-28 04:01:18.000000 pywwa-1.6/examples/SHEF/RR8MSR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2023-10-28 04:01:18.000000 pywwa-1.6/examples/SHEF/RRSNMC.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      942 2021-07-23 18:27:50.000000 pywwa-1.6/examples/SHEF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      287 2020-11-30 13:25:40.000000 pywwa-1.6/examples/SIGC.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    14700 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SMF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1301 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SMW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1924 2020-11-30 04:37:51.000000 pywwa-1.6/examples/SPE.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      960 2021-03-14 03:44:33.000000 pywwa-1.6/examples/SPS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      952 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SPW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1890 2021-07-27 16:41:27.000000 pywwa-1.6/examples/SQW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2371 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SRF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4651 2020-11-24 02:23:22.000000 pywwa-1.6/examples/STF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1803 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SVR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      779 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SVS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1919 2020-11-24 02:23:22.000000 pywwa-1.6/examples/SWOMCD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      213 2021-03-23 02:10:30.000000 pywwa-1.6/examples/TAF.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1734 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TCD.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1431 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TCM.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2141 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TCP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1014 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TCU.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2206 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TIB.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1303 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TID.txt
+-rw-rw-r--   0 akrherz  (43306) domain-users   (101)    57048 2017-08-15 13:00:42.000000 pywwa-1.6/examples/TIGH05
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      410 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TOE.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1526 2021-03-18 16:14:42.000000 pywwa-1.6/examples/TOR.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      268 2020-11-24 02:23:22.000000 pywwa-1.6/examples/TWO.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      355 2020-11-24 02:23:22.000000 pywwa-1.6/examples/VAA.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1131 2020-11-24 02:23:22.000000 pywwa-1.6/examples/WCN.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3232 2020-11-24 02:23:22.000000 pywwa-1.6/examples/WCNMEG.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      185 2020-11-24 02:23:22.000000 pywwa-1.6/examples/WRK.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      425 2020-11-24 02:23:22.000000 pywwa-1.6/examples/WSV.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      513 2020-11-24 02:23:22.000000 pywwa-1.6/examples/WSW.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1038 2022-05-02 20:46:04.000000 pywwa-1.6/examples/WWP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1026 2022-05-01 19:50:13.000000 pywwa-1.6/examples/WWP9.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3214 2022-12-28 17:27:33.000000 pywwa-1.6/examples/XTEUS.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    43582 2020-11-24 02:23:22.000000 pywwa-1.6/examples/ZFP.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      532 2024-01-10 17:11:57.000000 pywwa-1.6/examples/nldn.bin
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.514999 pywwa-1.6/goes/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3303 2024-03-07 16:39:12.000000 pywwa-1.6/goes/conus_composite.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      305 2024-03-07 16:39:12.000000 pywwa-1.6/goes/greys_cmap.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3716 2019-11-22 14:49:01.000000 pywwa-1.6/goes/greysramp.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1184 2024-03-07 16:39:12.000000 pywwa-1.6/goes/ir_cmap.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4226 2019-11-22 05:04:56.000000 pywwa-1.6/goes/irramp.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3118 2024-03-07 16:39:12.000000 pywwa-1.6/goes/make_ramp_legend.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6750 2024-03-07 16:39:12.000000 pywwa-1.6/goes/netcdf2png.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      168 2022-06-28 16:13:34.000000 pywwa-1.6/goes/run_goes.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      802 2024-03-07 16:39:12.000000 pywwa-1.6/goes/wv_cmap.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3965 2019-11-22 04:42:36.000000 pywwa-1.6/goes/wvramp.txt
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.524000 pywwa-1.6/parsers/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      100 2024-01-09 21:00:48.000000 pywwa-1.6/parsers/afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      130 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/aviation.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1652 2024-01-11 03:51:07.000000 pywwa-1.6/parsers/awos_ingest.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      148 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/bufr_surface.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      131 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/cf6_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      336 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/cli_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/cwa_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      158 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/dsm2afos.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      134 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/dsm_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/ero_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      136 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/fake_afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      129 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/fd_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       95 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/ffg_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/gairmet_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      122 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/generic_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      250 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/gini2gis.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      103 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/hml_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/lsr_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      145 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/mcd_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      319 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/metar_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      119 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/mos_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      161 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/nexrad3_attr.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       97 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/nldn_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      107 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/pirep_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      128 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/rr7.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      111 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/scp_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/shef_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      165 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/spammer.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/spc_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      115 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/spe_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      153 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/split_mav.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/sps_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      111 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/taf_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      526 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/vtec_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      112 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/watch_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      116 2024-03-07 16:39:12.000000 pywwa-1.6/parsers/xteus_parser.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.526000 pywwa-1.6/pqact.d/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      647 2020-11-26 12:41:43.000000 pywwa-1.6/pqact.d/README.md
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2231 2024-02-22 13:46:19.000000 pywwa-1.6/pqact.d/pqact.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1802 2024-01-17 14:13:08.000000 pywwa-1.6/pqact.d/pqact_afos.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      187 2024-01-07 18:54:00.000000 pywwa-1.6/pqact.d/pqact_gini.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1309 2024-01-19 14:05:45.000000 pywwa-1.6/pqact.d/pqact_iemingest.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       94 2024-01-07 18:54:00.000000 pywwa-1.6/pqact.d/pqact_nexrad.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      926 2024-01-07 18:54:00.000000 pywwa-1.6/pqact.d/pqact_shef.conf
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3019 2024-04-03 15:12:41.000000 pywwa-1.6/pyproject.toml
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      352 2024-01-07 18:54:00.000000 pywwa-1.6/pywwa_settings.json-example
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       38 2024-05-06 11:18:59.563000 pywwa-1.6/setup.cfg
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       61 2024-03-07 20:26:50.000000 pywwa-1.6/setup.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.473999 pywwa-1.6/src/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.527999 pywwa-1.6/src/pywwa/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1713 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/__init__.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8479 2024-04-19 17:42:39.000000 pywwa-1.6/src/pywwa/common.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.535000 pywwa-1.6/src/pywwa/data/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)   136412 2024-01-07 18:54:00.000000 pywwa-1.6/src/pywwa/data/conus.shp
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      108 2024-01-07 18:54:00.000000 pywwa-1.6/src/pywwa/data/conus.shx
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)  1497650 2024-01-07 18:54:00.000000 pywwa-1.6/src/pywwa/data/faa_apt.tbl
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    16560 2024-01-07 18:54:00.000000 pywwa-1.6/src/pywwa/data/nexrad.stns
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)   514809 2024-04-11 12:59:37.000000 pywwa-1.6/src/pywwa/data/pirep_navaids.tbl
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    30715 2024-01-07 18:54:00.000000 pywwa-1.6/src/pywwa/data/vors.tbl
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3049 2024-04-03 15:12:41.000000 pywwa-1.6/src/pywwa/data/wmo2iso3166.tbl
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3526 2024-01-11 03:51:07.000000 pywwa-1.6/src/pywwa/database.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1923 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/ldm.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5248 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/ldmbridge.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      501 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/memclient.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      436 2024-03-07 20:26:50.000000 pywwa-1.6/src/pywwa/testing.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.544000 pywwa-1.6/src/pywwa/workflows/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)       30 2024-01-09 21:00:48.000000 pywwa-1.6/src/pywwa/workflows/__init__.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2792 2024-04-19 17:42:39.000000 pywwa-1.6/src/pywwa/workflows/afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2201 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/aviation.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    14950 2024-04-05 14:18:20.000000 pywwa-1.6/src/pywwa/workflows/bufr_surface.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      630 2024-01-09 21:49:01.000000 pywwa-1.6/src/pywwa/workflows/cf6.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1674 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/cli.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2367 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/cwa.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1491 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/dsm.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1083 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/dsm2afos.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      895 2024-01-11 03:51:07.000000 pywwa-1.6/src/pywwa/workflows/ero.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2689 2024-04-19 17:42:39.000000 pywwa-1.6/src/pywwa/workflows/fake_afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      639 2024-01-09 21:49:01.000000 pywwa-1.6/src/pywwa/workflows/fd.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      791 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/ffg.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      601 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/gairmet.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2192 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/generic.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8205 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/gini2gis.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      604 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/hml.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2526 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/lsr.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1411 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/mcd.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     5243 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/metar.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      663 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/mos.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     6122 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/nexrad3_attr.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/nldn.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3476 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/pirep.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      774 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/rr7.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      614 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/scp.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    20127 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/shef.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3840 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/spammer.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      898 2024-01-11 03:51:07.000000 pywwa-1.6/src/pywwa/workflows/spc.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1418 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/spe.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1691 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/split_mav.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1244 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/sps.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      797 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/taf.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2853 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/vtec.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2769 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/watch.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      596 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/workflows/xteus.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8002 2024-03-07 16:39:12.000000 pywwa-1.6/src/pywwa/xmpp.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.562000 pywwa-1.6/src/pywwa.egg-info/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      949 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/PKG-INFO
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     8146 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/SOURCES.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        1 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/dependency_links.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1673 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/entry_points.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      142 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/requires.txt
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)        6 2024-05-06 11:18:59.000000 pywwa-1.6/src/pywwa.egg-info/top_level.txt
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.547000 pywwa-1.6/tests/
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.547000 pywwa-1.6/tests/bin/
+-rwxr-xr-x   0 akrherz  (43306) domain-users   (101)       26 2023-09-27 19:09:12.000000 pywwa-1.6/tests/bin/pqinsert
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1102 2024-04-19 17:42:39.000000 pywwa-1.6/tests/test_common.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      533 2024-03-07 16:39:12.000000 pywwa-1.6/tests/test_common_syslog.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      446 2024-01-09 21:00:48.000000 pywwa-1.6/tests/test_database.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      609 2024-03-07 16:39:12.000000 pywwa-1.6/tests/test_init.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      159 2024-03-07 16:39:12.000000 pywwa-1.6/tests/test_ldm.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      984 2024-03-07 16:39:12.000000 pywwa-1.6/tests/test_ldmbridge.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1269 2024-03-07 16:39:12.000000 pywwa-1.6/tests/test_workflow_main.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3151 2024-01-19 14:05:45.000000 pywwa-1.6/tests/test_xmpp.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.555000 pywwa-1.6/tests/workflows/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2095 2024-04-03 15:12:41.000000 pywwa-1.6/tests/workflows/test_afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      913 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_aviation.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2506 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_bufr_surface.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      454 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_cf6_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1406 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_cli_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      433 2024-01-09 22:42:41.000000 pywwa-1.6/tests/workflows/test_cwa.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      223 2024-01-09 21:00:48.000000 pywwa-1.6/tests/workflows/test_dsm2afos.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      779 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_dsm_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      342 2024-01-20 14:02:58.000000 pywwa-1.6/tests/workflows/test_ero.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      771 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_fake_afos_dump.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      453 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_fd_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      554 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_generic_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      819 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_gini2gis.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      222 2024-01-09 21:00:48.000000 pywwa-1.6/tests/workflows/test_lsr_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      281 2024-01-29 17:16:02.000000 pywwa-1.6/tests/workflows/test_mcd.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1180 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_metar_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      275 2024-01-09 21:49:01.000000 pywwa-1.6/tests/workflows/test_mos.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1046 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_nexrad3_attr.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      948 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_nldn.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      503 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_pirep_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      330 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_rr7.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    10141 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_shef_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      990 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_spammer.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      409 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_spe_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      310 2024-03-07 16:39:12.000000 pywwa-1.6/tests/workflows/test_taf_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      276 2024-01-09 21:00:48.000000 pywwa-1.6/tests/workflows/test_vtec_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      523 2024-01-09 21:00:48.000000 pywwa-1.6/tests/workflows/test_watch_parser.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      329 2024-01-09 21:49:01.000000 pywwa-1.6/tests/workflows/test_xteus.py
+drwxr-xr-x   0 akrherz  (43306) domain-users   (101)        0 2024-05-06 11:18:59.562000 pywwa-1.6/util/
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      676 2022-02-26 13:06:57.000000 pywwa-1.6/util/archive_noaaport.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      384 2022-08-16 15:33:18.000000 pywwa-1.6/util/archive_nwwsoi.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3663 2024-04-06 16:14:54.000000 pywwa-1.6/util/awx_metar_supplement.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2078 2024-04-03 15:12:41.000000 pywwa-1.6/util/check_pireps_against_aviationwx.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1546 2024-03-07 16:39:12.000000 pywwa-1.6/util/compress_madis.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1586 2024-03-07 16:39:12.000000 pywwa-1.6/util/copy_iem_network.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1783 2024-03-07 16:39:12.000000 pywwa-1.6/util/feed_archived_ncr.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    19206 2024-05-04 11:56:58.000000 pywwa-1.6/util/gen_channels_html_table.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1135 2024-03-07 16:39:12.000000 pywwa-1.6/util/get_text_from_nwschat.py
+-rwxr-xr-x   0 akrherz  (43306) domain-users   (101)      217 2022-02-26 13:06:57.000000 pywwa-1.6/util/gr.csh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      368 2024-03-07 16:39:12.000000 pywwa-1.6/util/make_text_noaaportish.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3011 2024-03-07 16:39:12.000000 pywwa-1.6/util/merge_hvtec_nwsli.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     4478 2024-01-09 21:00:48.000000 pywwa-1.6/util/nwws_oi_ingest.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      332 2024-03-07 16:39:12.000000 pywwa-1.6/util/prod_feeder_loop.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     3927 2024-03-07 16:39:12.000000 pywwa-1.6/util/ridge_processor.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      409 2024-03-07 16:39:12.000000 pywwa-1.6/util/ridge_runner.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1104 2024-03-07 16:39:12.000000 pywwa-1.6/util/rotate.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2456 2024-01-10 17:11:57.000000 pywwa-1.6/util/run_examples.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1604 2024-03-07 16:39:12.000000 pywwa-1.6/util/save_iowa_level3.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      426 2023-01-30 19:55:59.000000 pywwa-1.6/util/store_madis.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1461 2024-03-07 16:39:12.000000 pywwa-1.6/util/sync_stations.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      113 2023-09-19 15:39:59.000000 pywwa-1.6/util/touch.sh
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    10852 2024-03-07 16:39:12.000000 pywwa-1.6/util/ugcs_update.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     1178 2024-03-07 16:39:12.000000 pywwa-1.6/util/unzip.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      963 2024-03-07 16:39:12.000000 pywwa-1.6/util/watch_OP5R.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      481 2024-03-07 16:39:12.000000 pywwa-1.6/util/watch_feeder.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)    10817 2024-04-17 16:52:01.000000 pywwa-1.6/util/wpc_ero_geojson.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)     2174 2024-03-07 16:39:12.000000 pywwa-1.6/util/wpc_ero_ingest.py
+-rw-r--r--   0 akrherz  (43306) domain-users   (101)      715 2024-03-07 16:39:12.000000 pywwa-1.6/util/xcheck_nwwsoi.py
```

### Comparing `pywwa-1.5/.github/workflows/build.yml` & `pywwa-1.6/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         python util/copy_iem_network.py NY_COOP
         python util/copy_iem_network.py NWSCLI
         python util/copy_iem_network.py NEXRAD
         python util/copy_iem_network.py TWDR
         sh util/run_examples.sh
         # get pqinsert available as a dummy command
         export PATH=$PATH:$(pwd)/tests/bin
-        coverage run --source=pywwa setup.py test
-        coverage xml
+        python -m pytest -vv --cov=pywwa --cov-report=xml
 
     - name: Run console scripts without database
       run: |
         set -x
         set -e
         sudo systemctl stop postgresql@15-main.service
         sudo cp /etc/hosts.save /etc/hosts
```

### Comparing `pywwa-1.5/.github/workflows/codeql.yml` & `pywwa-1.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/.github/workflows/etchosts.txt` & `pywwa-1.6/.github/workflows/etchosts.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/CHANGELOG.md` & `pywwa-1.6/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 <!-- markdownlint-configure-file {"MD024": { "siblings_only": true } } -->
 # Changelog
 
 All notable changes to this library are documented in this file.
 
+## **1.6.0** (6 May 2024)
+
+### API Changes
+
+- Change AFOS database save to not include windows carriage return nor the
+start of product ``\001`` control character.
+
+### New Features
+
+### Bug Fixes
+
+- Correct `get_example_filepath` logic to assume `pwd` for location of examples.
+- Swallow BUFR situation of year==0, which is likely some climatology product?
+
 ## **1.5.0** (7 Mar 2024)
 
 ### API Changes
 
 ### New Features
 
 - [SHEF] Add `pywwa_shef_afos_exclude` setting to allow skipping ill-formed
```

### Comparing `pywwa-1.5/LICENSE` & `pywwa-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/README.md` & `pywwa-1.6/README.md`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/conftest.py` & `pywwa-1.6/conftest.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/environment.yml` & `pywwa-1.6/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
  # Models
  - pydantic
  # Used by wpc_ero_geojson
  - pyogrio
  # gini reader
  - pyproj
  - pytest
+ - pytest-cov
  - pytest-mpl
  - pytest-runner
  # For testing
  - pytest-twisted
  - rasterstats
  # util scripts
  - requests
```

### Comparing `pywwa-1.5/examples/ADMNES.txt` & `pywwa-1.6/examples/ADMNES.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AFD.txt` & `pywwa-1.6/examples/AFD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AQA.txt` & `pywwa-1.6/examples/AQA.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AQI.txt` & `pywwa-1.6/examples/AQI.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AVA.txt` & `pywwa-1.6/examples/AVA.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AVG.txt` & `pywwa-1.6/examples/AVG.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AVW.txt` & `pywwa-1.6/examples/AVW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/AWU.txt` & `pywwa-1.6/examples/AWU.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISAB02_CWAO.bufr` & `pywwa-1.6/examples/BUFR/ISAB02_CWAO.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISAE01_SKBO.bufr` & `pywwa-1.6/examples/BUFR/ISAE01_SKBO.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISAI01_SBBR.bufr` & `pywwa-1.6/examples/BUFR/ISAI01_SBBR.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISCI01_SABM.bufr` & `pywwa-1.6/examples/BUFR/ISCI01_SABM.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISIA14_CWAO.bufr` & `pywwa-1.6/examples/BUFR/ISIA14_CWAO.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISMA01_FNLU.bufr` & `pywwa-1.6/examples/BUFR/ISMA01_FNLU.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISMA01_FNLU_badid.bufr` & `pywwa-1.6/examples/BUFR/ISMA01_FNLU_badid.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISMA01_FNLU_badid2.bufr` & `pywwa-1.6/examples/BUFR/ISMA01_FNLU_badid2.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISMD21_UAST.bufr` & `pywwa-1.6/examples/BUFR/ISMD21_UAST.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISND01_LEMM.bufr` & `pywwa-1.6/examples/BUFR/ISND01_LEMM.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISNN26_LFPW.bufr` & `pywwa-1.6/examples/BUFR/ISNN26_LFPW.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/ISXT14_EGRR.bufr` & `pywwa-1.6/examples/BUFR/ISXT14_EGRR.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/BUFR/IS_2023120401.bufr` & `pywwa-1.6/examples/BUFR/IS_2023120401.bufr`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CAE.txt` & `pywwa-1.6/examples/CAE.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CEM.txt` & `pywwa-1.6/examples/CEM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CF6.txt` & `pywwa-1.6/examples/CF6.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CFW.txt` & `pywwa-1.6/examples/CFW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CLI.txt` & `pywwa-1.6/examples/CLI.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CLIANN.txt` & `pywwa-1.6/examples/CLIANN.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CLIHOU.txt` & `pywwa-1.6/examples/CLIHOU.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CLM.txt` & `pywwa-1.6/examples/CLM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CRF.txt` & `pywwa-1.6/examples/CRF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/CWF.txt` & `pywwa-1.6/examples/CWF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/DGT.txt` & `pywwa-1.6/examples/DGT.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/DSM.txt` & `pywwa-1.6/examples/DSM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/EQI.txt` & `pywwa-1.6/examples/EQI.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/EQR.txt` & `pywwa-1.6/examples/EQR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/ESF.txt` & `pywwa-1.6/examples/ESF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/EVI.txt` & `pywwa-1.6/examples/EVI.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/EWW.txt` & `pywwa-1.6/examples/EWW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FD1US1.txt` & `pywwa-1.6/examples/FD1US1.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FFA.txt` & `pywwa-1.6/examples/FFA.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FFGDMX.txt` & `pywwa-1.6/examples/FFGDMX.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FFS.txt` & `pywwa-1.6/examples/FFS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FFW.txt` & `pywwa-1.6/examples/FFW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FFWTWC_tilde.txt` & `pywwa-1.6/examples/FFWTWC_tilde.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FLS.txt` & `pywwa-1.6/examples/FLS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FLW.txt` & `pywwa-1.6/examples/FLW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FRW.txt` & `pywwa-1.6/examples/FRW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FRWOUN.txt` & `pywwa-1.6/examples/FRWOUN.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FWA.txt` & `pywwa-1.6/examples/FWA.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FWF.txt` & `pywwa-1.6/examples/FWF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/FWS.txt` & `pywwa-1.6/examples/FWS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/GLF.txt` & `pywwa-1.6/examples/GLF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HCM.txt` & `pywwa-1.6/examples/HCM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HLS.txt` & `pywwa-1.6/examples/HLS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HMD.txt` & `pywwa-1.6/examples/HMD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HMLARX.txt` & `pywwa-1.6/examples/HMLARX.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HWO.txt` & `pywwa-1.6/examples/HWO.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/HYD.txt` & `pywwa-1.6/examples/HYD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/ICE.txt` & `pywwa-1.6/examples/ICE.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/LAE.txt` & `pywwa-1.6/examples/LAE.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/LCO.txt` & `pywwa-1.6/examples/LCO.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/LSR.txt` & `pywwa-1.6/examples/LSR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/LWGE86.txt` & `pywwa-1.6/examples/LWGE86.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/MCD.txt` & `pywwa-1.6/examples/MCD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/METAR.txt` & `pywwa-1.6/examples/METAR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/METNC1.txt` & `pywwa-1.6/examples/METNC1.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/MIS.txt` & `pywwa-1.6/examples/MIS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/MPD.txt` & `pywwa-1.6/examples/MPD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/MWS.txt` & `pywwa-1.6/examples/MWS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/MWW.txt` & `pywwa-1.6/examples/MWW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/NCR_20121127_1413` & `pywwa-1.6/examples/NCR_20121127_1413`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/NCR_20200519_1950` & `pywwa-1.6/examples/NCR_20200519_1950`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/NCR_20210911_0023` & `pywwa-1.6/examples/NCR_20210911_0023`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/NPW.txt` & `pywwa-1.6/examples/NPW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/NSH.txt` & `pywwa-1.6/examples/NSH.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/OAV.txt` & `pywwa-1.6/examples/OAV.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PFM.txt` & `pywwa-1.6/examples/PFM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PFWFD1.txt` & `pywwa-1.6/examples/PFWFD1.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PFWFD2.txt` & `pywwa-1.6/examples/PFWFD2.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PNS.txt` & `pywwa-1.6/examples/PNS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PNS_damage.txt` & `pywwa-1.6/examples/PNS_damage.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PNS_damage_multi.txt` & `pywwa-1.6/examples/PNS_damage_multi.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PNS_damage_multi2.txt` & `pywwa-1.6/examples/PNS_damage_multi2.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PSH.txt` & `pywwa-1.6/examples/PSH.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PTS.txt` & `pywwa-1.6/examples/PTS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PTSDY1.txt` & `pywwa-1.6/examples/PTSDY1.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/PTSDY2.txt` & `pywwa-1.6/examples/PTSDY2.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/QPS.txt` & `pywwa-1.6/examples/QPS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RBG.txt` & `pywwa-1.6/examples/RBG.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RBG94E.txt` & `pywwa-1.6/examples/RBG94E.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RBG98E.txt` & `pywwa-1.6/examples/RBG98E.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RBG99E.txt` & `pywwa-1.6/examples/RBG99E.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/REC.txt` & `pywwa-1.6/examples/REC.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/REROKC.txt` & `pywwa-1.6/examples/REROKC.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RFD.txt` & `pywwa-1.6/examples/RFD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RFW.txt` & `pywwa-1.6/examples/RFW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RR7.txt` & `pywwa-1.6/examples/RR7.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RRM.txt` & `pywwa-1.6/examples/RRM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RRSJAN.txt` & `pywwa-1.6/examples/RRSJAN.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RTP.txt` & `pywwa-1.6/examples/RTP.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RVA.txt` & `pywwa-1.6/examples/RVA.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RVD.txt` & `pywwa-1.6/examples/RVD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RVF.txt` & `pywwa-1.6/examples/RVF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RVS.txt` & `pywwa-1.6/examples/RVS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/RWS.txt` & `pywwa-1.6/examples/RWS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SAW.txt` & `pywwa-1.6/examples/SAW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SCPPR2.txt` & `pywwa-1.6/examples/SCPPR2.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SEL.txt` & `pywwa-1.6/examples/SEL.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SHEF/RR8KRF.txt` & `pywwa-1.6/examples/SHEF/RR8KRF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SHEF/RR8MSR.txt` & `pywwa-1.6/examples/SHEF/RR8MSR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SHEF.txt` & `pywwa-1.6/examples/SHEF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SMF.txt` & `pywwa-1.6/examples/SMF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SMW.txt` & `pywwa-1.6/examples/SMW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SPE.txt` & `pywwa-1.6/examples/SPE.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SPS.txt` & `pywwa-1.6/examples/SPS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SPW.txt` & `pywwa-1.6/examples/SPW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SQW.txt` & `pywwa-1.6/examples/SQW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SRF.txt` & `pywwa-1.6/examples/SRF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/STF.txt` & `pywwa-1.6/examples/STF.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SVR.txt` & `pywwa-1.6/examples/SVR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SVS.txt` & `pywwa-1.6/examples/SVS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/SWOMCD.txt` & `pywwa-1.6/examples/SWOMCD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TCD.txt` & `pywwa-1.6/examples/TCD.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TCM.txt` & `pywwa-1.6/examples/TCM.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TCP.txt` & `pywwa-1.6/examples/TCP.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TCU.txt` & `pywwa-1.6/examples/TCU.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TIB.txt` & `pywwa-1.6/examples/TIB.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TID.txt` & `pywwa-1.6/examples/TID.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TIGH05` & `pywwa-1.6/examples/TIGH05`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/TOR.txt` & `pywwa-1.6/examples/TOR.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/WCN.txt` & `pywwa-1.6/examples/WCN.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/WCNMEG.txt` & `pywwa-1.6/examples/WCNMEG.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/WSW.txt` & `pywwa-1.6/examples/WSW.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/WWP.txt` & `pywwa-1.6/examples/WWP.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/WWP9.txt` & `pywwa-1.6/examples/WWP9.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/XTEUS.txt` & `pywwa-1.6/examples/XTEUS.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/ZFP.txt` & `pywwa-1.6/examples/ZFP.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/examples/nldn.bin` & `pywwa-1.6/examples/nldn.bin`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/conus_composite.py` & `pywwa-1.6/goes/conus_composite.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/greysramp.txt` & `pywwa-1.6/goes/greysramp.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/ir_cmap.py` & `pywwa-1.6/goes/ir_cmap.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/irramp.txt` & `pywwa-1.6/goes/irramp.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/make_ramp_legend.py` & `pywwa-1.6/goes/make_ramp_legend.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/netcdf2png.py` & `pywwa-1.6/goes/netcdf2png.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/wv_cmap.py` & `pywwa-1.6/goes/wv_cmap.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/goes/wvramp.txt` & `pywwa-1.6/goes/wvramp.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/parsers/awos_ingest.py` & `pywwa-1.6/parsers/awos_ingest.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/parsers/vtec_parser.py` & `pywwa-1.6/parsers/vtec_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/pqact.d/README.md` & `pywwa-1.6/pqact.d/README.md`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/pqact.d/pqact.conf` & `pywwa-1.6/pqact.d/pqact.conf`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/pqact.d/pqact_afos.conf` & `pywwa-1.6/pqact.d/pqact_afos.conf`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/pqact.d/pqact_iemingest.conf` & `pywwa-1.6/pqact.d/pqact_iemingest.conf`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/pqact.d/pqact_shef.conf` & `pywwa-1.6/pqact.d/pqact_shef.conf`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/__init__.py` & `pywwa-1.6/src/pywwa/__init__.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/common.py` & `pywwa-1.6/src/pywwa/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,14 +200,26 @@
 
 def disable_xmpp(f):
     """Decorator to disable XMPP."""
     f.disable_xmpp = True
     return f
 
 
+def afosclean(text: str) -> str:
+    """Clean a string for AFOS database storage.
+
+    Removes the \r \001 and \003 characters, trims whitespace and
+    slaps one \n at the end of the string.
+    """
+    return (
+        text.replace("\r", "").replace("\001", "").replace("\003", "").strip()
+        + "\n"
+    )
+
+
 def init(f):
     """Decorator to setup all things."""
 
     @click.option(
         "-d",
         "--disable-dbwrite",
         is_flag=True,
```

### Comparing `pywwa-1.5/src/pywwa/data/conus.shp` & `pywwa-1.6/src/pywwa/data/conus.shp`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/data/faa_apt.tbl` & `pywwa-1.6/src/pywwa/data/faa_apt.tbl`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/data/nexrad.stns` & `pywwa-1.6/src/pywwa/data/nexrad.stns`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/data/pirep_navaids.tbl` & `pywwa-1.6/src/pywwa/data/pirep_navaids.tbl`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,15 @@
 CEU2            Beaverlodge                      -- CA  5518 -11945     0  0
 CEU8            Norman Wells                     -- CA  6526 -12669     0  0
 CEU9            Trout Lake                       -- CA  6042 -12127     0  0
 CEV3            Vegreville                       -- CA  5351 -11203     0  0
 CEV5            Mayerthorpe                      -- CA  5394 -11518     0  0
 CEV7            Tofield                          -- CA  5337 -11270     0  0
 CEW3            St Paul                          -- CA  5399 -11138     0  0
+CEW7            Edmonton - Stollery              AB CA  5352 -11352     0  0
 CEW9            Canmore                          -- CA  5108 -11534     0  0
 CEX3            Wetaskiwin                       -- CA  5297 -11341     0  0
 CEY3            Fort Macleod                     -- CA  4970 -11342     0  0
 ## CEYV
 CEZ3            Edmonton                         -- CA  5343 -11312     0  0
 CEZ4            Fort Vermillion                  -- CA  5840 -11595     0  0
 CEZ5            Whitehorse Seaplane              -- CA  6069 -13504     0  0
@@ -412,14 +413,15 @@
 CMA2            Mattawa                          ON CA  4630  -7875     0  0
 CMB2            Meadowbank                       -- CA  6503  -9607     0  0
 CMB7            Maxville                         -- CA  4525  -7481     0  0
 CMB9            Port Renfrew Mill Bay            -- CA  4856 -12441     0  0
 CMF2            Edmonton Calmar Maplelane        AB CA  5318 -11374     0  0
 CMH3            Lacombe                          AB CA  5238 -11382     0  0
 CML2            Quamichan Lake Raven             BC CA  4882 -12365     0  0
+CML8            St Mathieu de Laprairie          QC CA  4531  -7357     0  0
 CMN5            Manic-5                          -- CA  5066  -6883     0  0
 CMR2            Mary River                       -- CA  7132  -7935     0  0
 CMW3            Matawatchan                      ON CA  4516  -7710     0  0
 CMX2            Maxville                         -- CA  4530  -7485     0  0
 CNA3            Springwater Barrie               -- CA  4441  -7973     0  0
 CNA4            Emsdale                          -- CA  4555  -7935     0  0
 CNA9            Tomvale                          -- CA  4492  -7694     0  0
@@ -499,14 +501,15 @@
 CPQ3            Niagra Falls Heliport            ON CA  4312  -7908     0  0
 CPR3            Palmerston                       -- CA  4385  -8078     0  0
 CPR5            Woodstock                        -- CA  4311  -8082     0  0
 CPR7            Wingham                          -- CA  4387  -8129     0  0
 CPS1            Parry Sound Harbour              ON CA  4534  -8003     0  0
 CPS2            Elmhirst Resort                  -- CA  4425  -7811     0  0
 CPS4            Lucan                            -- CA  4316  -8141     0  0
+CPS5            Miminiska                        ON CA  5160  -8858     0  0
 CPT2            Killarney                        -- CA  4598  -8150     0  0
 CPT3            Rockton                          -- CA  4332  -8018     0  0
 CPT9            Pintendre                        QB CA  4676  -7111     0  0
 CPU6            Tyendinaga Mohawk                -- CA  4419  -7711     0  0
 CPV2            Orangeville Castlewood Field     ON CA  4396  -8016     0  0
 CPV7            Poplar Hill                      -- CA  5211  -9426     0  0
 CPV8            Keewaywin                        -- CA  5299  -9284     0  0
```

### Comparing `pywwa-1.5/src/pywwa/data/vors.tbl` & `pywwa-1.6/src/pywwa/data/vors.tbl`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/data/wmo2iso3166.tbl` & `pywwa-1.6/src/pywwa/data/wmo2iso3166.tbl`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 SAWB 32 Argentina
 SCSC 152 Chile
 SGAS 858 Uruguay
 SKBO 170 Colombia
 SBBR 76 Brazil
 SEQU 218 Ecuador
 SLLP 68 Bolivia
+SMJP 740 Suriname
 SOCA 74 French Guiana
 SOWR 724 Spain
 SPIM 604 Peru
 SUMU 858 Uruguay
 TBPB 52 Barbados
 TLPC 662 Saint Lucia
 TLPL 662 Saint Lucia
```

### Comparing `pywwa-1.5/src/pywwa/database.py` & `pywwa-1.6/src/pywwa/database.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/ldm.py` & `pywwa-1.6/src/pywwa/ldm.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/ldmbridge.py` & `pywwa-1.6/src/pywwa/ldmbridge.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/afos_dump.py` & `pywwa-1.6/src/pywwa/workflows/afos_dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     nws = product.TextProduct(buf, utcnow=utcnow, parse_segments=False)
 
     # When we are in realtime processing, do not consider old data, typically
     # when a WFO fails to update the date in their MND
     if not common.replace_enabled():
         delta = (nws.valid - utcnow).total_seconds()
         if delta < (-180 * 86400):  # 180 days
-            raise Exception(f"Very Latent Product! {nws.valid}")
+            raise ValueError(f"Very Latent Product! {nws.valid}")
         if delta > (6 * 3600):  # Six Hours
-            raise Exception(f"Product from the future! {nws.valid}")
+            raise ValueError(f"Product from the future! {nws.valid}")
     if nws.warnings:
         common.email_error("\n".join(nws.warnings), buf)
     if nws.afos is None:
         if nws.source[0] not in ["K", "P"]:
             return None
-        raise Exception("TextProduct.afos is null")
+        raise ValueError("TextProduct.afos is null")
 
     if common.replace_enabled():
         args = [nws.afos.strip(), nws.source, nws.valid]
         bbb = ""
         if nws.bbb:
             bbb = " and bbb = %s "
             args.append(nws.bbb)
@@ -70,15 +70,22 @@
             args,
         )
         LOG.info("Removed %s rows for %s", txn.rowcount, nws.get_product_id())
 
     txn.execute(
         "INSERT into products (pil, data, entered, "
         "source, wmo, bbb) VALUES(%s, %s, %s, %s, %s, %s)",
-        (nws.afos.strip(), nws.text, nws.valid, nws.source, nws.wmo, nws.bbb),
+        (
+            nws.afos.strip(),
+            common.afosclean(nws.text),
+            nws.valid,
+            nws.source,
+            nws.wmo,
+            nws.bbb,
+        ),
     )
     if nws.afos[:3] in MEMCACHE_EXCLUDE:
         return None
     # We are on a thread, so we need to send this back to the main thread
     reactor.callFromThread(write2memcache, nws.get_product_id(), nws.unixtext)
     return nws
```

### Comparing `pywwa-1.5/src/pywwa/workflows/aviation.py` & `pywwa-1.6/src/pywwa/workflows/aviation.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/bufr_surface.py` & `pywwa-1.6/src/pywwa/workflows/bufr_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             data["gust"] = bounds_check(
                 convert_value(msg["value"], "meter per second", "knot"), 0, 200
             )
             continue
         if msg["id"] == "011043" and displacement >= -10:
             data["gust_drct"] = bounds_check(msg["value"], 0, 360)
             continue
-    if "year" not in data:
+    if "year" not in data or data["year"] == 0:
         return {}
     data["valid"] = utc(
         data["year"],
         data["month"],
         data["day"],
         data.get("hour", 0),  # Unsure if this is too forgiving
         data.get("minute", 0),
```

### Comparing `pywwa-1.5/src/pywwa/workflows/cf6.py` & `pywwa-1.6/src/pywwa/workflows/cf6.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/cli.py` & `pywwa-1.6/src/pywwa/workflows/cli.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/cwa.py` & `pywwa-1.6/src/pywwa/workflows/cwa.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/dsm.py` & `pywwa-1.6/src/pywwa/workflows/dsm.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/dsm2afos.py` & `pywwa-1.6/src/pywwa/workflows/dsm2afos.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/ero.py` & `pywwa-1.6/src/pywwa/workflows/ero.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/fake_afos_dump.py` & `pywwa-1.6/src/pywwa/workflows/fake_afos_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     sql = (
         "INSERT into products "
         "(pil, data, source, wmo, entered, bbb) values(%s,%s,%s,%s,%s,%s)"
     )
 
     sqlargs = (
         tp.afos,
-        tp.text,
+        common.afosclean(tp.text),
         tp.source,
         tp.wmo,
         tp.valid.strftime("%Y-%m-%d %H:%M+00"),
         tp.bbb,
     )
     if common.dbwrite_enabled():
         txn.execute(sql, sqlargs)
```

### Comparing `pywwa-1.5/src/pywwa/workflows/fd.py` & `pywwa-1.6/src/pywwa/workflows/fd.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/ffg.py` & `pywwa-1.6/src/pywwa/workflows/ffg.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/gairmet.py` & `pywwa-1.6/src/pywwa/workflows/gairmet.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/generic.py` & `pywwa-1.6/src/pywwa/workflows/generic.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/gini2gis.py` & `pywwa-1.6/src/pywwa/workflows/gini2gis.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/hml.py` & `pywwa-1.6/src/pywwa/workflows/hml.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/lsr.py` & `pywwa-1.6/src/pywwa/workflows/lsr.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/mcd.py` & `pywwa-1.6/src/pywwa/workflows/mcd.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/metar.py` & `pywwa-1.6/src/pywwa/workflows/metar.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/mos.py` & `pywwa-1.6/src/pywwa/workflows/mos.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/nexrad3_attr.py` & `pywwa-1.6/src/pywwa/workflows/nexrad3_attr.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/nldn.py` & `pywwa-1.6/src/pywwa/workflows/nldn.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/pirep.py` & `pywwa-1.6/src/pywwa/workflows/pirep.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/rr7.py` & `pywwa-1.6/src/pywwa/workflows/rr7.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/scp.py` & `pywwa-1.6/src/pywwa/workflows/scp.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/shef.py` & `pywwa-1.6/src/pywwa/workflows/shef.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/spammer.py` & `pywwa-1.6/src/pywwa/workflows/spammer.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/spc.py` & `pywwa-1.6/src/pywwa/workflows/spc.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/spe.py` & `pywwa-1.6/src/pywwa/workflows/spe.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/split_mav.py` & `pywwa-1.6/src/pywwa/workflows/split_mav.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/sps.py` & `pywwa-1.6/src/pywwa/workflows/sps.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/taf.py` & `pywwa-1.6/src/pywwa/workflows/taf.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/vtec.py` & `pywwa-1.6/src/pywwa/workflows/vtec.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/watch.py` & `pywwa-1.6/src/pywwa/workflows/watch.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/workflows/xteus.py` & `pywwa-1.6/src/pywwa/workflows/xteus.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa/xmpp.py` & `pywwa-1.6/src/pywwa/xmpp.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/src/pywwa.egg-info/SOURCES.txt` & `pywwa-1.6/src/pywwa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 LICENSE
 MANIFEST.in
 README.md
 conftest.py
 environment.yml
 pyproject.toml
 pywwa_settings.json-example
-setup.cfg
 setup.py
 .github/workflows/build.yml
 .github/workflows/codeql.yml
 .github/workflows/etchosts.txt
 examples/ADA.txt
 examples/ADM.txt
 examples/ADMNES.txt
@@ -160,14 +159,15 @@
 examples/WWP9.txt
 examples/XTEUS.txt
 examples/ZFP.txt
 examples/nldn.bin
 examples/BUFR/ISAB02_CWAO.bufr
 examples/BUFR/ISAE01_SKBO.bufr
 examples/BUFR/ISAI01_SBBR.bufr
+examples/BUFR/ISCD01_OPKC.bufr
 examples/BUFR/ISCI01_SABM.bufr
 examples/BUFR/ISIA14_CWAO.bufr
 examples/BUFR/ISMA01_FNLU.bufr
 examples/BUFR/ISMA01_FNLU_badid.bufr
 examples/BUFR/ISMA01_FNLU_badid2.bufr
 examples/BUFR/ISMD21_UAST.bufr
 examples/BUFR/ISMI60_SBBR.bufr
@@ -327,14 +327,15 @@
 tests/workflows/test_spe_parser.py
 tests/workflows/test_taf_parser.py
 tests/workflows/test_vtec_parser.py
 tests/workflows/test_watch_parser.py
 tests/workflows/test_xteus.py
 util/archive_noaaport.sh
 util/archive_nwwsoi.sh
+util/awx_metar_supplement.py
 util/check_pireps_against_aviationwx.py
 util/compress_madis.py
 util/copy_iem_network.py
 util/feed_archived_ncr.py
 util/gen_channels_html_table.py
 util/get_text_from_nwschat.py
 util/gr.csh
```

### Comparing `pywwa-1.5/src/pywwa.egg-info/entry_points.txt` & `pywwa-1.6/src/pywwa.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/test_common.py` & `pywwa-1.6/tests/test_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """Test pywwa.common"""
 
 from pyiem.util import utc
 from pywwa import CTX, common
 
 
+def test_afosclean():
+    """Test that we strip things right."""
+    instr = "\001\r\r\n000 \r\r\nDARYL\r\r"
+    assert common.afosclean(instr) == "000 \nDARYL\n"
+
+
 def test_setup_syslog():
     """API exercice."""
     CTX["stdout_logging"] = True
     common.setup_syslog()
 
 
 def test_parse_utcnow():
```

### Comparing `pywwa-1.5/tests/test_common_syslog.py` & `pywwa-1.6/tests/test_common_syslog.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/test_init.py` & `pywwa-1.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/test_ldmbridge.py` & `pywwa-1.6/tests/test_ldmbridge.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/test_workflow_main.py` & `pywwa-1.6/tests/test_workflow_main.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/test_xmpp.py` & `pywwa-1.6/tests/test_xmpp.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_afos_dump.py` & `pywwa-1.6/tests/workflows/test_afos_dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @pytest.mark.parametrize("database", ["afos"])
 def test_future_product(cursor):
     """Test exception for product from the future."""
     data = get_example_file("AFD.txt")
     pywwa.CTX["utcnow"] = utc(2015, 6, 8, 11, 56)
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError):
         afos_dump.process_data(cursor, data)
 
 
 @pytest.mark.parametrize("database", ["afos"])
 def test_memcache_write_api(cursor):
     """Exercise, but does not actually run the write :("""
     data = get_example_file("AFD.txt")
@@ -29,24 +29,24 @@
 
 
 @pytest.mark.parametrize("database", ["afos"])
 def test_processor(cursor):
     """Test basic parsing."""
     data = get_example_file("AFD.txt")
     # 0. Very latent product
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError):
         afos_dump.process_data(cursor, data)
     pywwa.CTX["utcnow"] = utc(2015, 6, 9, 11, 56)
     # 1. straight through
     prod = afos_dump.process_data(cursor, data)
     assert prod.afos == "AFDDMX"
     # 2. Corrupt the AFOS
     data = data.replace("AFDDMX", "AFDDMX123")
-    with pytest.raises(Exception):
-        afos_dump.rprocess_data(cursor, data)
+    with pytest.raises(ValueError):
+        afos_dump.process_data(cursor, data)
     # 3. Corrupt the AFOS and WMO source
     data = data.replace("KDMX", "QQQQ")
     res = afos_dump.process_data(cursor, data)
     assert res is None
     # 4. Have something in exclude from memcache
     data = data.replace("AFDDMX123", "RR1DMX")
     res = afos_dump.process_data(cursor, data)
```

### Comparing `pywwa-1.5/tests/workflows/test_aviation.py` & `pywwa-1.6/tests/workflows/test_aviation.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_bufr_surface.py` & `pywwa-1.6/tests/workflows/test_bufr_surface.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_cli_parser.py` & `pywwa-1.6/tests/workflows/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_dsm_parser.py` & `pywwa-1.6/tests/workflows/test_dsm_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_fake_afos_dump.py` & `pywwa-1.6/tests/workflows/test_fake_afos_dump.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_generic_parser.py` & `pywwa-1.6/tests/workflows/test_generic_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_gini2gis.py` & `pywwa-1.6/tests/workflows/test_gini2gis.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_metar_parser.py` & `pywwa-1.6/tests/workflows/test_metar_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_nexrad3_attr.py` & `pywwa-1.6/tests/workflows/test_nexrad3_attr.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_nldn.py` & `pywwa-1.6/tests/workflows/test_nldn.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_shef_parser.py` & `pywwa-1.6/tests/workflows/test_shef_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_spammer.py` & `pywwa-1.6/tests/workflows/test_spammer.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/tests/workflows/test_watch_parser.py` & `pywwa-1.6/tests/workflows/test_watch_parser.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/archive_noaaport.sh` & `pywwa-1.6/util/archive_noaaport.sh`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/check_pireps_against_aviationwx.py` & `pywwa-1.6/util/check_pireps_against_aviationwx.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                     mine[key][2],
                     lon,
                     lat,
                     location,
                 )
             del mine[key]
 
-    for key, item in mine.items():
+    for _, item in mine.items():
         if item[0] < floor:
             continue
         log.info("AVWX MISS %s %s", item[0], item[3])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pywwa-1.5/util/compress_madis.py` & `pywwa-1.6/util/compress_madis.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/copy_iem_network.py` & `pywwa-1.6/util/copy_iem_network.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/feed_archived_ncr.py` & `pywwa-1.6/util/feed_archived_ncr.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/gen_channels_html_table.py` & `pywwa-1.6/util/gen_channels_html_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,32 +31,32 @@
 C5 = "&lt;vtec_phenomena&gt;.&lt;vtec_significance&gt;.&lt;ugc&gt;"
 C5s = "&lt;vtec_phenomena&gt;.&lt;vtec_significance&gt;.&lt;state&gt;"
 C6 = "&lt;ugc&gt;"
 C7 = "&lt;afos_pil&gt;.&lt;wfo&gt;"
 C8 = "&lt;wmo_source&gt;.&lt;aaa&gt;"
 C9 = "&lt;afos_pil&gt;.&lt;ugc&gt;"
 D = {
-    "10-313": "https://www.nws.noaa.gov/directives/sym/pd01003013curr.pdf",
-    "10-314": "https://www.nws.noaa.gov/directives/sym/pd01003014curr.pdf",
-    "10-315": "https://www.nws.noaa.gov/directives/sym/pd01003015curr.pdf",
-    "10-320": "https://www.nws.noaa.gov/directives/sym/pd01003020curr.pdf",
-    "10-330": "https://www.nws.noaa.gov/directives/sym/pd01003030curr.pdf",
-    "10-401": "https://www.nws.noaa.gov/directives/sym/pd01004001curr.pdf",
-    "10-511": "https://www.nws.noaa.gov/directives/sym/pd01005011curr.pdf",
-    "10-512": "https://www.nws.noaa.gov/directives/sym/pd01005012curr.pdf",
-    "10-513": "https://www.nws.noaa.gov/directives/sym/pd01005013curr.pdf",
-    "10-515": "https://www.nws.noaa.gov/directives/sym/pd01005015curr.pdf",
-    "10-517": "https://www.nws.noaa.gov/directives/sym/pd01005017curr.pdf",
-    "10-601": "https://www.nws.noaa.gov/directives/sym/pd01006001curr.pdf",
-    "10-803": "https://www.nws.noaa.gov/directives/sym/pd01008003curr.pdf",
-    "10-912": "https://www.nws.noaa.gov/directives/sym/pd01009012curr.pdf",
-    "10-922": "https://www.nws.noaa.gov/directives/sym/pd01009022curr.pdf",
-    "10-930": "https://www.nws.noaa.gov/directives/sym/pd01009030curr.pdf",
-    "10-1004": "https://www.nws.noaa.gov/directives/sym/pd01010004curr.pdf",
-    "10-1701": "https://www.nws.noaa.gov/directives/sym/pd01017001curr.pdf",
+    "10-313": "https://weather.gov/directives/sym/pd01003013curr.pdf",
+    "10-314": "https://weather.gov/directives/sym/pd01003014curr.pdf",
+    "10-315": "https://weather.gov/directives/sym/pd01003015curr.pdf",
+    "10-320": "https://weather.gov/directives/sym/pd01003020curr.pdf",
+    "10-330": "https://weather.gov/directives/sym/pd01003030curr.pdf",
+    "10-401": "https://weather.gov/directives/sym/pd01004001curr.pdf",
+    "10-511": "https://weather.gov/directives/sym/pd01005011curr.pdf",
+    "10-512": "https://weather.gov/directives/sym/pd01005012curr.pdf",
+    "10-513": "https://weather.gov/directives/sym/pd01005013curr.pdf",
+    "10-515": "https://weather.gov/directives/sym/pd01005015curr.pdf",
+    "10-517": "https://weather.gov/directives/sym/pd01005017curr.pdf",
+    "10-601": "https://weather.gov/directives/sym/pd01006001curr.pdf",
+    "10-803": "https://weather.gov/directives/sym/pd01008003curr.pdf",
+    "10-912": "https://weather.gov/directives/sym/pd01009012curr.pdf",
+    "10-922": "https://weather.gov/directives/sym/pd01009022curr.pdf",
+    "10-930": "https://weather.gov/directives/sym/pd01009030curr.pdf",
+    "10-1004": "https://weather.gov/directives/sym/pd01010004curr.pdf",
+    "10-1701": "https://weather.gov/directives/sym/pd01017001curr.pdf",
 }
 SPECIAL = {
     "PTSDY1": "Storm Prediction Center Day 1 Convective Outlook",
     "PTSDY2": "Storm Prediction Center Day 2 Convective Outlook",
     "PFWFD1": "Storm Prediction Center Day 1 Fire Weather Outlook",
     "PFWFD2": "Storm Prediction Center Day 2 Fire Weather Outlook",
     "RBG94E": "Weather Prediction Center Day 1 Excessive Rainfall Outlook",
```

### Comparing `pywwa-1.5/util/get_text_from_nwschat.py` & `pywwa-1.6/util/get_text_from_nwschat.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/merge_hvtec_nwsli.py` & `pywwa-1.6/util/merge_hvtec_nwsli.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/nwws_oi_ingest.py` & `pywwa-1.6/util/nwws_oi_ingest.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/ridge_processor.py` & `pywwa-1.6/util/ridge_processor.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/rotate.py` & `pywwa-1.6/util/rotate.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/run_examples.sh` & `pywwa-1.6/util/run_examples.sh`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/save_iowa_level3.py` & `pywwa-1.6/util/save_iowa_level3.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/sync_stations.py` & `pywwa-1.6/util/sync_stations.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/ugcs_update.py` & `pywwa-1.6/util/ugcs_update.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/unzip.py` & `pywwa-1.6/util/unzip.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/watch_OP5R.py` & `pywwa-1.6/util/watch_OP5R.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/wpc_ero_geojson.py` & `pywwa-1.6/util/wpc_ero_geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,20 @@
 import subprocess
 import tempfile
 import warnings
 from copy import deepcopy
 from datetime import timezone
 
 import geopandas as gpd
+import httpx
 import pandas as pd
-import requests
 import xmpp
+from pyiem.database import get_dbconn, get_sqlalchemy_conn
 from pyiem.nws.products import ero
-from pyiem.util import (
-    get_dbconn,
-    get_properties,
-    get_sqlalchemy_conn,
-    logger,
-    utc,
-)
+from pyiem.util import get_properties, logger, utc
 
 # Stop warnings about pyogrio usage of errors=ignore in to_datetime
 # https://github.com/geopandas/pyogrio/issues/344
 warnings.simplefilter("ignore", FutureWarning)
 LOG = logger()
 # No akami
 BASEURI = "https://origin.wpc.ncep.noaa.gov/exper/eromap/geojson/"
@@ -77,15 +72,28 @@
     if valid.hour in range(17, 22):
         return 20
     return -1
 
 
 def fetch_ero(day) -> gpd.GeoDataFrame:
     """Get the ERO from the WPC website."""
-    gdf = gpd.read_file(f"{BASEURI}Day{day}_Latest.geojson", engine="pyogrio")
+    # origin is IDP, www is akamai
+    gdf = None
+    for prefix in ["origin", "www"]:
+        url = BASEURI.replace("origin", prefix)
+        try:
+            gdf = gpd.read_file(
+                f"{url}Day{day}_Latest.geojson", engine="pyogrio"
+            )
+            break
+        except Exception as exp:
+            LOG.info("Failed to fetch %s: %s", url, exp)
+    if gdf is None:
+        LOG.warning("Failed to fetch Day%s", day)
+        return None, None
     # Uppercase all the column names
     gdf.columns = [x.upper() if x != "geometry" else x for x in gdf.columns]
     cols = ["ISSUE_TIME", "START_TIME", "END_TIME"]
     for col in cols:
         gdf[col] = pd.to_datetime(
             gdf[col], format="%Y-%m-%d %H:%M:%S"
         ).dt.tz_localize(timezone.utc)
@@ -277,15 +285,15 @@
             },
         )
         # To prevent a bomb against iembot, we need to seed the cache by
         # requesting these twitter_media URLs
         try:
             LOG.info("Fetching %s", xtra["twitter_media"])
             # 30 seconds found to be not quite enough
-            requests.get(xtra["twitter_media"], timeout=45)
+            httpx.get(xtra["twitter_media"], timeout=45)
         except Exception as exp:
             print(exp)
         msg.addChild(node=xbot)
         conn.send(msg)
 
 
 def main():
```

### Comparing `pywwa-1.5/util/wpc_ero_ingest.py` & `pywwa-1.6/util/wpc_ero_ingest.py`

 * *Files identical despite different names*

### Comparing `pywwa-1.5/util/xcheck_nwwsoi.py` & `pywwa-1.6/util/xcheck_nwwsoi.py`

 * *Files identical despite different names*

