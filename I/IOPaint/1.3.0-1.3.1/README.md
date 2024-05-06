# Comparing `tmp/IOPaint-1.3.0.tar.gz` & `tmp/IOPaint-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IOPaint-1.3.0.tar", last modified: Mon May  6 14:30:21 2024, max compression
+gzip compressed data, was "IOPaint-1.3.1.tar", last modified: Mon May  6 14:49:15 2024, max compression
```

## Comparing `IOPaint-1.3.0.tar` & `IOPaint-1.3.1.tar`

### file list

```diff
@@ -1,200 +1,207 @@
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.491247 IOPaint-1.3.0/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.455853 IOPaint-1.3.0/IOPaint.egg-info/
--rw-r--r--   0 cwq        (501) staff       (20)     7428 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     6803 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/SOURCES.txt
--rw-r--r--   0 cwq        (501) staff       (20)        1 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/dependency_links.txt
--rw-r--r--   0 cwq        (501) staff       (20)       48 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/entry_points.txt
--rw-r--r--   0 cwq        (501) staff       (20)      309 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/requires.txt
--rw-r--r--   0 cwq        (501) staff       (20)        8 2024-05-06 14:30:21.000000 IOPaint-1.3.0/IOPaint.egg-info/top_level.txt
--rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-11-15 00:50:32.000000 IOPaint-1.3.0/LICENSE
--rw-r--r--   0 cwq        (501) staff       (20)     7428 2024-05-06 14:30:21.491103 IOPaint-1.3.0/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     6696 2024-04-08 12:09:07.000000 IOPaint-1.3.0/README.md
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.459701 IOPaint-1.3.0/iopaint/
--rw-r--r--   0 cwq        (501) staff       (20)      832 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)       78 2024-02-03 13:30:22.000000 IOPaint-1.3.0/iopaint/__main__.py
--rw-r--r--   0 cwq        (501) staff       (20)    15183 2024-02-16 02:14:38.000000 IOPaint-1.3.0/iopaint/api.py
--rw-r--r--   0 cwq        (501) staff       (20)     4099 2024-05-06 14:07:17.000000 IOPaint-1.3.0/iopaint/batch_processing.py
--rw-r--r--   0 cwq        (501) staff       (20)     3224 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/benchmark.py
--rw-r--r--   0 cwq        (501) staff       (20)     7799 2024-02-09 07:17:49.000000 IOPaint-1.3.0/iopaint/cli.py
--rw-r--r--   0 cwq        (501) staff       (20)     4103 2024-04-12 05:24:09.000000 IOPaint-1.3.0/iopaint/const.py
--rw-r--r--   0 cwq        (501) staff       (20)    10785 2024-04-12 10:51:58.000000 IOPaint-1.3.0/iopaint/download.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.460741 IOPaint-1.3.0/iopaint/file_manager/
--rw-r--r--   0 cwq        (501) staff       (20)       38 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/file_manager/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     7143 2024-02-09 07:17:49.000000 IOPaint-1.3.0/iopaint/file_manager/file_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     1293 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/file_manager/storage_backends.py
--rw-r--r--   0 cwq        (501) staff       (20)     1835 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/file_manager/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)    12017 2024-02-18 01:21:15.000000 IOPaint-1.3.0/iopaint/helper.py
--rw-r--r--   0 cwq        (501) staff       (20)      232 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/installer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.465829 IOPaint-1.3.0/iopaint/model/
--rw-r--r--   0 cwq        (501) staff       (20)     1028 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/__init__.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.467008 IOPaint-1.3.0/iopaint/model/anytext/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2536 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/anytext_model.py
--rw-r--r--   0 cwq        (501) staff       (20)    15191 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/anytext_pipeline.py
--rw-r--r--   0 cwq        (501) staff       (20)     2777 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/anytext_sd15.yaml
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.468506 IOPaint-1.3.0/iopaint/model/anytext/cldm/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    28531 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/cldm.py
--rw-r--r--   0 cwq        (501) staff       (20)    17275 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/ddim_hacked.py
--rw-r--r--   0 cwq        (501) staff       (20)     6083 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/embedding_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     3699 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/hack.py
--rw-r--r--   0 cwq        (501) staff       (20)     1373 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/model.py
--rwxr-xr-x   0 cwq        (501) staff       (20)    11447 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/cldm/recognizer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.468779 IOPaint-1.3.0/iopaint/model/anytext/ldm/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/__init__.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.469039 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     8614 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/autoencoder.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.469913 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    18214 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/ddim.py
--rw-r--r--   0 cwq        (501) staff       (20)    89020 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.470444 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 cwq        (501) staff       (20)       37 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    65969 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 cwq        (501) staff       (20)     2990 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)    12971 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/plms.py
--rw-r--r--   0 cwq        (501) staff       (20)      753 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.470883 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    10738 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/attention.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.471697 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    30615 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 cwq        (501) staff       (20)    30462 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 cwq        (501) staff       (20)     3468 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 cwq        (501) staff       (20)     9995 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.471993 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/distributions/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/distributions/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2970 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/distributions/distributions.py
--rw-r--r--   0 cwq        (501) staff       (20)     3110 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/ema.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.472265 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/encoders/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/encoders/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    14135 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/encoders/modules.py
--rw-r--r--   0 cwq        (501) staff       (20)     7250 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ldm/util.py
--rw-r--r--   0 cwq        (501) staff       (20)     1554 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/main.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.473549 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/
--rwxr-xr-x   0 cwq        (501) staff       (20)     6607 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RNN.py
--rwxr-xr-x   0 cwq        (501) staff       (20)     1260 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecCTCHead.py
--rwxr-xr-x   0 cwq        (501) staff       (20)     1673 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecModel.py
--rw-r--r--   0 cwq        (501) staff       (20)     6709 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecMv1_enhance.py
--rw-r--r--   0 cwq        (501) staff       (20)    19468 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecSVTR.py
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2180 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/common.py
--rw-r--r--   0 cwq        (501) staff       (20)    26249 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/ppocr_keys_v1.txt
--rw-r--r--   0 cwq        (501) staff       (20)     4989 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/anytext/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)    13463 2024-04-24 12:15:10.000000 IOPaint-1.3.0/iopaint/model/base.py
--rw-r--r--   0 cwq        (501) staff       (20)     7077 2024-04-12 05:21:36.000000 IOPaint-1.3.0/iopaint/model/controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     6863 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/ddim_sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)    57219 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/fcf.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.474349 IOPaint-1.3.0/iopaint/model/helper/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/helper/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2117 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/helper/controlnet_preprocess.py
--rw-r--r--   0 cwq        (501) staff       (20)     1409 2024-02-10 04:35:12.000000 IOPaint-1.3.0/iopaint/model/helper/cpu_text_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     1913 2024-04-24 12:02:35.000000 IOPaint-1.3.0/iopaint/model/helper/g_diffuser_bot.py
--rw-r--r--   0 cwq        (501) staff       (20)     2436 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)     2041 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/kandinsky.py
--rw-r--r--   0 cwq        (501) staff       (20)     1608 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/lama.py
--rw-r--r--   0 cwq        (501) staff       (20)    11481 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/ldm.py
--rw-r--r--   0 cwq        (501) staff       (20)     3097 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/manga.py
--rw-r--r--   0 cwq        (501) staff       (20)    62704 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/mat.py
--rw-r--r--   0 cwq        (501) staff       (20)     3438 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/mi_gan.py
--rw-r--r--   0 cwq        (501) staff       (20)      735 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/opencv2.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.475434 IOPaint-1.3.0/iopaint/model/original_sd_configs/
--rw-r--r--   0 cwq        (501) staff       (20)      590 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/original_sd_configs/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2784 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/original_sd_configs/sd_xl_base.yaml
--rw-r--r--   0 cwq        (501) staff       (20)     2589 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/original_sd_configs/sd_xl_refiner.yaml
--rw-r--r--   0 cwq        (501) staff       (20)     1873 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/original_sd_configs/v1-inference.yaml
--rw-r--r--   0 cwq        (501) staff       (20)     1815 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/original_sd_configs/v2-inference-v.yaml
--rw-r--r--   0 cwq        (501) staff       (20)     2792 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/paint_by_example.py
--rw-r--r--   0 cwq        (501) staff       (20)    11833 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/plms_sampler.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.476401 IOPaint-1.3.0/iopaint/model/power_paint/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/power_paint/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    56636 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/power_paint/pipeline_powerpaint.py
--rw-r--r--   0 cwq        (501) staff       (20)     3658 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/power_paint/power_paint.py
--rw-r--r--   0 cwq        (501) staff       (20)     6964 2024-04-29 14:15:25.000000 IOPaint-1.3.0/iopaint/model/power_paint/power_paint_v2.py
--rw-r--r--   0 cwq        (501) staff       (20)     9439 2024-04-18 13:28:38.000000 IOPaint-1.3.0/iopaint/model/power_paint/powerpaint_tokenizer.py
--rw-r--r--   0 cwq        (501) staff       (20)     4425 2024-04-12 05:21:36.000000 IOPaint-1.3.0/iopaint/model/sd.py
--rw-r--r--   0 cwq        (501) staff       (20)     3993 2024-04-12 05:21:36.000000 IOPaint-1.3.0/iopaint/model/sdxl.py
--rw-r--r--   0 cwq        (501) staff       (20)    37847 2024-02-05 13:45:11.000000 IOPaint-1.3.0/iopaint/model/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)    16327 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/model/zits.py
--rw-r--r--   0 cwq        (501) staff       (20)     9788 2024-04-25 14:18:35.000000 IOPaint-1.3.0/iopaint/model_manager.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.478904 IOPaint-1.3.0/iopaint/plugins/
--rw-r--r--   0 cwq        (501) staff       (20)     2423 2024-02-08 14:13:37.000000 IOPaint-1.3.0/iopaint/plugins/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    13787 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/anime_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)      730 2024-02-08 14:13:37.000000 IOPaint-1.3.0/iopaint/plugins/base_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)    14976 2024-04-08 12:07:58.000000 IOPaint-1.3.0/iopaint/plugins/briarmbg.py
--rw-r--r--   0 cwq        (501) staff       (20)     2507 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/gfpgan_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)     2750 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/gfpganer.py
--rw-r--r--   0 cwq        (501) staff       (20)     3717 2024-02-18 01:48:00.000000 IOPaint-1.3.0/iopaint/plugins/interactive_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)     3989 2024-03-03 11:07:10.000000 IOPaint-1.3.0/iopaint/plugins/realesrgan.py
--rw-r--r--   0 cwq        (501) staff       (20)     2211 2024-04-08 12:08:35.000000 IOPaint-1.3.0/iopaint/plugins/remove_bg.py
--rw-r--r--   0 cwq        (501) staff       (20)     1854 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/restoreformer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.480012 IOPaint-1.3.0/iopaint/plugins/segment_anything/
--rw-r--r--   0 cwq        (501) staff       (20)      420 2024-02-18 01:14:34.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     7864 2024-02-18 01:29:24.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/build_sam.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.482715 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/
--rw-r--r--   0 cwq        (501) staff       (20)      385 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     1479 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/common.py
--rw-r--r--   0 cwq        (501) staff       (20)    14407 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)    14795 2024-02-18 01:29:24.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/image_encoder_hq.py
--rw-r--r--   0 cwq        (501) staff       (20)    15490 2024-02-18 00:55:27.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     8594 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     7225 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/sam.py
--rw-r--r--   0 cwq        (501) staff       (20)     7474 2024-02-18 01:20:30.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/sam_hq.py
--rw-r--r--   0 cwq        (501) staff       (20)    26182 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/tiny_vit_sam.py
--rw-r--r--   0 cwq        (501) staff       (20)     8396 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/transformer.py
--rw-r--r--   0 cwq        (501) staff       (20)    11845 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/predictor.py
--rw-r--r--   0 cwq        (501) staff       (20)    12157 2024-02-18 01:24:38.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/predictor_hq.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.483064 IOPaint-1.3.0/iopaint/plugins/segment_anything/utils/
--rw-r--r--   0 cwq        (501) staff       (20)      197 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/utils/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     4054 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/plugins/segment_anything/utils/transforms.py
--rw-r--r--   0 cwq        (501) staff       (20)     2509 2024-02-08 14:13:37.000000 IOPaint-1.3.0/iopaint/runtime.py
--rw-r--r--   0 cwq        (501) staff       (20)    15152 2024-04-26 05:15:14.000000 IOPaint-1.3.0/iopaint/schema.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.486623 IOPaint-1.3.0/iopaint/tests/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)      716 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_adjust_mask.py
--rw-r--r--   0 cwq        (501) staff       (20)     1461 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_anytext.py
--rw-r--r--   0 cwq        (501) staff       (20)     3632 2024-04-29 14:20:16.000000 IOPaint-1.3.0/iopaint/tests/test_brushnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     3388 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     1194 2024-02-10 04:36:58.000000 IOPaint-1.3.0/iopaint/tests/test_instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)      552 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_load_img.py
--rw-r--r--   0 cwq        (501) staff       (20)     2944 2024-04-25 14:18:35.000000 IOPaint-1.3.0/iopaint/tests/test_low_mem.py
--rw-r--r--   0 cwq        (501) staff       (20)     1101 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_match_histograms.py
--rw-r--r--   0 cwq        (501) staff       (20)     4957 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_model.py
--rw-r--r--   0 cwq        (501) staff       (20)      476 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_model_md5.py
--rw-r--r--   0 cwq        (501) staff       (20)     1787 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_model_switch.py
--rw-r--r--   0 cwq        (501) staff       (20)     4310 2024-04-25 14:12:42.000000 IOPaint-1.3.0/iopaint/tests/test_outpainting.py
--rw-r--r--   0 cwq        (501) staff       (20)     1765 2024-04-30 05:12:50.000000 IOPaint-1.3.0/iopaint/tests/test_paint_by_example.py
--rw-r--r--   0 cwq        (501) staff       (20)     3725 2024-04-08 12:08:35.000000 IOPaint-1.3.0/iopaint/tests/test_plugins.py
--rw-r--r--   0 cwq        (501) staff       (20)     1637 2024-02-03 13:29:32.000000 IOPaint-1.3.0/iopaint/tests/test_save_exif.py
--rw-r--r--   0 cwq        (501) staff       (20)     7463 2024-04-30 05:16:27.000000 IOPaint-1.3.0/iopaint/tests/test_sd_model.py
--rw-r--r--   0 cwq        (501) staff       (20)     3265 2024-04-25 14:18:35.000000 IOPaint-1.3.0/iopaint/tests/test_sdxl.py
--rw-r--r--   0 cwq        (501) staff       (20)     2431 2024-04-21 06:23:18.000000 IOPaint-1.3.0/iopaint/tests/utils.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.486852 IOPaint-1.3.0/iopaint/web_app/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:30:21.490784 IOPaint-1.3.0/iopaint/web_app/assets/
--rw-r--r--   0 cwq        (501) staff       (20)   108748 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Black-jiII8dog.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   115364 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-BlackItalic-1413vuen.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111040 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Bold-srYz_-1B.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   118392 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-BoldItalic-dE_gZyur.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111360 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraBold-TduDdwUu.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   118604 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraBoldItalic-BJafRE5I.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   110176 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraLight-w5HAp5iF.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   116296 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraLightItalic-ZptecSuc.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   114576 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Italic-f6M78thn.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   109992 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Light-DFhX0qo-.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   116516 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-LightItalic-fu56_DRc.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111380 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Medium-dDRaJ8tM.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   118392 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-MediumItalic-zr3roggP.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   108488 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Regular-dEFHw1tF.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111588 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-SemiBold-PyS8DO2L.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   118216 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-SemiBoldItalic-uIDb7hsH.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   106620 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-Thin-eKObIkJC.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   113384 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/Inter-ThinItalic-L6uBn3RP.woff2
--rw-r--r--   0 cwq        (501) staff       (20)    40287 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/index-0foJStMW.css
--rw-r--r--   0 cwq        (501) staff       (20)   768047 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/index-KHQKnmqj.js
--rw-r--r--   0 cwq        (501) staff       (20)   207929 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/assets/kofi_button_black-XI_Dr2zg.png
--rw-r--r--   0 cwq        (501) staff       (20)      392 2024-05-06 14:30:21.000000 IOPaint-1.3.0/iopaint/web_app/index.html
--rw-r--r--   0 cwq        (501) staff       (20)    10752 2024-03-26 01:37:38.000000 IOPaint-1.3.0/iopaint/web_config.py
--rw-r--r--   0 cwq        (501) staff       (20)       38 2024-05-06 14:30:21.491302 IOPaint-1.3.0/setup.cfg
--rw-r--r--   0 cwq        (501) staff       (20)     1984 2024-05-06 14:28:56.000000 IOPaint-1.3.0/setup.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.303765 IOPaint-1.3.1/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.266784 IOPaint-1.3.1/IOPaint.egg-info/
+-rw-r--r--   0 cwq        (501) staff       (20)     7434 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     7049 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/SOURCES.txt
+-rw-r--r--   0 cwq        (501) staff       (20)        1 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/dependency_links.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       48 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/entry_points.txt
+-rw-r--r--   0 cwq        (501) staff       (20)      309 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/requires.txt
+-rw-r--r--   0 cwq        (501) staff       (20)        8 2024-05-06 14:49:15.000000 IOPaint-1.3.1/IOPaint.egg-info/top_level.txt
+-rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-11-15 00:50:32.000000 IOPaint-1.3.1/LICENSE
+-rw-r--r--   0 cwq        (501) staff       (20)     7434 2024-05-06 14:49:15.303636 IOPaint-1.3.1/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     6702 2024-05-06 14:32:37.000000 IOPaint-1.3.1/README.md
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.269836 IOPaint-1.3.1/iopaint/
+-rw-r--r--   0 cwq        (501) staff       (20)      832 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)       78 2024-02-03 13:30:22.000000 IOPaint-1.3.1/iopaint/__main__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15183 2024-02-16 02:14:38.000000 IOPaint-1.3.1/iopaint/api.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4099 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/batch_processing.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3224 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/benchmark.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7799 2024-02-09 07:17:49.000000 IOPaint-1.3.1/iopaint/cli.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4103 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/const.py
+-rw-r--r--   0 cwq        (501) staff       (20)    10785 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/download.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.270739 IOPaint-1.3.1/iopaint/file_manager/
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/file_manager/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7143 2024-02-09 07:17:49.000000 IOPaint-1.3.1/iopaint/file_manager/file_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1293 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/file_manager/storage_backends.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1835 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/file_manager/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)    12017 2024-02-18 01:21:15.000000 IOPaint-1.3.1/iopaint/helper.py
+-rw-r--r--   0 cwq        (501) staff       (20)      232 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/installer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.275134 IOPaint-1.3.1/iopaint/model/
+-rw-r--r--   0 cwq        (501) staff       (20)     1028 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/__init__.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.276298 IOPaint-1.3.1/iopaint/model/anytext/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2536 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/anytext_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15191 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/anytext_pipeline.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2777 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/anytext_sd15.yaml
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.277818 IOPaint-1.3.1/iopaint/model/anytext/cldm/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    28531 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/cldm.py
+-rw-r--r--   0 cwq        (501) staff       (20)    17275 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/ddim_hacked.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6083 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/embedding_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3699 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/hack.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1373 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/model.py
+-rwxr-xr-x   0 cwq        (501) staff       (20)    11447 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/cldm/recognizer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.278092 IOPaint-1.3.1/iopaint/model/anytext/ldm/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/__init__.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.278369 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8614 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/autoencoder.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.279405 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    18214 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 cwq        (501) staff       (20)    89020 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.279967 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 cwq        (501) staff       (20)       37 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    65969 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2990 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)    12971 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/plms.py
+-rw-r--r--   0 cwq        (501) staff       (20)      753 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.280415 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    10738 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/attention.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.281234 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    30615 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 cwq        (501) staff       (20)    30462 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3468 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 cwq        (501) staff       (20)     9995 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.281489 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/distributions/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2970 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3110 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/ema.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.281728 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/encoders/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14135 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/encoders/modules.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7250 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ldm/util.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1554 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/main.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.282902 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/
+-rwxr-xr-x   0 cwq        (501) staff       (20)     6607 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RNN.py
+-rwxr-xr-x   0 cwq        (501) staff       (20)     1260 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecCTCHead.py
+-rwxr-xr-x   0 cwq        (501) staff       (20)     1673 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecModel.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6709 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecMv1_enhance.py
+-rw-r--r--   0 cwq        (501) staff       (20)    19468 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecSVTR.py
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2180 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/common.py
+-rw-r--r--   0 cwq        (501) staff       (20)    26249 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/ppocr_keys_v1.txt
+-rw-r--r--   0 cwq        (501) staff       (20)     4989 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/anytext/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)    13463 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/base.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.284318 IOPaint-1.3.1/iopaint/model/brushnet/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/brushnet/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    47487 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/brushnet/brushnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)    16316 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/brushnet/brushnet_unet_forward.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6379 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/brushnet/brushnet_wrapper.py
+-rw-r--r--   0 cwq        (501) staff       (20)    65581 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/brushnet/pipeline_brushnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14794 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/brushnet/unet_2d_blocks.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7077 2024-05-06 14:32:37.000000 IOPaint-1.3.1/iopaint/model/controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6863 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/ddim_sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)    57219 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/fcf.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.285164 IOPaint-1.3.1/iopaint/model/helper/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/helper/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2117 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/helper/controlnet_preprocess.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1409 2024-02-10 04:35:12.000000 IOPaint-1.3.1/iopaint/model/helper/cpu_text_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1913 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/helper/g_diffuser_bot.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2436 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2041 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/kandinsky.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1608 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/lama.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11481 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/ldm.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3097 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/manga.py
+-rw-r--r--   0 cwq        (501) staff       (20)    62704 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/mat.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3438 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/mi_gan.py
+-rw-r--r--   0 cwq        (501) staff       (20)      735 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/opencv2.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.286081 IOPaint-1.3.1/iopaint/model/original_sd_configs/
+-rw-r--r--   0 cwq        (501) staff       (20)      590 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/original_sd_configs/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2784 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/original_sd_configs/sd_xl_base.yaml
+-rw-r--r--   0 cwq        (501) staff       (20)     2589 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/original_sd_configs/sd_xl_refiner.yaml
+-rw-r--r--   0 cwq        (501) staff       (20)     1873 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/original_sd_configs/v1-inference.yaml
+-rw-r--r--   0 cwq        (501) staff       (20)     1815 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/original_sd_configs/v2-inference-v.yaml
+-rw-r--r--   0 cwq        (501) staff       (20)     2792 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/paint_by_example.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11833 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/plms_sampler.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.286845 IOPaint-1.3.1/iopaint/model/power_paint/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/power_paint/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    56636 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/power_paint/pipeline_powerpaint.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3658 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/power_paint/power_paint.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6964 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/power_paint/power_paint_v2.py
+-rw-r--r--   0 cwq        (501) staff       (20)     9439 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model/power_paint/powerpaint_tokenizer.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4425 2024-05-06 14:32:37.000000 IOPaint-1.3.1/iopaint/model/sd.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3993 2024-05-06 14:32:37.000000 IOPaint-1.3.1/iopaint/model/sdxl.py
+-rw-r--r--   0 cwq        (501) staff       (20)    37847 2024-02-05 13:45:11.000000 IOPaint-1.3.1/iopaint/model/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)    16327 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/model/zits.py
+-rw-r--r--   0 cwq        (501) staff       (20)     9788 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/model_manager.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.289202 IOPaint-1.3.1/iopaint/plugins/
+-rw-r--r--   0 cwq        (501) staff       (20)     2423 2024-02-08 14:13:37.000000 IOPaint-1.3.1/iopaint/plugins/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    13787 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/anime_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)      730 2024-02-08 14:13:37.000000 IOPaint-1.3.1/iopaint/plugins/base_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14976 2024-04-08 12:07:58.000000 IOPaint-1.3.1/iopaint/plugins/briarmbg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2507 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/gfpgan_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2750 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/gfpganer.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3717 2024-02-18 01:48:00.000000 IOPaint-1.3.1/iopaint/plugins/interactive_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3989 2024-03-03 11:07:10.000000 IOPaint-1.3.1/iopaint/plugins/realesrgan.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2211 2024-04-08 12:08:35.000000 IOPaint-1.3.1/iopaint/plugins/remove_bg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1854 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/restoreformer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.290232 IOPaint-1.3.1/iopaint/plugins/segment_anything/
+-rw-r--r--   0 cwq        (501) staff       (20)      420 2024-02-18 01:14:34.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7864 2024-02-18 01:29:24.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/build_sam.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.292449 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/
+-rw-r--r--   0 cwq        (501) staff       (20)      385 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1479 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/common.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14407 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14795 2024-02-18 01:29:24.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/image_encoder_hq.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15490 2024-02-18 00:55:27.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8594 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7225 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/sam.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7474 2024-02-18 01:20:30.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/sam_hq.py
+-rw-r--r--   0 cwq        (501) staff       (20)    26182 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/tiny_vit_sam.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8396 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/transformer.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11845 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/predictor.py
+-rw-r--r--   0 cwq        (501) staff       (20)    12157 2024-02-18 01:24:38.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/predictor_hq.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.292748 IOPaint-1.3.1/iopaint/plugins/segment_anything/utils/
+-rw-r--r--   0 cwq        (501) staff       (20)      197 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/utils/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4054 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/plugins/segment_anything/utils/transforms.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2509 2024-02-08 14:13:37.000000 IOPaint-1.3.1/iopaint/runtime.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15152 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/schema.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.295785 IOPaint-1.3.1/iopaint/tests/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)      716 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_adjust_mask.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1461 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_anytext.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3632 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_brushnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3388 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1194 2024-02-10 04:36:58.000000 IOPaint-1.3.1/iopaint/tests/test_instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)      552 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_load_img.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2944 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_low_mem.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1101 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_match_histograms.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4957 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)      476 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_model_md5.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1787 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_model_switch.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4310 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_outpainting.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1765 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_paint_by_example.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3725 2024-04-08 12:08:35.000000 IOPaint-1.3.1/iopaint/tests/test_plugins.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1637 2024-02-03 13:29:32.000000 IOPaint-1.3.1/iopaint/tests/test_save_exif.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7463 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_sd_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3265 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/test_sdxl.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2431 2024-05-06 14:32:48.000000 IOPaint-1.3.1/iopaint/tests/utils.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.295895 IOPaint-1.3.1/iopaint/web_app/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2024-05-06 14:49:15.300221 IOPaint-1.3.1/iopaint/web_app/assets/
+-rw-r--r--   0 cwq        (501) staff       (20)   108748 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Black-jiII8dog.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   115364 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-BlackItalic-1413vuen.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111040 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Bold-srYz_-1B.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   118392 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-BoldItalic-dE_gZyur.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111360 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraBold-TduDdwUu.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   118604 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraBoldItalic-BJafRE5I.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   110176 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraLight-w5HAp5iF.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   116296 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraLightItalic-ZptecSuc.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   114576 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Italic-f6M78thn.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   109992 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Light-DFhX0qo-.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   116516 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-LightItalic-fu56_DRc.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111380 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Medium-dDRaJ8tM.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   118392 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-MediumItalic-zr3roggP.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   108488 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Regular-dEFHw1tF.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111588 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-SemiBold-PyS8DO2L.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   118216 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-SemiBoldItalic-uIDb7hsH.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   106620 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-Thin-eKObIkJC.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   113384 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/Inter-ThinItalic-L6uBn3RP.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)    40287 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/index-0foJStMW.css
+-rw-r--r--   0 cwq        (501) staff       (20)   768047 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/index-KHQKnmqj.js
+-rw-r--r--   0 cwq        (501) staff       (20)   207929 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/assets/kofi_button_black-XI_Dr2zg.png
+-rw-r--r--   0 cwq        (501) staff       (20)      392 2024-05-06 14:49:14.000000 IOPaint-1.3.1/iopaint/web_app/index.html
+-rw-r--r--   0 cwq        (501) staff       (20)    10752 2024-03-26 01:37:38.000000 IOPaint-1.3.1/iopaint/web_config.py
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2024-05-06 14:49:15.303814 IOPaint-1.3.1/setup.cfg
+-rw-r--r--   0 cwq        (501) staff       (20)     1984 2024-05-06 14:48:30.000000 IOPaint-1.3.1/setup.py
```

### Comparing `IOPaint-1.3.0/IOPaint.egg-info/PKG-INFO` & `IOPaint-1.3.1/IOPaint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOPaint
-Version: 1.3.0
+Version: 1.3.1
 Summary: Image inpainting, outpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/IOPaint
 Author: PanicByte
 Author-email: cwq1913@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -140,11 +140,11 @@
 ```bash
 npm run dev
 ```
 
 Install back-end requirements and start back-end service
 ```bash
 pip install -r requirements.txt
-python3 main.py --model lama --port 8080
+python3 main.py start --model lama --port 8080
 ```
 
 Then you can visit `http://localhost:5173/` for development. The front-end code will automatically update after being modified, but the back-end needs to restart the service after modifying the python code.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: IOPaint Version: 1.3.0 Summary: Image inpainting,
+Metadata-Version: 2.1 Name: IOPaint Version: 1.3.1 Summary: Image inpainting,
 outpainting tool powered by SOTA AI Model Home-page: https://github.com/
 Sanster/IOPaint Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
@@ -74,11 +74,11 @@
 You can see more information about the available models and plugins supported
 by IOPaint below. ## Development Install [nodejs](https://nodejs.org/en), then
 install the front-end dependencies. ```bash git clone https://github.com/
 Sanster/IOPaint.git cd IOPaint/web_app npm install ``` Create a `.env.local`
 file in `web_app` and fill in the backend IP and port. ``` VITE_BACKEND=http://
 127.0.0.1:8080 ``` Start front-end development environment ```bash npm run dev
 ``` Install back-end requirements and start back-end service ```bash pip
-install -r requirements.txt python3 main.py --model lama --port 8080 ``` Then
-you can visit `http://localhost:5173/` for development. The front-end code will
-automatically update after being modified, but the back-end needs to restart
-the service after modifying the python code.
+install -r requirements.txt python3 main.py start --model lama --port 8080 ```
+Then you can visit `http://localhost:5173/` for development. The front-end code
+will automatically update after being modified, but the back-end needs to
+restart the service after modifying the python code.
```

### Comparing `IOPaint-1.3.0/IOPaint.egg-info/SOURCES.txt` & `IOPaint-1.3.1/IOPaint.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 iopaint/model/anytext/ocr_recog/RecCTCHead.py
 iopaint/model/anytext/ocr_recog/RecModel.py
 iopaint/model/anytext/ocr_recog/RecMv1_enhance.py
 iopaint/model/anytext/ocr_recog/RecSVTR.py
 iopaint/model/anytext/ocr_recog/__init__.py
 iopaint/model/anytext/ocr_recog/common.py
 iopaint/model/anytext/ocr_recog/ppocr_keys_v1.txt
+iopaint/model/brushnet/__init__.py
+iopaint/model/brushnet/brushnet.py
+iopaint/model/brushnet/brushnet_unet_forward.py
+iopaint/model/brushnet/brushnet_wrapper.py
+iopaint/model/brushnet/pipeline_brushnet.py
+iopaint/model/brushnet/unet_2d_blocks.py
 iopaint/model/helper/__init__.py
 iopaint/model/helper/controlnet_preprocess.py
 iopaint/model/helper/cpu_text_encoder.py
 iopaint/model/helper/g_diffuser_bot.py
 iopaint/model/original_sd_configs/__init__.py
 iopaint/model/original_sd_configs/sd_xl_base.yaml
 iopaint/model/original_sd_configs/sd_xl_refiner.yaml
```

### Comparing `IOPaint-1.3.0/LICENSE` & `IOPaint-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/PKG-INFO` & `IOPaint-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IOPaint
-Version: 1.3.0
+Version: 1.3.1
 Summary: Image inpainting, outpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/IOPaint
 Author: PanicByte
 Author-email: cwq1913@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -140,11 +140,11 @@
 ```bash
 npm run dev
 ```
 
 Install back-end requirements and start back-end service
 ```bash
 pip install -r requirements.txt
-python3 main.py --model lama --port 8080
+python3 main.py start --model lama --port 8080
 ```
 
 Then you can visit `http://localhost:5173/` for development. The front-end code will automatically update after being modified, but the back-end needs to restart the service after modifying the python code.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: IOPaint Version: 1.3.0 Summary: Image inpainting,
+Metadata-Version: 2.1 Name: IOPaint Version: 1.3.1 Summary: Image inpainting,
 outpainting tool powered by SOTA AI Model Home-page: https://github.com/
 Sanster/IOPaint Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
@@ -74,11 +74,11 @@
 You can see more information about the available models and plugins supported
 by IOPaint below. ## Development Install [nodejs](https://nodejs.org/en), then
 install the front-end dependencies. ```bash git clone https://github.com/
 Sanster/IOPaint.git cd IOPaint/web_app npm install ``` Create a `.env.local`
 file in `web_app` and fill in the backend IP and port. ``` VITE_BACKEND=http://
 127.0.0.1:8080 ``` Start front-end development environment ```bash npm run dev
 ``` Install back-end requirements and start back-end service ```bash pip
-install -r requirements.txt python3 main.py --model lama --port 8080 ``` Then
-you can visit `http://localhost:5173/` for development. The front-end code will
-automatically update after being modified, but the back-end needs to restart
-the service after modifying the python code.
+install -r requirements.txt python3 main.py start --model lama --port 8080 ```
+Then you can visit `http://localhost:5173/` for development. The front-end code
+will automatically update after being modified, but the back-end needs to
+restart the service after modifying the python code.
```

### Comparing `IOPaint-1.3.0/README.md` & `IOPaint-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -121,11 +121,11 @@
 ```bash
 npm run dev
 ```
 
 Install back-end requirements and start back-end service
 ```bash
 pip install -r requirements.txt
-python3 main.py --model lama --port 8080
+python3 main.py start --model lama --port 8080
 ```
 
 Then you can visit `http://localhost:5173/` for development. The front-end code will automatically update after being modified, but the back-end needs to restart the service after modifying the python code.
```

#### html2text {}

```diff
@@ -64,11 +64,11 @@
 You can see more information about the available models and plugins supported
 by IOPaint below. ## Development Install [nodejs](https://nodejs.org/en), then
 install the front-end dependencies. ```bash git clone https://github.com/
 Sanster/IOPaint.git cd IOPaint/web_app npm install ``` Create a `.env.local`
 file in `web_app` and fill in the backend IP and port. ``` VITE_BACKEND=http://
 127.0.0.1:8080 ``` Start front-end development environment ```bash npm run dev
 ``` Install back-end requirements and start back-end service ```bash pip
-install -r requirements.txt python3 main.py --model lama --port 8080 ``` Then
-you can visit `http://localhost:5173/` for development. The front-end code will
-automatically update after being modified, but the back-end needs to restart
-the service after modifying the python code.
+install -r requirements.txt python3 main.py start --model lama --port 8080 ```
+Then you can visit `http://localhost:5173/` for development. The front-end code
+will automatically update after being modified, but the back-end needs to
+restart the service after modifying the python code.
```

### Comparing `IOPaint-1.3.0/iopaint/__init__.py` & `IOPaint-1.3.1/iopaint/__init__.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/api.py` & `IOPaint-1.3.1/iopaint/api.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/batch_processing.py` & `IOPaint-1.3.1/iopaint/batch_processing.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/benchmark.py` & `IOPaint-1.3.1/iopaint/benchmark.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/cli.py` & `IOPaint-1.3.1/iopaint/cli.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/const.py` & `IOPaint-1.3.1/iopaint/const.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/download.py` & `IOPaint-1.3.1/iopaint/download.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/file_manager/file_manager.py` & `IOPaint-1.3.1/iopaint/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/file_manager/storage_backends.py` & `IOPaint-1.3.1/iopaint/file_manager/storage_backends.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/file_manager/utils.py` & `IOPaint-1.3.1/iopaint/file_manager/utils.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/helper.py` & `IOPaint-1.3.1/iopaint/helper.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/__init__.py` & `IOPaint-1.3.1/iopaint/model/__init__.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/anytext_model.py` & `IOPaint-1.3.1/iopaint/model/anytext/anytext_model.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/anytext_pipeline.py` & `IOPaint-1.3.1/iopaint/model/anytext/anytext_pipeline.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/anytext_sd15.yaml` & `IOPaint-1.3.1/iopaint/model/anytext/anytext_sd15.yaml`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/cldm.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/ddim_hacked.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/ddim_hacked.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/embedding_manager.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/embedding_manager.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/hack.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/hack.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/model.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/model.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/cldm/recognizer.py` & `IOPaint-1.3.1/iopaint/model/anytext/cldm/recognizer.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/autoencoder.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/ddim.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/ddpm.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/sampler.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/plms.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/models/diffusion/sampling_util.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/attention.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/model.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/openaimodel.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/upscaling.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/diffusionmodules/util.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/distributions/distributions.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/ema.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/modules/encoders/modules.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ldm/util.py` & `IOPaint-1.3.1/iopaint/model/anytext/ldm/util.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/main.py` & `IOPaint-1.3.1/iopaint/model/anytext/main.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RNN.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RNN.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecCTCHead.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecCTCHead.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecModel.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecModel.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecMv1_enhance.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecMv1_enhance.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/RecSVTR.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/RecSVTR.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/common.py` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/common.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/ocr_recog/ppocr_keys_v1.txt` & `IOPaint-1.3.1/iopaint/model/anytext/ocr_recog/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/anytext/utils.py` & `IOPaint-1.3.1/iopaint/model/anytext/utils.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/base.py` & `IOPaint-1.3.1/iopaint/model/base.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/controlnet.py` & `IOPaint-1.3.1/iopaint/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/ddim_sampler.py` & `IOPaint-1.3.1/iopaint/model/ddim_sampler.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/fcf.py` & `IOPaint-1.3.1/iopaint/model/fcf.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/helper/controlnet_preprocess.py` & `IOPaint-1.3.1/iopaint/model/helper/controlnet_preprocess.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/helper/cpu_text_encoder.py` & `IOPaint-1.3.1/iopaint/model/helper/cpu_text_encoder.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/helper/g_diffuser_bot.py` & `IOPaint-1.3.1/iopaint/model/helper/g_diffuser_bot.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/instruct_pix2pix.py` & `IOPaint-1.3.1/iopaint/model/instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/kandinsky.py` & `IOPaint-1.3.1/iopaint/model/kandinsky.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/lama.py` & `IOPaint-1.3.1/iopaint/model/lama.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/ldm.py` & `IOPaint-1.3.1/iopaint/model/ldm.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/manga.py` & `IOPaint-1.3.1/iopaint/model/manga.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/mat.py` & `IOPaint-1.3.1/iopaint/model/mat.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/mi_gan.py` & `IOPaint-1.3.1/iopaint/model/mi_gan.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/opencv2.py` & `IOPaint-1.3.1/iopaint/model/opencv2.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/original_sd_configs/__init__.py` & `IOPaint-1.3.1/iopaint/model/original_sd_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/original_sd_configs/sd_xl_base.yaml` & `IOPaint-1.3.1/iopaint/model/original_sd_configs/sd_xl_base.yaml`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/original_sd_configs/sd_xl_refiner.yaml` & `IOPaint-1.3.1/iopaint/model/original_sd_configs/sd_xl_refiner.yaml`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/original_sd_configs/v1-inference.yaml` & `IOPaint-1.3.1/iopaint/model/original_sd_configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/original_sd_configs/v2-inference-v.yaml` & `IOPaint-1.3.1/iopaint/model/original_sd_configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/paint_by_example.py` & `IOPaint-1.3.1/iopaint/model/paint_by_example.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/plms_sampler.py` & `IOPaint-1.3.1/iopaint/model/plms_sampler.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/power_paint/pipeline_powerpaint.py` & `IOPaint-1.3.1/iopaint/model/power_paint/pipeline_powerpaint.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/power_paint/power_paint.py` & `IOPaint-1.3.1/iopaint/model/power_paint/power_paint.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/power_paint/power_paint_v2.py` & `IOPaint-1.3.1/iopaint/model/power_paint/power_paint_v2.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/power_paint/powerpaint_tokenizer.py` & `IOPaint-1.3.1/iopaint/model/power_paint/powerpaint_tokenizer.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/sd.py` & `IOPaint-1.3.1/iopaint/model/sd.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/sdxl.py` & `IOPaint-1.3.1/iopaint/model/sdxl.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/utils.py` & `IOPaint-1.3.1/iopaint/model/utils.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model/zits.py` & `IOPaint-1.3.1/iopaint/model/zits.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/model_manager.py` & `IOPaint-1.3.1/iopaint/model_manager.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/__init__.py` & `IOPaint-1.3.1/iopaint/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/anime_seg.py` & `IOPaint-1.3.1/iopaint/plugins/anime_seg.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/base_plugin.py` & `IOPaint-1.3.1/iopaint/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/briarmbg.py` & `IOPaint-1.3.1/iopaint/plugins/briarmbg.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/gfpgan_plugin.py` & `IOPaint-1.3.1/iopaint/plugins/gfpgan_plugin.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/gfpganer.py` & `IOPaint-1.3.1/iopaint/plugins/gfpganer.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/interactive_seg.py` & `IOPaint-1.3.1/iopaint/plugins/interactive_seg.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/realesrgan.py` & `IOPaint-1.3.1/iopaint/plugins/realesrgan.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/remove_bg.py` & `IOPaint-1.3.1/iopaint/plugins/remove_bg.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/restoreformer.py` & `IOPaint-1.3.1/iopaint/plugins/restoreformer.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/build_sam.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/common.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/image_encoder.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/image_encoder_hq.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/image_encoder_hq.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/mask_decoder.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/prompt_encoder.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/sam.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/sam_hq.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/sam_hq.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/tiny_vit_sam.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/tiny_vit_sam.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/modeling/transformer.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/predictor.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/predictor_hq.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/predictor_hq.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/plugins/segment_anything/utils/transforms.py` & `IOPaint-1.3.1/iopaint/plugins/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/runtime.py` & `IOPaint-1.3.1/iopaint/runtime.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/schema.py` & `IOPaint-1.3.1/iopaint/schema.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_adjust_mask.py` & `IOPaint-1.3.1/iopaint/tests/test_adjust_mask.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_anytext.py` & `IOPaint-1.3.1/iopaint/tests/test_anytext.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_brushnet.py` & `IOPaint-1.3.1/iopaint/tests/test_brushnet.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_controlnet.py` & `IOPaint-1.3.1/iopaint/tests/test_controlnet.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_instruct_pix2pix.py` & `IOPaint-1.3.1/iopaint/tests/test_instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_load_img.py` & `IOPaint-1.3.1/iopaint/tests/test_load_img.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_low_mem.py` & `IOPaint-1.3.1/iopaint/tests/test_low_mem.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_match_histograms.py` & `IOPaint-1.3.1/iopaint/tests/test_match_histograms.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_model.py` & `IOPaint-1.3.1/iopaint/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_model_switch.py` & `IOPaint-1.3.1/iopaint/tests/test_model_switch.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_outpainting.py` & `IOPaint-1.3.1/iopaint/tests/test_outpainting.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_paint_by_example.py` & `IOPaint-1.3.1/iopaint/tests/test_paint_by_example.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_plugins.py` & `IOPaint-1.3.1/iopaint/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_save_exif.py` & `IOPaint-1.3.1/iopaint/tests/test_save_exif.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_sd_model.py` & `IOPaint-1.3.1/iopaint/tests/test_sd_model.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/test_sdxl.py` & `IOPaint-1.3.1/iopaint/tests/test_sdxl.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/tests/utils.py` & `IOPaint-1.3.1/iopaint/tests/utils.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Black-jiII8dog.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Black-jiII8dog.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-BlackItalic-1413vuen.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-BlackItalic-1413vuen.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Bold-srYz_-1B.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Bold-srYz_-1B.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-BoldItalic-dE_gZyur.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-BoldItalic-dE_gZyur.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraBold-TduDdwUu.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraBold-TduDdwUu.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraBoldItalic-BJafRE5I.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraBoldItalic-BJafRE5I.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraLight-w5HAp5iF.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraLight-w5HAp5iF.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-ExtraLightItalic-ZptecSuc.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-ExtraLightItalic-ZptecSuc.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Italic-f6M78thn.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Italic-f6M78thn.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Light-DFhX0qo-.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Light-DFhX0qo-.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-LightItalic-fu56_DRc.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-LightItalic-fu56_DRc.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Medium-dDRaJ8tM.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Medium-dDRaJ8tM.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-MediumItalic-zr3roggP.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-MediumItalic-zr3roggP.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Regular-dEFHw1tF.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Regular-dEFHw1tF.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-SemiBold-PyS8DO2L.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-SemiBold-PyS8DO2L.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-SemiBoldItalic-uIDb7hsH.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-SemiBoldItalic-uIDb7hsH.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-Thin-eKObIkJC.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-Thin-eKObIkJC.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/Inter-ThinItalic-L6uBn3RP.woff2` & `IOPaint-1.3.1/iopaint/web_app/assets/Inter-ThinItalic-L6uBn3RP.woff2`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/index-0foJStMW.css` & `IOPaint-1.3.1/iopaint/web_app/assets/index-0foJStMW.css`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/index-KHQKnmqj.js` & `IOPaint-1.3.1/iopaint/web_app/assets/index-KHQKnmqj.js`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_app/assets/kofi_button_black-XI_Dr2zg.png` & `IOPaint-1.3.1/iopaint/web_app/assets/kofi_button_black-XI_Dr2zg.png`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/iopaint/web_config.py` & `IOPaint-1.3.1/iopaint/web_config.py`

 * *Files identical despite different names*

### Comparing `IOPaint-1.3.0/setup.py` & `IOPaint-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 requires.append(line.strip())
     return requires
 
 
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files
 setuptools.setup(
     name="IOPaint",
-    version="1.3.0",
+    version="1.3.1",
     author="PanicByte",
     author_email="cwq1913@gmail.com",
     description="Image inpainting, outpainting tool powered by SOTA AI Model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sanster/IOPaint",
     packages=setuptools.find_packages("."),
```

