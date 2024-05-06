# Comparing `tmp/easypaddleocr-0.2.0.tar.gz` & `tmp/easypaddleocr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypaddleocr-0.2.0.tar", last modified: Tue Apr 30 08:25:23 2024, max compression
+gzip compressed data, was "easypaddleocr-0.2.1.tar", last modified: Mon May  6 14:35:37 2024, max compression
```

## Comparing `easypaddleocr-0.2.0.tar` & `easypaddleocr-0.2.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/base_ocr_v20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_det.py
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_rec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/predict_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.798332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.802332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd_sast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/e2e_resnet_vd_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_vitstr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_resnet_vd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_db_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_east_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_fce_head.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_pse_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_sast_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/e2e_pg_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_can_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    32230 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_srn_head.py
--rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/self_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/sr_rensnet_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/table_att_head.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/east_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fce_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/intracl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/pg_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/sast_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/table_fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.806332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/stn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tbsrn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps_spatial_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tsrn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/db_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/east_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pg_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    27043 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/rec_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/poly_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    18308 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/easypaddleocr/pytorchocr_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/easypaddleocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 08:25:23.000000 easypaddleocr-0.2.0/easypaddleocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 08:25:15.000000 easypaddleocr-0.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:25:23.810332 easypaddleocr-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.996957 easypaddleocr-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 14:35:36.996957 easypaddleocr-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.976957 easypaddleocr-0.2.1/easypaddleocr/
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/base_ocr_v20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/predict_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/predict_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/predict_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/predict_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.980957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.980957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.980957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14205 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.980957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.980957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/architectures/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.984957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd_sast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/e2e_resnet_vd_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15839 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19950 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_vitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/table_mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/table_resnet_vd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.988957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_db_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_east_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_fce_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_pse_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_sast_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/e2e_pg_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_can_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32230 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10383 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_srn_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/sr_rensnet_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/table_att_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.988957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/east_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/fce_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/intracl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/pg_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/sast_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/table_fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.992957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tbsrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tps_spatial_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tsrn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.992957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/db_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/east_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pg_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.992957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.992957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27043 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/rec_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.992957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.996957 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/poly_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18308 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/easypaddleocr/pytorchocr_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:36.996957 easypaddleocr-0.2.1/easypaddleocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 14:35:36.000000 easypaddleocr-0.2.1/easypaddleocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-06 14:35:36.000000 easypaddleocr-0.2.1/easypaddleocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:35:36.000000 easypaddleocr-0.2.1/easypaddleocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 14:35:36.000000 easypaddleocr-0.2.1/easypaddleocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 14:35:36.000000 easypaddleocr-0.2.1/easypaddleocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 14:35:32.000000 easypaddleocr-0.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:35:36.996957 easypaddleocr-0.2.1/setup.cfg
```

### Comparing `easypaddleocr-0.2.0/LICENCE` & `easypaddleocr-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/PKG-INFO` & `easypaddleocr-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
```

### Comparing `easypaddleocr-0.2.0/easypaddleocr/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,76 @@
+import pathlib
 import numpy as np
 import torch
 from huggingface_hub import hf_hub_download
 from loguru import logger
 from .predict_system import PredictSystem
 
 
 class EasyPaddleOCR:
-    def __init__(self, use_angle_cls=False, devices="auto", needWarmUp=False,
+    def __init__(self, use_angle_cls=False, devices="auto", model_local_dir=None, needWarmUp=False,
                  warmup_size=(640, 640), drop_score=0.5, **kwargs):
         """
         Initialize EasyPaddleOCR object with specified parameters.
         :param use_angle_cls: Whether to use angle classifier. This is used to detect text that is 180' rotated.
         :param devices: Device to use in pytorch. "auto" for auto-detect, "cpu" for cpu, "cuda" for cuda.
         :param needWarmUp: Whether to warm up the model. This will take some time.
         :param warmup_size: Size of the image to use in warm up. Please specify the **MAX** image size you want to
         inference with in this parameter when possible. This can reduce the usage of VMEM.
+        :param model_local_dir: Defaults to None, if filled, the model is loaded from the local folder
+        :param drop_score: Minimum score to keep the detected text.
         :param kwargs: other parameters to pass to InferSystem. See original PaddleOCR documentation for more details.
         """
+        self.config_default_dict = {
+            "det_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_det_infer.pth",
+            "rec_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_rec_infer.pth",
+            "cls_model_path": "PaddleOCR2Pytorch/ch_ptocr_mobile_v2.0_cls_infer.pth",
+            "det_model_config_path": "PaddleOCR2Pytorch/configs/det/ch_PP-OCRv4/ch_PP-OCRv4_det_student.yml",
+            "rec_model_config_path": "PaddleOCR2Pytorch/configs/rec/PP-OCRv4/ch_PP-OCRv4_rec.yml",
+            "character_dict_path": "ppocr_keys_v1.txt"
+        }
         self._modelFileKeys = ["det_model_path", "rec_model_path", "cls_model_path",
                                "det_model_config_path", "rec_model_config_path", "character_dict_path"]
         self._modelFilePaths = {key: kwargs.get(key, None) for key in self._modelFileKeys}
         if devices == "auto":
             self._use_gpu = True if torch.cuda.is_available() else False
         else:
             self._use_gpu = True if devices == "cuda" else False
         logger.info(f"Using device: {devices}")
-        self._download_file(self._modelFilePaths)
+        self._model_local_dir = model_local_dir
+        if self._model_local_dir:
+            self._load_local_file(self._modelFilePaths)
+        else:
+            self._download_file(self._modelFilePaths)
         self.ocr = PredictSystem(use_angle_cls=use_angle_cls,
                                  det_yaml_path=self._modelFilePaths["det_model_config_path"],
                                  det_model_path=self._modelFilePaths["det_model_path"],
                                  rec_yaml_path=self._modelFilePaths["rec_model_config_path"],
                                  rec_model_path=self._modelFilePaths["rec_model_path"],
                                  cls_model_path=self._modelFilePaths["cls_model_path"],
                                  rec_char_dict_path=self._modelFilePaths["character_dict_path"],
                                  drop_score=drop_score,
                                  use_gpu=self._use_gpu)
         self.needWarmUp = needWarmUp
         self._warm_up(warmup_size) if self.needWarmUp else None
 
-    @staticmethod
-    def _download_file(fileDict):
-        config_default_dict = {
-            "det_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_det_infer.pth",
-            "rec_model_path": "PaddleOCR2Pytorch/ch_ptocr_v4_rec_infer.pth",
-            "cls_model_path": "PaddleOCR2Pytorch/ch_ptocr_mobile_v2.0_cls_infer.pth",
-            "det_model_config_path": "PaddleOCR2Pytorch/configs/det/ch_PP-OCRv4/ch_PP-OCRv4_det_student.yml",
-            "rec_model_config_path": "PaddleOCR2Pytorch/configs/rec/PP-OCRv4/ch_PP-OCRv4_rec.yml",
-            "character_dict_path": "ppocr_keys_v1.txt"
-        }
+    def _load_local_file(self, fileDict):
+        for key, val in fileDict.items():
+            if not val:
+                logger.warning(f"Unspecified {key[:-5]}, using default value {self.config_default_dict[key]}")
+                fileDict[key] = pathlib.Path(self._model_local_dir, self.config_default_dict[key])
+                if not fileDict[key].exists():
+                    raise FileNotFoundError(f"File {fileDict[key]} not found.")
+        logger.info(fileDict)
+
+    def _download_file(self, fileDict):
         for key, val in fileDict.items():
             if not val:
-                logger.warning(f"Unspecified {key[:-5]}, using default value {config_default_dict[key]}")
-                fileDict[key] = hf_hub_download(repo_id="pk5ls20/PaddleModel", filename=config_default_dict[key])
+                logger.warning(f"Unspecified {key[:-5]}, using default value {self.config_default_dict[key]}")
+                fileDict[key] = hf_hub_download(repo_id="pk5ls20/PaddleModel", filename=self.config_default_dict[key])
         logger.info(fileDict)
 
     def _warm_up(self, warmup_size):
         logger.info("Warm up started")
         assert (isinstance(warmup_size, (list, tuple)) and
                 len(warmup_size) == 2), "warmup_size must be tuple or list with 2 elems."
         img = np.random.uniform(0, 255, [warmup_size[0], warmup_size[1], 3]).astype(np.uint8)
```

### Comparing `easypaddleocr-0.2.0/easypaddleocr/base_ocr_v20.py` & `easypaddleocr-0.2.1/easypaddleocr/base_ocr_v20.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/config.py` & `easypaddleocr-0.2.1/easypaddleocr/config.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/predict_cls.py` & `easypaddleocr-0.2.1/easypaddleocr/predict_cls.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/predict_det.py` & `easypaddleocr-0.2.1/easypaddleocr/predict_det.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/predict_rec.py` & `easypaddleocr-0.2.1/easypaddleocr/predict_rec.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/predict_system.py` & `easypaddleocr-0.2.1/easypaddleocr/predict_system.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/gen_table_mask.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/data/imaug/operators.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/data/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/architectures/base_model.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/architectures/base_model.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd_sast.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/det_resnet_vd_sast.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/e2e_resnet_vd_pg.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/e2e_resnet_vd_pg.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_densenet.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_densenet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_hgnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_lcnetv3_bak.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_mv1_enhance.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_nrtr_mtb.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_31.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_svtrnet.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/rec_vitstr.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/rec_vitstr.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_mobilenet_v3.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/table_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/backbones/table_resnet_vd.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/backbones/table_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/common.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/common.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/cls_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_db_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_db_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_east_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_east_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_fce_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_fce_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_pse_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_pse_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/det_sast_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/det_sast_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/e2e_pg_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/e2e_pg_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/multiheadAttention.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_att_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_can_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_can_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_ctc_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_multi_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_nrtr_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_sar_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/rec_srn_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/rec_srn_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/self_attention.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/self_attention.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/sr_rensnet_transformer.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/sr_rensnet_transformer.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/heads/table_att_head.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/heads/table_att_head.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/db_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/east_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/east_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fce_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/fce_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/intracl.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/intracl.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/pg_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/pg_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/rnn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/rnn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/sast_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/sast_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/necks/table_fpn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/necks/table_fpn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/stn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/stn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tbsrn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tbsrn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tps.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tps_spatial_transformer.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tps_spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/modeling/transforms/tsrn.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/modeling/transforms/tsrn.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/db_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/east_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/fce_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pg_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/__init__.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/rec_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_batchsize.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/e2e_utils/visual.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/logging.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/logging.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/poly_nms.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/poly_nms.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr/utils/utility.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr/utils/utility.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr/pytorchocr_utility.py` & `easypaddleocr-0.2.1/easypaddleocr/pytorchocr_utility.py`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/easypaddleocr.egg-info/PKG-INFO` & `easypaddleocr-0.2.1/easypaddleocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easypaddleocr
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch.
 Author: pk5ls20, hv0905
 Project-URL: Code, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Documentation, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Download, https://pypi.org/project/easypaddleocr
 Project-URL: Homepage, https://github.com/pk5ls20/EasyPaddleOCR
 Project-URL: Issues, https://github.com/pk5ls20/EasyPaddleOCR/issues
```

### Comparing `easypaddleocr-0.2.0/easypaddleocr.egg-info/SOURCES.txt` & `easypaddleocr-0.2.1/easypaddleocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easypaddleocr-0.2.0/pyproject.toml` & `easypaddleocr-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easypaddleocr"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "pk5ls20" },
     { name = "hv0905" }
 ]
 description = "A simple, optional tool for PaddleOCR Detection, direction classification and recognition on CPU and GPU using torch."
 readme = "readme.md"
 license = { file="LICENSE" }
```

### Comparing `easypaddleocr-0.2.0/readme.md` & `easypaddleocr-0.2.1/readme.md`

 * *Files identical despite different names*

