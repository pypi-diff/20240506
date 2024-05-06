# Comparing `tmp/unimernet-0.0.7-py2.py3-none-any.whl.zip` & `tmp/unimernet-0.0.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 2222926 bytes, number of entries: 69
+Zip file size: 2223227 bytes, number of entries: 70
 -rw-r--r--  2.0 unx     2134 b- defN 80-Jan-01 00:00 demo.py
+-rw-r--r--  2.0 unx      209 b- defN 80-Jan-01 00:00 run_unimernet_app.py
 -rw-r--r--  2.0 unx     7751 b- defN 80-Jan-01 00:00 test.py
 -rw-r--r--  2.0 unx     2750 b- defN 80-Jan-01 00:00 train.py
 -rw-r--r--  2.0 unx      950 b- defN 80-Jan-01 00:00 unimernet/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 unimernet/common/__init__.py
 -rw-r--r--  2.0 unx    15074 b- defN 80-Jan-01 00:00 unimernet/common/config.py
 -rw-r--r--  2.0 unx     3614 b- defN 80-Jan-01 00:00 unimernet/common/dist_utils.py
 -rw-r--r--  2.0 unx      815 b- defN 80-Jan-01 00:00 unimernet/common/gradcam.py
@@ -59,13 +60,13 @@
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 unimernet/runners/__init__.py
 -rw-r--r--  2.0 unx    23307 b- defN 80-Jan-01 00:00 unimernet/runners/runner_base.py
 -rw-r--r--  2.0 unx    11842 b- defN 80-Jan-01 00:00 unimernet/runners/runner_iter.py
 -rw-r--r--  2.0 unx      717 b- defN 80-Jan-01 00:00 unimernet/tasks/__init__.py
 -rw-r--r--  2.0 unx     9180 b- defN 80-Jan-01 00:00 unimernet/tasks/base_task.py
 -rw-r--r--  2.0 unx     6318 b- defN 80-Jan-01 00:00 unimernet/tasks/unimernet_train.py
 -rw-r--r--  2.0 unx    10874 b- defN 80-Jan-01 00:00 unimernet_app.py
--rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5534 b- defN 80-Jan-01 00:00 unimernet-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 unimernet-0.0.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6494 b- defN 16-Jan-01 00:00 unimernet-0.0.7.dist-info/RECORD
-69 files, 2596095 bytes uncompressed, 2212424 bytes compressed:  14.8%
+-rw-r--r--  2.0 unx    11342 b- defN 80-Jan-01 00:00 unimernet-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5534 b- defN 80-Jan-01 00:00 unimernet-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 unimernet-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 unimernet-0.0.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6570 b- defN 16-Jan-01 00:00 unimernet-0.0.8.dist-info/RECORD
+70 files, 2596380 bytes uncompressed, 2212609 bytes compressed:  14.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: demo.py
 Comment: 
 
+Filename: run_unimernet_app.py
+Comment: 
+
 Filename: test.py
 Comment: 
 
 Filename: train.py
 Comment: 
 
 Filename: unimernet/__init__.py
@@ -186,23 +189,23 @@
 
 Filename: unimernet/tasks/unimernet_train.py
 Comment: 
 
 Filename: unimernet_app.py
 Comment: 
 
-Filename: unimernet-0.0.7.dist-info/LICENSE
+Filename: unimernet-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: unimernet-0.0.7.dist-info/METADATA
+Filename: unimernet-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: unimernet-0.0.7.dist-info/WHEEL
+Filename: unimernet-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: unimernet-0.0.7.dist-info/entry_points.txt
+Filename: unimernet-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: unimernet-0.0.7.dist-info/RECORD
+Filename: unimernet-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `unimernet-0.0.7.dist-info/LICENSE` & `unimernet-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `unimernet-0.0.7.dist-info/METADATA` & `unimernet-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimernet
-Version: 0.0.7
+Version: 0.0.8
 Summary: UniMERNet: A Universal Network for Real-World Mathematical Expression Recognition
 Home-page: https://github.com/opendatalab/UniMERNet
 License: Apache-2.0
 Keywords: MER,latex,markdown,pdf
 Author: Bin Wang
 Author-email: ictwangbin@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `unimernet-0.0.7.dist-info/RECORD` & `unimernet-0.0.8.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 demo.py,sha256=fX0kIXHV4ROvQ6FqH1OvzEOBTD2Rq9-icIdwWHf7ENM,2134
+run_unimernet_app.py,sha256=N95N2TxiOAhkGa6QdWcYhOfBaM-nXf0sYgg3meN030g,209
 test.py,sha256=ntRcfI0yJkpvHKb90iqvPgtRMBYqlrWB5zRv8lPMPO0,7751
 train.py,sha256=-_6MtzdlIVFyq8Az-Y1S9JkQlzRG4V0xMD0Orc5UxzQ,2750
 unimernet/__init__.py,sha256=_X_jKwoWeW7weEGkwyrxOEKmSIGLjNtzvZ0PX7JSn6k,950
 unimernet/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unimernet/common/config.py,sha256=Jil79ecALCzrIAKRBuVoOrmLoGgKanNqGk3rW5JabCY,15074
 unimernet/common/dist_utils.py,sha256=gKxSkR4fTy3GqlUScqJc91qK2x2yiLTWp0iFZri5Fuk,3614
 unimernet/common/gradcam.py,sha256=4rRJBLo_CcfapKqpzEHwfqpgg06OiLPxYjkjFO9_waI,815
@@ -58,12 +59,12 @@
 unimernet/runners/__init__.py,sha256=RXvSvxFZ2_Q5Lq_0OHe8x53uiLC6vO-SgVmtiKZnEeY,368
 unimernet/runners/runner_base.py,sha256=XN1OLAq5t68u5-BCVnALXnhZSVFDLur7z0CyIpSSti8,23307
 unimernet/runners/runner_iter.py,sha256=tz88ZTLymApeEe5A-wVynscWuc7uTymQFngCxI2Tqes,11842
 unimernet/tasks/__init__.py,sha256=5_T40TR9RVIURJDppFO-fgQjUxygtlvEtZpoZFEKLp4,717
 unimernet/tasks/base_task.py,sha256=FujbWh9o6a4tnDIR3pSYPqSnkTppGPhmdg9648AsVcE,9180
 unimernet/tasks/unimernet_train.py,sha256=ut8QUVOPgnLbiuGfIpHbM4SJwbmVr2SbVvR_q46AzjQ,6318
 unimernet_app.py,sha256=C3a04T22YV-BJgpYIxU9-5Ad1aSDK5F5gc_iHrnXT0c,10874
-unimernet-0.0.7.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
-unimernet-0.0.7.dist-info/METADATA,sha256=WyIw0uJ_umaRsGDodmnQ3XF3wMy399gTe-RBmGfpWXI,5534
-unimernet-0.0.7.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
-unimernet-0.0.7.dist-info/entry_points.txt,sha256=Rf8abP2GIEJ4mrnRLaUTQ8j2ztVlVrbOXxU5hY19pRo,110
-unimernet-0.0.7.dist-info/RECORD,,
+unimernet-0.0.8.dist-info/LICENSE,sha256=l0-K-Od_DnsxSadei3hwQHq_dgykSc49eSt2aRiHwnE,11342
+unimernet-0.0.8.dist-info/METADATA,sha256=zHCyzjxkeDm6vhdal5aW3_DriudpC1c1ceN489txaUA,5534
+unimernet-0.0.8.dist-info/WHEEL,sha256=IrRNNNJ-uuL1ggO5qMvT1GGhQVdQU54d6ZpYqEZfEWo,92
+unimernet-0.0.8.dist-info/entry_points.txt,sha256=Rf8abP2GIEJ4mrnRLaUTQ8j2ztVlVrbOXxU5hY19pRo,110
+unimernet-0.0.8.dist-info/RECORD,,
```

