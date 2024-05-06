# Comparing `tmp/acetone_nnet-0.2.1.post1.tar.gz` & `tmp/acetone_nnet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.1.post1.tar", last modified: Tue Apr 23 15:08:26 2024, max compression
+gzip compressed data, was "acetone_nnet-0.2.2.tar", last modified: Mon May  6 08:28:56 2024, max compression
```

## Comparing `acetone_nnet-0.2.1.post1.tar` & `acetone_nnet-0.2.2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.038810 acetone_nnet-0.2.1.post1/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.1.post1/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.1.post1/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.1.post1/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7882 2024-04-23 15:08:26.037810 acetone_nnet-0.2.1.post1/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6497 2024-04-19 14:35:17.000000 acetone_nnet-0.2.1.post1/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2060 2024-04-23 15:08:21.000000 acetone_nnet-0.2.1.post1/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-23 15:08:26.038810 acetone_nnet-0.2.1.post1/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.015810 acetone_nnet-0.2.1.post1/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.019810 acetone_nnet-0.2.1.post1/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.020810 acetone_nnet-0.2.1.post1/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.021810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-18 12:29:33.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.023810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3168 2024-04-17 09:50:55.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.024810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.025810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.026810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.026810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.027810 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-22 07:07:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.027810 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.028810 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18280 2024-04-23 15:04:24.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.028810 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14173 2024-04-19 12:59:15.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.028810 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.028810 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    27783 2024-04-23 14:51:14.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4062 2024-04-23 14:52:35.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2976 2024-04-23 13:01:02.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.029810 acetone_nnet-0.2.1.post1/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.030810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.032810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.034810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.034810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.035810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.036810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-22 07:07:11.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.036810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.037810 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 15:08:26.037810 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7882 2024-04-23 15:08:25.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-04-23 15:08:26.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-23 15:08:25.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-04-23 15:08:25.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-23 15:08:26.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-23 15:08:26.000000 acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.074707 acetone_nnet-0.2.2/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.2/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.2/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.2/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7882 2024-05-06 08:28:56.074707 acetone_nnet-0.2.2/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6497 2024-04-19 14:35:17.000000 acetone_nnet-0.2.2/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2065 2024-05-06 08:28:13.000000 acetone_nnet-0.2.2/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-06 08:28:56.075707 acetone_nnet-0.2.2/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.796704 acetone_nnet-0.2.2/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.818704 acetone_nnet-0.2.2/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.2.2/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.819704 acetone_nnet-0.2.2/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.2/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.2/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.2/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.819704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-26 12:50:09.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4612 2024-04-30 13:54:15.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.821704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3248 2024-04-25 07:54:18.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.822704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.823704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8174 2024-04-24 12:59:50.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.824704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.825704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.825704 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10588 2024-05-06 08:24:39.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6667 2024-05-06 08:24:16.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5128 2024-05-06 08:24:06.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.2.2/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.826704 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.826704 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    19049 2024-04-26 09:35:35.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.826704 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    15073 2024-04-25 13:20:44.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.826704 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.827704 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    30031 2024-04-25 13:23:24.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4361 2024-04-25 09:51:05.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2976 2024-04-24 07:19:46.000000 acetone_nnet-0.2.2/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.827704 acetone_nnet-0.2.2/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.903705 acetone_nnet-0.2.2/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:55.978706 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.029707 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.035707 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.038707 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.048707 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.059707 acetone_nnet-0.2.2/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.069707 acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1244 2024-05-06 08:26:40.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-06 08:28:56.074707 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7882 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-06 08:28:55.000000 acetone_nnet-0.2.2/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2.1.post1/AUTHORS.md` & `acetone_nnet-0.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/COPYING` & `acetone_nnet-0.2.2/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/LICENSE` & `acetone_nnet-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/PKG-INFO` & `acetone_nnet-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.1.post1
+Version: 0.2.2
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
+Requires-Python: <3.12,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS.md
 Requires-Dist: numpy==1.23.5
 Requires-Dist: numpyencoder==0.3.0
 Requires-Dist: onnx==1.14.0
```

### Comparing `acetone_nnet-0.2.1.post1/README.md` & `acetone_nnet-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/pyproject.toml` & `acetone_nnet-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2.1-1"
-requires-python = ">=3.10"
+version = "0.2.2"
+requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Benjamin LESAGE", email="benjamin.lesage@onera.fr"},
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.2.2/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.2.2/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.2.2/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,15 +72,18 @@
     def __init__(self,alpha):
         super().__init__()
         self.name = 'leakyrelu'
         self.comment = ' and apply rectifier'
         self.alpha = alpha
     
     def compute(self, z):
-        return np.maximum(self.alpha*z,z)
+        if(z<0):
+            return self.alpha*z
+        else:
+            return z
 
     def write_activation_str(self, local_var):
 
         s = local_var +' > 0 ? '+ local_var +' : '+str(self.alpha)+'*'+local_var # output = condition ? value_if_true : value_if_false
         
         return s
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['output_str'] = output_str
         mustach_hash['path'] = self.path
         
         if(self.activation_function.name != 'linear'):
-            mustach_hash['activation_function'] = self.activation_function.write_activation_str()
+            mustach_hash['activation_function'] = self.activation_function.write_activation_str('output_'+str(self.path)+'[k + '+str(self.output_height*self.output_width)+'*f]')
 
         mustach_hash['input_channels'] = self.output_channels
         mustach_hash['channel_size'] = self.output_height*self.output_width
         mustach_hash['epsilon'] = self.epsilon
 
         with open(self.template_path+'layers/template_BatchNormalization.c.tpl','r') as template_file:
             template = template_file.read()
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,19 @@
         with open(self.template_path+'layers/Gemm/template_gemm_tt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self,input):
-        input = input.reshape(self.input_height,self.input_width)
+        if(self.transpo[0]):
+            input = input.reshape(self.input_width,self.input_height).transpose()
+        else:
+            input = input.reshape(self.input_height,self.input_width)
+            
         if(self.transpo[1]):
             self.weights = self.weights.transpose()
         
         return self.activation_function.compute(self.alpha * np.dot(input,self.weights) + self.beta * self.biases)
     
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,43 +15,54 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Resize import Resize
-import tensorflow as tf
 import numpy as np
+import math
 import pystache
 
 #The mode Nearest of the Resize layers.
 #The value in the new tensor is found by applying an rounding operation
 class ResizeNearest(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode='nearest'
         self.nearest_mode_mapping = {"round_prefer_floor":self.round_prefer_floor,
                                      "round_prefer_ceil":self.round_prefer_ceil,
                                      "floor":self.floor,
                                      "ceil":self.ceil}
+        
+        self.nearest_mode_implem_mapping = {"round_prefer_floor":self.round_prefer_floor_implem,
+                                            "round_prefer_ceil":self.round_prefer_ceil_implem,
+                                            "floor":math.floor,
+                                            "ceil":math.ceil}
     
     #Defining the several method to chose the nearest
     def floor(self,x,y):
         return x+' = floor('+y+');'
     
     def ceil(self,x,y):
         return x+' = ceil('+y+');'
     
     def round_prefer_floor(self,x,y):
         return x+' = floor(ceil(2 * ' + y + ') / 2);'
     
+    def round_prefer_floor_implem(self,x):
+        return math.floor(math.ceil(2*x)/2)
+    
     def round_prefer_ceil(self,x,y):
         return x+' = ceil(floor(2 * ' + y + ') / 2);'
     
+    def round_prefer_ceil_implem(self,x):
+        return math.ceil(math.floor(2*x)/2)
+    
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
 
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
@@ -76,11 +87,18 @@
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)    
     
     def forward_path_layer(self, input):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
-        input= np.transpose(input,(1,2,0))#Function resize in tensorflow take a format channel last
-        output = (tf.image.resize(input, [self.output_height,self.output_width], method='nearest')).numpy() #No numpy method for this layer
-        output= np.transpose(output,(2,0,1))
-        return self.activation_function.compute(output)
+        output = np.zeros((self.output_channels,self.output_height,self.output_width))
+        for f in range(self.output_channels):
+            for i in range(self.output_height):
+                for j in range(self.output_width):
+                    x = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](i,2)
+                    x0 = self.nearest_mode_implem_mapping[self.nearest_mode](x)
+                    y = self.coordinate_transformation_mode_implem_mapping[self.coordinate_transformation_mode](j,3)
+                    y0 = self.nearest_mode_implem_mapping[self.nearest_mode](y)
+
+                    output[f,i,j] = input[f,x0,y0]
+        return output
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.2.2/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,25 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import keras
-import keras.layers
-import keras.activations
+from keras import activations
 from itertools import islice
 import numpy as np
 
 from ...graph import graph_interpretor
 
 from ...code_generator import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Constant_Pad,
     Add, Multiply, Subtract, Maximum, Minimum, Average,
-    ResizeCubic, ResizeLinear, ResizeNearest,
     Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten, BatchNormalization,
     Linear, ReLu, Sigmoid, TanH, LeakyReLu
 )
 
 def get_layer_size(keras_layer):
     size = 1
     if type(keras_layer.output_shape) is list:
@@ -70,25 +68,25 @@
             dimensions = [(shape[0],shape[3],shape[1],shape[2]) for shape in dimensions]
         elif(type(dimensions) is not list and len(dimensions) == 4):
             dimensions =  (dimensions[0],dimensions[3],dimensions[1],dimensions[2])
     
     return np.array(dimensions)
 
 def create_actv_function_obj(kears_activation_obj):
-        if kears_activation_obj == keras.activations.sigmoid:
+        if kears_activation_obj == activations.sigmoid:
             return Sigmoid()
-        elif kears_activation_obj == keras.activations.relu:
+        elif kears_activation_obj == activations.relu:
             return ReLu()
-        elif kears_activation_obj == keras.activations.tanh:
+        elif kears_activation_obj == activations.tanh:
             return TanH()
-        elif kears_activation_obj == keras.activations.linear:
+        elif kears_activation_obj == activations.linear:
             return Linear()
-        elif kears_activation_obj == keras.activations.leaky_relu:
+        elif kears_activation_obj == activations.leaky_relu:
             return LeakyReLu(0.2)
-        elif kears_activation_obj == keras.activations.softmax:
+        elif kears_activation_obj == activations.softmax:
             return Linear()
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
@@ -304,23 +302,43 @@
                                          pads = pads,
                                          constant_value = 0,
                                          axes = [],
                                          input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
                                          activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'BatchNormalization':
-            current_layer = BatchNormalization(idx = idx,
-                                               size = get_layer_size(layer_keras),
-                                               input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
-                                               epsilon = layer_keras.epsilon,
-                                               scale = data_type_py(layer_keras.get_weights()[0]),
-                                               biases = data_type_py(layer_keras.get_weights()[1]),
-                                               mean = data_type_py(layer_keras.get_weights()[2]),
-                                               var = data_type_py(layer_keras.get_weights()[3]),
-                                               activation_function = Linear())
+            if(layers[-1].name == 'Conv2D'):
+                scale = data_type_py(layer_keras.get_weights()[0])
+                bias = data_type_py(layer_keras.get_weights()[1])
+                mean = data_type_py(layer_keras.get_weights()[2])
+                var = data_type_py(layer_keras.get_weights()[3])
+
+                weights = layers[-1].weights
+                biases = layers[-1].biases
+
+                for z in range(len(weights[0,0,0,:])):
+                    alpha = scale[z]/np.sqrt(var[z] + layer_keras.epsilon)
+                    B = bias[z] - (mean[z]*alpha)
+                    weights[:,:,:,z] = alpha*weights[:,:,:,z]
+                    biases[z] = alpha*biases[z] + B
+    
+                layers[-1].weights = weights
+                layers[-1].biases = biases
+
+                continue
+            else:
+                current_layer = BatchNormalization(idx = idx,
+                                                   size = get_layer_size(layer_keras),
+                                                   input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
+                                                   epsilon = layer_keras.epsilon,
+                                                   scale = data_type_py(layer_keras.get_weights()[0]),
+                                                   biases = data_type_py(layer_keras.get_weights()[1]),
+                                                   mean = data_type_py(layer_keras.get_weights()[2]),
+                                                   var = data_type_py(layer_keras.get_weights()[3]),
+                                                   activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'Reshape':
             continue
 
         elif layer_keras.__class__.__name__ == 'Dropout':
             continue
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,23 +239,44 @@
                                             pads = pads,
                                             constant_value = 0,
                                             axes = [],
                                             input_shape = layer['config']['input_shape'],
                                             activation_function = Linear())
         
         elif layer['class_name'] == 'BatchNormalization':
-            current_layer = BatchNormalization(idx = layer['config']['idx'],
-                                                size = layer['config']['size'],
-                                                input_shape = layer['config']['input_shape'],
-                                                epsilon = layer['config']['epsilon'],
-                                                scale = np.array(data_type_py(layer['gamma'])),
-                                                biases = np.array(data_type_py(layer['beta'])),
-                                                mean = np.array(data_type_py(layer['moving_mean'])),
-                                                var = np.array(data_type_py(layer['moving_var'])),
-                                                activation_function = Linear())
+            if(layers[-1].name == 'Conv2D'):
+                scale = np.array(data_type_py(layer['gamma']))
+                bias = np.array(data_type_py(layer['beta']))
+                mean = np.array(data_type_py(layer['moving_mean']))
+                var = np.array(data_type_py(layer['moving_var']))
+
+                weights = layers[-1].weights
+                biases = layers[-1].biases
+
+                for z in range(len(weights[0,0,0,:])):
+                    alpha = scale[z]/np.sqrt(var[z] + layer['config']['epsilon'])
+                    print(alpha)
+                    B = bias[z] - (mean[z]*alpha)
+                    weights[:,:,:,z] = alpha*weights[:,:,:,z]
+                    biases[z] = alpha*biases[z] + B
+    
+                layers[-1].weights = weights
+                layers[-1].biases = biases
+
+                continue
+            else:
+                current_layer = BatchNormalization(idx = layer['config']['idx'],
+                                                    size = layer['config']['size'],
+                                                    input_shape = layer['config']['input_shape'],
+                                                    epsilon = layer['config']['epsilon'],
+                                                    scale = np.array(data_type_py(layer['gamma'])),
+                                                    biases = np.array(data_type_py(layer['beta'])),
+                                                    mean = np.array(data_type_py(layer['moving_mean'])),
+                                                    var = np.array(data_type_py(layer['moving_var'])),
+                                                    activation_function = Linear())
         
         
         elif  'Normalization' in layer['class_name']:
             continue
 
         elif  'Dropout' in layer['class_name']:
             continue
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from ...code_generator.layers import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
-    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias
+    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias, BatchNormalization
 )
 
 from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm, **kwargs):
@@ -355,14 +355,41 @@
         return Dot(idx = idx,
                     size = size,
                     axis = [-1,-2],
                     input_shapes = input_shapes,
                     output_shape = output_shape,
                     activation_function = Linear())
 
+def create_BatchNorm(node,idx,dict_input,dict_output,model):
+    output_shape = get_shape(node.output[0],model)
+    size = find_size(output_shape)
+    dict_input[idx] = [node.input[0]]
+    dict_output[node.output[0]] = idx
+    attributs = extract_attribut(node)
+    
+    if('epsilon' not in attributs):
+        attributs['epsilon'] = 1e-05
+    
+    scale = look_for_initializer(node.input[1],model)
+    biases = look_for_initializer(node.input[2],model)
+    mean = look_for_initializer(node.input[3],model)
+    var = look_for_initializer(node.input[4],model)
+
+    return BatchNormalization(idx = idx,
+                              size = size,
+                              input_shape = output_shape,
+                              epsilon = attributs['epsilon'],
+                              scale = onnx.numpy_helper.to_array(scale),
+                              biases = onnx.numpy_helper.to_array(biases),
+                              mean = onnx.numpy_helper.to_array(mean),
+                              var = onnx.numpy_helper.to_array(var),
+                              activation_function = Linear())
+
+
+
 ### Pooling layers ###
 
 #Create a layer MaxPool
 def create_MaxPool(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
@@ -641,16 +668,15 @@
 
 ###### Dict of all the functions ######
 unused_layers = {"Dropout":bypass,
                   "Constant":create_initializer,
                   "Unsqueeze":bypass,
                   "Reshape":bypass,
                   "LRN":bypass,
-                  "Shape":bypass,
-                  "BatchNormalization":bypass}
+                  "Shape":bypass}
 
 ###### Function to fuse to ONNX layers ######
 
 #Fuse the activation layer ReLu with the prior layer
 def fuse_ReLu(node,dict_output,model,layers):
     layers[dict_output[node.input[0]]].activation_function = ReLu()
     bypass(node,dict_output,model)
@@ -684,17 +710,46 @@
         max = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))[0]
     layers[dict_output[node.input[0]]].activation_function = Clip(max=max,min=min)
     bypass(node,dict_output,model)
 
 #Fuse the activation layer LeakyRelu with the prior layer
 def fuse_LeakyReLu(node,dict_output,model,layers):
     attribut = extract_attribut(node)
+    if('alpha' not in attribut):
+        attribut['alpha'] = 0.01
     layers[dict_output[node.input[0]]].activation_function = LeakyReLu(alpha=attribut['alpha'])
     bypass(node,dict_output,model)
+
+#Fuse a BatchNormalization layer with the previous Conv2D layer
+def fuse_BatchNormalization(node,dict_output,model,layers):
+    attributs = extract_attribut(node)
+    if('epsilon' not in attributs):
+        attributs['epsilon'] = 1e-05
     
+    scale = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))
+    bias = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))
+    mean = onnx.numpy_helper.to_array(look_for_initializer(node.input[3],model))
+    var = onnx.numpy_helper.to_array(look_for_initializer(node.input[4],model))
+
+    weights = layers[dict_output[node.input[0]]].weights
+    biases = layers[dict_output[node.input[0]]].biases
+
+    print(weights.shape)
+
+    for z in range(len(weights[0,0,0,:])):
+        alpha = scale[z]/np.sqrt(var[z] + attributs['epsilon'])
+        B = bias[z] - (mean[z]*alpha)
+        weights[:,:,:,z] = alpha*weights[:,:,:,z]
+        biases[z] = alpha*biases[z] + B
+    
+    layers[dict_output[node.input[0]]].weights = weights
+    layers[dict_output[node.input[0]]].biases = biases
+
+    bypass(node, dict_output, model)
+
 ###### Dict of all the functions ######
 activation_layers = {"Relu":fuse_ReLu,
                      "Tanh":fuse_Tanh,
                      "Sigmoid":fuse_Sigmoid,
                      "Clip":fuse_Clip,
                      "Exp":fuse_Exp,
                      "Log":fuse_Log,
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,21 @@
 
     #Creating and adding all the input layers to the list
     layers.append(create_Input_Layer(model.graph.input[0],idx,dict_output))
     idx+=1
     
     #Going through all the nodes to creat the layers and add them to the list
     for node in model.graph.node:
-        if(node.op_type in layer_type): #If the node is a useful layer, we add it to the list
+        if(node.op_type == 'BatchNormalization'):
+            if(layers[-1].name == 'Conv2D'):
+                fuse_BatchNormalization(node, dict_output, model, layers)
+            else:
+                layers.append(create_BatchNorm(node,idx,dict_input,dict_output,model))
+                idx+=1
+        elif(node.op_type in layer_type): #If the node is a useful layer, we add it to the list
             if(node.op_type == "Conv"):    
                 layers.append(layer_type[node.op_type](node,idx,dict_input,dict_output,model,conv_algorithm))
                 idx+=1
             else:
                 layers.append(layer_type[node.op_type](node,idx,dict_input,dict_output,model))
                 idx+=1
         elif(node.op_type in unused_layers): #If the node is a layer only used in trainning, we do layer_input=layer_output
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.2.2/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.2.2/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,20 @@
         for (i = 0; i < {{output_height}}; ++i)
         {
             for(j = 0; j < {{output_width}}; ++j)
             {
                 {{{coordinate_transformation_mode}}}
                 x0 = floor(x);
 
-                f_1 = {{output_str}}[x0-1 + {{dimension}}*f];
-                f0 = {{output_str}}[x0 + {{dimension}}*f];
-                f1 = {{output_str}}[x0+1 + {{dimension}}*f];
-                f2 = {{output_str}}[x0+2 + {{dimension}}*f];
-                s = x - floor(x);
+                f_1 = x0-1 < 0 ? {{output_str}}[0 + {{dimension}}*f] : x0-1 >= {{dimension}} ? {{output_str}}[{{dimension}} - 1 + {{dimension}}*f] : {{output_str}}[x0-1 + {{dimension}}*f];
+                f0 = x0 < 0 ? {{output_str}}[0 + {{dimension}}*f] : x0 >= {{dimension}} ? {{output_str}}[{{dimension}} - 1 + {{dimension}}*f] : {{output_str}}[x0 + {{dimension}}*f];
+                f1 = x0+1 < 0 ? {{output_str}}[0 + {{dimension}}*f] : x0+1 >= {{dimension}} ? {{output_str}}[{{dimension}} - 1 + {{dimension}}*f] : {{output_str}}[x0+1 + {{dimension}}*f];
+                f2 = x0+ 2 < 0 ? {{output_str}}[0 + {{dimension}}*f] : x0+2 >= {{dimension}} ? {{output_str}}[{{dimension}} - 1 + {{dimension}}*f] : {{output_str}}[x0+2 + {{dimension}}*f];
+
+                s = x - x0;
 
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = f_1*a*s*(1 + s*(s - 2)) + f0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + f1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + f2*a*s*s*(1 - s);
                 {{#activation_function}}
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{activation_function}}};
                 {{/activation_function}}
                 {{#fused_layer}}
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{fused_layer}}};
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,33 @@
     // {{name}}_{{idx}}{{comment}}
-    a = {{cubic_coeff_a}};
-
     for (f = 0; f < {{output_channels}}; ++f)
     {
         for (i = 0; i < {{output_height}}; ++i)
         {
-            for(j = 0; j < {{output_width}}; ++j)
+            for (j = 0; j < {{output_width}}; ++j)
             {
-                {{{coordinate_transformation_mode_x}}}
-                x0 = floor(x);
-                {{{coordinate_transformation_mode_y}}}
-                y0 = floor(y);
-                
-                f_1 = {{output_str}}[y0-1 + {{input_width}}*(x0-1 + {{input_height}}*f)];
-                f0 = {{output_str}}[y0-1 + {{input_width}}*(x0 + {{input_height}}*f)];
-                f1 = {{output_str}}[y0-1 + {{input_width}}*(x0+1 + {{input_height}}*f)];
-                f2 = {{output_str}}[y0-1 + {{input_width}}*(x0+2 + {{input_height}}*f)];
-                s = x - x0;
-                float register b_1 = f_1*a*s*(1 + s*(s - 2)) + f0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + f1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + f2*a*s*s*(1 - s);
-
-                f_1 = {{output_str}}[y0 + {{input_width}}*(x0-1 + {{input_height}}*f)];
-                f0 = {{output_str}}[y0 + {{input_width}}*(x0 + {{input_height}}*f)];
-                f1 = {{output_str}}[y0 + {{input_width}}*(x0+1 + {{input_height}}*f)];
-                f2 = {{output_str}}[y0 + {{input_width}}*(x0+2 + {{input_height}}*f)];
-                s = x - x0;
-                float register b0 = f_1*a*s*(1 + s*(s - 2)) + f0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + f1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + f2*a*s*s*(1 - s);
-
-                f_1 = {{output_str}}[y0+1 + {{input_width}}*(x0-1 + {{input_height}}*f)];
-                f0 = {{output_str}}[y0+1 + {{input_width}}*(x0 + {{input_height}}*f)];
-                f1 = {{output_str}}[y0+1 + {{input_width}}*(x0+1 + {{input_height}}*f)];
-                f2 = {{output_str}}[y0+1 + {{input_width}}*(x0+2 + {{input_height}}*f)];
-                s = x - x0;
-                float register b1 = f_1*a*s*(1 + s*(s - 2)) + f0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + f1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + f2*a*s*s*(1 - s);
-
-                f_1 = {{output_str}}[y0+2 + {{input_width}}*(x0-1 + {{input_height}}*f)];
-                f0 = {{output_str}}[y0+2 + {{input_width}}*(x0 + {{input_height}}*f)];
-                f1 = {{output_str}}[y0+2 + {{input_width}}*(x0+1 + {{input_height}}*f)];
-                f2 = {{output_str}}[y0+2 + {{input_width}}*(x0+2 + {{input_height}}*f)];
-                s = x - x0;
-                float register b2 = f_1*a*s*(1 + s*(s - 2)) + f0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + f1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + f2*a*s*s*(1 - s);
-
-                s = y - y0;
-
-                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = b_1*a*s*(1 + s*(s - 2)) + b0*(s*s*(a*(s - 1) + 2*s - 3) + 1) + b1*s*(s*(-s*(2 + a) + 2*a + 3) - a) + b2*a*s*s*(1 - s);
-                {{#linear}}
-                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{activation_function}}};
-                {{/linear}}
-                {{#fused_layer}}
-                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{fused_layer}}};
-                {{/fused_layer}}
+                {{#max}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{output_str0}}[(j%{{input_width0}}) + {{input_width0}}*((i%{{input_height0}}) + {{input_height0}}*(f % {{input_channels0}}))];
+                {{#broadcast}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = fmax(tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)],{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]);
+                {{/broadcast}}
+                {{/max}}
+                {{#min}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{output_str0}}[(j%{{input_width0}}) + {{input_width0}}*((i%{{input_height0}}) + {{input_height0}}*(f % {{input_channels0}}))];
+                {{#broadcast}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = fmin(tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)],{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]);
+                {{/broadcast}}
+                {{/min}}
+                {{#Average}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = ({{#broadcast}}{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]{{operator}}{{/broadcast}})/{{prev_size}};
+                {{/Average}}
+                {{#other}}
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{#broadcast}}{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]{{operator}}{{/broadcast}}{{#constant}}{{operator}}constant_{{name}}_{{idx}}[(j%{{cst_width}}) + {{cst_width}}*((i%{{cst_height}}) + {{cst_height}}*(f % {{cst_channels}}))]{{/constant}};
+                {{/other}}
             }
         }
     }
-
-    for(k = 0; k < {{size}}; ++k)
+    
+    for (k = 0; k < {{size}}; ++k)
     {
-        output_{{road}}[k] = tensor_temp[k];
+        output_{{road}}[k] = {{{activation_function}}};
     }
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
     // {{name}}_{{idx}}{{comment}}
-    x1 = {{len_height}};
-    x0 = 0;
-    y0 = 0;
-    y1 = {{len_width}};
 
     for (f = 0; f < {{output_channels}}; ++f)
     {
-        f11 = {{output_str}}[y0 + {{input_width}}*(x0 + {{input_height}}*f)];
-        f12 = {{output_str}}[y0 + {{input_width}}*(x1 + {{input_height}}*f)];
-        f22 = {{output_str}}[y1 + {{input_width}}*(x1 + {{input_height}}*f)];
-        f21 = {{output_str}}[y1 + {{input_width}}*(x0 + {{input_height}}*f)];
-
         for (i = 0; i < {{output_height}}; ++i)
         {
             for(j = 0; j < {{output_width}}; ++j)
             {
                 {{{coordinate_transformation_mode_x}}}
                 {{{coordinate_transformation_mode_y}}}
-                x = x<x0 ? x0 : (x>x1 ? x1: x);
-                y = y<y0 ? y0 : (y>y1 ? y1: y);
+                x = x<0 ? 0 : (x>{{len_height}} ? {{len_height}}: x);
+                y = y<0 ? 0 : (y>{{len_width}} ? {{len_width}}: y);
+
+                x1 = floor(x) + 1;
+                x0 = floor(x);
+                y0 = floor(y);
+                y1 = floor(y) + 1;
+
+                f11 = {{output_str}}[y0 + {{input_width}}*(x0 + {{input_height}}*f)];
+                f21 = x1 >= {{input_height}} ? 0 : {{output_str}}[y0 + {{input_width}}*(x1 + {{input_height}}*f)];
+                f22 = x1 >= {{input_height}} || y1 >= {{input_width}}? 0 : {{output_str}}[y1 + {{input_width}}*(x1 + {{input_height}}*f)];
+                f12 = y1 >= {{input_width}} ? 0 : {{output_str}}[y1 + {{input_width}}*(x0 + {{input_height}}*f)];
 
-                tensor_temp[i + {{output_height}}*(j + {{output_width}}*f)] = (f11*(x1 - x)*(y1 - y) + f21*(x - x0)*(y1 - y) + f12*(x1 - x)*(y - y0) + f22*(x - x0)*(y - y0))/((x1 - x0)*(y1 - y0));
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = (f11*(x1 - x)*(y1 - y) + f21*(x - x0)*(y1 - y) + f12*(x1 - x)*(y - y0) + f22*(x - x0)*(y - y0))/((x1 - x0)*(y1 - y0));
                 {{#linear}}
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{activation_function}}};
                 {{/linear}}
                 {{#fused_layer}}
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{{fused_layer}}};
                 {{/fused_layer}}
             }
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.2.2/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 {{#is_resize}}
     float x;
     float y;
     int x0;
     int y0;
 {{/is_resize}}
 {{#is_cubic_interpolation}}
+    int col_index;
     float a;
     float f_1;
     float f0;
     float f1;
     float f2;
     float s;
 {{/is_cubic_interpolation}}
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.2.2/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2.1.post1
+Version: 0.2.2
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
+Requires-Python: <3.12,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: COPYING
 License-File: AUTHORS.md
 Requires-Dist: numpy==1.23.5
 Requires-Dist: numpyencoder==0.3.0
 Requires-Dist: onnx==1.14.0
```

### Comparing `acetone_nnet-0.2.1.post1/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.2.2/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

