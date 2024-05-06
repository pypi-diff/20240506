# Comparing `tmp/iinfer-0.7.2.tar.gz` & `tmp/iinfer-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.7.2.tar", last modified: Sat May  4 14:25:37 2024, max compression
+gzip compressed data, was "iinfer-0.7.3.tar", last modified: Mon May  6 13:44:21 2024, max compression
```

## Comparing `iinfer-0.7.2.tar` & `iinfer-0.7.3.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.497782 iinfer-0.7.2/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-05-04 14:25:37.496655 iinfer-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.792142 iinfer-0.7.2/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.837139 iinfer-0.7.2/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.2/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    51232 2024-05-04 02:38:57.000000 iinfer-0.7.2/iinfer/app/app.py
--rw-rw-rw-   0        0        0    34473 2024-05-03 08:22:57.000000 iinfer-0.7.2/iinfer/app/client.py
--rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.2/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.845140 iinfer-0.7.2/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.2/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7868 2024-05-04 02:31:10.000000 iinfer-0.7.2/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0     3613 2024-05-03 05:30:54.000000 iinfer-0.7.2/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.2/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.875142 iinfer-0.7.2/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.2/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.2/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.2/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.2/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.2/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.2/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.2/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.2/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    15606 2024-05-04 00:27:42.000000 iinfer-0.7.2/iinfer/app/install.py
--rw-rw-rw-   0        0        0   157090 2024-05-04 14:14:31.000000 iinfer-0.7.2/iinfer/app/options.py
--rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.2/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.910142 iinfer-0.7.2/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.2/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.2/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.2/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.2/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.2/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.951140 iinfer-0.7.2/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     3511 2024-05-04 02:00:36.000000 iinfer-0.7.2/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
--rw-rw-rw-   0        0        0     7618 2024-05-04 02:00:29.000000 iinfer-0.7.2/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-05-04 02:00:22.000000 iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-05-04 02:00:25.000000 iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-05-04 02:00:14.000000 iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-05-04 02:00:18.000000 iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-05-04 02:00:10.000000 iinfer-0.7.2/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-05-04 02:00:06.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_San.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    51835 2024-05-04 00:33:11.000000 iinfer-0.7.2/iinfer/app/server.py
--rw-rw-rw-   0        0        0    25891 2024-05-04 13:34:13.000000 iinfer-0.7.2/iinfer/app/web.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.967141 iinfer-0.7.2/iinfer/docker/
--rw-rw-rw-   0        0        0      835 2024-05-03 11:17:19.000000 iinfer-0.7.2/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.976140 iinfer-0.7.2/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.737139 iinfer-0.7.2/iinfer/extensions/configs/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.997139 iinfer-0.7.2/iinfer/extensions/configs/mmdet/
--rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tta.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.014143 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/
--rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
--rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.059145 iinfer-0.7.2/iinfer/extensions/configs/mmseg/
--rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.093141 iinfer-0.7.2/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.2/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.2/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.2/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.2/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.2/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.2/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.2/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.2/iinfer/extensions/injection/before_gray_injection.json
--rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/label_coco.txt
--rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/label_voc.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.342355 iinfer-0.7.2/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.2/iinfer/logconf_web.yml
--rw-rw-rw-   0        0        0     1009 2024-05-04 14:24:26.000000 iinfer-0.7.2/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.344875 iinfer-0.7.2/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.744139 iinfer-0.7.2/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.365879 iinfer-0.7.2/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.391820 iinfer-0.7.2/iinfer/web/assets/iinfer/
--rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/filer_modal.js
--rw-rw-rw-   0        0        0    16699 2024-05-04 14:05:33.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/list_cmd.js
--rw-rw-rw-   0        0        0     6537 2024-04-30 13:37:34.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/list_pipe.js
--rw-rw-rw-   0        0        0     5958 2024-05-01 13:45:13.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/main.js
--rw-rw-rw-   0        0        0      421 2024-04-30 13:38:58.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/open_capture.js
--rw-rw-rw-   0        0        0      441 2024-04-30 13:39:09.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/open_output_json.js
--rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.css
--rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.js
--rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/view_raw.js
--rw-rw-rw-   0        0        0     6154 2024-05-02 12:27:53.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/view_result.js
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.394844 iinfer-0.7.2/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.397842 iinfer-0.7.2/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.432508 iinfer-0.7.2/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.459640 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.743140 iinfer-0.7.2/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.461936 iinfer-0.7.2/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.476307 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.480754 iinfer-0.7.2/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.745139 iinfer-0.7.2/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.483598 iinfer-0.7.2/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.492071 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.494480 iinfer-0.7.2/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    31056 2024-05-02 03:04:28.000000 iinfer-0.7.2/iinfer/web/gui.html
-drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.806139 iinfer-0.7.2/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8706 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 14:25:37.498305 iinfer-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.230419 iinfer-0.7.3/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-05-06 13:44:21.229422 iinfer-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.191863 iinfer-0.7.3/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.329862 iinfer-0.7.3/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.3/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    51232 2024-05-04 02:38:57.000000 iinfer-0.7.3/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    34708 2024-05-06 10:14:38.000000 iinfer-0.7.3/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.3/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.336860 iinfer-0.7.3/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.3/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7868 2024-05-04 02:31:10.000000 iinfer-0.7.3/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0     3613 2024-05-06 11:42:49.000000 iinfer-0.7.3/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.3/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.379865 iinfer-0.7.3/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.3/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.3/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.3/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.3/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.3/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.3/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.3/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.3/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    15606 2024-05-06 13:43:20.000000 iinfer-0.7.3/iinfer/app/install.py
+-rw-rw-rw-   0        0        0   157617 2024-05-06 06:48:17.000000 iinfer-0.7.3/iinfer/app/options.py
+-rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.3/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.426863 iinfer-0.7.3/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.3/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.3/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.3/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.3/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.3/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.3/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.503862 iinfer-0.7.3/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     3511 2024-05-04 02:00:36.000000 iinfer-0.7.3/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
+-rw-rw-rw-   0        0        0     7618 2024-05-04 02:00:29.000000 iinfer-0.7.3/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-05-04 02:00:22.000000 iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-05-04 02:00:25.000000 iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-05-04 02:00:14.000000 iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-05-04 02:00:18.000000 iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-05-04 02:00:10.000000 iinfer-0.7.3/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-05-04 02:00:06.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_San.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    52240 2024-05-06 13:43:15.000000 iinfer-0.7.3/iinfer/app/server.py
+-rw-rw-rw-   0        0        0    26325 2024-05-06 11:47:13.000000 iinfer-0.7.3/iinfer/app/web.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.530866 iinfer-0.7.3/iinfer/docker/
+-rw-rw-rw-   0        0        0      835 2024-05-03 11:17:19.000000 iinfer-0.7.3/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.535862 iinfer-0.7.3/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.032858 iinfer-0.7.3/iinfer/extensions/configs/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.550863 iinfer-0.7.3/iinfer/extensions/configs/mmdet/
+-rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tta.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.565857 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/
+-rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
+-rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.595859 iinfer-0.7.3/iinfer/extensions/configs/mmseg/
+-rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.634860 iinfer-0.7.3/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.3/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.3/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.3/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.3/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.3/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.3/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.3/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.3/iinfer/extensions/injection/before_gray_injection.json
+-rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/label_coco.txt
+-rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/extensions/label_voc.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.955863 iinfer-0.7.3/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.3/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.3/iinfer/logconf_web.yml
+-rw-rw-rw-   0        0        0     1009 2024-05-06 07:29:42.000000 iinfer-0.7.3/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.959860 iinfer-0.7.3/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.046859 iinfer-0.7.3/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.979862 iinfer-0.7.3/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.024860 iinfer-0.7.3/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5860 2024-05-06 08:38:02.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    17895 2024-05-06 07:34:09.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6656 2024-05-06 07:47:25.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     6108 2024-05-06 08:52:26.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      433 2024-05-06 08:59:02.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      453 2024-05-06 08:59:20.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    25087 2024-05-06 11:21:46.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1299 2024-05-06 11:27:57.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     6234 2024-05-06 11:33:29.000000 iinfer-0.7.3/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.068859 iinfer-0.7.3/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.079861 iinfer-0.7.3/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.109858 iinfer-0.7.3/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.153007 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.046859 iinfer-0.7.3/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.159007 iinfer-0.7.3/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.184598 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.188115 iinfer-0.7.3/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.048860 iinfer-0.7.3/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.192715 iinfer-0.7.3/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.221422 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:21.226422 iinfer-0.7.3/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.3/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    31077 2024-05-06 05:48:36.000000 iinfer-0.7.3/iinfer/web/gui.html
+drwxrwxrwx   0        0        0        0 2024-05-06 13:44:20.222862 iinfer-0.7.3/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8706 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 13:44:19.000000 iinfer-0.7.3/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:44:21.231421 iinfer-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.3/setup.py
```

### Comparing `iinfer-0.7.2/LICENSE` & `iinfer-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/PKG-INFO` & `iinfer-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.2
+Version: 0.7.3
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.2/README.md` & `iinfer-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/app.py` & `iinfer-0.7.3/iinfer/app/app.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/client.py` & `iinfer-0.7.3/iinfer/app/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,58 +504,58 @@
         Args:
             svpath (Path): サーバー上のファイルパス
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
-        res_json = self._proc(self.svname, 'file_list', [str(svpath)], timeout=timeout)
+        res_json = self._proc(self.svname, 'file_list', [convert.str2b64str(str(svpath))], timeout=timeout)
         return res_json
 
     def file_mkdir(self, svpath:str, timeout:int = 60):
         """
         サーバー上にディレクトリを作成する
 
         Args:
             svpath (Path): サーバー上のディレクトリパス
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
-        res_json = self._proc(self.svname, 'file_mkdir', [str(svpath)], timeout=timeout)
+        res_json = self._proc(self.svname, 'file_mkdir', [convert.str2b64str(str(svpath))], timeout=timeout)
         return res_json
     
     def file_rmdir(self, svpath:str, timeout:int = 60):
         """
         サーバー上のディレクトリを削除する
 
         Args:
             svpath (Path): サーバー上のディレクトリパス
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
-        res_json = self._proc(self.svname, 'file_rmdir', [str(svpath)], timeout=timeout)
+        res_json = self._proc(self.svname, 'file_rmdir', [convert.str2b64str(str(svpath))], timeout=timeout)
         return res_json
     
     def file_download(self, svpath:str, download_file:Path, timeout:int = 60):
         """
         サーバー上のファイルをダウンロードする
 
         Args:
             svpath (Path): サーバー上のファイルパス
             download_file (Path): ローカルのファイルパス
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             bytes: ダウンロードファイルの内容
         """
-        res_json = self._proc(self.svname, 'file_download', [str(svpath)], timeout=timeout)
+        res_json = self._proc(self.svname, 'file_download', [convert.str2b64str(str(svpath))], timeout=timeout)
         if "success" in res_json:
             if download_file is not None:
                 if download_file.is_dir():
                     download_file = download_file / res_json["success"]["name"]
                 if download_file.exists():
                     self.logger.error(f"download_file {download_file} already exists.")
                     return {"error": f"download_file {download_file} already exists."}
@@ -583,29 +583,32 @@
         if not upload_file.exists():
             self.logger.error(f"input_file {upload_file} does not exist.")
             return {"error": f"input_file {upload_file} does not exist."}
         if upload_file.is_dir():
             self.logger.error(f"input_file {upload_file} is directory.")
             return {"error": f"input_file {upload_file} is directory."}
         with open(upload_file, "rb") as f:
-            res_json = self._proc(self.svname, 'file_upload', [str(svpath), upload_file.name, base64.b64encode(f.read()).decode('utf-8')], timeout=timeout)
+            res_json = self._proc(self.svname, 'file_upload',
+                                  [convert.str2b64str(str(svpath)),
+                                   convert.str2b64str(upload_file.name),
+                                   convert.bytes2b64str(f.read())], timeout=timeout)
             return res_json
 
     def file_remove(self, svpath:str, timeout:int = 60):
         """
         サーバー上のファイルを削除する
 
         Args:
             svpath (Path): サーバー上のファイルパス
             timeout (int, optional): タイムアウト時間. Defaults to 60.
 
         Returns:
             dict: Redisサーバーからの応答
         """
-        res_json = self._proc(self.svname, 'file_remove', [str(svpath)], timeout=timeout)
+        res_json = self._proc(self.svname, 'file_remove', [convert.str2b64str(str(svpath))], timeout=timeout)
         return res_json
 
     def capture(self, capture_device='0', image_type:str='capture', capture_frame_width:int=None, capture_frame_height:int=None, capture_fps:int=1000, output_preview:bool=False):
         """
         ビデオをキャプチャしてその結果を出力する
 
         Args:
```

### Comparing `iinfer-0.7.2/iinfer/app/common.py` & `iinfer-0.7.3/iinfer/app/common.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/commons/convert.py` & `iinfer-0.7.3/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/commons/module.py` & `iinfer-0.7.3/iinfer/app/commons/module.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/gui.py` & `iinfer-0.7.3/iinfer/app/gui.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injection.py` & `iinfer-0.7.3/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_det_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_http_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.7.3/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.7.3/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/install.py` & `iinfer-0.7.3/iinfer/app/install.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/options.py` & `iinfer-0.7.3/iinfer/app/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,29 @@
 
 class Options:
     def __init__(self):
         self._options = dict()
         self.init_options()
 
     def get_mode_opt(self):
-        return [''] + [mode for mode in self._options["mode"]["choise"]]
+        return [''] + [{key:val} for key,val in self._options["mode"].items() if type(val) == dict]
 
     def get_cmd_opt(self, mode):
         if mode not in self._options["cmd"]:
             return ['Please select mode.']
-        ret = [key for key in self._options["cmd"][mode].keys()]
+        ret = [{key:val} for key,val in self._options["cmd"][mode].items() if type(val) == dict]
         if len(ret) > 0:
             return [''] + ret
         return ['Please select mode.']
 
     def get_opt_opt(self, mode, cmd):
         if mode not in self._options["cmd"]:
             return [f'Unknown mode. ({mode})']
-        if cmd not in self._options["cmd"][mode]:
-            return [f'Unknown cmd. ({cmd})']
-        if cmd is None or cmd == "":
-            return ['Please select command.']
+        if cmd is None or cmd == "" or cmd not in self._options["cmd"][mode]:
+            return []
         return self._options["cmd"][mode][cmd]["choise"]
 
     def init_options(self):
         self._options = dict()
         self._options["useopt"] = dict(
             short="u", type="str", default=None, required=False, multi=False, hide=True,
             discription_ja="オプションを保存しているファイルを使用します。",
@@ -45,29 +43,26 @@
             choise=None)
         self._options["version"] = dict(
             short="v", type="bool", default=None, required=False, multi=False, hide=True,
             discription_ja="バージョン表示",
             discription_en="Display version",
             choise=None)
         self._options["mode"] = dict(
-            short="m",
-            type="str",
-            default=None,
-            required=True,
-            multi=False,
-            hide=True,
+            short="m", type="str", default=None, required=True, multi=False, hide=True,
             discription_ja="起動モードを指定します。",
             discription_en="Specify the startup mode.",
             choise=[])
         self._options["cmd"] = dict(
             short="c", type="str", default=None, required=True, multi=False, hide=True,
             discription_ja="コマンドを指定します。",
             discription_en="Specify the command.",
             choise=[],
             client=dict(
+                discription_ja="クライアントモード",
+                discription_en="Client mode",
                 deploy=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="AIモデルをサーバーに配備します。",
                     discription_en="Deploy AI model to server.",
                     choise=[
                         dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
                             discription_ja="Redisサーバーのサービスホストを指定します。",
@@ -126,15 +121,15 @@
                             discription_en="Specify the setting file for post-processing."),
                         dict(opt="after_injection_py", type="file", default="", required=False, multi=True, hide=True, choise=None, fileio="in",
                             discription_ja="独自の後処理を作成するときに指定。",
                             discription_en="Specify when creating custom post-processing."),
                         dict(opt="overwrite", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False],
                             discription_ja="デプロイ済みであっても上書きする指定。",
                             discription_en="Specify to overwrite even if it is already deployed."),
-                        dict(opt="timeout", type="bool", default=True, required=False, multi=False, hide=False, choise=[True, False],
+                        dict(opt="timeout", type="int", default=120, required=False, multi=False, hide=False, choise=None,
                             discription_ja="サーバーの応答が返ってくるまでの最大待ち時間を指定。",
                             discription_en="Specify the maximum waiting time until the server responds."),
                         dict(opt="output_json", short="o", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                             discription_ja="処理結果jsonの保存先ファイルを指定。",
                             discription_en="Specify the destination file for saving the processing result json."),
                         dict(opt="output_json_append", short="a", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False],
                             discription_ja="処理結果jsonファイルを追記保存します。",
@@ -640,14 +635,16 @@
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
             ),
             postprocess=dict(
+                discription_ja="後処理モード",
+                discription_en="Post-processing mode",
                 cls_jadge=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="推論結果を使用して画像分類判定を行います。",
                     discription_en="Perform image classification judgment using the inference result.",
                     choise=[
                         dict(short="i", opt="input_file", type="file", default="", required=False, multi=False, hide=False, choise=None, fileio="in",
                              discription_ja="後処理させる推論結果をファイルで指定します。",
@@ -1017,14 +1014,16 @@
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
             ),
             server=dict(
+                discription_ja="サーバーモード",
+                discription_en="Server mode",
                 start=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="推論サーバーを起動します。installモードで `iinfer -m install -c server` を実行している場合は、 `docker-compose up -d` を使用してください。",
                     discription_en="Start the inference server. If you are running `iinfer -m install -c server` in install mode, use `docker-compose up -d`.",
                     choise=[
                         dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスホストを指定します。",
@@ -1118,14 +1117,16 @@
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
             ),
             redis=dict(
+                discription_ja="Redisモード",
+                discription_en="Redis mode",
                 docker_run=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="installモードで `iinfer -m install -c server` を実行している場合は、 `docker-compose up -d` を使用してください。",
                     discription_en="If you are running `iinfer -m install -c server` in install mode, use `docker-compose up -d`.",
                     choise=[
                         dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None,
                              discription_ja="Redisサーバーのサービスポートを指定します。",
@@ -1176,14 +1177,16 @@
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
             ),
             install=dict(
+                discription_ja="インストールモード",
+                discription_en="Install mode",
                 onnx=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="`onnxruntime` をインストールします。",
                     discription_en="Install `onnxruntime`.",
                     choise=[
                         dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None, fileio="out",
                              discription_ja="処理結果jsonの保存先ファイルを指定。",
@@ -1359,14 +1362,16 @@
                         dict(opt="capture_stdout", type="bool", default=True, required=False, multi=False, hide=True, choise=[True, False],
                              discription_ja="GUIモードでのみ使用可能です。コマンド実行時の標準出力をキャプチャーし、実行結果画面に表示します。",
                              discription_en="Available only in GUI mode. Captures standard output during command execution and displays it on the execution result screen."),
                     ]
                 ),
             ),
             web=dict(
+                discription_ja="Webモード",
+                discription_en="Web mode",
                 start=dict(
                     type="str", default=None, required=False, multi=False, hide=False,
                     discription_ja="Webモードを起動します。",
                     discription_en="Start Web mode.",
                     choise=[
                         dict(opt="data", type="file", default=None, required=False, multi=False, hide=False, choise=None,
                              discription_ja="省略した時は `$HONE/.iinfer` を使用します。",
@@ -1398,9 +1403,9 @@
             )
         )
         for key, mode in self._options["cmd"].items():
             if type(mode) is not dict:
                 continue
             self._options["cmd"]["choise"] += [cmd for cmd in mode.keys()]
             self._options["mode"][key] = mode
-            self._options["mode"]["choise"] += [key]
+            self._options["mode"]["choise"] += [mode]
```

### Comparing `iinfer-0.7.2/iinfer/app/postprocess.py` & `iinfer-0.7.3/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.7.3/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/csv.py` & `iinfer-0.7.3/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.7.3/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.7.3/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.7.3/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.7.3/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.7.3/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.7.3/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.7.3/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predict.py` & `iinfer-0.7.3/iinfer/app/predict.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py` & `iinfer-0.7.3/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/insightface_det.py` & `iinfer-0.7.3/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.7.3/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.7.3/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.7.3/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.7.3/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.7.3/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.7.3/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.7.3/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/redis.py` & `iinfer-0.7.3/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/app/server.py` & `iinfer-0.7.3/iinfer/app/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,26 +226,33 @@
                     image = convert.npy2img(img_npy)
                     st = self.predict(msg[1], msg[2], image, output_image_name, nodraw)
                 elif msg[0] == 'stop_server':
                     self.is_running = False
                     self.responce(msg[1], {"success": f"Successful stop server. svname={self.svname}"})
                     break
                 elif msg[0] == 'file_list':
-                    st = self.file_list(msg[1], msg[2])
+                    svpath = convert.b64str2str(msg[2])
+                    st = self.file_list(msg[1], svpath)
                 elif msg[0] == 'file_mkdir':
-                    st = self.file_mkdir(msg[1], msg[2])
+                    svpath = convert.b64str2str(msg[2])
+                    st = self.file_mkdir(msg[1], svpath)
                 elif msg[0] == 'file_rmdir':
-                    st = self.file_rmdir(msg[1], msg[2])
+                    svpath = convert.b64str2str(msg[2])
+                    st = self.file_rmdir(msg[1], svpath)
                 elif msg[0] == 'file_download':
-                    st = self.file_download(msg[1], msg[2])
+                    svpath = convert.b64str2str(msg[2])
+                    st = self.file_download(msg[1], svpath)
                 elif msg[0] == 'file_upload':
+                    svpath = convert.b64str2str(msg[2])
+                    file_name = convert.b64str2str(msg[3])
                     file_data = convert.b64str2bytes(msg[4])
-                    st = self.file_upload(msg[1], msg[2], msg[3], file_data)
+                    st = self.file_upload(msg[1], svpath, file_name, file_data)
                 elif msg[0] == 'file_remove':
-                    st = self.file_remove(msg[1], msg[2])
+                    svpath = convert.b64str2str(msg[2])
+                    st = self.file_remove(msg[1], svpath)
                 else:
                     self.logger.warn(f"Unknown command {msg}")
                     st = self.RESP_WARN
 
                 if st==self.RESP_SCCESS:
                     sccess_cnt += 1
                     self.redis_cli.hset(self.hbname, 'sccess_cnt', str(sccess_cnt))
```

### Comparing `iinfer-0.7.2/iinfer/app/web.py` & `iinfer-0.7.3/iinfer/app/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,53 +203,62 @@
         for i, part in enumerate(current_path.parts):
             path = Path('/'.join(current_path.parts[:i+1]))
             if not os.access(path, os.R_OK):
                 continue
             path_key = mk_key(path)
             children = None
             if path.is_dir():
-                children = {mk_key(p):dict(name=p.name, is_dir=p.is_dir(), path=str(p), size=p.stat().st_size, last=ts2str(p.stat().st_mtime)) for p in path.iterdir()}
+                try:
+                    children = {mk_key(p):dict(name=p.name, is_dir=p.is_dir(), path=str(p), size=p.stat().st_size, last=ts2str(p.stat().st_mtime)) for p in path.iterdir()}
+                except:
+                    children = {}
             path_tree[path_key] = dict(name=part, is_dir=path.is_dir(), path=str(path), children=children, size=path.stat().st_size, last=ts2str(path.stat().st_mtime))
         return path_tree
 
     def load_result(self, current_path):
         current_path = Path(current_path)
         if not current_path.is_file():
             return {'warn': f'A non-file was selected.: {current_path}'}
-        with open(current_path, 'r', encoding='utf-8') as f:
-            ret = []
-            for line in f:
-                res_json = json.loads(line)
-                if 'output_image' in res_json and 'output_image_shape' in res_json:
-                    img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
-                    img_bytes = convert.npy2imgfile(img_npy, image_type='jpeg')
-                    res_json["output_image"] = convert.bytes2b64str(img_bytes)
-                ret.append(res_json)
-        return ret
+        try:
+            with open(current_path, 'r', encoding='utf-8') as f:
+                ret = []
+                for line in f:
+                    res_json = json.loads(line)
+                    if 'output_image' in res_json and 'output_image_shape' in res_json:
+                        img_npy = convert.b64str2npy(res_json["output_image"], res_json["output_image_shape"])
+                        img_bytes = convert.npy2imgfile(img_npy, image_type='jpeg')
+                        res_json["output_image"] = convert.bytes2b64str(img_bytes)
+                    ret.append(res_json)
+            return ret
+        except:
+            return {'warn': f'An error occurred while reading the file.: {current_path}'}
 
     def load_capture(self, current_path):
         current_path = Path(current_path)
         if not current_path.is_file():
             return {'warn': f'A non-file was selected.: {current_path}'}
-        with open(current_path, 'r', encoding='utf-8') as f:
-            ret = []
-            for line in f:
-                cel = line.split(',')
-                res_json = dict(success=dict(image_name=cel[5]),
-                                output_image=None,
-                                output_image_shape=(int(cel[2]),int(cel[3]),int(cel[4])),
-                                output_image_name=cel[5])
-                if cel[0] == 'capture':
-                    img_npy = convert.b64str2npy(cel[1], res_json["output_image_shape"])
-                    img_bytes = convert.npy2imgfile(img_npy, image_type='jpeg')
-                    res_json["output_image"] = convert.bytes2b64str(img_bytes)
-                else:
-                    res_json["output_image"] = cel[1]
-                ret.append(res_json)
-        return ret
+        try:
+            with open(current_path, 'r', encoding='utf-8') as f:
+                ret = []
+                for line in f:
+                    cel = line.split(',')
+                    res_json = dict(success=dict(image_name=cel[5]),
+                                    output_image=None,
+                                    output_image_shape=(int(cel[2]),int(cel[3]),int(cel[4])),
+                                    output_image_name=cel[5])
+                    if cel[0] == 'capture':
+                        img_npy = convert.b64str2npy(cel[1], res_json["output_image_shape"])
+                        img_bytes = convert.npy2imgfile(img_npy, image_type='jpeg')
+                        res_json["output_image"] = convert.bytes2b64str(img_bytes)
+                    else:
+                        res_json["output_image"] = cel[1]
+                    ret.append(res_json)
+            return ret
+        except:
+            return {'warn': f'An error occurred while reading the file.: {current_path}'}
     
     def list_pipe(self, kwd):
         if kwd is None or kwd == '':
             kwd = '*'
         paths = glob.glob(str(self.data / f"pipe-{kwd}.json"))
         return [common.loadopt(path) for path in paths]
```

### Comparing `iinfer-0.7.2/iinfer/docker/Dockerfile` & `iinfer-0.7.3/iinfer/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tta.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmdet/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.3/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/extensions/label_coco.txt` & `iinfer-0.7.3/iinfer/extensions/label_coco.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.7.3/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/licenses/files.txt` & `iinfer-0.7.3/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_client.yml` & `iinfer-0.7.3/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_gui.yml` & `iinfer-0.7.3/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_install.yml` & `iinfer-0.7.3/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_postprocess.yml` & `iinfer-0.7.3/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_redis.yml` & `iinfer-0.7.3/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_server.yml` & `iinfer-0.7.3/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/logconf_web.yml` & `iinfer-0.7.3/iinfer/logconf_web.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/version.py` & `iinfer-0.7.3/iinfer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 5, 4)
+dt_now = datetime.datetime(2024, 5, 6)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.7.2'
+__version__ = '0.7.3'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.7.3/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/filer_modal.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/filer_modal.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,97 @@
 // ファイラーモーダル
 filer_modal_func = async (target_id, modal_title, current_path, call_back_func) => {
-    filer_modal = $('#filer_modal');
+    const filer_modal = $('#filer_modal');
     filer_modal.find('.modal-title').text(modal_title);
     filer_modal.find('.modal-body').html('<ul class="tree-menu overflow-auto border col-4"></ul><div class="file-list overflow-auto col-8"></div>');
     filer_modal.find('.tree-menu').css('height', 'calc(100vh - 180px)');
     filer_modal.find('.file-list').css('height', 'calc(100vh - 180px)');
     //filer_modal.find('.tree-menu').resizable({ghost:true});
     filer_modal.find('.filer_address_bot').off('click').on('click', async () => {
-        current_path = filer_modal.find('.filer_address').val();
-        key = current_path.replace(/[\s\:\\\/\,\.\#\$\%\^\&\!\@\*\(\)\{\}\[\]\'\"\`]/g, `_`);
-        current_node = $(`#${key}`);
+        const c_path = filer_modal.find('.filer_address').val();
+        const key = c_path.replace(/[\s\:\\\/\,\.\#\$\%\^\&\!\@\*\(\)\{\}\[\]\'\"\`]/g, `_`);
+        const current_node = $(`#${key}`);
         if (current_node.length <= 0) {
             alert(`invalid path:${key}`);
             return;
         }
-        await reload_tree(target_id, filer_modal.find('.tree-menu'), current_path, filer_modal.find('.file-list'));
+        await reload_tree(target_id, filer_modal.find('.tree-menu'), c_path, filer_modal.find('.file-list'));
     });
 
-    reload_tree = async (target_id, current_node, current_path, file_list_elem) => {
+    const reload_tree = async (target_id, current_node, current_path, file_list_elem) => {
         //dict(name=part, is_dir=path.is_dir(), path=str(path), children=children)
-        py_list_tree = await eel.list_tree(current_path)();
+        const py_list_tree = await eel.list_tree(current_path)();
         current_node.html('');
-        $.each(py_list_tree, (key, node) => {
+        Object.entries(py_list_tree).forEach(([key, node]) => {
             if (!node['is_dir']) return;
-            li_elem = $(`#${key}`);
+            let li_elem = $(`#${key}`);
             if (li_elem.length > 0) {
                 li_elem.html(`<a href="#" class="folder-open">${node['name']}</a>`);
             } else {
                 li_elem = $(`<li id="${key}"><a href="#" class="folder-open">${node['name']}</a></li>`);
                 current_node.append(li_elem);
             }
-            mk_func = (target_id, current_node, current_path) => {
+            const mk_func = (target_id, current_node, current_path) => {
                 // 左側ペインのフォルダを選択した時の処理
                 return () => reload_tree(target_id, current_node, current_path);
             }
             li_elem.find('a').off('click').on('click', mk_func(target_id, current_node, node['path']));
             if (node['children']) {
-                ul_elem = $('<ul/>');
+                const ul_elem = $('<ul/>');
                 li_elem.append(ul_elem);
-                $.each(node['children'], (k, n) => {
+                Object.entries(node['children']).forEach(([k, n]) => {
                     if (!n['is_dir']) return;
-                    li = $(`<li id="${k}"><a href="#" class="folder-close">${n['name']}</a></li>`);
+                    const li = $(`<li id="${k}"><a href="#" class="folder-close">${n['name']}</a></li>`);
                     li.find('a').click(mk_func(target_id, ul_elem, n['path']));
                     ul_elem.append(li);
                 });
             }
         });
-        py_list_tree_keys = Object.keys(py_list_tree);
+        const py_list_tree_keys = Object.keys(py_list_tree);
         if (py_list_tree_keys.length > 0) {
-            node = py_list_tree[py_list_tree_keys[py_list_tree_keys.length - 1]];
-            table = $('<table class="table table-bordered table-hover table-sm"></table>');
+            const node = py_list_tree[py_list_tree_keys[py_list_tree_keys.length - 1]];
+            const table = $('<table class="table table-bordered table-hover table-sm"></table>');
             filer_modal.find('.file-list').html('');
             filer_modal.find('.file-list').append(table);
-            table_head = $('<thead class="table-dark bg-dark"></thead>');
+            const table_head = $('<thead class="table-dark bg-dark"></thead>');
             table_head.append($('<tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr>'));
             table.append(table_head);
-            table_body = $('<tbody></tbody>');
+            const table_body = $('<tbody></tbody>');
             table.append(table_body);
             filer_modal.find('.filer_address').val(node['path']);
             if (node['children']) {
-                mk_func = (target_id, current_node, current_path) => {
+                const mk_file_func = (target_id, current_node, current_path) => {
                     // 右側ペインのフォルダを選択した時の処理
                     return () => reload_tree(target_id, current_node, current_path);
                 }
-                $.each(node['children'], (k, n) => {
+                Object.entries(node['children']).forEach(([k, n]) => {
                     if (!n['is_dir']) return;
-                    tr_elem = $('<tr/>');
+                    const tr_elem = $('<tr/>');
                     table_body.append(tr_elem);
-                    td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
-                    td.find('a').click(mk_func(target_id, $(`#${k}`), n['path']));
+                    const td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
+                    td.find('a').click(mk_file_func(target_id, $(`#${k}`), n['path']));
                     tr_elem.append($('<td><img src="/assets/tree-menu/image/folder-close.png"></td>'));
                     tr_elem.append(td);
                     tr_elem.append($(`<td>${n['size']}</td>`));
                     tr_elem.append($(`<td>${n['last']}</td>`));
                 });
-                mk_func = (target_id, current_node, current_path) => {
+                const mk_dir_func = (target_id, current_node, current_path) => {
                     // 右側ペインのファイルを選択した時の処理
                     return () => {
                         $(`[id="${target_id}"]`).val(current_path);
                         filer_modal.modal('hide');
                         if (call_back_func) call_back_func(current_path);
                     }
                 }
-                $.each(node['children'], (k, n) => {
+                Object.entries(node['children']).forEach(([k, n]) => {
                     if (n['is_dir']) return;
-                    tr_elem = $('<tr/>');
+                    const tr_elem = $('<tr/>');
                     table_body.append(tr_elem);
-                    td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
-                    td.find('a').click(mk_func(target_id, $(`#${k}`), n['path']));
+                    const td = $(`<td><a href="#" class="folder-close">${n['name']}</a></td>`);
+                    td.find('a').click(mk_dir_func(target_id, $(`#${k}`), n['path']));
                     tr_elem.append($('<td><img src="/assets/tree-menu/image/file.png"></td>'));
                     tr_elem.append(td);
                     tr_elem.append($(`<td>${n['size']}</td>`));
                     tr_elem.append($(`<td>${n['last']}</td>`));
                 });
             }
         }
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/list_cmd.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/list_cmd.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,168 +1,182 @@
 // 保存済みコマンドファイル一覧の取得
-list_cmd_func = async () => {
+const list_cmd_func = async () => {
     $('#cmd_items').html('');
-    kwd = $('#cmd_kwd').val();
-    py_list_cmd = await eel.list_cmd(kwd ? `*${kwd}*` : '*')();
-    $.each(py_list_cmd, (i, row) => {
-        elem = $($('#cmd_template').html());
-        elem.find('.cmd_title').text(row['title']);
-        elem.find('.cmd_mode').text(row['mode']);
-        elem.find('.cmd_cmd').text(row['cmd']);
+    const kwd = $('#cmd_kwd').val();
+    const py_list_cmd = await eel.list_cmd(kwd ? `*${kwd}*` : '*')();
+    py_list_cmd.forEach(row => {
+        const elem = $($('#cmd_template').html());
+        elem.find('.cmd_title').text(row.title);
+        elem.find('.cmd_mode').text(row.mode);
+        elem.find('.cmd_cmd').text(row.cmd);
         $('#cmd_items').append(elem);
     });
     $('#cmd_items').append($($('#cmd_add').html()));
 }
 // コマンドファイルの取得が出来た時の処理
-list_cmd_func_then = () => {
+const list_cmd_func_then = () => {
     // 配列をoptionタグに変換
-    mkopt = (arr) => {
-        var opt = '';
-        for (var i = 0; arr && i < arr.length; i++) {
-            opt += `<option value="${arr[i]}">${arr[i]}</option>`;
-        }
+    const mkopt = (arr) => {
+        if (!arr) return '';
+        const opt = arr.map(row => {
+            if (typeof row === 'object') {
+                key = Object.keys(row)[0];
+                d = window.navigator.language == 'ja' ? row[key].discription_ja : row[key].discription_en;
+                return `<option value="${key}" discription="${d}">${key}</option>`;
+            }
+            return `<option value="${row}" discription="">${row}</option>`;
+        }).join('');
         return opt;
     }
     // コマンドカードクリック時の処理（モーダルダイアログを開く）
-    cmd_card_func = async (e) => {
-        py_get_mode_opt = await eel.get_mode_opt()();
-        cmd_modal = $('#cmd_modal');
+    const cmd_card_func = async (e) => {
+        const py_get_mode_opt = await eel.get_mode_opt()();
+        const cmd_modal = $('#cmd_modal');
         cmd_modal.find('[name="mode"]').html(mkopt(py_get_mode_opt));
         // モード変更時の処理（モードに対するコマンド一覧を取得）
-        mode_change = async () => {
-            mode = cmd_modal.find('[name="mode"]').val();
-            py_get_cmd_opt = await eel.get_cmd_opt(mode)();
+        const mode_change = async () => {
+            const mode = cmd_modal.find('[name="mode"]').val();
+            const py_get_cmd_opt = await eel.get_cmd_opt(mode)();
             cmd_modal.find('[name="cmd"]').html(mkopt(py_get_cmd_opt));
+            const selected_mode = cmd_modal.find('[name="mode"] option:selected');
+            cmd_modal.find('.mode_label').attr('title', selected_mode.attr('discription'));
+            const row_content = cmd_modal.find('.row_content');
+            row_content.html('');
         }
         cmd_modal.find('[name="mode"]').off('change');
         cmd_modal.find('[name="mode"]').change(mode_change);
         cmd_modal.find('.is-invalid, .is-valid').removeClass('is-invalid').removeClass('is-valid');
-        row_content = cmd_modal.find('.row_content');
+        cmd_modal.find('.cmd_label').removeAttr('title');
+        const row_content = cmd_modal.find('.row_content');
         row_content.html('');
         // コマンド変更時の処理（コマンドに対するオプション一覧を取得）
-        cmd_change = async () => {
-            mode = cmd_modal.find('[name="mode"]').val();
-            cmd = cmd_modal.find('[name="cmd"]').val();
-            py_get_opt_opt = await eel.get_opt_opt(mode, cmd)();
+        const cmd_change = async () => {
+            const mode = cmd_modal.find('[name="mode"]').val();
+            const cmd = cmd_modal.find('[name="cmd"]').val();
+            const selected_cmd = cmd_modal.find('[name="cmd"] option:selected');
+            cmd_modal.find('.cmd_label').attr('title', selected_cmd.attr('discription'));
+            const py_get_opt_opt = await eel.get_opt_opt(mode, cmd)();
             row_content.html('');
             // オプション一覧をフォームに追加
-            add_form_func = (i, row, next_elem) => {
-                target_name = row['opt'];
-                if (!row['choise']) {
+            const add_form_func = (i, row, next_elem) => {
+                const target_name = row.opt;
+                let input_elem, elem;
+                if (!row.choise) {
                     elem = $(cmd_modal.find('.row_content_template_str').html());
                     if (next_elem) next_elem.after(elem);
                     else row_content.append(elem);
                     input_elem = elem.find('.row_content_template_input');
                     input_elem.removeClass('row_content_template_input');
-                    input_elem.val(row['default']);
+                    input_elem.val(row.default);
                 } else {
                     elem = $(cmd_modal.find('.row_content_template_choice').html());
                     if (next_elem) next_elem.after(elem);
                     else row_content.append(elem);
                     input_elem = elem.find('.row_content_template_select');
                     input_elem.removeClass('row_content_template_select');
-                    input_elem.html(mkopt(row['choise']));
-                    input_elem.val(`${row['default']}`);
+                    input_elem.html(mkopt(row.choise));
+                    input_elem.val(`${row.default}`);
                 }
-                index = 0;
+                let index = 0;
                 if (cmd_modal.find(`[name="${target_name}"]`).length > 0) {
                     index = 0;
-                    $.each(cmd_modal.find(`[name="${target_name}"][param_data_index]`), (i, val) => {
+                    cmd_modal.find(`[name="${target_name}"][param_data_index]`).each((i, val) => {
                         v = Number($(val).attr('param_data_index'));
                         if (index <= v) index = v + 1;
                     });
                 }
                 input_elem.attr('name', target_name);
                 input_elem.attr('id', target_name + index);
                 input_elem.attr('param_data_index', index);
-                input_elem.attr('required', row['required']);
-                input_elem.attr('param_data_type', row['type']);
-                input_elem.attr('param_data_multi', row['multi']);
+                input_elem.attr('required', row.required);
+                input_elem.attr('param_data_type', row.type);
+                input_elem.attr('param_data_multi', row.multi);
                 // ファイルタイプの場合はファイラーモーダルを開くボタンを追加
-                if (row['type'] == 'file') {
-                    btn = $('<button class="btn btn-secondary" type="button">file</button>');
+                if (row.type == 'file') {
+                    const btn = $('<button class="btn btn-secondary" type="button">file</button>');
                     input_elem.parent().append(btn);
-                    mk_func = (tid, tn) => {
+                    const mk_func = (tid, tn) => {
                         // tid, tnの値を残すためにクロージャーにする
                         return () => {
-                            current_path = $(`[id="${tid}"]`).val();
+                            const current_path = $(`[id="${tid}"]`).val();
                             filer_modal_func(tid, tn, current_path);
                         }
                     }
                     btn.click(mk_func(input_elem.attr('id'), input_elem.attr('name')));
                 }
                 // マルチの場合は追加ボタンを追加
-                if (row['multi']) {
-                    btn_a = $('<button class="btn btn-secondary add_buton" type="button"></button>');
+                if (row.multi) {
+                    const btn_a = $('<button class="btn btn-secondary add_buton" type="button"></button>');
                     btn_a.append('<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-plus" viewBox="0 0 16 16">' +
                         '<path d="M8 4a.5.5 0 0 1 .5.5v3h3a.5.5 0 0 1 0 1h-3v3a.5.5 0 0 1-1 0v-3h-3a.5.5 0 0 1 0-1h3v-3A.5.5 0 0 1 8 4z"/>' +
                         '</svg>');
                     input_elem.parent().append(btn_a);
-                    mk_func = (row, next_elem) => {
+                    let mk_func = (row, next_elem) => {
                         // row, next_elemの値を残すためにクロージャーにする
                         return () => {
                             add_form_func(0, row, next_elem);
                         }
                     }
                     btn_a.click(mk_func(row, input_elem.parent().parent()));
                     // 2個目以降は削除ボタンを追加
                     if (cmd_modal.find(`[name="${target_name}"]`).length > 1) {
                         mk_func = (del_elem, row) => {
                             // del_elemの値を残すためにクロージャーにする
                             return () => del_elem.remove();
                         }
-                        btn_t = $('<button class="btn btn-secondary" type="button"></button>');
+                        const btn_t = $('<button class="btn btn-secondary" type="button"></button>');
                         btn_t.append('<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-trash" viewBox="0 0 16 16">' +
                             '<path d="M5.5 5.5A.5.5 0 0 1 6 6v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm2.5 0a.5.5 0 0 1 .5.5v6a.5.5 0 0 1-1 0V6a.5.5 0 0 1 .5-.5zm3 .5a.5.5 0 0 0-1 0v6a.5.5 0 0 0 1 0V6z"/>' +
                             '<path fill-rule="evenodd" d="M14.5 3a1 1 0 0 1-1 1H13v9a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V4h-.5a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1H6a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1h3.5a1 1 0 0 1 1 1v1zM4.118 4 4 4.059V13a1 1 0 0 0 1 1h6a1 1 0 0 0 1-1V4.059L11.882 4H4.118zM2.5 3V2h11v1h-11z"/>' +
                             '</svg>');
                         input_elem.parent().append(btn_t);
                         btn_t.click(mk_func(input_elem.parent().parent(), row));
                     }
                 }
-                title = elem.find('.row_content_template_title');
+                const title = elem.find('.row_content_template_title');
                 title.html('');
-                title.attr('title', window.navigator.language == 'ja' ? row['discription_ja'] : row['discription_en'])
-                if (row['required']) {
+                title.attr('title', window.navigator.language == 'ja' ? row.discription_ja : row.discription_en)
+                if (row.required) {
                     title.append('<span class="text-danger">*</span>');
                 }
-                title.append(`<span>${row['opt']}</span>`);
-                if (row['hide']) {
-                    elem.addClass('row_content_hide');
+                title.append(`<span>${row.opt}</span>`);
+                if (row.hide) {
+                    elem.addClass('row_content_hide').hide();
                 } else {
                     title.addClass('text-decoration-underline');
                 }
             }
-            $.each(py_get_opt_opt, add_form_func);
-            row_content.find('.row_content_hide').hide();
+            // 表示オプションを追加
+            py_get_opt_opt.filter(row => !row.hide).forEach((row, i) => add_form_func(i, row, null));
             // 高度なオプションを表示するリンクを追加
-            if (row_content.children().is('.row_content_hide')) {
-                show_link = $('<div class="text-center card-hover"><a href="#">[ advanced options ]</a></div>');
-                show_link.click(() => row_content.find('.row_content_hide').toggle());
-                row_content.append(show_link);
-            }
+            const show_link = $('<div class="text-center card-hover mb-3"><a href="#">[ advanced options ]</a></div>');
+            show_link.click(() => row_content.find('.row_content_hide').toggle());
+            row_content.append(show_link);
+            // 非表示オプションを追加
+            py_get_opt_opt.filter(row => row.hide).forEach((row, i) => add_form_func(i, row, null));
         }
         //row_content.find('is-invalid, is-valid').removeClass('is-invalid').removeClass('is-valid');
         cmd_modal.find('[name="cmd"]').off('change');
         cmd_modal.find('[name="cmd"]').change(cmd_change);
-        modal_title = $(e.currentTarget).find('.cmd_title').text();
+        let modal_title = $(e.currentTarget).find('.cmd_title').text();
         if (modal_title != '') {
             // コマンドファイルの読み込み
-            py_load_cmd = await eel.load_cmd(modal_title)();
-            cmd_modal.find('[name="mode"]').val(py_load_cmd['mode']);
+            const py_load_cmd = await eel.load_cmd(modal_title)();
+            cmd_modal.find('[name="mode"]').val(py_load_cmd.mode);
             await mode_change();
-            cmd_modal.find('[name="cmd"]').val(py_load_cmd['cmd']);
+            cmd_modal.find('[name="cmd"]').val(py_load_cmd.cmd);
             await cmd_change();
-            $.each(py_load_cmd, (key, val) => {
+            Object.entries(py_load_cmd).forEach(([key, val]) => {
+                //$.each(py_load_cmd, (key, val) => {
                 if (typeof val === 'boolean') {
                     val = val.toString();
                 }
                 // フォームに値をセット
                 if (Array.isArray(val)) {
-                    $.each(val, (i, v) => {
+                    val.forEach((v, i) => {
                         e = cmd_modal.find(`[name="${key}"]`).parent().find('.add_buton')[i];
                         $(e).click();
                     });
                     cmd_modal.find(`[name="${key}"]`).each((i, e) => {
                         if (val[i] && val[i] != "" || i == 0) $(e).val(val[i]);
                         else $(e).parent().parent().remove();
                     });
@@ -190,43 +204,43 @@
         cmd_modal.find('.row_content_hide').hide();
         cmd_modal.modal('show');
     }
     $('.cmd_card').off('click').on('click', cmd_card_func);
     // コマンドフォームからパラメータを取得
     get_param = (modal_elem) => {
         modal_elem.find('.is-invalid, .is-valid').removeClass('is-invalid').removeClass('is-valid');
-        var opt = {};
-        var title = modal_elem.find('[name="title"]').val();
+        const opt = {};
+        const title = modal_elem.find('[name="title"]').val();
         opt["mode"] = modal_elem.find('[name="mode"]').val();
         opt["cmd"] = modal_elem.find('[name="cmd"]').val();
         if (!opt["mode"]) delete opt["mode"];
         if (!opt["cmd"]) delete opt["cmd"];
         opt["title"] = title;
-        isFloat = (i) => {
+        const isFloat = (i) => {
             try {
                 n = Number(i);
                 return n % 1 !== 0;
             } catch (e) {
                 return false;
             }
         }
-        isInt = (i) => {
+        const isInt = (i) => {
             try {
                 n = Number(i);
                 return n % 1 === 0;
             } catch (e) {
                 return false;
             }
         }
         // フォームの入力値をチェック（不正な値があればフォームに'is-invalid'クラスを付加する）
         modal_elem.find('.row_content, .row_content_common').find('input, select').each((i, elem) => {
-            data_name = $(elem).attr('name');
-            data_val = $(elem).val();
-            data_type = $(elem).attr('param_data_type');
-            data_multi = $(elem).attr('param_data_multi');
+            const data_name = $(elem).attr('name');
+            let data_val = $(elem).val();
+            const data_type = $(elem).attr('param_data_type');
+            const data_multi = $(elem).attr('param_data_multi');
             if ($(elem).attr('required') && (!data_val || data_val == '')) {
                 $(elem).addClass('is-invalid');
             } else if (data_type == 'int') {
                 if (data_val && data_val != '') {
                     if (!isInt(data_val)) $(elem).addClass('is-invalid');
                     else {
                         $(elem).removeClass('is-invalid');
@@ -269,55 +283,55 @@
                 else if (data_val == false) opt[data_name] = data_val;
             }
         });
         return [title, opt];
     }
     // コマンドファイルの保存
     $('#cmd_save').off('click').on('click', async () => {
-        cmd_modal = $('#cmd_modal');
-        var [title, opt] = get_param(cmd_modal);
+        const cmd_modal = $('#cmd_modal');
+        const [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
-        result = await eel.save_cmd(title, opt)();
+        const result = await eel.save_cmd(title, opt)();
         await list_cmd_func();
         $('.cmd_card').off('click').on('click', cmd_card_func);
-        if (result['success']) alert(result['success']);
-        else if (result['warn']) alert(result['warn']);
+        if (result.success) alert(result.success);
+        else if (result.warn) alert(result.warn);
         hide_loading();
     });
     // コマンドファイルの削除
     $('#cmd_del').off('click').on('click', async () => {
-        cmd_modal = $('#cmd_modal');
-        var title = cmd_modal.find('[name="title"]').val();
+        const cmd_modal = $('#cmd_modal');
+        const title = cmd_modal.find('[name="title"]').val();
         show_loading();
         if (window.confirm(`delete "${title}"?`)) {
             await eel.del_cmd(title)();
             cmd_modal.modal('hide');
             await list_cmd_func();
             $('.cmd_card').off('click').on('click', cmd_card_func);
         }
         hide_loading();
     });
     // コマンドファイルの実行
     $('#cmd_exec').off('click').on('click', async () => {
-        cmd_modal = $('#cmd_modal');
-        var [title, opt] = get_param(cmd_modal);
+        const cmd_modal = $('#cmd_modal');
+        const [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
         // コマンドの実行
         eel.exec_cmd(title, opt)().then((result) => {});
     });
     // RAW表示の実行
     $('#cmd_raw').off('click').on('click', async () => {
-        cmd_modal = $('#cmd_modal');
-        var [title, opt] = get_param(cmd_modal);
+        const cmd_modal = $('#cmd_modal');
+        const [title, opt] = get_param(cmd_modal);
         if (cmd_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
         // コマンドの実行
         eel.raw_cmd(title, opt)().then((result) => {
             view_raw_func(title, result);
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/list_pipe.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/list_pipe.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,67 +1,67 @@
 // 保存済みパイプラインファイル一覧の取得
 list_pipe_func = async () => {
     $('#pipe_items').html('');
-    kwd = $('#pipe_kwd').val();
-    py_list_pipe = await eel.list_pipe(kwd ? `*${kwd}*` : '*')();
-    $.each(py_list_pipe, (i, row) => {
-        elem = $($('#pipe_template').html());
+    const kwd = $('#pipe_kwd').val();
+    const py_list_pipe = await eel.list_pipe(kwd ? `*${kwd}*` : '*')();
+    py_list_pipe.forEach(row => {
+        const elem = $($('#pipe_template').html());
         elem.find('.pipe_title').text(row['title']);
         elem.find('.pipe_desc').text(row['description']);
         $('#pipe_items').append(elem);
     });
     $('#pipe_items').append($($('#pipe_add').html()));
 }
 list_pipe_func_then = () => {
     // パイプラインカードクリック時の処理（モーダルダイアログを開く）
-    pipe_card_func = async (e) => {
-        pipe_modal = $('#pipe_modal');
+    const pipe_card_func = async (e) => {
+        const pipe_modal = $('#pipe_modal');
         pipe_modal.find('.is-invalid, .is-valid').removeClass('is-invalid').removeClass('is-valid');
-        row_content = pipe_modal.find('.row_content');
+        let row_content = pipe_modal.find('.row_content');
         row_content.html('');
-        modal_title = $(e.currentTarget).find('.pipe_title').text();
+        let modal_title = $(e.currentTarget).find('.pipe_title').text();
         cmd_select_template_func = (add_buton, py_list_cmd) => {
-            cmd_select_template = $(pipe_modal.find('.cmd_select_template').html());
+            const cmd_select_template = $(pipe_modal.find('.cmd_select_template').html());
             row_content = pipe_modal.find('.row_content');
             if (row_content.find('.cmd_select_item').length > 0) {
                 add_buton.parents('.cmd_select_item').after(cmd_select_template);
             } else {
                 row_content.append(cmd_select_template);
                 cmd_select_template.find('[name="pipe_cmd"]').attr('required', true);
                 cmd_select_template.find('.del_buton').hide();
             }
-            pipe_cmd_select = cmd_select_template.find('[name="pipe_cmd"]');
+            const pipe_cmd_select = cmd_select_template.find('[name="pipe_cmd"]');
             pipe_cmd_select.append('<option></option>');
-            $.each(py_list_cmd, (i, cmd) => {
-                option = $('<option></option>');
+            py_list_cmd.forEach(cmd => {
+                const option = $('<option></option>');
                 pipe_cmd_select.append(option);
                 option.attr('value', cmd['title']);
                 option.text(`${cmd['title']}(mode=${cmd['mode']}, cmd=${cmd['cmd']})`);
             });
             cmd_select_template.find('.add_buton').click((e) => {
                 cmd_select_template_func($(e.currentTarget), py_list_cmd);
             });
             cmd_select_template.find('.del_buton').click((e) => {
                 $(e.currentTarget).parents('.cmd_select_item').remove();
             });
             return cmd_select_template;
         }
         if (modal_title != '') {
             // パイプラインファイルの読み込み
-            py_list_cmd = await eel.list_cmd(null)();
-            cmd_select = cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
-            py_load_pipe = await eel.load_pipe(modal_title)();
-            $.each(py_load_pipe, (key, val) => {
+            const py_list_cmd = await eel.list_cmd(null)();
+            const cmd_select = cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
+            const py_load_pipe = await eel.load_pipe(modal_title)();
+            Object.entries(py_load_pipe).forEach(([key, val]) => {
                 if (typeof val === 'boolean') {
                     val = val.toString();
                 }
                 // フォームに値をセット
                 if (Array.isArray(val)) {
-                    $.each(val, (i, v) => {
-                        e = pipe_modal.find(`[name="${key}"]`).parent().find('.add_buton')[i];
+                    val.forEach((v, i) => {
+                        const e = pipe_modal.find(`[name="${key}"]`).parent().find('.add_buton')[i];
                         $(e).click();
                     });
                     pipe_modal.find(`[name="${key}"]`).each((i, e) => {
                         if (val[i] && val[i] != "" || i == 0) $(e).val(val[i]);
                         else $(e).parent().find('.del_buton').click();
                     });
                 } else {
@@ -73,65 +73,65 @@
         } else {
             // 新規パイプラインファイルの作成
             modal_title = 'New Pipeline';
             $('#cmd_del').hide();
             pipe_modal.find('[name="title"]').val('');
             pipe_modal.find('[name="title"]').attr('readonly', false);
             pipe_modal.find('[name="description"]').val('');
-            py_list_cmd = await eel.list_cmd(null)();
-            cmd_select = cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
+            const py_list_cmd = await eel.list_cmd(null)();
+            cmd_select_template_func(pipe_modal.find('.add_buton'), py_list_cmd)
         }
         pipe_modal.find('.modal-title').text(`Pipeline : ${modal_title}`);
         pipe_modal.modal('show');
     }
     $('.pipe_card').off('click').on('click', pipe_card_func);
     // パイプラインファイルの保存
     $('#pipe_save').off('click').on('click', async () => {
-        pipe_modal = $('#pipe_modal');
-        var [title, opt] = get_param(pipe_modal);
+        const pipe_modal = $('#pipe_modal');
+        const [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content, .row_content_common').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
-        result = await eel.save_pipe(title, opt)();
+        const result = await eel.save_pipe(title, opt)();
         await list_pipe_func();
         $('.pipe_card').off('click').on('click', pipe_card_func);
         if (result['success']) alert(result['success']);
         else if (result['warn']) alert(result['warn']);
         hide_loading();
     });
     // パイプラインファイルの削除
     $('#pipe_del').off('click').on('click', async () => {
-        pipe_modal = $('#pipe_modal');
-        var title = pipe_modal.find('[name="title"]').val();
+        const pipe_modal = $('#pipe_modal');
+        const title = pipe_modal.find('[name="title"]').val();
         show_loading();
         if (window.confirm(`delete "${title}"?`)) {
             await eel.del_pipe(title)();
             pipe_modal.modal('hide');
             await list_pipe_func();
             $('.pipe_card').off('click').on('click', pipe_card_func);
         }
         hide_loading();
     });
     // パイプラインファイルの実行
     $('#pipe_exec').off('click').on('click', async () => {
-        pipe_modal = $('#pipe_modal');
-        var [title, opt] = get_param(pipe_modal);
+        const pipe_modal = $('#pipe_modal');
+        const [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
         // コマンドの実行
         $('#loading').find('.bbforce').addClass('pipe_executed');
         eel.exec_pipe(title, opt)().then((result) => {});
     });
     // RAW表示の実行
     $('#pipe_raw').off('click').on('click', async () => {
-        pipe_modal = $('#pipe_modal');
-        var [title, opt] = get_param(pipe_modal);
+        const pipe_modal = $('#pipe_modal');
+        const [title, opt] = get_param(pipe_modal);
         if (pipe_modal.find('.row_content').find('.is-invalid').length > 0) {
             return;
         }
         show_loading();
         // コマンドの実行
         eel.raw_pipe(title, opt)().then((result) => {
             view_raw_func(title, result);
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/main.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/main.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,74 +1,74 @@
-change_dark_mode = (dark_mode) => {
-    html = $('html');
+const change_dark_mode = (dark_mode) => {
+    const html = $('html');
     if (dark_mode) html.attr('data-bs-theme', 'dark');
     else if (html.attr('data-bs-theme') == 'dark') html.removeAttr('data-bs-theme');
     else html.attr('data-bs-theme', 'dark');
 }
-show_loading = () => {
-    elem = $('#loading');
+const show_loading = () => {
+    const elem = $('#loading');
     elem.removeClass('d-none');
 }
-hide_loading = () => {
-    elem = $('#loading');
+const hide_loading = () => {
+    const elem = $('#loading');
     elem.addClass('d-none');
 }
 $(() => {
     // ダークモード対応
     change_dark_mode(window.matchMedia('(prefers-color-scheme: dark)').matches);
     // copyright情報取得
-    copyright_func = async () => {
-        copyright = await eel.copyright()();
+    const copyright_func = async () => {
+        const copyright = await eel.copyright()();
         $('.copyright').text(copyright);
     };
     copyright_func();
     // コマンド一覧の取得と表示
     list_cmd_func().then(list_cmd_func_then);
     // コマンド一覧の検索
     $('#cmd_kwd').off('change').on('change', (e) => list_cmd_func().then(list_cmd_func_then));
     // パイプライン一覧の取得と表示
     list_pipe_func().then(list_pipe_func_then);
     // パイプライン一覧の検索
     $('#pipe_kwd').off('change').on('change', (e) => list_pipe_func().then(list_pipe_func_then));
 
     $('#versions_modal').on('shown.bs.modal	', () => {
         // iinferのバージョン情報取得
-        versions_iinfer_func = async () => {
-            versions_iinfer = await eel.versions_iinfer()();
+        const versions_iinfer_func = async () => {
+            const versions_iinfer = await eel.versions_iinfer()();
             $('#versions_iinfer').html('');
-            $.each(versions_iinfer, (i, v) => {
+            versions_iinfer.forEach((v, i) => {
                 v = v.replace(/<([^>]+)>/g, '<a href="$1" target="_blank">$1</a>');
-                div = $('<div class="d-block"></div>');
+                const div = $('<div class="d-block"></div>');
                 $('#versions_iinfer').append(div);
                 if (i == 0) {
                     div.addClass('m-3');
                     div.append(`<h4>${v}</h4>`);
                 } else {
                     div.addClass('ms-5 me-5');
                     div.append(`<h6>${v}</h6>`);
                 }
             });
         };
         versions_iinfer_func();
         // usedのバージョン情報取得
-        versions_used_func = async () => {
-            versions_used = await eel.versions_used()();
+        const versions_used_func = async () => {
+            const versions_used = await eel.versions_used()();
             $('#versions_used').html('');
-            div = $('<div class="overflow-auto" style="height:calc(100vh - 260px);"></div>');
-            table = $('<table class="table table-bordered table-hover table-sm"></table>');
-            table_head = $('<thead class="table-dark bg-dark"></thead>');
-            table_body = $('<tbody></tbody>');
+            const div = $('<div class="overflow-auto" style="height:calc(100vh - 260px);"></div>');
+            const table = $('<table class="table table-bordered table-hover table-sm"></table>');
+            const table_head = $('<thead class="table-dark bg-dark"></thead>');
+            const table_body = $('<tbody></tbody>');
             table.append(table_head);
             table.append(table_body);
             div.append(table);
             $('#versions_used').append(div);
-            $.each(versions_used, (i, row) => {
-                tr = $('<tr></tr>');
-                $.each(row, (j, cel) => {
-                    td = $('<td></td>').text(cel);
+            versions_used.forEach((row, i) => {
+                const tr = $('<tr></tr>');
+                row.forEach((cel, j) => {
+                    const td = $('<td></td>').text(cel);
                     tr.append(td);
                 });
                 if (i == 0) table_head.append(tr);
                 else table_body.append(tr);
             });
         };
         versions_used_func();
@@ -118,37 +118,37 @@
     /*$(window).on('beforeunload', () => {
         event.preventDefault();
         event.returnValue = 'Check';
     });*/
     eel.expose(js_console_modal_log_func);
 
     function js_console_modal_log_func(line) {
-        elem = $('#console_modal_log');
-        text = elem.val() + line;
+        const elem = $('#console_modal_log');
+        const text = elem.val() + line;
         elem.val(text);
         elem.get(0).setSelectionRange(text.length - 1, text.length - 1);
     };
     eel.expose(js_return_cmd_exec_func);
 
     function js_return_cmd_exec_func(title, result) {
-        cmd_modal = $('#cmd_modal');
+        const cmd_modal = $('#cmd_modal');
         cmd_modal.modal('hide');
         view_result_func(title, result);
         hide_loading();
     }
     eel.expose(js_return_pipe_exec_func);
 
     function js_return_pipe_exec_func(title, result) {
-        pipe_modal = $('#pipe_modal');
+        const pipe_modal = $('#pipe_modal');
         pipe_modal.modal('hide');
         view_result_func(title, result);
         hide_loading();
     }
     eel.expose(js_return_stream_log_func);
 
     function js_return_stream_log_func(result) {
-        size_th = 1024 * 1024 * 5;
+        const size_th = 1024 * 1024 * 5;
         view_result_func('stream log', result);
-        result_modal = $('#result_modal');
+        const result_modal = $('#result_modal');
         result_modal.find('.btn_window').click();
     };
 });
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/svfiler.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -116,16 +116,15 @@
                 alert(res['warn']);
                 hide_loading();
                 return;
             }
             list_tree = res[0]['success'];
             hide_loading();
             // 左側ペイン
-            Object.keys(list_tree).map((key) => {
-                node = list_tree[key];
+            Object.entries(list_tree).forEach(([key, node]) => {
                 if (!node['is_dir']) return;
                 children = node['children'];
                 current_li_elem = modal.find(`#${key}`);
                 if (current_li_elem.length > 0) {
                     current_li_elem.find('.folder-close').remove();
                 } else {
                     current_li_elem = $(`<li id="${key}" data_path="${node['path']}"/>`);
@@ -146,38 +145,37 @@
                     ul_elem = $('<ul class="tree_ul"/>').append(`<li id="${k}" data_path="${n['path']}"><a href="#" class="folder-close">${n['name']}</a></li>`);
                     current_li_elem.append(ul_elem);
                     modal.find(`#${k}`).off('click');
                     modal.find(`#${k}`).on('click', mk_func(n['path'], current_ul_elem));
                 });
             });
             // 右側ペイン
-            list_tree_keys = Object.keys(list_tree);
-            if (list_tree_keys.length > 0) {
-                node = list_tree[list_tree_keys[list_tree_keys.length - 1]];
+            Object.entries(list_tree).forEach(([key, node]) => {
+                if (!node['path']) return;
                 modal.find('.filer_address').val(node['path']);
-                table = $('<table class="table table-bordered table-hover table-sm">' +
+                const table = $('<table class="table table-bordered table-hover table-sm">' +
                     '<thead class="table-dark bg-dark"><tr><th scope="col">-</th><th scope="col">name</th><th scope="col">size</th><th scope="col">last</th></tr></thead>' +
                     '</table>');
-                table_body = $('<tbody></tbody>');
+                const table_body = $('<tbody></tbody>');
                 modal.find('.file-list').html('');
                 modal.find('.file-list').append(table);
                 table.append(table_body);
-                children = node['children'];
+                const children = node['children'];
                 if (children) {
                     // ツリー表示関数の生成
-                    mk_tree = (_p, _e) => {
+                    const mk_tree = (_p, _e) => {
                         return () => tree(_p, _e)
                     }
                     // 削除関数の生成
-                    mk_delete = (_p, _e, is_dir) => {
+                    const mk_delete = (_p, _e, is_dir) => {
                         return () => {
-                            if (confirm(`「${_p}」を削除しますか？${is_dir?"\n【注意】ディレクトリの場合は中身も削除されます。":""}`)) {
-                                remote = is_dir ? 'file_rmdir' : 'file_remove';
+                            if (confirm(`Do you want to delete "${_p}"？${is_dir?"\nNote: In the case of directories, the contents will also be deleted.":""}`)) {
+                                const remote = is_dir ? 'file_rmdir' : 'file_remove';
                                 show_loading();
-                                opt = get_server_opt();
+                                const opt = get_server_opt();
                                 opt['mode'] = 'client';
                                 opt['cmd'] = remote;
                                 opt['capture_stdout'] = true;
                                 opt['svpath'] = _p;
                                 eel.exec_cmd(remote, opt, true)().then(async res => {
                                     if (res['warn']) {
                                         alert(res['warn']);
@@ -192,39 +190,39 @@
                                     console.log(error);
                                     hide_loading();
                                 });
                             }
                         }
                     };
                     mk_blob = (base64) => {
-                        bin = atob(base64.replace(/^.*,/, ''));
-                        buffer = new Uint8Array(bin.length);
+                        const bin = atob(base64.replace(/^.*,/, ''));
+                        const buffer = new Uint8Array(bin.length);
                         for (i = 0; i < bin.length; i++) buffer[i] = bin.charCodeAt(i);
-                        blob = new Blob([buffer.buffer], {
+                        const blob = new Blob([buffer.buffer], {
                             type: 'application/octet-stream'
                         });
                         return blob;
                     }
                     // ダウンロード関数の生成
                     mk_download = (_p) => {
                         return () => {
                             show_loading();
-                            opt = get_server_opt();
+                            const opt = get_server_opt();
                             opt['mode'] = 'client';
                             opt['cmd'] = 'file_download';
                             opt['capture_stdout'] = true;
                             opt['svpath'] = _p;
                             eel.exec_cmd('file_download', opt, true)().then(async res => {
                                 if (res['warn']) {
                                     alert(res['warn']);
                                     hide_loading();
                                     return;
                                 }
-                                blob = mk_blob(res[0]['success']['data']);
-                                link = modal.find('.filer_download');
+                                const blob = mk_blob(res[0]['success']['data']);
+                                const link = modal.find('.filer_download');
                                 link.attr('download', res[0]['success']['name']);
                                 link.get(0).href = window.URL.createObjectURL(blob);
                                 link.get(0).click();
                                 URL.revokeObjectURL(link.get(0).href);
                             }).then(() => {
                                 hide_loading();
                             }, (error) => {
@@ -233,22 +231,22 @@
                             });
                         }
                     };
                     // フォルダ作成関数の生成
                     mk_mkdir = (_p, _e, is_dir) => {
                         return () => {
                             _p = _p.substring(0, _p.lastIndexOf('/') + 1);
-                            prompt_text = prompt('Enter a new folder name.');
+                            const prompt_text = prompt('Enter a new folder name.');
                             if (prompt_text) {
                                 show_loading();
-                                opt = get_server_opt();
+                                const opt = get_server_opt();
                                 opt['mode'] = 'client';
                                 opt['cmd'] = 'file_mkdir';
                                 opt['capture_stdout'] = true;
-                                opt['svpath'] = `${_p}/${prompt_text}`;
+                                opt['svpath'] = `${_p=="/"?"":_p}/${prompt_text}`;
                                 eel.exec_cmd('file_mkdir', opt, true)().then(async res => {
                                     if (res['warn']) {
                                         alert(res['warn']);
                                         hide_loading();
                                         return;
                                     }
                                     hide_loading();
@@ -259,79 +257,77 @@
                                     console.log(error);
                                     hide_loading();
                                 });
                             }
                         }
                     };
                     // ファイルリストの生成
-                    mk_tr = (_p, _e, is_dir) => {
-                        png = is_dir ? 'folder-close.png' : 'file.png';
-                        dt = is_dir ? '-' : new Date(n['last']).toLocaleDateString('ja-JP', {
+                    const mk_tr = (_p, _e, _n) => {
+                        const png = _n["is_dir"] ? 'folder-close.png' : 'file.png';
+                        const dt = _n["is_dir"] ? '-' : new Date(_n["last"]).toLocaleDateString('ja-JP', {
                             year: 'numeric',
                             month: '2-digit',
                             day: '2-digit',
                             hour: '2-digit',
                             minute: '2-digit',
                             second: '2-digit'
                         });
-                        tr = $('<tr>' +
+                        const tr = $('<tr>' +
                             `<td><img src="/assets/tree-menu/image/${png}"></td>` +
                             '<td>' +
                             '<div class="droudown">' +
-                            `<a class="dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">${n['name']}</a>` +
+                            `<a class="dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">${_n['name']}</a>` +
                             '<ul class="dropdown-menu"/>' +
                             '</div>' +
                             '</td>' +
-                            `<td class="text-end">${calc_size(n['size'])}</td>` +
+                            `<td class="text-end">${calc_size(_n['size'])}</td>` +
                             `<td class="text-end">${dt}</td>` +
                             '</tr>');
-                        if (is_dir) {
+                        if (_n["is_dir"]) {
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item open" href="#">Open</a></li>');
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>');
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item delete" href="#">Delete</a></li>');
                         } else {
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item download" href="#">Download</a></li>');
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item mkdir" href="#">Create Folder</a></li>');
                             tr.find('.dropdown-menu').append('<li><a class="dropdown-item delete" href="#">Delete</a></li>');
                         }
                         tr.find('.open').off('click').on('click', mk_tree(_p, _e));
-                        tr.find('.delete').off('click').on('click', mk_delete(_p, _e, is_dir));
-                        tr.find('.mkdir').off('click').on('click', mk_mkdir(_p, _e, is_dir));
+                        tr.find('.delete').off('click').on('click', mk_delete(_p, _e, _n["is_dir"]));
+                        tr.find('.mkdir').off('click').on('click', mk_mkdir(_p, _e, _n["is_dir"]));
                         tr.find('.download').off('click').on('click', mk_download(_p));
                         return tr;
                     };
                     // ディレクトリを先に表示
-                    Object.keys(children).map((k, i) => {
-                        n = children[k];
+                    Object.entries(children).forEach(([k, n]) => {
                         if (!n['is_dir'] || node['path'] == n['path']) return;
-                        tr = mk_tr(n['path'], current_ul_elem, n['is_dir']);
+                        const tr = mk_tr(n['path'], current_ul_elem, n);
                         table_body.append(tr);
                     });
                     // ファイルを表示
-                    Object.keys(children).map((k, i) => {
-                        n = children[k];
+                    Object.entries(children).forEach(([k, n]) => {
                         if (n['is_dir']) return;
-                        tr = mk_tr(n['path'], current_ul_elem, n['is_dir']);
+                        const tr = mk_tr(n['path'], current_ul_elem, n);
                         table_body.append(tr);
                     });
                 }
-            }
+            });
         }).then(() => {
             hide_loading();
         }, (error) => {
             console.log(error);
             hide_loading();
         });
     }
     // サーバー一覧を取得 ========================================================
     const get_server_opt = () => {
-        filer_host = modal.find('.filer_host').val();
-        filer_port = modal.find('.filer_port').val();
-        filer_password = modal.find('.filer_password').val();
-        filer_svname = modal.find('.filer_svname').val();
+        let filer_host = modal.find('.filer_host').val();
+        let filer_port = modal.find('.filer_port').val();
+        let filer_password = modal.find('.filer_password').val();
+        let filer_svname = modal.find('.filer_svname').val();
         if (!filer_host) {
             filer_host = localStorage.getItem('filer_host');
             filer_host = filer_host ? filer_host : 'localhost';
             modal.find('.filer_host').val(filer_host);
         }
         if (!filer_port) {
             filer_port = localStorage.getItem('filer_port');
@@ -354,15 +350,15 @@
             "password": filer_password,
             "svname": filer_svname
         };
     }
     const load_server_list = () => {
         show_loading();
         modal.find('.filer_svnames').remove();
-        opt = get_server_opt();
+        const opt = get_server_opt();
         opt['mode'] = 'server';
         opt['cmd'] = 'list';
         opt["capture_stdout"] = true;
         delete opt['svname'];
         eel.exec_cmd("server_list", opt, true)().then(async res => {
             if (res["warn"]) {
                 alert(res["warn"]);
@@ -370,60 +366,60 @@
                 return;
             }
             if (res.length <= 0 || !res[0]['success']) {
                 hide_loading();
                 return;
             }
             res[0]['success'].forEach(elem => {
-                a_elem = $(`<a class="dropdown-item" href="#" data-host="${opt['host']}" data-port="${opt['port']}" data-password="${opt['password']}" data-svname="${elem['svname']}">${elem['svname']} ( ${opt['host']}:${opt['port']} )</a>`);
-                mk_func = (elem) => {
+                const a_elem = $(`<a class="dropdown-item" href="#" data-host="${opt['host']}" data-port="${opt['port']}" data-password="${opt['password']}" data-svname="${elem['svname']}">${elem['svname']} ( ${opt['host']}:${opt['port']} )</a>`);
+                const mk_func = (elem) => {
                     return () => {
                         modal.find('.filer_host').val(elem.attr('data-host'));
                         modal.find('.filer_port').val(elem.attr('data-port'));
                         modal.find('.filer_password').val(elem.attr('data-password'));
                         modal.find('.filer_svname').val(elem.attr('data-svname'));
                         localStorage.setItem('filer_host', elem.attr('data-host'));
                         localStorage.setItem('filer_port', elem.attr('data-port'));
                         localStorage.setItem('filer_password', elem.attr('data-password'));
                         localStorage.setItem('filer_svname', elem.attr('data-svname'));
                         tree("/", modal.find('.tree-menu'))
                     }
                 };
                 a_elem.off("click").on("click", mk_func(a_elem));
-                li_elem = $('<li class="filer_svnames"></li>').append(a_elem);
+                const li_elem = $('<li class="filer_svnames"></li>').append(a_elem);
                 modal.find('.filer_server').append(li_elem);
             });
             modal.find('.filer_server').find('.dropdown-item:first').click();
         }).then(() => {
             hide_loading();
         }, (error) => {
             console.log(error);
             hide_loading();
         });
     }
     // ファイルアップロード ========================================================
     const upload = async (event) => {
         show_loading();
         const progress = (_min, _max, _now, _text, _show, _cycle) => {
-            prog_elem = modal.find('.progress');
-            bar_elem = prog_elem.find('.progress-bar');
+            const prog_elem = modal.find('.progress');
+            const bar_elem = prog_elem.find('.progress-bar');
             if (_show) prog_elem.removeClass('d-none');
             else prog_elem.addClass('d-none');
             prog_elem.attr('aria-valuemin', _min);
             prog_elem.attr('aria-valuemax', _max);
             prog_elem.attr('aria-valuenow', _now);
             if (!_cycle) {
-                par = Math.floor((_now / (_max - _min)) * 10000) / 100
+                const par = Math.floor((_now / (_max - _min)) * 10000) / 100
                 bar_elem.css('left', 'auto').css('width', `${par}%`);
                 bar_elem.text(`${par}% ( ${_now} / ${_max} ) ${_text}`);
                 clearTimeout(progress_handle);
             } else {
-                maxwidth = prog_elem.css('width');
+                let maxwidth = prog_elem.css('width');
                 maxwidth = parseInt(maxwidth.replace('px', ''));
-                left = bar_elem.css('left');
+                let left = bar_elem.css('left');
                 if (!left || left == 'auto') left = 0;
                 else left = parseInt(left.replace('px', ''));
                 if (left > maxwidth) left = -200;
                 left += 2;
                 bar_elem.css('width', '200px').css('position', 'relative').css('left', `${left}px`);
                 bar_elem.text('Server processing...');
                 var progress_handle = setTimeout(() => {
@@ -500,15 +496,15 @@
             url: `/filer/upload?host=${encodeURI(opt['host'])}&port=${encodeURI(opt['port'])}&password=${encodeURI(opt['password'])}&svname=${encodeURI(opt['svname'])}&svpath=${encodeURI(svpath)}`,
             type: 'POST',
             processData: false,
             contentType: false,
             async: true,
             data: formData,
             xhr: function() {
-                var xhr = $.ajaxSettings.xhr();
+                const xhr = $.ajaxSettings.xhr();
                 xhr.upload.onprogress = function(e) {
                     if (e.lengthComputable) {
                         progress(0, e.total, e.loaded, '', true, e.total == e.loaded);
                     }
                 };
                 return xhr;
             },
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/view_raw.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/view_raw.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 // RAW結果をモーダルダイアログに表示
-view_raw_func = (title, result) => {
-    result_modal = $('#result_modal');
+const view_raw_func = (title, result) => {
+    const result_modal = $('#result_modal');
     result_modal.find('.modal-title').text(title);
     result_modal.find('.modal-body').html('');
-    table = $('<table class="table table-bordered table-hover table-sm"></table>');
-    table_head = $('<thead class="table-dark bg-dark"></thead>');
-    table_body = $('<tbody></tbody>');
+    const table = $('<table class="table table-bordered table-hover table-sm"></table>');
+    const table_head = $('<thead class="table-dark bg-dark"></thead>');
+    const table_body = $('<tbody></tbody>');
     table.append(table_head);
     table.append(table_body);
     result_modal.find('.modal-body').append(table);
     // list型の結果をテーブルに変換
     list2table = (data, table_head, table_body) => {
-        $.each(data, (i, row) => {
-            tr = $('<tr></tr>');
+        data.forEach((row, i) => {
+            const tr = $('<tr></tr>');
             if (typeof row === 'string') {
                 tr.append($(`<td>${row}</td>`));
             } else {
-                $.each(row, (key, val) => {
+                Object.entries(row).forEach(([key, val]) => {
                     if (i == 0) {
                         table_head.append($(`<th scope="col">${key}</th>`));
                     }
                     tr.append($(`<td>${val}</td>`));
                 });
             }
             table_body.append(tr);
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/iinfer/view_result.js` & `iinfer-0.7.3/iinfer/web/assets/iinfer/view_result.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,121 +1,121 @@
-cell_chop = (val) => {
+const cell_chop = (val) => {
     if (val && val.length > 150) {
         return `${val.substring(0, 150)}...`;
     }
     return val;
 }
 // 実行結果をモーダルダイアログに表示
-view_result_func = (title, result) => {
+const view_result_func = (title, result) => {
     if (!result | Array.isArray(result) && result.length <= 0) return;
-    let result_modal = $('#result_modal');
+    const result_modal = $('#result_modal');
     result_modal.find('.modal-title').text(title);
     result_modal.find('.modal-body').html('');
-    mk_table_func = () => {
-        let table = $('<table class="table table-bordered table-hover table-sm"></table>');
-        let table_head = $('<thead class="table-dark bg-dark"></thead>');
-        let table_body = $('<tbody></tbody>');
+    const mk_table_func = () => {
+        const table = $('<table class="table table-bordered table-hover table-sm"></table>');
+        const table_head = $('<thead class="table-dark bg-dark"></thead>');
+        const table_body = $('<tbody></tbody>');
         table.append(table_head);
         table.append(table_body);
         return table;
     }
-    let table = mk_table_func();
+    const table = mk_table_func();
     result_modal.find('.modal-body').append(table);
     // list型の結果をテーブルに変換
-    list2table = (data, table_head, table_body) => {
+    const list2table = (data, table_head, table_body) => {
         Object.keys(data).forEach(i => {
-            let row = data[i];
+            const row = data[i];
             if (row['success'] && typeof row['success'] == "object" && !Array.isArray(row['success'])) {
                 dict2table(row['success'], i == 0 ? table_head : null, table_body, row['output_image']);
                 return;
             }
             if (typeof row == 'string' || row instanceof String) {
-                let tr = $('<tr></tr>');
+                const tr = $('<tr></tr>');
                 table_body.append(tr);
                 tr.append($(`<td>${row}</td>`));
                 return;
             }
             if (Array.isArray(row) && row.length > 0 && typeof row[0] != "object") {
-                let tr = $('<tr></tr>');
+                const tr = $('<tr></tr>');
                 table_body.append(tr);
                 val = cell_chop(JSON.stringify(row));
                 tr.append($(`<td>${row}</td>`));
                 return;
             }
-            let tr = $('<tr></tr>');
+            const tr = $('<tr></tr>');
             table_body.append(tr);
             Object.keys(row).forEach(key => {
-                let val = row[key];
+                const val = row[key];
                 if (i == 0) {
                     table_head.append($(`<th scope="col" style="word-break:normal">${key}</th>`));
                 }
                 if (val && val['success'] && Array.isArray(val['success'])) {
-                    let tbl = mk_table_func()
-                    let td = $('<td></td>');
+                    const tbl = mk_table_func()
+                    const td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     list2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
                 } else if (val && val['success'] && typeof val['success'] == "object") {
-                    let tbl = mk_table_func()
-                    let td = $('<td></td>');
+                    const tbl = mk_table_func()
+                    const td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     dict2table(val['success'], tbl.find('thead'), tbl.find('tbody'));
                 } else if (val && Array.isArray(val) && val.length > 0 && typeof val[0] == "object") {
-                    let tbl = mk_table_func()
-                    let td = $('<td></td>');
+                    const tbl = mk_table_func()
+                    const td = $('<td></td>');
                     td.append(tbl);
                     tr.append(td);
                     list2table(val, tbl.find('thead'), tbl.find('tbody'));
                 } else {
                     tr.append($(`<td>${val}</td>`));
                 }
             });
         });
     }
     // dict型の結果をテーブルに変換
-    dict2table = (data, table_head, table_body, output_image) => {
-        let tr = $('<tr></tr>');
+    const dict2table = (data, table_head, table_body, output_image) => {
+        const tr = $('<tr></tr>');
         if (output_image) {
             if (table_head) table_head.append($('<th scope="col" style="word-break:normal">output_image</th>'));
-            let img = $('<img class="img-thumbnail">').attr('src', `data:image/png;base64,${output_image}`);
+            const img = $('<img class="img-thumbnail">').attr('src', `data:image/png;base64,${output_image}`);
             img.css('width', '100px').css('height', 'auto');
-            let anchor = $(`<a href="data:image/jpeg;base64,${output_image}" data-lightbox="output_image"></a>`).append(img);
+            const anchor = $(`<a href="data:image/jpeg;base64,${output_image}" data-lightbox="output_image"></a>`).append(img);
             tr.append($('<td></td>').append(anchor));
         }
         table_body.append(tr);
         Object.keys(data).forEach(key => {
             let val = data[key];
             if (table_head) table_head.append($(`<th scope="col" style="word-break:normal">${key}</th>`));
             if (key != 'warn' && val) {
                 if (Array.isArray(val)) {
                     if (val.length > 0 && typeof val[0] == "object") {
-                        let tbl = mk_table_func()
-                        let td = $('<td></td>');
+                        const tbl = mk_table_func()
+                        const td = $('<td></td>');
                         td.append(tbl);
                         list2table(val, tbl.find('thead'), tbl.find('tbody'));
                         val = td.html();
                     } else {
                         val = cell_chop(JSON.stringify(val));
                     }
                 } else if (typeof val == "object") {
-                    let tbl = mk_table_func()
-                    let td = $('<td></td>');
+                    const tbl = mk_table_func()
+                    const td = $('<td></td>');
                     td.append(tbl);
                     dict2table(val, tbl.find('thead'), tbl.find('tbody'));
                     val = td.html();
                 } else if ((typeof val === 'string' || val instanceof String) && val.length > 150) {
                     val = cell_chop(val);
                 }
             }
             tr.append($(`<td style="overflow-wrap:break-word;word-break:break-all;">${val}</td>`));
         });
     }
-    let table_head = table.find('thead')
-    let table_body = table.find('tbody')
+    const table_head = table.find('thead')
+    const table_body = table.find('tbody')
     // 結果をテーブルに変換
     if (result['success'] && Array.isArray(result['success'])) {
         list2table(result['success'], table_head, table_body);
     } else if (result['success'] && typeof result['success'] == "object") {
         dict2table(result['success'], table_head, table_body, result['output_image']);
     } else if (Array.isArray(result)) {
         list2table(result, table_head, table_body);
```

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.7.3/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.7.3/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.7.3/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.7.3/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.7.3/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.7.3/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.7.3/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.7.3/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/iinfer/web/gui.html` & `iinfer-0.7.3/iinfer/web/gui.html`

 * *Files 0% similar despite different names*

```diff
@@ -155,25 +155,25 @@
                                     title
                                 </label>
                                 <input name="title" type="text" class="form-control" param_data_type="str" param_data_multi="false" required>
                             </div>
                         </div>
                         <div class="col-6 mb-3">
                             <div class="input-group">
-                                <label class="input-group-text text-decoration-underline">
+                                <label class="mode_label input-group-text text-decoration-underline">
                                     <span class="text-danger">*</span>
                                     mode
                                 </label>
                                 <select name="mode" class="form-select form-select" param_data_type="str" param_data_multi="false" required>
                                 </select>
                             </div>
                         </div>
                         <div class="col-6 mb-3">
                             <div class="input-group">
-                                <span class="input-group-text text-decoration-underline">
+                                <span class="cmd_label input-group-text text-decoration-underline">
                                     <span class="text-danger">*</span>
                                     cmd
                                 </span>
                                 <select name="cmd" class="form-select form-select" param_data_type="str" param_data_multi="false" required>
                                 </select>
                             </div>
                         </div>
```

### Comparing `iinfer-0.7.2/iinfer.egg-info/PKG-INFO` & `iinfer-0.7.3/iinfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.2
+Version: 0.7.3
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.2/iinfer.egg-info/SOURCES.txt` & `iinfer-0.7.3/iinfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.2/setup.py` & `iinfer-0.7.3/setup.py`

 * *Files identical despite different names*

