# Comparing `tmp/unimernet-0.0.4-py2.py3-none-any.whl.zip` & `tmp/unimernet-0.0.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2218173 bytes, number of entries: 68
+Zip file size: 2222424 bytes, number of entries: 69
+-rw-r--r--  2.0 unx     2134 b- defN 80-Jan-01 00:00 demo.py
+-rw-r--r--  2.0 unx    10874 b- defN 80-Jan-01 00:00 streamlit_app.py
 -rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 test.py
 -rw-r--r--  2.0 unx     2750 b- defN 80-Jan-01 00:00 train.py
 -rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 unimernet/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/common/__init__.py
 -rw-r--r--  2.0 unx    15074 b- defN 80-Jan-01 00:00 unimernet/common/config.py
 -rw-r--r--  2.0 unx     3614 b- defN 80-Jan-01 00:00 unimernet/common/dist_utils.py
 -rw-r--r--  2.0 unx      815 b- defN 80-Jan-01 00:00 unimernet/common/gradcam.py
@@ -10,15 +12,15 @@
 -rw-r--r--  2.0 unx     3558 b- defN 80-Jan-01 00:00 unimernet/common/optims.py
 -rw-r--r--  2.0 unx     9922 b- defN 80-Jan-01 00:00 unimernet/common/registry.py
 -rw-r--r--  2.0 unx    13802 b- defN 80-Jan-01 00:00 unimernet/common/utils.py
 -rw-r--r--  2.0 unx      209 b- defN 80-Jan-01 00:00 unimernet/configs/datasets/formula/formula_eval.yaml
 -rw-r--r--  2.0 unx      212 b- defN 80-Jan-01 00:00 unimernet/configs/datasets/formula/formula_train.yaml
 -rw-r--r--  2.0 unx      537 b- defN 80-Jan-01 00:00 unimernet/configs/datasets/formula/multi_scale_formula_train.yaml
 -rw-r--r--  2.0 unx      359 b- defN 80-Jan-01 00:00 unimernet/configs/default.yaml
--rw-r--r--  2.0 unx      575 b- defN 80-Jan-01 00:00 unimernet/configs/models/unimernet_base.yaml
+-rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 unimernet/configs/models/unimernet_base.yaml
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/datasets/__init__.py
 -rw-r--r--  2.0 unx     1941 b- defN 80-Jan-01 00:00 unimernet/datasets/builders/__init__.py
 -rw-r--r--  2.0 unx     8061 b- defN 80-Jan-01 00:00 unimernet/datasets/builders/base_dataset_builder.py
 -rw-r--r--  2.0 unx     3552 b- defN 80-Jan-01 00:00 unimernet/datasets/builders/formula.py
 -rw-r--r--  2.0 unx     9518 b- defN 80-Jan-01 00:00 unimernet/datasets/data_utils.py
 -rw-r--r--  2.0 unx     3197 b- defN 80-Jan-01 00:00 unimernet/datasets/datasets/base_dataset.py
 -rw-r--r--  2.0 unx     6511 b- defN 80-Jan-01 00:00 unimernet/datasets/datasets/dataloader_utils.py
@@ -35,15 +37,14 @@
 -rw-r--r--  2.0 unx     9744 b- defN 80-Jan-01 00:00 unimernet/models/clip_vit.py
 -rw-r--r--  2.0 unx    19584 b- defN 80-Jan-01 00:00 unimernet/models/eva_vit.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/models/unimernet/__init__.py
 -rw-r--r--  2.0 unx    38188 b- defN 80-Jan-01 00:00 unimernet/models/unimernet/encoder_decoder.py
 -rw-r--r--  2.0 unx     7302 b- defN 80-Jan-01 00:00 unimernet/models/unimernet/processor.py
 -rw-r--r--  2.0 unx     3808 b- defN 80-Jan-01 00:00 unimernet/models/unimernet/unimernet.py
 -rw-r--r--  2.0 unx     2148 b- defN 80-Jan-01 00:00 unimernet/models/unimernet/utils.py
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 unimernet/models/unimernet.py
 -rw-r--r--  2.0 unx    19744 b- defN 80-Jan-01 00:00 unimernet/models/vit.py
 -rw-r--r--  2.0 unx      948 b- defN 80-Jan-01 00:00 unimernet/processors/__init__.py
 -rw-r--r--  2.0 unx      604 b- defN 80-Jan-01 00:00 unimernet/processors/base_processor.py
 -rw-r--r--  2.0 unx     7854 b- defN 80-Jan-01 00:00 unimernet/processors/blip_processors.py
 -rw-r--r--  2.0 unx     6141 b- defN 80-Jan-01 00:00 unimernet/processors/formula_processor.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/processors/formula_processor_helper/__init__.py
 -rw-r--r--  2.0 unx  1199930 b- defN 80-Jan-01 00:00 unimernet/processors/formula_processor_helper/frost/frost1.png
@@ -58,13 +59,13 @@
 -rw-r--r--  2.0 unx    11292 b- defN 80-Jan-01 00:00 unimernet/processors/randaugment.py
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 unimernet/runners/__init__.py
 -rw-r--r--  2.0 unx    23307 b- defN 80-Jan-01 00:00 unimernet/runners/runner_base.py
 -rw-r--r--  2.0 unx    11842 b- defN 80-Jan-01 00:00 unimernet/runners/runner_iter.py
 -rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 unimernet/tasks/__init__.py
 -rw-r--r--  2.0 unx     9180 b- defN 80-Jan-01 00:00 unimernet/tasks/base_task.py
 -rw-r--r--  2.0 unx     6318 b- defN 80-Jan-01 00:00 unimernet/tasks/unimernet_train.py
--rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4019 b- defN 80-Jan-01 00:00 unimernet-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 unimernet-0.0.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6439 b- defN 16-Jan-01 00:00 unimernet-0.0.4.dist-info/RECORD
-68 files, 2581533 bytes uncompressed, 2207735 bytes compressed:  14.5%
+-rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4207 b- defN 80-Jan-01 00:00 unimernet-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       97 b- defN 80-Jan-01 00:00 unimernet-0.0.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6493 b- defN 16-Jan-01 00:00 unimernet-0.0.5.dist-info/RECORD
+69 files, 2594754 bytes uncompressed, 2211922 bytes compressed:  14.8%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: demo.py
+Comment: 
+
+Filename: streamlit_app.py
+Comment: 
+
 Filename: test.py
 Comment: 
 
 Filename: train.py
 Comment: 
 
 Filename: unimernet/__init__.py
@@ -114,17 +120,14 @@
 
 Filename: unimernet/models/unimernet/unimernet.py
 Comment: 
 
 Filename: unimernet/models/unimernet/utils.py
 Comment: 
 
-Filename: unimernet/models/unimernet.py
-Comment: 
-
 Filename: unimernet/models/vit.py
 Comment: 
 
 Filename: unimernet/processors/__init__.py
 Comment: 
 
 Filename: unimernet/processors/base_processor.py
@@ -183,23 +186,23 @@
 
 Filename: unimernet/tasks/base_task.py
 Comment: 
 
 Filename: unimernet/tasks/unimernet_train.py
 Comment: 
 
-Filename: unimernet-0.0.4.dist-info/LICENSE
+Filename: unimernet-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: unimernet-0.0.4.dist-info/METADATA
+Filename: unimernet-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: unimernet-0.0.4.dist-info/WHEEL
+Filename: unimernet-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: unimernet-0.0.4.dist-info/entry_points.txt
+Filename: unimernet-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: unimernet-0.0.4.dist-info/RECORD
+Filename: unimernet-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unimernet/configs/models/unimernet_base.yaml

```diff
@@ -2,15 +2,15 @@
   arch: unimernet
   load_finetuned: False
   load_pretrained: False
   pretrained: "path/to/pretrained/weight"
   finetuned: ""
   tokenizer_name: nougat
   tokenizer_config:
-    path: ../models/nougat-token
+    path: ./models/unimernet
   model_name: unimernet
   model_config:
     max_seq_len: 384
 
 
 preprocess:
   vis_processor:
```

## Comparing `unimernet-0.0.4.dist-info/LICENSE` & `unimernet-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unimernet-0.0.4.dist-info/METADATA` & `unimernet-0.0.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimernet
-Version: 0.0.4
+Version: 0.0.5
 Summary: UniMERNet: A Universal Network for Real-World Mathematical Expression Recognition
 Home-page: https://github.com/opendatalab/UniMERNet
 License: Apache-2.0
 Keywords: MER,latex,markdown,pdf
 Author: Bin Wang
 Author-email: ictwangbin@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
@@ -28,16 +28,20 @@
 Requires-Dist: iopath (>=0.1.10,<0.2.0)
 Requires-Dist: jupyterlab (>=4.1.6,<5.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.9.0,<5.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pdf2image (>=1.17.0,<2.0.0)
+Requires-Dist: pypdfium2 (>=4.29.0,<5.0.0)
 Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: streamlit (>=1.33.0,<2.0.0)
+Requires-Dist: streamlit_drawable_canvas (>=0.9.3,<0.10.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Requires-Dist: timm (>=0.9.16,<0.10.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: torchtext (>=0.17.2,<0.18.0)
 Requires-Dist: torchvision (>=0.17.2,<0.18.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
```

## Comparing `unimernet-0.0.4.dist-info/RECORD` & `unimernet-0.0.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+demo.py,sha256=fX0kIXHV4ROvQ6FqH1OvzEOBTD2Rq9-icIdwWHf7ENM,2134
+streamlit_app.py,sha256=C3a04T22YV-BJgpYIxU9-5Ad1aSDK5F5gc_iHrnXT0c,10874
 test.py,sha256=ntRcfI0yJkpvHKb90iqvPgtRMBYqlrWB5zRv8lPMPO0,7751
 train.py,sha256=-_6MtzdlIVFyq8Az-Y1S9JkQlzRG4V0xMD0Orc5UxzQ,2750
 unimernet/__init__.py,sha256=_X_jKwoWeW7weEGkwyrxOEKmSIGLjNtzvZ0PX7JSn6k,950
 unimernet/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unimernet/common/config.py,sha256=Jil79ecALCzrIAKRBuVoOrmLoGgKanNqGk3rW5JabCY,15074
 unimernet/common/dist_utils.py,sha256=gKxSkR4fTy3GqlUScqJc91qK2x2yiLTWp0iFZri5Fuk,3614
 unimernet/common/gradcam.py,sha256=4rRJBLo_CcfapKqpzEHwfqpgg06OiLPxYjkjFO9_waI,815
@@ -9,15 +11,15 @@
 unimernet/common/optims.py,sha256=GRkVYtUincqbZagmTYSio4_49GlSckXZo6Ms7bzAOBU,3558
 unimernet/common/registry.py,sha256=ybGL85quZgd4o_4weIV_yCsAXmw3NhGllyk3tAnJzZQ,9922
 unimernet/common/utils.py,sha256=yFj7hc79Cwo_qKWYHJv---VQOevk9sik_2oKDiSGSQg,13802
 unimernet/configs/datasets/formula/formula_eval.yaml,sha256=gBUnT4_pjFLj9QUSbuN4DvpUtAf7b3zQKe3FAJnLVM8,209
 unimernet/configs/datasets/formula/formula_train.yaml,sha256=hLtOJNp83AMCyZRCPDHzGBK_5WqBMGIr9Sq9thWveYs,212
 unimernet/configs/datasets/formula/multi_scale_formula_train.yaml,sha256=XQFVblUHtPCuCWYjl7oTr6GV5YVWnsn-Z0NjOF1da2s,537
 unimernet/configs/default.yaml,sha256=qimBlGDN87Ct7TObdNgnxUjLoHliW0Gsiy_pKbgbiiQ,359
-unimernet/configs/models/unimernet_base.yaml,sha256=Pylrc5gD7iE8MHVjZRe4oceVKR1GmH2dHRgNxSypLhE,575
+unimernet/configs/models/unimernet_base.yaml,sha256=T6cyMgh421FMBmEU9W31HnRjQtYveaF86dbVW4zKTi0,571
 unimernet/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unimernet/datasets/builders/__init__.py,sha256=eTVMf4swNsgkcuk7YOf9RS9RSH-3kJ8gFCT54lBjtCo,1941
 unimernet/datasets/builders/base_dataset_builder.py,sha256=rayAdCeH0WXKsqgzIHUElIPj42g9M5wY2NG1p2Q1RO4,8061
 unimernet/datasets/builders/formula.py,sha256=BNpyWIQ62t_Ynji8Tt85op-4PpPX1YbInchj5mEttFg,3552
 unimernet/datasets/data_utils.py,sha256=TvGtYK4s8leoVdPb81rNfTiq7Ux4VdZeNpCEiO-oJGY,9518
 unimernet/datasets/datasets/base_dataset.py,sha256=sXIETAHraYni6IKb14e96Wa-TxYsQzTk-NYazFkxPZs,3197
 unimernet/datasets/datasets/dataloader_utils.py,sha256=DPof5pmvpwAD9Opk72EPaM6k_UxouQIKcbfSWlghrwA,6511
@@ -34,15 +36,14 @@
 unimernet/models/clip_vit.py,sha256=Woe7B2KKdRNeoKgqBOYWp2fPFcTjEoM9sc9pgvTtjps,9744
 unimernet/models/eva_vit.py,sha256=RkrXJ-BcP_LbKDNLUiPOX8DyNbrtCrAcLBwVLByy7Ko,19584
 unimernet/models/unimernet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unimernet/models/unimernet/encoder_decoder.py,sha256=kOSR5uqbqh97tl0-kdszdOEuO7yVu3TrlY2UZ9CQYFI,38188
 unimernet/models/unimernet/processor.py,sha256=gC15w_AjW7hwDllQP7VHkDFHlUs9P5-SxqPs6HP4UWo,7302
 unimernet/models/unimernet/unimernet.py,sha256=3tD0apvnahroEzrfAz19L0GHA9aG7LHWZnZuv5utwcY,3808
 unimernet/models/unimernet/utils.py,sha256=JmqcCSK3cVgFqxdjh_5b5yrexH3oCgcn0UQDYH6h59g,2148
-unimernet/models/unimernet.py,sha256=nCb-InaTN-iaRDv-FZVQ0o4RUxY0rTeezZJ28esrVr8,50
 unimernet/models/vit.py,sha256=-SUq3jFTSFb-capc0TttI_f53MKr52y4LaJuLvNc2mw,19744
 unimernet/processors/__init__.py,sha256=HAwyqHz9428-_2PGs04f1sQLwpJTGv_bsCdodj3ZhFc,948
 unimernet/processors/base_processor.py,sha256=CMDti5b5pwPMA7C_pLRN8sBcgXCqAxsD353SFNaUO18,604
 unimernet/processors/blip_processors.py,sha256=Su1ZgbS_uQu5sngCaBTSVo2h_H1veMSkAgVz1RBvKlk,7854
 unimernet/processors/formula_processor.py,sha256=js9-pcHg8Y0fxROz3wVsTCw4ngjbCGkrXn4r7fwb1J4,6141
 unimernet/processors/formula_processor_helper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unimernet/processors/formula_processor_helper/frost/frost1.png,sha256=_5-QeGC9eoNdRZ4y-dWIBit_Ye4mc0PMciK1Z1OhR1U,1199930
@@ -57,12 +58,12 @@
 unimernet/processors/randaugment.py,sha256=mNaXux-SCMNBYIubeG9k9YRxIkv7p6JMecTJqq4AabM,11292
 unimernet/runners/__init__.py,sha256=RXvSvxFZ2_Q5Lq_0OHe8x53uiLC6vO-SgVmtiKZnEeY,368
 unimernet/runners/runner_base.py,sha256=XN1OLAq5t68u5-BCVnALXnhZSVFDLur7z0CyIpSSti8,23307
 unimernet/runners/runner_iter.py,sha256=tz88ZTLymApeEe5A-wVynscWuc7uTymQFngCxI2Tqes,11842
 unimernet/tasks/__init__.py,sha256=5_T40TR9RVIURJDppFO-fgQjUxygtlvEtZpoZFEKLp4,717
 unimernet/tasks/base_task.py,sha256=FujbWh9o6a4tnDIR3pSYPqSnkTppGPhmdg9648AsVcE,9180
 unimernet/tasks/unimernet_train.py,sha256=ut8QUVOPgnLbiuGfIpHbM4SJwbmVr2SbVvR_q46AzjQ,6318
-unimernet-0.0.4.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
-unimernet-0.0.4.dist-info/METADATA,sha256=CCiJmkeGHWadg5PiBnFlPFf-4CDq0wHLrq9GcWav3P8,4019
-unimernet-0.0.4.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
-unimernet-0.0.4.dist-info/entry_points.txt,sha256=zISHJOfWynQr_VgZmV7Z6LBRwjH8VmuNjU1rFXeGbSk,72
-unimernet-0.0.4.dist-info/RECORD,,
+unimernet-0.0.5.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
+unimernet-0.0.5.dist-info/METADATA,sha256=qSjmV6kHiHqqphiK_2V9NKj7b2iNnZeOiFoEZLVUfIQ,4207
+unimernet-0.0.5.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
+unimernet-0.0.5.dist-info/entry_points.txt,sha256=1jEVIc-pdX0sTki9RmD_Bwc47uyg1qd4AzKTbqeomd0,97
+unimernet-0.0.5.dist-info/RECORD,,
```

