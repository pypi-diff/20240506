# Comparing `tmp/unitxt-1.7.9.tar.gz` & `tmp/unitxt-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.7.9.tar", last modified: Sun May  5 12:46:03 2024, max compression
+gzip compressed data, was "unitxt-1.8.0.tar", last modified: Sun May  5 14:53:31 2024, max compression
```

## Comparing `unitxt-1.7.9.tar` & `unitxt-1.8.0.tar`

### file list

```diff
@@ -1,1106 +1,1107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.607733 unitxt-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 12:45:59.000000 unitxt-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 12:45:59.000000 unitxt-1.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-05 12:46:03.607733 unitxt-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-05 12:45:59.000000 unitxt-1.7.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-05 12:46:00.000000 unitxt-1.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:46:03.607733 unitxt-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-05 12:46:00.000000 unitxt-1.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.435735 unitxt-1.7.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.455735 unitxt-1.7.9/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.463735 unitxt-1.7.9/src/unitxt/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/card.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.443735 unitxt-1.7.9/src/unitxt/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.463735 unitxt-1.7.9/src/unitxt/catalog/augmentors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/augmentors/no_augmentation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.471735 unitxt-1.7.9/src/unitxt/catalog/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.471735 unitxt-1.7.9/src/unitxt/catalog/cards/20_newsgroups/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/20_newsgroups.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.435735 unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.471735 unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/product/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/product/2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/product/watsonx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ag_news.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.475735 unitxt-1.7.9/src/unitxt/catalog/cards/ai2_arc/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.475735 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/it.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.483735 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.483735 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/all_1/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/am_ET.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/da_DK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/de_DE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/el_GR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/en_US.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/es_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/he_IL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/id_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/is_IS.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/it_IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/km_KH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/my_MM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/te_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/th_TH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/argument_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/atis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/atta_q.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.483735 unitxt-1.7.9/src/unitxt/catalog/cards/babi/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/babi/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/banking77.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.503734 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/acm_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/afr_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/als_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/amh_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/apc_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ars_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ary_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arz_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/asm_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/azj_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bam_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ben_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ben_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bod_tibt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bul_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/cat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ceb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ces_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ckb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/dan_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/deu_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ell_grek.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/eng_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/est_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/eus_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fra_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fuv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/gaz_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/grn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/guj_gujr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hau_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/heb_hebr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hin_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hrv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hye_armn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ibo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ilo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ind_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/isl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ita_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/jav_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/jpn_jpan.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kac_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kan_knda.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kat_geor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kea_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/khk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/khm_khmr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kir_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kor_hang.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lao_laoo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lit_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lug_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/luo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lvs_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mal_mlym.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mar_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mlt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mri_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mya_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nld_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nob_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/npi_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/npi_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nya_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ory_orya.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pan_guru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pbt_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pes_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/plt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/por_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ron_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/rus_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/shn_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sin_sinh.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/slk_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/slv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sna_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/snd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/som_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sot_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/spa_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/srp_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ssw_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/swe_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/swh_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tam_taml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tel_telu.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tgl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tha_thai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tir_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tsn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tur_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/urd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/urd_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/uzn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/vie_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/war_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/wol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/xho_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/yor_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zho_hans.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zho_hant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zsm_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zul_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/bold.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.503734 unitxt-1.7.9/src/unitxt/catalog/cards/boolq/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/boolq/classification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/boolq/multiple_choice.json
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/claim_stance_topic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/plus.json
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/small.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cnn_dailymail.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/coedit/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit/paraphrase.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit/rewriting.json
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit/selection.json
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit_error_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coedit_gec.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.439735 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/cola.json
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/copa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/coqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coqa/completion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/coqa/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/dart.json
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/dbpedia_14.json
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ethos_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.507734 unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/16k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/2k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/4k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/8k.json
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/financial_tweets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.511734 unitxt-1.7.9/src/unitxt/catalog/cards/head_qa/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/head_qa/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/head_qa/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/hellaswag.json
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/hh_rlhf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/human_eval.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/law_stack_exchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/ledgar.json
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mbpp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/medical_abstracts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.511734 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/de.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/tu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/anatomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/astronomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/business_ethics.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/computer_security.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/econometrics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/formal_logic.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/global_facts.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_geography.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/human_aging.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/human_sexuality.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/international_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/jurisprudence.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/machine_learning.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/management.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/marketing.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/medical_genetics.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/miscellaneous.json
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/moral_disputes.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/nutrition.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/philosophy.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/prehistory.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_accounting.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/public_relations.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/security_studies.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/sociology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/virology.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/world_religions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/mrpc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/multidoc2dial/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/multidoc2dial/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/news_category_classification_headline.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/openbook_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/piqa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/pop_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/qnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/qqp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/race_all.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/race_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/race_middle.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.439735 unitxt-1.7.9/src/unitxt/catalog/cards/rag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModApte.json
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModHayes.json
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModLewis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/rte.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/sciq.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/sst2.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/stsb.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/summarize_from_human_feedback.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/tab_fact.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/tablerow_classify.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/toxigen.json
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/trec.json
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/unfair_tos.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.439735 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ceb/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/da/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/da/ddt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/de/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/en/ewt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/en/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/hr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/pt/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.519734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ru/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sk/snk.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sv/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/tl/trg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wiki_bio.json
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wikitq.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/debiased.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/l.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/m.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/s.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/xl.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/xs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/wmt/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_de.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_ro.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.523734 unitxt-1.7.9/src/unitxt/catalog/cards/wnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wnli/truthfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/wsc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.531734 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/amharic.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/arabic.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/azerbaijani.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/bengali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/burmese.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/english.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/french.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/gujarati.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/hausa.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/hindi.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/igbo.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/indonesian.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/japanese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/kirundi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/korean.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/kyrgyz.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/marathi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/nepali.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/oromo.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/pashto.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/persian.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/pidgin.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/portuguese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/punjabi.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/russian.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/serbian_latin.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/sinhala.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/somali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/spanish.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/swahili.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/tamil.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/telugu.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/thai.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/tigrinya.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/turkish.json
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/ukrainian.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/urdu.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/uzbek.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/vietnamese.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/welsh.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/yoruba.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.531734 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/bg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/hi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/sw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/th.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ur.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/vi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xnli/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xsum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/jp.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/cards/yahoo_answers_topics.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/empty_input_output_separator.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/human_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/models/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/alpaca_instruct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/models/flan/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/flan/exq_exa.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/flan/few_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/models/labradorite/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/labradorite/few_shot.json
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/models/mistral/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.535734 unitxt-1.7.9/src/unitxt/catalog/formats/models/mistral/instruction/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/models/mistral/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/textual_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/formats/user_assistant.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/accuracy_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/bleu.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/char_edit_distance.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_macro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_micro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/f1_weighted.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/kendalltau_b.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/kpa.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/map.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/matthews_correlation.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/max_accuracy_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/max_f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/ndcg.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/ner.json
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/normalized_sacrebleu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_a/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_chat/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_nli/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.543734 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_q/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/precision_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/precision_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/precision_micro_multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.547734 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_inference.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_reward.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_recall_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_perplexity.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.547734 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/correctness/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/faithfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/map.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.547734 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rag/recall.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/recall_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/recall_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/recall_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/regard.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rerank_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/retrieval_at_k.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.547734 unitxt-1.7.9/src/unitxt/catalog/metrics/reward/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/roc_auc.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rouge.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/sacrebleu.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/safety.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/metrics/sentence_bert/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/spearman.json
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/token_overlap_with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/metrics/wer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.443735 unitxt-1.7.9/src/unitxt/catalog/operators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.443735 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/classification/by_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.551734 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/operators/balancers/qa/by_answer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.555734 unitxt-1.7.9/src/unitxt/catalog/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/capitalize.json
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/convert_to_boolean.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/extract_from_double_brackets.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/extract_mt_bench_judgment.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/first_character.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/get_string_after_colon.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/load_json.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/load_json_from_predictions.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/lower_case.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/lower_case_till_punc.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/match_closest_option.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/remove_none_from_list.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/stance_to_pro_con.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/str_to_float_format.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/take_first_non_empty_line.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/take_first_word.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_list_by_comma.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_span_label_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_string_stripped.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/to_yes_or_none.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/toxic_or_not_toxic.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/processors/yes_no_to_int.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.555734 unitxt-1.7.9/src/unitxt/catalog/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/default.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/diverse_labels_sampler.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/large_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/large_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/small_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/small_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/splitters/test_only.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.443735 unitxt-1.7.9/src/unitxt/catalog/system_prompt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.555734 unitxt-1.7.9/src/unitxt/catalog/system_prompt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompt/models/japanese_llama.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.555734 unitxt-1.7.9/src/unitxt/catalog/system_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompts/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.555734 unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/alpaca.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/labradorite.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/binary/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/binary/zero_or_one.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/multi_class/relation.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/multi_class.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/classification/multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/completion/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/completion/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/completion/multiple_choice.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/evaluation/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/generation.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/grammatical_error_correction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/ner/all_entity_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/ner/single_entity_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/qa/with_context/extractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/rag/model_response_assessment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.559734 unitxt-1.7.9/src/unitxt/catalog/tasks/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/regression/single_text.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/regression/two_texts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/rewriting/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/rewriting/by_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/rewriting/paraphrase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/selection/by_attribute.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/span_labeling/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/span_labeling/extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/summarization/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/summarization/abstractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/tasks/translation/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/tasks/translation/directed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.447735 unitxt-1.7.9/src/unitxt/catalog/templates/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/instruction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.563734 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.447735 unitxt-1.7.9/src/unitxt/catalog/templates/completion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/completion/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/abstractive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/abstractive/standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/completion/multiple_choice/title.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.447735 unitxt-1.7.9/src/unitxt/catalog/templates/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/evaluation/preference/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/evaluation/preference/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/evaluation/preference/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/generation/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/generation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/generation/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_correction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.567734 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_detection/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/key_val.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/key_val_with_new_lines.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.571734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.575734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.579734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.579734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.579734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.579734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.579734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.583734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/open/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/ffqa.json
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/question_first.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/qa/with_context/with_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/rag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/regression/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/regression/single_text/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/single_text/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/single_text/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/single_text/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.587734 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/paraphrase/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/selection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.591734 unitxt-1.7.9/src/unitxt/catalog/templates/selection/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/selection/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/selection/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.591734 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/having.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/span_labeling/extraction/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.591734 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/full.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/passive.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/professional.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.591734 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.451735 unitxt-1.7.9/src/unitxt/catalog/templates/translation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/instructional.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/playful.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog/templates/translation/directed/title.json
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/collections_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/dialog_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/llm_as_judge.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   137081 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    80904 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/parsing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/prepare_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/prepare_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/prepare_utils/card_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/prepare_utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.595734 unitxt-1.7.9/src/unitxt/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.599733 unitxt-1.7.9/src/unitxt/service/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/service/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/service/metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/service/metrics/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/settings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/span_lableing_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/string_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/struct_data_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/system_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    20531 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.599733 unitxt-1.7.9/src/unitxt/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/card.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.599733 unitxt-1.7.9/src/unitxt/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/gradio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/load_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/ui/ui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 12:46:00.000000 unitxt-1.7.9/src/unitxt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:46:03.599733 unitxt-1.7.9/src/unitxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    50188 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 12:46:03.000000 unitxt-1.7.9/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.671681 unitxt-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 14:53:28.000000 unitxt-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 14:53:28.000000 unitxt-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-05 14:53:31.671681 unitxt-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-05 14:53:28.000000 unitxt-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-05 14:53:28.000000 unitxt-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:53:31.671681 unitxt-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-05 14:53:28.000000 unitxt-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.491681 unitxt-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.507681 unitxt-1.8.0/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.515681 unitxt-1.8.0/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/card.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.519681 unitxt-1.8.0/src/unitxt/catalog/augmentors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/augmentors/no_augmentation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.527681 unitxt-1.8.0/src/unitxt/catalog/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.527681 unitxt-1.8.0/src/unitxt/catalog/cards/20_newsgroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/20_newsgroups.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.491681 unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.527681 unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/product/2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/product/watsonx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ag_news.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.527681 unitxt-1.8.0/src/unitxt/catalog/cards/ai2_arc/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.527681 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.535681 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.535681 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/all_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/am_ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/da_DK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/de_DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/el_GR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/en_US.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/es_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/he_IL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/id_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/is_IS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/it_IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/km_KH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/my_MM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/te_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/th_TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/argument_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/atis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/atta_q.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.535681 unitxt-1.8.0/src/unitxt/catalog/cards/babi/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/babi/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/banking77.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.555681 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/acm_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/afr_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/als_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/amh_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/apc_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ars_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ary_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arz_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/asm_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/azj_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bam_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ben_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ben_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bod_tibt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bul_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/cat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ceb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ces_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ckb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/dan_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/deu_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ell_grek.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/eng_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/est_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/eus_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fra_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fuv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/gaz_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/grn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/guj_gujr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hau_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/heb_hebr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hin_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hrv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hye_armn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ibo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ilo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ind_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/isl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ita_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/jav_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/jpn_jpan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kac_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kan_knda.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kat_geor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kea_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/khk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/khm_khmr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kir_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kor_hang.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lao_laoo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lit_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lug_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/luo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lvs_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mal_mlym.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mar_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mlt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mri_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mya_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nld_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nob_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/npi_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/npi_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nya_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ory_orya.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pan_guru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pbt_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pes_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/plt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/por_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ron_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/rus_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/shn_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sin_sinh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/slk_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/slv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sna_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/snd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/som_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sot_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/spa_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/srp_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ssw_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/swe_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/swh_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tam_taml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tel_telu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tgl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tha_thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tir_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tsn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tur_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/urd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/urd_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/uzn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/vie_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/war_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/wol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/xho_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/yor_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zho_hans.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zho_hant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zsm_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zul_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/bold.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.555681 unitxt-1.8.0/src/unitxt/catalog/cards/boolq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/boolq/classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/boolq/multiple_choice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/claim_stance_topic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.555681 unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/plus.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/small.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cnn_dailymail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/coedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit/paraphrase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit/rewriting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit/selection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit_error_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coedit_gec.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.491681 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/cola.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/copa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/coqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coqa/completion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/coqa/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/dart.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/dbpedia_14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ethos_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/16k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/2k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/4k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/8k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/financial_tweets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.559681 unitxt-1.8.0/src/unitxt/catalog/cards/head_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/head_qa/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/head_qa/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/hellaswag.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/hh_rlhf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/human_eval.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/law_stack_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/ledgar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mbpp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/medical_abstracts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.563681 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/tu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/anatomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/astronomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/business_ethics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/computer_security.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/econometrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/formal_logic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/global_facts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_geography.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/human_aging.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/human_sexuality.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/international_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/jurisprudence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/machine_learning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/management.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/marketing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/medical_genetics.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/miscellaneous.json
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/moral_disputes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/nutrition.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/philosophy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/prehistory.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_accounting.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/public_relations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/security_studies.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/sociology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/virology.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/world_religions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/mrpc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/multidoc2dial/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/multidoc2dial/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/news_category_classification_headline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/openbook_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/piqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/pop_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/qnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/qqp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/race_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/race_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/race_middle.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.495681 unitxt-1.8.0/src/unitxt/catalog/cards/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModApte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModHayes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModLewis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/rte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/sciq.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/sst2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/stsb.json
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/summarize_from_human_feedback.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/tab_fact.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/tablerow_classify.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/toxigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/trec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/unfair_tos.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.495681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ceb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/da/ddt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/de/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/en/ewt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/en/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/hr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/pt/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ru/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sk/snk.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.571681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sv/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.575681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/tl/trg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.575681 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wiki_bio.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wikitq.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.575681 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/debiased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/l.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/m.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/s.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/xl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/xs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.575681 unitxt-1.8.0/src/unitxt/catalog/cards/wmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_ro.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.575681 unitxt-1.8.0/src/unitxt/catalog/cards/wnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wnli/truthfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/wsc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.583681 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/amharic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/arabic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/azerbaijani.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/bengali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/burmese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/english.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/french.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/gujarati.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/hausa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/hindi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/igbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/indonesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/japanese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/kirundi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/korean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/kyrgyz.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/marathi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/nepali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/oromo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/pashto.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/persian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/pidgin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/portuguese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/punjabi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/russian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/serbian_latin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/sinhala.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/somali.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/spanish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/swahili.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/tamil.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/telugu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/tigrinya.json
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/turkish.json
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/ukrainian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/urdu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/uzbek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/vietnamese.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/welsh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/yoruba.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.583681 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/bg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/hi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/sw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/th.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ur.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/vi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xnli/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xsum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/jp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/cards/yahoo_answers_topics.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/empty_input_output_separator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/human_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/alpaca_instruct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/models/flan/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/flan/exq_exa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/flan/few_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/models/labradorite/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/labradorite/few_shot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/models/mistral/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.587681 unitxt-1.8.0/src/unitxt/catalog/formats/models/mistral/instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/models/mistral/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/textual_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/formats/user_assistant.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/accuracy_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/bleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/char_edit_distance.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_macro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_micro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/f1_weighted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/kendalltau_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/kpa.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/matthews_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/max_accuracy_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/max_f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/ndcg.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/ner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/normalized_sacrebleu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_nli/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.595681 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_q/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/precision_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/precision_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/precision_micro_multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.599681 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_inference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_reward.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_recall_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_perplexity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.599681 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/correctness/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/faithfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/map.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.599681 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rag/recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/recall_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/recall_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/recall_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/regard.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rerank_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/retrieval_at_k.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.599681 unitxt-1.8.0/src/unitxt/catalog/metrics/reward/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.599681 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/roc_auc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rouge.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/sacrebleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/safety.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.603681 unitxt-1.8.0/src/unitxt/catalog/metrics/sentence_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/spearman.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/token_overlap_with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/metrics/wer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.495681 unitxt-1.8.0/src/unitxt/catalog/operators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.603681 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/classification/by_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.603681 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.603681 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.603681 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/operators/balancers/qa/by_answer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/capitalize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/cast_to_float_return_nan_if_failed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/convert_to_boolean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/extract_from_double_brackets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/extract_mt_bench_judgment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/first_character.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/get_string_after_colon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/load_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/load_json_from_predictions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/lower_case.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/lower_case_till_punc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/match_closest_option.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/remove_none_from_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/stance_to_pro_con.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/str_to_float_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/take_first_non_empty_line.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/take_first_word.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_list_by_comma.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_span_label_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_string_stripped.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/to_yes_or_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/toxic_or_not_toxic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/processors/yes_no_to_int.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/diverse_labels_sampler.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/large_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/large_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/small_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/small_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/splitters/test_only.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/system_prompt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/system_prompt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompt/models/japanese_llama.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/system_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompts/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/alpaca.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/labradorite.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.607681 unitxt-1.8.0/src/unitxt/catalog/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/binary/zero_or_one.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/multi_class/relation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/multi_class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/classification/multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/completion/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/completion/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/completion/multiple_choice.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/evaluation/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/generation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/grammatical_error_correction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/ner/all_entity_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/ner/single_entity_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/qa/with_context/extractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/rag/model_response_assessment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/regression/single_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/regression/two_texts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/rewriting/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/rewriting/by_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/rewriting/paraphrase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/selection/by_attribute.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/span_labeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/span_labeling/extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/summarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/summarization/abstractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.611681 unitxt-1.8.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/tasks/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/tasks/translation/directed.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/templates/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/instruction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.615681 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/templates/completion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/completion/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/abstractive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/abstractive/standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/completion/multiple_choice/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.499681 unitxt-1.8.0/src/unitxt/catalog/templates/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/evaluation/preference/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/evaluation/preference/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/evaluation/preference/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/generation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/generation/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_correction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_detection/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/key_val.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/key_val_with_new_lines.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.503681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.619681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.623681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.627681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.631681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.635681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/open/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/ffqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/question_first.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/qa/with_context/with_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.503681 unitxt-1.8.0/src/unitxt/catalog/templates/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/rag/model_response_assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.503681 unitxt-1.8.0/src/unitxt/catalog/templates/regression/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/regression/single_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/single_text/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/single_text/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/single_text/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.503681 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/paraphrase/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.503681 unitxt-1.8.0/src/unitxt/catalog/templates/selection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.639681 unitxt-1.8.0/src/unitxt/catalog/templates/selection/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/selection/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/selection/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.507681 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.643681 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/having.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/span_labeling/extraction/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.507681 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.643681 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/full.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/passive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/professional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.643681 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.647681 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.647681 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.647681 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.647681 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.507681 unitxt-1.8.0/src/unitxt/catalog/templates/translation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.651681 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/instructional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/playful.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog/templates/translation/directed/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/collections_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/dialog_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/llm_as_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137555 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80904 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/parsing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.651681 unitxt-1.8.0/src/unitxt/prepare_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/prepare_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/prepare_utils/card_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/prepare_utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.651681 unitxt-1.8.0/src/unitxt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.651681 unitxt-1.8.0/src/unitxt/service/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/service/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/service/metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/service/metrics/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/settings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/span_lableing_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/string_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/struct_data_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/system_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20531 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.651681 unitxt-1.8.0/src/unitxt/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.655681 unitxt-1.8.0/src/unitxt/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/gradio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/load_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/ui/ui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 14:53:28.000000 unitxt-1.8.0/src/unitxt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 14:53:31.655681 unitxt-1.8.0/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 14:53:31.000000 unitxt-1.8.0/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.7.9/LICENSE` & `unitxt-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/PKG-INFO` & `unitxt-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.9
+Version: 1.8.0
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -66,53 +66,53 @@
 Requires-Dist: transformers; extra == "ui"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Provides-Extra: all
-Requires-Dist: ibm-cos-sdk; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
-Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: evaluate; extra == "all"
 Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: SentencePiece; extra == "all"
 Requires-Dist: transformers; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
-Requires-Dist: gradio; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: codespell; extra == "all"
-Requires-Dist: bert_score; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
 Requires-Dist: editdistance; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: torch==1.12.1; extra == "all"
 Requires-Dist: sphinxext-opengraph; extra == "all"
-Requires-Dist: ipadic; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
 Requires-Dist: nltk; extra == "all"
-Requires-Dist: datasets; extra == "all"
 Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: jiwer; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: rouge-score; extra == "all"
 Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: codespell; extra == "all"
+Requires-Dist: ipadic; extra == "all"
+Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
+Requires-Dist: datasets; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: absl-py; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: ibm-cos-sdk; extra == "all"
+Requires-Dist: bert_score; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: torch==1.12.1; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
```

### Comparing `unitxt-1.7.9/README.md` & `unitxt-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/pyproject.toml` & `unitxt-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/setup.py` & `unitxt-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/__init__.py` & `unitxt-1.8.0/src/unitxt/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/api.py` & `unitxt-1.8.0/src/unitxt/api.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/artifact.py` & `unitxt-1.8.0/src/unitxt/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/blocks.py` & `unitxt-1.8.0/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/card.py` & `unitxt-1.8.0/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/20_newsgroups/sklearn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/20_newsgroups/sklearn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/20_newsgroups.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/20_newsgroups.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/product/2023.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/product/2023.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/CFPB/product/watsonx.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/CFPB/product/watsonx.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ag_news.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ag_news.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ai2_arc/arc_easy.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ai2_arc/arc_easy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/de.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/en.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/es.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/fr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/it.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/it.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/nl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/nl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/pt.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/pt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil/ru.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/almost_evil.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/almost_evil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/af_ZA.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/af_ZA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/all.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/all_1/1.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/all_1/1.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/am_ET.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/am_ET.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ar_SA.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ar_SA.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/az_AZ.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/az_AZ.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/bn_BD.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/bn_BD.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ca_ES.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ca_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/cy_GB.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/cy_GB.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/da_DK.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/da_DK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/de_DE.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/de_DE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/el_GR.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/el_GR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/en_US.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/en_US.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/es_ES.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/es_ES.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fa_IR.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fa_IR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fi_FI.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fi_FI.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/fr_FR.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/fr_FR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/he_IL.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/he_IL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hi_IN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hi_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hu_HU.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hu_HU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/hy_AM.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/hy_AM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/id_ID.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/id_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/is_IS.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/is_IS.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/it_IT.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/it_IT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ja_JP.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ja_JP.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/jv_ID.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/jv_ID.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ka_GE.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ka_GE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/km_KH.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/km_KH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/kn_IN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/kn_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ko_KR.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ko_KR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/lv_LV.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/lv_LV.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ml_IN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ml_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/mn_MN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/mn_MN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ms_MY.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ms_MY.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/my_MM.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/my_MM.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/nb_NO.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/nb_NO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/nl_NL.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/nl_NL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/pl_PL.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/pl_PL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/pt_PT.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/pt_PT.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ro_RO.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ro_RO.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ru_RU.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ru_RU.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sl_SL.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sl_SL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sq_AL.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sq_AL.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sv_SE.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sv_SE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/sw_KE.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/sw_KE.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ta_IN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ta_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/te_IN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/te_IN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/th_TH.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/th_TH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/tl_PH.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/tl_PH.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/tr_TR.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/tr_TR.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/ur_PK.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/ur_PK.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/vi_VN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/vi_VN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/zh_CN.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/zh_CN.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/amazon_mass/zh_TW.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/amazon_mass/zh_TW.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/argument_topic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/argument_topic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/atis.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/atis.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/atta_q.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/atta_q.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/babi/qa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/babi/qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/banking77.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/banking77.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/acm_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/acm_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/afr_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/afr_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/als_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/als_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/amh_ethi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/amh_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/apc_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/apc_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arb_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arb_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ars_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ars_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ary_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ary_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/arz_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/arz_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/asm_beng.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/asm_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/azj_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/azj_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bam_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bam_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ben_beng.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ben_beng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ben_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ben_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bod_tibt.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bod_tibt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/bul_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/bul_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/cat_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/cat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ceb_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ceb_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ces_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ces_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ckb_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ckb_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/dan_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/dan_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/deu_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/deu_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ell_grek.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ell_grek.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/eng_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/eng_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/est_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/est_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/eus_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/eus_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fin_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fra_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fra_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/fuv_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/fuv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/gaz_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/gaz_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/grn_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/grn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/guj_gujr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/guj_gujr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hat_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hat_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hau_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hau_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/heb_hebr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/heb_hebr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hin_deva.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hin_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hin_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hrv_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hrv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hun_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/hye_armn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/hye_armn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ibo_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ibo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ilo_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ilo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ind_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ind_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/isl_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/isl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ita_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ita_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/jav_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/jav_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/jpn_jpan.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/jpn_jpan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kac_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kac_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kan_knda.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kan_knda.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kat_geor.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kat_geor.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kaz_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kaz_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kea_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kea_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/khk_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/khk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/khm_khmr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/khm_khmr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kin_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kir_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kir_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/kor_hang.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/kor_hang.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lao_laoo.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lao_laoo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lin_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lit_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lit_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lug_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lug_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/luo_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/luo_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/lvs_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/lvs_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mal_mlym.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mal_mlym.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mar_deva.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mar_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mkd_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mkd_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mlt_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mlt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mri_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mri_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/mya_mymr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/mya_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nld_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nld_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nob_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nob_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/npi_deva.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/npi_deva.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/npi_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/npi_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nso_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/nya_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/nya_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ory_orya.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ory_orya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pan_guru.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pan_guru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pbt_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pbt_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pes_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pes_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/plt_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/plt_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/pol_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/pol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/por_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/por_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ron_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ron_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/rus_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/rus_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/shn_mymr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/shn_mymr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sin_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sin_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sin_sinh.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sin_sinh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/slk_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/slk_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/slv_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/slv_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sna_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sna_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/snd_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/snd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/som_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/som_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sot_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sot_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/spa_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/spa_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/srp_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/srp_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ssw_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ssw_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/sun_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/sun_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/swe_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/swe_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/swh_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/swh_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tam_taml.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tam_taml.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tel_telu.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tel_telu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tgk_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tgk_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tgl_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tgl_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tha_thai.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tha_thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tir_ethi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tir_ethi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tsn_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tsn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tso_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tso_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/tur_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/tur_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/ukr_cyrl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/ukr_cyrl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/urd_arab.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/urd_arab.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/urd_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/urd_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/uzn_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/uzn_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/vie_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/vie_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/war_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/war_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/wol_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/wol_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/xho_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/xho_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/yor_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/yor_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zho_hans.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zho_hans.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zho_hant.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zho_hant.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zsm_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zsm_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/belebele/zul_latn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/belebele/zul_latn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/bold.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/bold.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/boolq/classification.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/boolq/classification.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/boolq/multiple_choice.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/boolq/multiple_choice.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/claim_stance_topic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/claim_stance_topic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/imbalanced.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/imbalanced.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/plus.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/plus.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/clinc_oos/small.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/clinc_oos/small.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cnn_dailymail.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cnn_dailymail.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit/paraphrase.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit/paraphrase.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit/preference.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit/preference.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit/rewriting.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit/rewriting.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit/selection.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit/selection.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit_error_detection.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit_error_detection.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coedit_gec.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coedit_gec.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/cola.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/cola.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/copa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/copa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coqa/completion.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coqa/completion.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/coqa/qa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/coqa/qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/dart.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/dart.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/dbpedia_14.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/dbpedia_14.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ethos_binary.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ethos_binary.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/16k.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/16k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/2k.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/2k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/4k.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/4k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ffqa_filtered/8k.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ffqa_filtered/8k.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/financial_tweets.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/financial_tweets.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/head_qa/en.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/head_qa/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/head_qa/es.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/head_qa/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/hellaswag.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/hellaswag.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/hh_rlhf.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/hh_rlhf.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/human_eval.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/human_eval.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/law_stack_exchange.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/law_stack_exchange.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/ledgar.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/ledgar.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mbpp.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mbpp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/medical_abstracts.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/medical_abstracts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/de.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/es.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/fr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/ru.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mlsum/tu.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mlsum/tu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/abstract_algebra.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/abstract_algebra.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/anatomy.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/anatomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/astronomy.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/astronomy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/business_ethics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/business_ethics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_biology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_chemistry.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_computer_science.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_mathematics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_medicine.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/college_physics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/college_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/computer_security.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/computer_security.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/conceptual_physics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/conceptual_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/econometrics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/econometrics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/electrical_engineering.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/electrical_engineering.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/formal_logic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/formal_logic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/global_facts.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/global_facts.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_biology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_biology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_european_history.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_european_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_geography.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_geography.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_physics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_physics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_psychology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_statistics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_statistics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_us_history.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_us_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/high_school_world_history.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/high_school_world_history.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/human_aging.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/human_aging.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/human_sexuality.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/human_sexuality.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/international_law.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/international_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/jurisprudence.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/jurisprudence.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/logical_fallacies.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/logical_fallacies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/machine_learning.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/machine_learning.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/management.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/management.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/marketing.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/marketing.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/medical_genetics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/medical_genetics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/miscellaneous.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/miscellaneous.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/moral_disputes.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/moral_disputes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/moral_scenarios.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/moral_scenarios.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/nutrition.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/nutrition.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/philosophy.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/philosophy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/prehistory.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/prehistory.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_accounting.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_accounting.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_law.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_law.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_medicine.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_medicine.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/professional_psychology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/professional_psychology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/public_relations.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/public_relations.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/security_studies.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/security_studies.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/sociology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/sociology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/virology.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/virology.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mmlu/world_religions.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mmlu/world_religions.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mnli.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/mrpc.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/mrpc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/multidoc2dial/abstractive.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/multidoc2dial/abstractive.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/multidoc2dial/extractive.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/multidoc2dial/extractive.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/news_category_classification_headline.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/news_category_classification_headline.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/openbook_qa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/openbook_qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/piqa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/piqa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/pop_qa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/pop_qa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/qnli.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/qnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/qqp.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/qqp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/race_all.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/race_all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/race_high.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/race_high.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/race_middle.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/race_middle.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModApte.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModApte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModHayes.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModHayes.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/reuters21578/ModLewis.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/reuters21578/ModLewis.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/rte.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/rte.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/sciq.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/sciq.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/squad.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/squad.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/sst2.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/sst2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/stsb.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/stsb.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/summarize_from_human_feedback.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/summarize_from_human_feedback.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/tab_fact.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/tab_fact.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/tablerow_classify.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/tablerow_classify.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/toxigen.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/toxigen.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/trec.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/trec.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/unfair_tos.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/unfair_tos.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ceb/gja.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ceb/gja.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/da/ddt.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/da/ddt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/de/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/de/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/en/ewt.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/en/ewt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/en/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/en/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/hr/set.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/hr/set.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/pt/bosque.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/pt/bosque.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/pt/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/pt/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/ru/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/ru/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sk/snk.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sk/snk.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sr/set.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sr/set.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sv/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sv/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/tl/trg.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/tl/trg.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/gsd.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/gsd.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/universal_ner/zh/pud.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/universal_ner/zh/pud.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wiki_bio.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wiki_bio.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wikitq.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wikitq.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/debiased.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/debiased.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/l.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/l.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/m.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/m.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/s.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/s.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/xl.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/xl.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/winogrande/xs.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/winogrande/xs.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_de.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_fr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wmt/en_ro.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wmt/en_ro.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wnli/truthfulness.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wnli/truthfulness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wnli.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wnli.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/wsc.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/wsc.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/amharic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/amharic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/arabic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/arabic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/azerbaijani.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/azerbaijani.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/bengali.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/bengali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/burmese.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/burmese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/chinese_simplified.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/chinese_simplified.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/chinese_traditional.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/chinese_traditional.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/english.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/english.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/french.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/french.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/gujarati.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/gujarati.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/hausa.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/hausa.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/hindi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/hindi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/igbo.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/igbo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/indonesian.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/indonesian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/japanese.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/japanese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/kirundi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/kirundi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/korean.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/korean.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/kyrgyz.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/kyrgyz.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/marathi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/marathi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/nepali.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/nepali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/oromo.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/oromo.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/pashto.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/pashto.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/persian.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/persian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/pidgin.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/pidgin.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/portuguese.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/portuguese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/punjabi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/punjabi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/russian.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/russian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/serbian_latin.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/serbian_latin.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/sinhala.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/sinhala.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/somali.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/somali.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/spanish.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/spanish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/swahili.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/swahili.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/tamil.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/tamil.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/telugu.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/telugu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/thai.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/thai.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/tigrinya.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/tigrinya.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/turkish.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/turkish.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/ukrainian.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/ukrainian.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/urdu.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/urdu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/uzbek.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/uzbek.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/vietnamese.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/vietnamese.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/welsh.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/welsh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xlsum/yoruba.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xlsum/yoruba.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ar.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ar.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/bg.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/bg.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/de.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/de.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/el.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/el.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/en.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/es.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/es.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/fr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/fr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/hi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/hi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ru.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/sw.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/sw.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/th.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/th.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/tr.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/tr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/ur.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/ur.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/vi.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/vi.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xnli/zh.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xnli/zh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/en.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/en.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/jp.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/jp.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/pt.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/pt.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/ru.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/ru.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/xwinogrande/zh.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/xwinogrande/zh.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/cards/yahoo_answers_topics.json` & `unitxt-1.8.0/src/unitxt/catalog/cards/yahoo_answers_topics.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/normalized_sacrebleu.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/normalized_sacrebleu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_correctness.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_correctness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_inference.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_inference.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/answer_reward.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/answer_reward.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_k_precision.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_k_precision.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_recall.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_recall.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/bert_recall_ml.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/bert_recall_ml.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_correctness.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_correctness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_perplexity.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_perplexity.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/context_relevance.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/context_relevance.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/faithfulness.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/faithfulness.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/k_precision.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/k_precision.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/map.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/map.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/mrr.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/mrr.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/rag/recall.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/rag/recall.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/sacrebleu.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/sacrebleu.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/squad.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/squad.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/metrics/token_overlap_with_context.json` & `unitxt-1.8.0/src/unitxt/catalog/metrics/token_overlap_with_context.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/processors/to_span_label_pairs.json` & `unitxt-1.8.0/src/unitxt/catalog/processors/to_span_label_pairs.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json` & `unitxt-1.8.0/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/labradorite.json` & `unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/labradorite.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/llama.json` & `unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/llama.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/system_prompts/models/llama2.json` & `unitxt-1.8.0/src/unitxt/catalog/system_prompts/models/llama2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/default.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/instruction.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/instruction.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/classification/multi_label/title.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/classification/multi_label/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/evaluation/preference/default.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/evaluation/preference/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/selection/by_attribute/default.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/selection/by_attribute/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/summarization/abstractive/all.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/summarization/abstractive/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json` & `unitxt-1.8.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/catalog.py` & `unitxt-1.8.0/src/unitxt/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/collections.py` & `unitxt-1.8.0/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/collections_operators.py` & `unitxt-1.8.0/src/unitxt/collections_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/dataclass.py` & `unitxt-1.8.0/src/unitxt/dataclass.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/dataset.py` & `unitxt-1.8.0/src/unitxt/dataset.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/dataset_utils.py` & `unitxt-1.8.0/src/unitxt/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/deprecation_utils.py` & `unitxt-1.8.0/src/unitxt/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/dialog_operators.py` & `unitxt-1.8.0/src/unitxt/dialog_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/dict_utils.py` & `unitxt-1.8.0/src/unitxt/dict_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/eval_utils.py` & `unitxt-1.8.0/src/unitxt/eval_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/file_utils.py` & `unitxt-1.8.0/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/formats.py` & `unitxt-1.8.0/src/unitxt/formats.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/fusion.py` & `unitxt-1.8.0/src/unitxt/fusion.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/generator_utils.py` & `unitxt-1.8.0/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/hf_utils.py` & `unitxt-1.8.0/src/unitxt/hf_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/inference.py` & `unitxt-1.8.0/src/unitxt/inference.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/llm_as_judge.py` & `unitxt-1.8.0/src/unitxt/llm_as_judge.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/loaders.py` & `unitxt-1.8.0/src/unitxt/loaders.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/logging_utils.py` & `unitxt-1.8.0/src/unitxt/logging_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/metric.py` & `unitxt-1.8.0/src/unitxt/metric.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/metric_utils.py` & `unitxt-1.8.0/src/unitxt/metric_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/metrics.py` & `unitxt-1.8.0/src/unitxt/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     StreamingOperator,
     StreamInstanceOperator,
 )
 from .operators import CopyFields
 from .random_utils import get_seed
 from .settings_utils import get_settings
 from .stream import MultiStream, Stream
-from .type_utils import isoftype, parse_type_string, to_float_or_default
+from .type_utils import isoftype, parse_type_string
 
 logger = get_logger()
 settings = get_settings()
 
 warnings.filterwarnings("ignore", category=DegenerateDataWarning)
 
 
@@ -1257,38 +1257,58 @@
 
 
 class F1Micro(F1):
     main_score = "f1_micro"
     average = "micro"
 
 
-class F1Binary(F1):
+class F1Binary(GlobalMetric):
     """Calculate f1 for a binary task, using 0.5 as the threshold in the case of float predictions."""
 
     process_single_instances = False
     main_score = "f1_binary"
-    average = "binary"
-    pos_classes = {"1", "1.0", "yes", "true"}
+    average = None
     threshold = 0.5
+    prediction_type = "Union[float, int]"
+    _metric = None
+    metric = "f1"
+    single_reference_per_prediction = True
 
-    def get_str_id(self, str):
-        return int(str)
+    def prepare(self):
+        super().prepare()
+        self._metric = evaluate.load(self.metric)
+
+    def _validate_reference(self, reference):
+        super()._validate_reference(reference)
+        assert reference[0] in [
+            0,
+            1,
+        ], f"all references of {self.main_score} must by 0 or 1"
 
     def compute(
         self,
         references: List[List[str]],
         predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
-        predictions_floats = [to_float_or_default(p) for p in predictions]
-        predictions = [str(int(p > self.threshold)) for p in predictions_floats]
-        references = [
-            ["1"] if r[0].lower() in self.pos_classes else ["0"] for r in references
-        ]
-        return super().compute(references, predictions, task_data)
+        flattened_int_references = [int(r[0]) for r in references]
+        int_predictions = [int(p > self.threshold) for p in predictions]
+
+        result = self._metric.compute(
+            references=flattened_int_references,
+            predictions=int_predictions,
+            labels=[0, 1],
+            average=self.average,
+        )
+        if isinstance(result[self.metric], numpy.ndarray):
+            return {
+                self.main_score: result[self.metric][1],
+                f"{self.main_score}_neg": result[self.metric][0],
+            }
+        return {self.main_score: result[self.metric]}
 
 
 class RecallBinary(F1Binary):
     main_score = "recall_binary"
     metric = "recall"
 
 
@@ -1534,15 +1554,15 @@
             )
 
 
 class KendallTauMetric(GlobalMetric):
     main_score = "kendalltau_b"
     variant = "b"
     process_single_instances = False
-    prediction_type = "str"
+    prediction_type = "float"
 
     _requirements_list: List[str] = ["scipy"]
 
     def prepare(self):
         from scipy.stats import kendalltau
 
         self.kendalltau = kendalltau
@@ -1551,16 +1571,14 @@
         self,
         references: List[List[str]],
         predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
         if isinstance(references[0], list):
             references = [reference[0] for reference in references]
-        references = [to_float_or_default(r) for r in references]
-        predictions = [to_float_or_default(p) for p in predictions]
 
         kendall_results = self.kendalltau(references, predictions, variant=self.variant)
         corr = kendall_results.correlation
         return {
             self.main_score: corr,
             f"{self.main_score}_p_val": kendall_results.pvalue,
         }
@@ -1598,15 +1616,15 @@
 
 
 class RocAuc(GlobalMetric):
     main_score = "roc_auc"
     process_single_instances = False
     _requirements_list: List[str] = ["sklearn"]
     single_reference_per_prediction = True
-    prediction_type = "str"
+    prediction_type = "float"
 
     def prepare(self):
         from sklearn import metrics
 
         self.roc_curve = metrics.roc_curve
         self.auc = metrics.auc
 
@@ -1614,16 +1632,14 @@
         self,
         references: List[List[str]],
         predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
         if isinstance(references[0], list):
             references = [reference[0] for reference in references]
-        references = [to_float_or_default(r) for r in references]
-        predictions = [to_float_or_default(p) for p in predictions]
 
         false_positive_rates, true_positive_rates, _ = self.roc_curve(
             y_true=references, y_score=predictions
         )
         roc_auc = self.auc(false_positive_rates, true_positive_rates)
         return {self.main_score: roc_auc}
 
@@ -3333,114 +3349,123 @@
     }
 
 
 class BinaryMaxF1(F1Binary):
     """Calculate the maximal F1 and the decision threshold that achieves it for a binary task with float predictions."""
 
     main_score = "max_f1_binary"
-    prediction_type = str
     single_reference_per_prediction = True
 
     def compute(
         self,
-        references: List[List[str]],
-        predictions: List[List[str]],
+        references: List[List[float]],
+        predictions: List[List[float]],
         task_data: List[Dict],
     ) -> dict:
-        float_predictions = [to_float_or_default(p) for p in predictions]
-
         best_thr = -1
         best_f1 = -1
-        thrs = {round(fp, 3) for fp in float_predictions}
+        best_thr_neg = -1
+        best_f1_neg = -1
+        thrs = {round(fp, 3) for fp in predictions}
         for thr in thrs:
             new_predictions = [
-                "1" if float_prediction >= thr else "0"
-                for float_prediction in float_predictions
-            ]
-            f1 = super().compute(references, new_predictions, task_data)[
-                self.main_score
+                1.0 if float_prediction >= thr else 0.0
+                for float_prediction in predictions
             ]
+            f1_results = super().compute(references, new_predictions, task_data)
+
+            f1 = f1_results[self.main_score]
             if f1 > best_f1:
                 best_f1 = f1
                 best_thr = thr
 
-        return {self.main_score: best_f1, "best_thr_maxf1": best_thr}
+            f1_neg = f1_results[f"{self.main_score}_neg"]
+            if f1_neg > best_f1_neg:
+                best_f1_neg = f1_neg
+                best_thr_neg = thr
+
+        return {
+            self.main_score: best_f1,
+            "best_thr_maxf1": best_thr,
+            f"{self.main_score}_neg": best_f1_neg,
+            "best_thr_maxf1_neg": best_thr_neg,
+        }
 
 
 class BinaryAccuracy(InstanceMetric):
     """Calculate accuracy for a binary task, using 0.5 as the threshold in the case of float predictions."""
 
     reduction_map = {"mean": ["accuracy_binary"]}
     main_score = "accuracy_binary"
     ci_scores = ["accuracy_binary"]
-    pos_classes = {"1", "1.0", "yes", "true"}
     threshold = 0.5
 
-    prediction_type = "str"
+    prediction_type = "Union[float,int]"
     single_reference_per_prediction = True
 
+    def _validate_reference(self, reference):
+        super()._validate_reference(reference)
+        assert reference[0] in [
+            0,
+            1,
+        ], f"all references of {self.main_score} must by 0 or 1"
+
     def compute(
-        self, references: List[Any], prediction: Any, task_data: List[Dict]
+        self, references: List[float], prediction: float, task_data: List[Dict]
     ) -> dict:
-        float_prediction = to_float_or_default(prediction)
-        prediction = str(int(float_prediction > self.threshold))
-        references = ["1"] if references[0].lower() in self.pos_classes else ["0"]
+        prediction = int(prediction > self.threshold)
+        reference = int(references[0])
 
-        result = {self.main_score: float([prediction] == references)}
+        result = {self.main_score: float(prediction == reference)}
         result["score"] = result[self.main_score]
         result["score_name"] = self.main_score
         return result
 
 
 class BinaryMaxAccuracy(GlobalMetric):
     """Calculate the maximal accuracy and the decision threshold that achieves it for a binary task with float predictions."""
 
     process_single_instances = False
     main_score = "max_accuracy_binary"
-    pos_classes = {"1", "1.0", "yes", "true"}
-
-    prediction_type = "str"
+    prediction_type = "Union[float,int]"
     single_reference_per_prediction = True
 
     def compute(
         self,
         references: List[List[str]],
         predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
-        float_predictions = [to_float_or_default(p) for p in predictions]
-        references = [
-            ["1"] if r[0].lower() in self.pos_classes else ["0"] for r in references
-        ]
+        references = [[int(r[0])] for r in references]
 
         # Sticking to the test >= thr, accuracy induced by threshold thr is the number of float predictions
         # that pass the test (are >= thr) and are paired with reference "1" plus the number of float predictions that
         # fail the test (are < thr) and are paired with reference "0".
         # A given threshold thr induces the same partition over the float predictions into passing and failing
         # as threshold thr' induces, with thr' being the smallest among the ones passing the test of thr.
         # Hence, we only need to review thresholds being float predictions, plus a threshold being larger than
         # the largest float predictions, to induce the partition into all-failing , none-passing.
 
         fp = [
-            (float_predictions[i], i, -1 if references[i][0] == "1" else +1)
-            for i in range(len(float_predictions))
+            (predictions[i], i, -1 if references[i][0] == 1 else +1)
+            for i in range(len(predictions))
         ]
         fp.sort()
         # each triplet above: float-prediction f; f's ordinal position in float_predictions, which is also
         # a means to obtain distinct triplets; and: the change in number of predictions that the test sends
         # to the reference they are paired with, a change implied by a move of thr that transfers f
         # from the set of passing the test to the set of failing it.
 
         rightmost_thr = 1.0 if fp[-1][0] < 1 else fp[-1][0] + 0.01
         # trying to be esthetic, have the threshold within [0,1], although this is not a requirement,
         # and even the float predictions are not guaranteed to be within the range [0,1]
 
         current_thr = fp[0][0]
         # partition float_predictions into all-passing, none-failing
-        current_acc = sum(r[0] == "1" for r in references)
+        current_acc = sum(r[0] == 1 for r in references)
         # number of predictions that thr sends to the reference they are paired with
 
         best_acc = current_acc
         best_thr = current_thr
 
         i = 0
         while (i < len(predictions)) and (best_acc < len(predictions)):
```

### Comparing `unitxt-1.7.9/src/unitxt/normalizers.py` & `unitxt-1.8.0/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/operator.py` & `unitxt-1.8.0/src/unitxt/operator.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/operators.py` & `unitxt-1.8.0/src/unitxt/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/parsing_utils.py` & `unitxt-1.8.0/src/unitxt/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/prepare_utils/card_types.py` & `unitxt-1.8.0/src/unitxt/prepare_utils/card_types.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/processors.py` & `unitxt-1.8.0/src/unitxt/processors.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/random_utils.py` & `unitxt-1.8.0/src/unitxt/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/register.py` & `unitxt-1.8.0/src/unitxt/register.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/schema.py` & `unitxt-1.8.0/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/service/metrics/main.py` & `unitxt-1.8.0/src/unitxt/service/metrics/main.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/service/metrics/tokens.py` & `unitxt-1.8.0/src/unitxt/service/metrics/tokens.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/settings_utils.py` & `unitxt-1.8.0/src/unitxt/settings_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/span_lableing_operators.py` & `unitxt-1.8.0/src/unitxt/span_lableing_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/split_utils.py` & `unitxt-1.8.0/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/splitters.py` & `unitxt-1.8.0/src/unitxt/splitters.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/standard.py` & `unitxt-1.8.0/src/unitxt/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,23 +221,25 @@
 
         self.processing.steps.append(self.card.task)
 
         if self.augmentor.augment_task_input:
             self.augmentor.set_task_input_fields(self.card.task.augmentable_inputs)
             self.processing.steps.append(self.augmentor)
 
-        if self.num_demos > 0:
+        if self.demos_pool_size is not None:
             self.processing.steps.append(
                 CreateDemosPool(
                     from_split=self.demos_taken_from,
                     to_split_names=[self.demos_pool_name, self.demos_taken_from],
                     to_split_sizes=[int(self.demos_pool_size)],
                     remove_targets_from_source_split=self.demos_removed_from_data,
                 )
             )
+
+        if self.num_demos > 0:
             if self.sampler is None:
                 if self.card.sampler is None:
                     raise ValueError(
                         "Unexpected None value for card.sampler. "
                         "To use num_demos > 0, please set a sampler on the TaskCard."
                     )
                 self.sampler = self.card.sampler
```

### Comparing `unitxt-1.7.9/src/unitxt/stream.py` & `unitxt-1.8.0/src/unitxt/stream.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/string_operators.py` & `unitxt-1.8.0/src/unitxt/string_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/struct_data_operators.py` & `unitxt-1.8.0/src/unitxt/struct_data_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/system_prompts.py` & `unitxt-1.8.0/src/unitxt/system_prompts.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/task.py` & `unitxt-1.8.0/src/unitxt/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import Any, Dict, List, Optional, Union
 
 from .artifact import fetch_artifact
 from .logging_utils import get_logger
 from .operator import StreamInstanceOperator
-from .type_utils import isoftype, parse_type_string, verify_required_schema
+from .type_utils import (
+    get_args,
+    get_origin,
+    isoftype,
+    parse_type_string,
+    verify_required_schema,
+)
 
 
 class Tasker:
     pass
 
 
 class FormTask(Tasker, StreamInstanceOperator):
@@ -75,14 +81,18 @@
             metric = fetch_artifact(metric_name)[0]
             metric_prediction_type = metric.get_prediction_type()
 
             if (
                 prediction_type == metric_prediction_type
                 or prediction_type == Any
                 or metric_prediction_type == Any
+                or (
+                    get_origin(metric_prediction_type) is Union
+                    and prediction_type in get_args(metric_prediction_type)
+                )
             ):
                 continue
 
             raise ValueError(
                 f"The task's prediction type ({prediction_type}) and '{metric_name}' "
                 f"metric's prediction type ({metric_prediction_type}) are different."
             )
```

### Comparing `unitxt-1.7.9/src/unitxt/templates.py` & `unitxt-1.8.0/src/unitxt/templates.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/test_utils/artifact.py` & `unitxt-1.8.0/src/unitxt/test_utils/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/test_utils/card.py` & `unitxt-1.8.0/src/unitxt/test_utils/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/test_utils/catalog.py` & `unitxt-1.8.0/src/unitxt/test_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/test_utils/metrics.py` & `unitxt-1.8.0/src/unitxt/test_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/test_utils/operators.py` & `unitxt-1.8.0/src/unitxt/test_utils/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/text_utils.py` & `unitxt-1.8.0/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/type_utils.py` & `unitxt-1.8.0/src/unitxt/type_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/__init__.py` & `unitxt-1.8.0/src/unitxt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/banner.png` & `unitxt-1.8.0/src/unitxt/ui/banner.png`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/gradio_utils.py` & `unitxt-1.8.0/src/unitxt/ui/gradio_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/load_catalog_data.py` & `unitxt-1.8.0/src/unitxt/ui/load_catalog_data.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/run.py` & `unitxt-1.8.0/src/unitxt/ui/run.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/settings.py` & `unitxt-1.8.0/src/unitxt/ui/settings.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/ui_tester.py` & `unitxt-1.8.0/src/unitxt/ui/ui_tester.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/ui/ui_utils.py` & `unitxt-1.8.0/src/unitxt/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/utils.py` & `unitxt-1.8.0/src/unitxt/utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt/validate.py` & `unitxt-1.8.0/src/unitxt/validate.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.7.9/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.8.0/src/unitxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.7.9
+Version: 1.8.0
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -66,53 +66,53 @@
 Requires-Dist: transformers; extra == "ui"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Provides-Extra: all
-Requires-Dist: ibm-cos-sdk; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: gradio; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
-Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: evaluate; extra == "all"
 Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: SentencePiece; extra == "all"
 Requires-Dist: transformers; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
-Requires-Dist: gradio; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
-Requires-Dist: scipy; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: codespell; extra == "all"
-Requires-Dist: bert_score; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
 Requires-Dist: editdistance; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: tomli; extra == "all"
-Requires-Dist: torch==1.12.1; extra == "all"
 Requires-Dist: sphinxext-opengraph; extra == "all"
-Requires-Dist: ipadic; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
 Requires-Dist: nltk; extra == "all"
-Requires-Dist: datasets; extra == "all"
 Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
 Requires-Dist: jiwer; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: evaluate; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
 Requires-Dist: rouge-score; extra == "all"
 Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: codespell; extra == "all"
+Requires-Dist: ipadic; extra == "all"
+Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
+Requires-Dist: datasets; extra == "all"
+Requires-Dist: sphinx_rtd_theme; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: absl-py; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: ibm-cos-sdk; extra == "all"
+Requires-Dist: bert_score; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: tomli; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: torch==1.12.1; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
```

### Comparing `unitxt-1.7.9/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.8.0/src/unitxt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -610,14 +610,15 @@
 src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
 src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
 src/unitxt/catalog/operators/balancers/classification/by_label.json
 src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
 src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
 src/unitxt/catalog/operators/balancers/qa/by_answer.json
 src/unitxt/catalog/processors/capitalize.json
+src/unitxt/catalog/processors/cast_to_float_return_nan_if_failed.json
 src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
 src/unitxt/catalog/processors/convert_to_boolean.json
 src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
 src/unitxt/catalog/processors/extract_from_double_brackets.json
 src/unitxt/catalog/processors/extract_mt_bench_judgment.json
 src/unitxt/catalog/processors/first_character.json
 src/unitxt/catalog/processors/get_string_after_colon.json
```

### Comparing `unitxt-1.7.9/src/unitxt.egg-info/requires.txt` & `unitxt-1.8.0/src/unitxt.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
 
 [all]
-ibm-cos-sdk
+uvicorn[standard]==0.27.0.post1
+sacrebleu[ko]
+sentence_transformers
+scipy
+gradio
 ruff
-sphinx_rtd_theme
-datasets>=2.16.0
-conllu
-fastapi==0.109.0
-crfm-helm[unitxt]>=0.5.0
-python-jose[cryptography]==3.3.0
-evaluate
 httpretty~=1.1.4
-SentencePiece
 transformers
-llama-index-llms-openai
-pytrec-eval
-gradio
-opendatasets
-scipy
-uvicorn[standard]==0.27.0.post1
-piccolo_theme
-codespell
-bert_score
+rouge_score
 editdistance
-pre-commit
-mecab-python3
-scikit-learn
-tomli
-torch==1.12.1
 sphinxext-opengraph
-ipadic
+llama-index-llms-openai
+pytrec-eval
+SentencePiece
+python-jose[cryptography]==3.3.0
 nltk
-datasets
 sacrebleu
-sacrebleu[ko]
 jiwer
-sentence_transformers
-rouge_score
+evaluate
+mecab-python3
 llama-index-core
+codespell
+ipadic
+crfm-helm[unitxt]>=0.5.0
+datasets
+sphinx_rtd_theme
+scikit-learn
 absl-py
+pre-commit
+conllu
+datasets>=2.16.0
+ibm-cos-sdk
+bert_score
+opendatasets
+tomli
+fastapi==0.109.0
+piccolo_theme
+torch==1.12.1
 
 [base]
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
```

