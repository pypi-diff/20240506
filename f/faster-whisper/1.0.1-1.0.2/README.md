# Comparing `tmp/faster-whisper-1.0.1.tar.gz` & `tmp/faster-whisper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster-whisper-1.0.1.tar", last modified: Fri Mar  1 10:44:14 2024, max compression
+gzip compressed data, was "faster-whisper-1.0.2.tar", last modified: Mon May  6 02:09:37 2024, max compression
```

## Comparing `faster-whisper-1.0.1.tar` & `faster-whisper-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:14.404090 faster-whisper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-03-01 10:44:14.404090 faster-whisper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:14.400090 faster-whisper-1.0.1/faster_whisper/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:14.400090 faster-whisper-1.0.1/faster_whisper/assets/
--rw-r--r--   0 runner    (1001) docker     (127)  1807524 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/assets/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    48470 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/faster_whisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:44:14.400090 faster-whisper-1.0.1/faster_whisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-03-01 10:44:14.000000 faster-whisper-1.0.1/faster_whisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-01 10:44:14.000000 faster-whisper-1.0.1/faster_whisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:44:14.000000 faster-whisper-1.0.1/faster_whisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-01 10:44:14.000000 faster-whisper-1.0.1/faster_whisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-01 10:44:14.000000 faster-whisper-1.0.1/faster_whisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/requirements.conversion.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-01 10:44:14.404090 faster-whisper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-01 10:44:11.000000 faster-whisper-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:09:37.861417 faster-whisper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 02:09:32.000000 faster-whisper-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 02:09:32.000000 faster-whisper-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-06 02:09:37.861417 faster-whisper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14305 2024-05-06 02:09:32.000000 faster-whisper-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:09:37.857417 faster-whisper-1.0.2/faster_whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:09:37.857417 faster-whisper-1.0.2/faster_whisper/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1807524 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/assets/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51978 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/faster_whisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:09:37.857417 faster-whisper-1.0.2/faster_whisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-06 02:09:37.000000 faster-whisper-1.0.2/faster_whisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 02:09:37.000000 faster-whisper-1.0.2/faster_whisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:09:37.000000 faster-whisper-1.0.2/faster_whisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 02:09:37.000000 faster-whisper-1.0.2/faster_whisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 02:09:37.000000 faster-whisper-1.0.2/faster_whisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/requirements.conversion.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 02:09:37.861417 faster-whisper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-06 02:09:33.000000 faster-whisper-1.0.2/setup.py
```

### Comparing `faster-whisper-1.0.1/LICENSE` & `faster-whisper-1.0.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Guillaume Klein
+Copyright (c) 2023 SYSTRAN
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `faster-whisper-1.0.1/PKG-INFO` & `faster-whisper-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Faster Whisper transcription with CTranslate2
-Home-page: https://github.com/guillaumekln/faster-whisper
+Home-page: https://github.com/SYSTRAN/faster-whisper
 Author: Guillaume Klein
 License: MIT
-Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
+Description: [![CI](https://github.com/SYSTRAN/faster-whisper/workflows/CI/badge.svg)](https://github.com/SYSTRAN/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
         
         **faster-whisper** is a reimplementation of OpenAI's Whisper model using [CTranslate2](https://github.com/OpenNMT/CTranslate2/), which is a fast inference engine for Transformer models.
         
         This implementation is up to 4 times faster than [openai/whisper](https://github.com/openai/whisper) for the same accuracy while using less memory. The efficiency can be further improved with 8-bit quantization on both CPU and GPU.
         
@@ -17,15 +17,15 @@
         
         ### Whisper
         
         For reference, here's the time and memory usage that are required to transcribe [**13 minutes**](https://www.youtube.com/watch?v=0u7tTptBo9I) of audio using different implementations:
         
         * [openai/whisper](https://github.com/openai/whisper)@[6dea21fd](https://github.com/openai/whisper/commit/6dea21fd7f7253bfe450f1e2512a0fe47ee2d258)
         * [whisper.cpp](https://github.com/ggerganov/whisper.cpp)@[3b010f9](https://github.com/ggerganov/whisper.cpp/commit/3b010f9bed9a6068609e9faf52383aea792b0362)
-        * [faster-whisper](https://github.com/guillaumekln/faster-whisper)@[cce6b53e](https://github.com/guillaumekln/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
+        * [faster-whisper](https://github.com/SYSTRAN/faster-whisper)@[cce6b53e](https://github.com/SYSTRAN/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
         
         ### Large-v2 model on GPU
         
         | Implementation | Precision | Beam size | Time | Max. GPU memory | Max. CPU memory |
         | --- | --- | --- | --- | --- | --- |
         | openai/whisper | fp16 | 5 | 4m30s | 11325MB | 9439MB |
         | faster-whisper | fp16 | 5 | 54s | 4755MB | 3244MB |
@@ -78,36 +78,43 @@
         
         Unlike openai-whisper, FFmpeg does **not** need to be installed on the system. The audio is decoded with the Python library [PyAV](https://github.com/PyAV-Org/PyAV) which bundles the FFmpeg libraries in its package.
         
         ### GPU
         
         GPU execution requires the following NVIDIA libraries to be installed:
         
-        * [cuBLAS for CUDA 11](https://developer.nvidia.com/cublas)
-        * [cuDNN 8 for CUDA 11](https://developer.nvidia.com/cudnn)
+        * [cuBLAS for CUDA 12](https://developer.nvidia.com/cublas)
+        * [cuDNN 8 for CUDA 12](https://developer.nvidia.com/cudnn)
         
-        There are multiple ways to install these libraries. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below.
+        **Note**: Latest versions of `ctranslate2` support CUDA 12 only. For CUDA 11, the current workaround is downgrading to the `3.24.0` version of `ctranslate2` (This can be done with `pip install --force-reinsall ctranslate2==3.24.0` or specifying the version in a `requirements.txt`).
+        
+        There are multiple ways to install the NVIDIA libraries mentioned above. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below. 
         
         <details>
         <summary>Other installation methods (click to expand)</summary>
         
+        
+        **Note:** For all these methods below, keep in mind the above note regarding CUDA versions. Depending on your setup, you may need to install the _CUDA 11_ versions of libraries that correspond to the CUDA 12 libraries listed in the instructions below.
+        
         #### Use Docker
         
-        The libraries are installed in this official NVIDIA Docker image: `nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu22.04`.
+        The libraries (cuBLAS, cuDNN) are installed in these official NVIDIA CUDA Docker images: `nvidia/cuda:12.0.0-runtime-ubuntu20.04` or `nvidia/cuda:12.0.0-runtime-ubuntu22.04`.
         
         #### Install with `pip` (Linux only)
         
         On Linux these libraries can be installed with `pip`. Note that `LD_LIBRARY_PATH` must be set before launching Python.
         
         ```bash
-        pip install nvidia-cublas-cu11 nvidia-cudnn-cu11
+        pip install nvidia-cublas-cu12 nvidia-cudnn-cu12
         
         export LD_LIBRARY_PATH=`python3 -c 'import os; import nvidia.cublas.lib; import nvidia.cudnn.lib; print(os.path.dirname(nvidia.cublas.lib.__file__) + ":" + os.path.dirname(nvidia.cudnn.lib.__file__))'`
         ```
         
+        **Note**: Version 9+ of `nvidia-cudnn-cu12` appears to cause issues due its reliance on cuDNN 9 (Faster-Whisper does not currently support cuDNN 9). Ensure your version of the Python package is for cuDNN 8.
+        
         #### Download the libraries from Purfview's repository (Windows & Linux)
         
         Purfview's [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) provides the required NVIDIA libraries for Windows & Linux in a [single archive](https://github.com/Purfview/whisper-standalone-win/releases/tag/libs). Decompress the archive and place the libraries in a directory included in the `PATH`.
         
         </details>
         
         ## Installation
@@ -120,21 +127,21 @@
         
         <details>
         <summary>Other installation methods (click to expand)</summary>
         
         ### Install the master branch
         
         ```bash
-        pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
+        pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/refs/heads/master.tar.gz"
         ```
         
         ### Install a specific commit
         
         ```bash
-        pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
+        pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
         ```
         
         </details>
         
         ## Usage
         
         ### Faster-whisper
@@ -162,26 +169,33 @@
         
         **Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
         
         ```python
         segments, _ = model.transcribe("audio.mp3")
         segments = list(segments)  # The transcription will actually run here.
         ```
-        ### Faster-distil-whisper
-        For usage of `faster-distil-whisper`, please refer to: https://github.com/guillaumekln/faster-whisper/issues/533
+        ### Faster Distil-Whisper
+        
+        The Distil-Whisper checkpoints are compatible with the Faster-Whisper package. In particular, the latest [distil-large-v3](https://huggingface.co/distil-whisper/distil-large-v3)
+        checkpoint is intrinsically designed to work with the Faster-Whisper transcription algorithm. The following code snippet 
+        demonstrates how to run inference with distil-large-v3 on a specified audio file:
         
         ```python
-        model_size = "distil-large-v2"
-        # model_size = "distil-medium.en"
+        from faster_whisper import WhisperModel
+        
+        model_size = "distil-large-v3"
+        
         model = WhisperModel(model_size, device="cuda", compute_type="float16")
-        segments, info = model.transcribe("audio.mp3", beam_size=5, 
-            language="en", max_new_tokens=128, condition_on_previous_text=False)
+        segments, info = model.transcribe("audio.mp3", beam_size=5, language="en", condition_on_previous_text=False)
         
+        for segment in segments:
+            print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
         ```
-        NOTE: Empirically, `condition_on_previous_text=True` will degrade the performance of `faster-distil-whisper` for long audio. Degradation on the first chunk was observed with `initial_prompt` too.
+        
+        For more information about the distil-large-v3 model, refer to the original [model card](https://huggingface.co/distil-whisper/distil-large-v3).
         
         ### Word-level timestamps
         
         ```python
         segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
         
         for segment in segments:
@@ -193,15 +207,15 @@
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
-        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe(
             "audio.mp3",
             vad_filter=True,
             vad_parameters=dict(min_silence_duration_ms=500),
         )
@@ -216,15 +230,15 @@
         
         logging.basicConfig()
         logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
         ```
         
         ### Going further
         
-        See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
+        See more model and transcription options in the [`WhisperModel`](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
         ## Community integrations
         
         Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
         
         * [WhisperX](https://github.com/m-bain/whisperX) is an award-winning Python library that offers speaker diarization and accurate word-level timestamps using wav2vec2 alignment
```

### Comparing `faster-whisper-1.0.1/README.md` & `faster-whisper-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
+[![CI](https://github.com/SYSTRAN/faster-whisper/workflows/CI/badge.svg)](https://github.com/SYSTRAN/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
 
 # Faster Whisper transcription with CTranslate2
 
 **faster-whisper** is a reimplementation of OpenAI's Whisper model using [CTranslate2](https://github.com/OpenNMT/CTranslate2/), which is a fast inference engine for Transformer models.
 
 This implementation is up to 4 times faster than [openai/whisper](https://github.com/openai/whisper) for the same accuracy while using less memory. The efficiency can be further improved with 8-bit quantization on both CPU and GPU.
 
@@ -10,15 +10,15 @@
 
 ### Whisper
 
 For reference, here's the time and memory usage that are required to transcribe [**13 minutes**](https://www.youtube.com/watch?v=0u7tTptBo9I) of audio using different implementations:
 
 * [openai/whisper](https://github.com/openai/whisper)@[6dea21fd](https://github.com/openai/whisper/commit/6dea21fd7f7253bfe450f1e2512a0fe47ee2d258)
 * [whisper.cpp](https://github.com/ggerganov/whisper.cpp)@[3b010f9](https://github.com/ggerganov/whisper.cpp/commit/3b010f9bed9a6068609e9faf52383aea792b0362)
-* [faster-whisper](https://github.com/guillaumekln/faster-whisper)@[cce6b53e](https://github.com/guillaumekln/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
+* [faster-whisper](https://github.com/SYSTRAN/faster-whisper)@[cce6b53e](https://github.com/SYSTRAN/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
 
 ### Large-v2 model on GPU
 
 | Implementation | Precision | Beam size | Time | Max. GPU memory | Max. CPU memory |
 | --- | --- | --- | --- | --- | --- |
 | openai/whisper | fp16 | 5 | 4m30s | 11325MB | 9439MB |
 | faster-whisper | fp16 | 5 | 54s | 4755MB | 3244MB |
@@ -71,36 +71,43 @@
 
 Unlike openai-whisper, FFmpeg does **not** need to be installed on the system. The audio is decoded with the Python library [PyAV](https://github.com/PyAV-Org/PyAV) which bundles the FFmpeg libraries in its package.
 
 ### GPU
 
 GPU execution requires the following NVIDIA libraries to be installed:
 
-* [cuBLAS for CUDA 11](https://developer.nvidia.com/cublas)
-* [cuDNN 8 for CUDA 11](https://developer.nvidia.com/cudnn)
+* [cuBLAS for CUDA 12](https://developer.nvidia.com/cublas)
+* [cuDNN 8 for CUDA 12](https://developer.nvidia.com/cudnn)
 
-There are multiple ways to install these libraries. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below.
+**Note**: Latest versions of `ctranslate2` support CUDA 12 only. For CUDA 11, the current workaround is downgrading to the `3.24.0` version of `ctranslate2` (This can be done with `pip install --force-reinsall ctranslate2==3.24.0` or specifying the version in a `requirements.txt`).
+
+There are multiple ways to install the NVIDIA libraries mentioned above. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below. 
 
 <details>
 <summary>Other installation methods (click to expand)</summary>
 
+
+**Note:** For all these methods below, keep in mind the above note regarding CUDA versions. Depending on your setup, you may need to install the _CUDA 11_ versions of libraries that correspond to the CUDA 12 libraries listed in the instructions below.
+
 #### Use Docker
 
-The libraries are installed in this official NVIDIA Docker image: `nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu22.04`.
+The libraries (cuBLAS, cuDNN) are installed in these official NVIDIA CUDA Docker images: `nvidia/cuda:12.0.0-runtime-ubuntu20.04` or `nvidia/cuda:12.0.0-runtime-ubuntu22.04`.
 
 #### Install with `pip` (Linux only)
 
 On Linux these libraries can be installed with `pip`. Note that `LD_LIBRARY_PATH` must be set before launching Python.
 
 ```bash
-pip install nvidia-cublas-cu11 nvidia-cudnn-cu11
+pip install nvidia-cublas-cu12 nvidia-cudnn-cu12
 
 export LD_LIBRARY_PATH=`python3 -c 'import os; import nvidia.cublas.lib; import nvidia.cudnn.lib; print(os.path.dirname(nvidia.cublas.lib.__file__) + ":" + os.path.dirname(nvidia.cudnn.lib.__file__))'`
 ```
 
+**Note**: Version 9+ of `nvidia-cudnn-cu12` appears to cause issues due its reliance on cuDNN 9 (Faster-Whisper does not currently support cuDNN 9). Ensure your version of the Python package is for cuDNN 8.
+
 #### Download the libraries from Purfview's repository (Windows & Linux)
 
 Purfview's [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) provides the required NVIDIA libraries for Windows & Linux in a [single archive](https://github.com/Purfview/whisper-standalone-win/releases/tag/libs). Decompress the archive and place the libraries in a directory included in the `PATH`.
 
 </details>
 
 ## Installation
@@ -113,21 +120,21 @@
 
 <details>
 <summary>Other installation methods (click to expand)</summary>
 
 ### Install the master branch
 
 ```bash
-pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
+pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/refs/heads/master.tar.gz"
 ```
 
 ### Install a specific commit
 
 ```bash
-pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
+pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
 ```
 
 </details>
 
 ## Usage
 
 ### Faster-whisper
@@ -155,26 +162,33 @@
 
 **Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
 
 ```python
 segments, _ = model.transcribe("audio.mp3")
 segments = list(segments)  # The transcription will actually run here.
 ```
-### Faster-distil-whisper
-For usage of `faster-distil-whisper`, please refer to: https://github.com/guillaumekln/faster-whisper/issues/533
+### Faster Distil-Whisper
+
+The Distil-Whisper checkpoints are compatible with the Faster-Whisper package. In particular, the latest [distil-large-v3](https://huggingface.co/distil-whisper/distil-large-v3)
+checkpoint is intrinsically designed to work with the Faster-Whisper transcription algorithm. The following code snippet 
+demonstrates how to run inference with distil-large-v3 on a specified audio file:
 
 ```python
-model_size = "distil-large-v2"
-# model_size = "distil-medium.en"
+from faster_whisper import WhisperModel
+
+model_size = "distil-large-v3"
+
 model = WhisperModel(model_size, device="cuda", compute_type="float16")
-segments, info = model.transcribe("audio.mp3", beam_size=5, 
-    language="en", max_new_tokens=128, condition_on_previous_text=False)
+segments, info = model.transcribe("audio.mp3", beam_size=5, language="en", condition_on_previous_text=False)
 
+for segment in segments:
+    print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
 ```
-NOTE: Empirically, `condition_on_previous_text=True` will degrade the performance of `faster-distil-whisper` for long audio. Degradation on the first chunk was observed with `initial_prompt` too.
+
+For more information about the distil-large-v3 model, refer to the original [model card](https://huggingface.co/distil-whisper/distil-large-v3).
 
 ### Word-level timestamps
 
 ```python
 segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
 
 for segment in segments:
@@ -186,15 +200,15 @@
 
 The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
 
 ```python
 segments, _ = model.transcribe("audio.mp3", vad_filter=True)
 ```
 
-The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
 
 ```python
 segments, _ = model.transcribe(
     "audio.mp3",
     vad_filter=True,
     vad_parameters=dict(min_silence_duration_ms=500),
 )
@@ -209,15 +223,15 @@
 
 logging.basicConfig()
 logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
 ```
 
 ### Going further
 
-See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
+See more model and transcription options in the [`WhisperModel`](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
 
 ## Community integrations
 
 Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
 
 
 * [WhisperX](https://github.com/m-bain/whisperX) is an award-winning Python library that offers speaker diarization and accurate word-level timestamps using wav2vec2 alignment
```

### Comparing `faster-whisper-1.0.1/faster_whisper/assets/silero_vad.onnx` & `faster-whisper-1.0.2/faster_whisper/assets/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `faster-whisper-1.0.1/faster_whisper/audio.py` & `faster-whisper-1.0.2/faster_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-1.0.1/faster_whisper/feature_extractor.py` & `faster-whisper-1.0.2/faster_whisper/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-1.0.1/faster_whisper/tokenizer.py` & `faster-whisper-1.0.2/faster_whisper/tokenizer.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-1.0.1/faster_whisper/transcribe.py` & `faster-whisper-1.0.2/faster_whisper/transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     max_initial_timestamp: float
     word_timestamps: bool
     prepend_punctuations: str
     append_punctuations: str
     max_new_tokens: Optional[int]
     clip_timestamps: Union[str, List[float]]
     hallucination_silence_threshold: Optional[float]
+    hotwords: Optional[str]
 
 
 class TranscriptionInfo(NamedTuple):
     language: str
     language_probability: float
     duration: float
     duration_after_vad: float
@@ -88,14 +89,16 @@
         device: str = "auto",
         device_index: Union[int, List[int]] = 0,
         compute_type: str = "default",
         cpu_threads: int = 0,
         num_workers: int = 1,
         download_root: Optional[str] = None,
         local_files_only: bool = False,
+        files: dict = None,
+        **model_kwargs,
     ):
         """Initializes the Whisper model.
 
         Args:
           model_size_or_path: Size of the model to use (tiny, tiny.en, base, base.en,
             small, small.en, medium, medium.en, large-v1, large-v2, large-v3, or large), a path to a
             converted model directory, or a CTranslate2-converted Whisper model ID from the HF Hub.
@@ -114,18 +117,26 @@
             having multiple workers enables true parallelism when running the model
             (concurrent calls to self.model.generate() will run in parallel).
             This can improve the global throughput at the cost of increased memory usage.
           download_root: Directory where the models should be saved. If not set, the models
             are saved in the standard Hugging Face cache directory.
           local_files_only:  If True, avoid downloading the file and return the path to the
             local cached file if it exists.
+          files: Load model files from the memory. This argument is a dictionary mapping file names
+            to file contents as file-like or bytes objects. If this is set, model_path acts as an
+            identifier for this model.
         """
         self.logger = get_logger()
 
-        if os.path.isdir(model_size_or_path):
+        tokenizer_bytes, preprocessor_bytes = None, None
+        if files:
+            model_path = model_size_or_path
+            tokenizer_bytes = files.pop("tokenizer.json", None)
+            preprocessor_bytes = files.pop("preprocessor_config.json", None)
+        elif os.path.isdir(model_size_or_path):
             model_path = model_size_or_path
         else:
             model_path = download_model(
                 model_size_or_path,
                 local_files_only=local_files_only,
                 cache_dir=download_root,
             )
@@ -133,25 +144,28 @@
         self.model = ctranslate2.models.Whisper(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
             intra_threads=cpu_threads,
             inter_threads=num_workers,
+            files=files,
+            **model_kwargs,
         )
 
         tokenizer_file = os.path.join(model_path, "tokenizer.json")
-        if os.path.isfile(tokenizer_file):
+        if tokenizer_bytes:
+            self.hf_tokenizer = tokenizers.Tokenizer.from_buffer(tokenizer_bytes)
+        elif os.path.isfile(tokenizer_file):
             self.hf_tokenizer = tokenizers.Tokenizer.from_file(tokenizer_file)
         else:
             self.hf_tokenizer = tokenizers.Tokenizer.from_pretrained(
                 "openai/whisper-tiny" + ("" if self.model.is_multilingual else ".en")
             )
-
-        self.feat_kwargs = self._get_feature_kwargs(model_path)
+        self.feat_kwargs = self._get_feature_kwargs(model_path, preprocessor_bytes)
         self.feature_extractor = FeatureExtractor(**self.feat_kwargs)
         self.num_samples_per_token = self.feature_extractor.hop_length * 2
         self.frames_per_second = (
             self.feature_extractor.sampling_rate // self.feature_extractor.hop_length
         )
         self.tokens_per_second = (
             self.feature_extractor.sampling_rate // self.num_samples_per_token
@@ -161,27 +175,29 @@
         self.max_length = 448
 
     @property
     def supported_languages(self) -> List[str]:
         """The languages supported by the model."""
         return list(_LANGUAGE_CODES) if self.model.is_multilingual else ["en"]
 
-    def _get_feature_kwargs(self, model_path) -> dict:
-        preprocessor_config_file = os.path.join(model_path, "preprocessor_config.json")
+    def _get_feature_kwargs(self, model_path, preprocessor_bytes=None) -> dict:
         config = {}
-        if os.path.isfile(preprocessor_config_file):
-            try:
-                with open(preprocessor_config_file, "r", encoding="utf-8") as json_file:
-                    config = json.load(json_file)
-                valid_keys = signature(FeatureExtractor.__init__).parameters.keys()
-                config = {k: v for k, v in config.items() if k in valid_keys}
-            except json.JSONDecodeError as e:
-                self.logger.warning(
-                    "Could not load preprocessor_config.json: %s", str(e)
-                )
+        try:
+            config_path = os.path.join(model_path, "preprocessor_config.json")
+            if preprocessor_bytes:
+                config = json.loads(preprocessor_bytes)
+            elif os.path.isfile(config_path):
+                with open(config_path, "r", encoding="utf-8") as file:
+                    config = json.load(file)
+            else:
+                return config
+            valid_keys = signature(FeatureExtractor.__init__).parameters.keys()
+            return {k: v for k, v in config.items() if k in valid_keys}
+        except json.JSONDecodeError as e:
+            self.logger.warning("Could not load preprocessor config: %s", e)
 
         return config
 
     def transcribe(
         self,
         audio: Union[str, BinaryIO, np.ndarray],
         language: Optional[str] = None,
@@ -216,14 +232,17 @@
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         vad_filter: bool = False,
         vad_parameters: Optional[Union[dict, VadOptions]] = None,
         max_new_tokens: Optional[int] = None,
         chunk_length: Optional[int] = None,
         clip_timestamps: Union[str, List[float]] = "0",
         hallucination_silence_threshold: Optional[float] = None,
+        hotwords: Optional[str] = None,
+        language_detection_threshold: Optional[float] = None,
+        language_detection_segments: int = 1,
     ) -> Tuple[Iterable[Segment], TranscriptionInfo]:
         """Transcribes an input file.
 
         Arguments:
           audio: Path to the input file (or a file-like object), or the audio waveform.
           language: The language spoken in the audio. It should be a language code such
             as "en" or "fr". If not set, the language will be detected in the first 30 seconds
@@ -271,21 +290,26 @@
             https://github.com/snakers4/silero-vad.
           vad_parameters: Dictionary of Silero VAD parameters or VadOptions class (see available
             parameters and default values in the class `VadOptions`).
           max_new_tokens: Maximum number of new tokens to generate per-chunk. If not set,
             the maximum will be set by the default max_length.
           chunk_length: The length of audio segments. If it is not None, it will overwrite the
             default chunk_length of the FeatureExtractor.
-          clip_timestamps: Union[str, List[float]]
+          clip_timestamps:
             Comma-separated list start,end,start,end,... timestamps (in seconds) of clips to
              process. The last end timestamp defaults to the end of the file.
-          hallucination_silence_threshold: Optional[float]
+             vad_filter will be ignored if clip_timestamps is used.
+          hallucination_silence_threshold:
             When word_timestamps is True, skip silent periods longer than this threshold
              (in seconds) when a possible hallucination is detected
-
+          hotwords:
+            Hotwords/hint phrases to provide the model with. Has no effect if prefix is not None.
+          language_detection_threshold: If the maximum probability of the language tokens is higher
+           than this value, the language is detected.
+          language_detection_segments: Number of segments to consider for the language detection.
         Returns:
           A tuple with:
 
             - a generator over transcribed segments
             - an instance of TranscriptionInfo
         """
         sampling_rate = self.feature_extractor.sampling_rate
@@ -296,15 +320,15 @@
         duration = audio.shape[0] / sampling_rate
         duration_after_vad = duration
 
         self.logger.info(
             "Processing audio with duration %s", format_timestamp(duration)
         )
 
-        if vad_filter:
+        if vad_filter and clip_timestamps == "0":
             if vad_parameters is None:
                 vad_parameters = VadOptions()
             elif isinstance(vad_parameters, dict):
                 vad_parameters = VadOptions(**vad_parameters)
             speech_chunks = get_speech_timestamps(audio, vad_parameters)
             audio = collect_chunks(audio, speech_chunks)
             duration_after_vad = audio.shape[0] / sampling_rate
@@ -336,23 +360,59 @@
         all_language_probs = None
 
         if language is None:
             if not self.model.is_multilingual:
                 language = "en"
                 language_probability = 1
             else:
-                segment = features[:, : self.feature_extractor.nb_max_frames]
-                encoder_output = self.encode(segment)
-                # results is a list of tuple[str, float] with language names and
-                # probabilities.
-                results = self.model.detect_language(encoder_output)[0]
-                # Parse language names to strip out markers
-                all_language_probs = [(token[2:-2], prob) for (token, prob) in results]
-                # Get top language token and probability
-                language, language_probability = all_language_probs[0]
+                if (
+                    language_detection_segments is None
+                    or language_detection_segments < 1
+                ):
+                    language_detection_segments = 1
+                seek = 0
+                detected_language_info = {}
+                content_frames = (
+                    features.shape[-1] - self.feature_extractor.nb_max_frames
+                )
+                while (
+                    seek <= content_frames
+                    and seek
+                    < self.feature_extractor.nb_max_frames * language_detection_segments
+                ):
+                    segment = features[
+                        :, seek : seek + self.feature_extractor.nb_max_frames
+                    ]
+                    encoder_output = self.encode(segment)
+                    # results is a list of tuple[str, float] with language names and
+                    # probabilities.
+                    results = self.model.detect_language(encoder_output)[0]
+                    # Parse language names to strip out markers
+                    all_language_probs = [
+                        (token[2:-2], prob) for (token, prob) in results
+                    ]
+                    # Get top language token and probability
+                    language, language_probability = all_language_probs[0]
+                    if (
+                        language_detection_threshold is None
+                        or language_probability > language_detection_threshold
+                    ):
+                        break
+                    detected_language_info.setdefault(language, []).append(
+                        language_probability
+                    )
+                    seek += segment.shape[-1]
+                else:
+                    # If no language detected for all segments, the majority vote of the highest
+                    # projected languages for all segments is used to determine the language.
+                    language = max(
+                        detected_language_info,
+                        key=lambda lang: len(detected_language_info[lang]),
+                    )
+                    language_probability = max(detected_language_info[language])
 
                 self.logger.info(
                     "Detected language '%s' with probability %.2f",
                     language,
                     language_probability,
                 )
         else:
@@ -395,14 +455,15 @@
             max_initial_timestamp=max_initial_timestamp,
             word_timestamps=word_timestamps,
             prepend_punctuations=prepend_punctuations,
             append_punctuations=append_punctuations,
             max_new_tokens=max_new_tokens,
             clip_timestamps=clip_timestamps,
             hallucination_silence_threshold=hallucination_silence_threshold,
+            hotwords=hotwords,
         )
 
         segments = self.generate_segments(features, tokenizer, options, encoder_output)
 
         if speech_chunks:
             segments = restore_speech_timestamps(segments, speech_chunks, sampling_rate)
 
@@ -501,14 +562,15 @@
 
             previous_tokens = all_tokens[prompt_reset_since:]
             prompt = self.get_prompt(
                 tokenizer,
                 previous_tokens,
                 without_timestamps=options.without_timestamps,
                 prefix=options.prefix if seek == 0 else None,
+                hotwords=options.hotwords,
             )
 
             if seek > 0 or encoder_output is None:
                 encoder_output = self.encode(segment)
 
             (
                 result,
@@ -893,20 +955,27 @@
 
     def get_prompt(
         self,
         tokenizer: Tokenizer,
         previous_tokens: List[int],
         without_timestamps: bool = False,
         prefix: Optional[str] = None,
+        hotwords: Optional[str] = None,
     ) -> List[int]:
         prompt = []
 
-        if previous_tokens:
+        if previous_tokens or (hotwords and not prefix):
             prompt.append(tokenizer.sot_prev)
-            prompt.extend(previous_tokens[-(self.max_length // 2 - 1) :])
+            if hotwords and not prefix:
+                hotwords_tokens = tokenizer.encode(" " + hotwords.strip())
+                if len(hotwords_tokens) >= self.max_length // 2:
+                    hotwords_tokens = hotwords_tokens[: self.max_length // 2 - 1]
+                prompt.extend(hotwords_tokens)
+            if previous_tokens:
+                prompt.extend(previous_tokens[-(self.max_length // 2 - 1) :])
 
         prompt.extend(tokenizer.sot_sequence)
 
         if without_timestamps:
             prompt.append(tokenizer.no_timestamps)
 
         if prefix:
```

### Comparing `faster-whisper-1.0.1/faster_whisper/utils.py` & `faster-whisper-1.0.2/faster_whisper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "large-v1": "Systran/faster-whisper-large-v1",
     "large-v2": "Systran/faster-whisper-large-v2",
     "large-v3": "Systran/faster-whisper-large-v3",
     "large": "Systran/faster-whisper-large-v3",
     "distil-large-v2": "Systran/faster-distil-whisper-large-v2",
     "distil-medium.en": "Systran/faster-distil-whisper-medium.en",
     "distil-small.en": "Systran/faster-distil-whisper-small.en",
+    "distil-large-v3": "Systran/faster-distil-whisper-large-v3",
 }
 
 
 def available_models() -> List[str]:
     """Returns the names of available models."""
     return list(_MODELS.keys())
 
@@ -48,15 +49,15 @@
     output_dir: Optional[str] = None,
     local_files_only: bool = False,
     cache_dir: Optional[str] = None,
 ):
     """Downloads a CTranslate2 Whisper model from the Hugging Face Hub.
 
     Args:
-      size_or_id: Size of the model to download from https://huggingface.co/guillaumekln
+      size_or_id: Size of the model to download from https://huggingface.co/Systran
         (tiny, tiny.en, base, base.en, small, small.en medium, medium.en, large-v1, large-v2,
         large-v3, large), or a CTranslate2-converted model ID from the Hugging Face Hub
         (e.g. Systran/faster-whisper-large-v3).
       output_dir: Directory where the model should be saved. If not set, the model is saved in
         the cache directory.
       local_files_only:  If True, avoid downloading the file and return the path to the local
         cached file if it exists.
```

### Comparing `faster-whisper-1.0.1/faster_whisper/vad.py` & `faster-whisper-1.0.2/faster_whisper/vad.py`

 * *Files identical despite different names*

### Comparing `faster-whisper-1.0.1/faster_whisper.egg-info/PKG-INFO` & `faster-whisper-1.0.2/faster_whisper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: faster-whisper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Faster Whisper transcription with CTranslate2
-Home-page: https://github.com/guillaumekln/faster-whisper
+Home-page: https://github.com/SYSTRAN/faster-whisper
 Author: Guillaume Klein
 License: MIT
-Description: [![CI](https://github.com/guillaumekln/faster-whisper/workflows/CI/badge.svg)](https://github.com/guillaumekln/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
+Description: [![CI](https://github.com/SYSTRAN/faster-whisper/workflows/CI/badge.svg)](https://github.com/SYSTRAN/faster-whisper/actions?query=workflow%3ACI) [![PyPI version](https://badge.fury.io/py/faster-whisper.svg)](https://badge.fury.io/py/faster-whisper)
         
         # Faster Whisper transcription with CTranslate2
         
         **faster-whisper** is a reimplementation of OpenAI's Whisper model using [CTranslate2](https://github.com/OpenNMT/CTranslate2/), which is a fast inference engine for Transformer models.
         
         This implementation is up to 4 times faster than [openai/whisper](https://github.com/openai/whisper) for the same accuracy while using less memory. The efficiency can be further improved with 8-bit quantization on both CPU and GPU.
         
@@ -17,15 +17,15 @@
         
         ### Whisper
         
         For reference, here's the time and memory usage that are required to transcribe [**13 minutes**](https://www.youtube.com/watch?v=0u7tTptBo9I) of audio using different implementations:
         
         * [openai/whisper](https://github.com/openai/whisper)@[6dea21fd](https://github.com/openai/whisper/commit/6dea21fd7f7253bfe450f1e2512a0fe47ee2d258)
         * [whisper.cpp](https://github.com/ggerganov/whisper.cpp)@[3b010f9](https://github.com/ggerganov/whisper.cpp/commit/3b010f9bed9a6068609e9faf52383aea792b0362)
-        * [faster-whisper](https://github.com/guillaumekln/faster-whisper)@[cce6b53e](https://github.com/guillaumekln/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
+        * [faster-whisper](https://github.com/SYSTRAN/faster-whisper)@[cce6b53e](https://github.com/SYSTRAN/faster-whisper/commit/cce6b53e4554f71172dad188c45f10fb100f6e3e)
         
         ### Large-v2 model on GPU
         
         | Implementation | Precision | Beam size | Time | Max. GPU memory | Max. CPU memory |
         | --- | --- | --- | --- | --- | --- |
         | openai/whisper | fp16 | 5 | 4m30s | 11325MB | 9439MB |
         | faster-whisper | fp16 | 5 | 54s | 4755MB | 3244MB |
@@ -78,36 +78,43 @@
         
         Unlike openai-whisper, FFmpeg does **not** need to be installed on the system. The audio is decoded with the Python library [PyAV](https://github.com/PyAV-Org/PyAV) which bundles the FFmpeg libraries in its package.
         
         ### GPU
         
         GPU execution requires the following NVIDIA libraries to be installed:
         
-        * [cuBLAS for CUDA 11](https://developer.nvidia.com/cublas)
-        * [cuDNN 8 for CUDA 11](https://developer.nvidia.com/cudnn)
+        * [cuBLAS for CUDA 12](https://developer.nvidia.com/cublas)
+        * [cuDNN 8 for CUDA 12](https://developer.nvidia.com/cudnn)
         
-        There are multiple ways to install these libraries. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below.
+        **Note**: Latest versions of `ctranslate2` support CUDA 12 only. For CUDA 11, the current workaround is downgrading to the `3.24.0` version of `ctranslate2` (This can be done with `pip install --force-reinsall ctranslate2==3.24.0` or specifying the version in a `requirements.txt`).
+        
+        There are multiple ways to install the NVIDIA libraries mentioned above. The recommended way is described in the official NVIDIA documentation, but we also suggest other installation methods below. 
         
         <details>
         <summary>Other installation methods (click to expand)</summary>
         
+        
+        **Note:** For all these methods below, keep in mind the above note regarding CUDA versions. Depending on your setup, you may need to install the _CUDA 11_ versions of libraries that correspond to the CUDA 12 libraries listed in the instructions below.
+        
         #### Use Docker
         
-        The libraries are installed in this official NVIDIA Docker image: `nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu22.04`.
+        The libraries (cuBLAS, cuDNN) are installed in these official NVIDIA CUDA Docker images: `nvidia/cuda:12.0.0-runtime-ubuntu20.04` or `nvidia/cuda:12.0.0-runtime-ubuntu22.04`.
         
         #### Install with `pip` (Linux only)
         
         On Linux these libraries can be installed with `pip`. Note that `LD_LIBRARY_PATH` must be set before launching Python.
         
         ```bash
-        pip install nvidia-cublas-cu11 nvidia-cudnn-cu11
+        pip install nvidia-cublas-cu12 nvidia-cudnn-cu12
         
         export LD_LIBRARY_PATH=`python3 -c 'import os; import nvidia.cublas.lib; import nvidia.cudnn.lib; print(os.path.dirname(nvidia.cublas.lib.__file__) + ":" + os.path.dirname(nvidia.cudnn.lib.__file__))'`
         ```
         
+        **Note**: Version 9+ of `nvidia-cudnn-cu12` appears to cause issues due its reliance on cuDNN 9 (Faster-Whisper does not currently support cuDNN 9). Ensure your version of the Python package is for cuDNN 8.
+        
         #### Download the libraries from Purfview's repository (Windows & Linux)
         
         Purfview's [whisper-standalone-win](https://github.com/Purfview/whisper-standalone-win) provides the required NVIDIA libraries for Windows & Linux in a [single archive](https://github.com/Purfview/whisper-standalone-win/releases/tag/libs). Decompress the archive and place the libraries in a directory included in the `PATH`.
         
         </details>
         
         ## Installation
@@ -120,21 +127,21 @@
         
         <details>
         <summary>Other installation methods (click to expand)</summary>
         
         ### Install the master branch
         
         ```bash
-        pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/refs/heads/master.tar.gz"
+        pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/refs/heads/master.tar.gz"
         ```
         
         ### Install a specific commit
         
         ```bash
-        pip install --force-reinstall "faster-whisper @ https://github.com/guillaumekln/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
+        pip install --force-reinstall "faster-whisper @ https://github.com/SYSTRAN/faster-whisper/archive/a4f1cc8f11433e454c3934442b5e1a4ed5e865c3.tar.gz"
         ```
         
         </details>
         
         ## Usage
         
         ### Faster-whisper
@@ -162,26 +169,33 @@
         
         **Warning:** `segments` is a *generator* so the transcription only starts when you iterate over it. The transcription can be run to completion by gathering the segments in a list or a `for` loop:
         
         ```python
         segments, _ = model.transcribe("audio.mp3")
         segments = list(segments)  # The transcription will actually run here.
         ```
-        ### Faster-distil-whisper
-        For usage of `faster-distil-whisper`, please refer to: https://github.com/guillaumekln/faster-whisper/issues/533
+        ### Faster Distil-Whisper
+        
+        The Distil-Whisper checkpoints are compatible with the Faster-Whisper package. In particular, the latest [distil-large-v3](https://huggingface.co/distil-whisper/distil-large-v3)
+        checkpoint is intrinsically designed to work with the Faster-Whisper transcription algorithm. The following code snippet 
+        demonstrates how to run inference with distil-large-v3 on a specified audio file:
         
         ```python
-        model_size = "distil-large-v2"
-        # model_size = "distil-medium.en"
+        from faster_whisper import WhisperModel
+        
+        model_size = "distil-large-v3"
+        
         model = WhisperModel(model_size, device="cuda", compute_type="float16")
-        segments, info = model.transcribe("audio.mp3", beam_size=5, 
-            language="en", max_new_tokens=128, condition_on_previous_text=False)
+        segments, info = model.transcribe("audio.mp3", beam_size=5, language="en", condition_on_previous_text=False)
         
+        for segment in segments:
+            print("[%.2fs -> %.2fs] %s" % (segment.start, segment.end, segment.text))
         ```
-        NOTE: Empirically, `condition_on_previous_text=True` will degrade the performance of `faster-distil-whisper` for long audio. Degradation on the first chunk was observed with `initial_prompt` too.
+        
+        For more information about the distil-large-v3 model, refer to the original [model card](https://huggingface.co/distil-whisper/distil-large-v3).
         
         ### Word-level timestamps
         
         ```python
         segments, _ = model.transcribe("audio.mp3", word_timestamps=True)
         
         for segment in segments:
@@ -193,15 +207,15 @@
         
         The library integrates the [Silero VAD](https://github.com/snakers4/silero-vad) model to filter out parts of the audio without speech:
         
         ```python
         segments, _ = model.transcribe("audio.mp3", vad_filter=True)
         ```
         
-        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
+        The default behavior is conservative and only removes silence longer than 2 seconds. See the available VAD parameters and default values in the [source code](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/vad.py). They can be customized with the dictionary argument `vad_parameters`:
         
         ```python
         segments, _ = model.transcribe(
             "audio.mp3",
             vad_filter=True,
             vad_parameters=dict(min_silence_duration_ms=500),
         )
@@ -216,15 +230,15 @@
         
         logging.basicConfig()
         logging.getLogger("faster_whisper").setLevel(logging.DEBUG)
         ```
         
         ### Going further
         
-        See more model and transcription options in the [`WhisperModel`](https://github.com/guillaumekln/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
+        See more model and transcription options in the [`WhisperModel`](https://github.com/SYSTRAN/faster-whisper/blob/master/faster_whisper/transcribe.py) class implementation.
         
         ## Community integrations
         
         Here is a non exhaustive list of open-source projects using faster-whisper. Feel free to add your project to the list!
         
         
         * [WhisperX](https://github.com/m-bain/whisperX) is an award-winning Python library that offers speaker diarization and accurate word-level timestamps using wav2vec2 alignment
```

### Comparing `faster-whisper-1.0.1/faster_whisper.egg-info/SOURCES.txt` & `faster-whisper-1.0.2/faster_whisper.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 faster_whisper/vad.py
 faster_whisper/version.py
 faster_whisper.egg-info/PKG-INFO
 faster_whisper.egg-info/SOURCES.txt
 faster_whisper.egg-info/dependency_links.txt
 faster_whisper.egg-info/requires.txt
 faster_whisper.egg-info/top_level.txt
+faster_whisper/assets/__init__.py
 faster_whisper/assets/silero_vad.onnx
```

### Comparing `faster-whisper-1.0.1/setup.py` & `faster-whisper-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="faster-whisper",
     version=get_project_version(),
     license="MIT",
     description="Faster Whisper transcription with CTranslate2",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Guillaume Klein",
-    url="https://github.com/guillaumekln/faster-whisper",
+    url="https://github.com/SYSTRAN/faster-whisper",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
```

