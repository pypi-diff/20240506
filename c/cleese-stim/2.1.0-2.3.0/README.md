# Comparing `tmp/cleese_stim-2.1.0.tar.gz` & `tmp/cleese_stim-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleese_stim-2.1.0.tar", last modified: Wed May  1 06:04:05 2024, max compression
+gzip compressed data, was "cleese_stim-2.3.0.tar", last modified: Sun May  5 17:52:54 2024, max compression
```

## Comparing `cleese_stim-2.1.0.tar` & `cleese_stim-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.339438 cleese_stim-2.1.0/cleese_stim/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/cleese.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/engines/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/audio_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/bpf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/audio_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim/third_party/mls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10362 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/mls/interp_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/cleese_stim/third_party/yin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:04:05.343438 cleese_stim-2.1.0/cleese_stim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 06:04:05.000000 cleese_stim-2.1.0/cleese_stim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 06:04:05.347438 cleese_stim-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:03:55.000000 cleese_stim-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.930997 cleese_stim-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.906998 cleese_stim-2.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/.github/workflows/version_update.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-05 17:52:54.930997 cleese_stim-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/cleese_stim/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/cleese.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/cleese_stim/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/cleese_stim/engines/face_warp/
+-rw-r--r--   0 runner    (1001) docker     (127)    20360 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/face_warp/face_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/audio_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/bpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.910997 cleese_stim-2.3.0/cleese_stim/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/audio_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.914998 cleese_stim-2.3.0/cleese_stim/third_party/mls/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/img_utils_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/interp_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/mls/requirments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/cleese_stim/third_party/yin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.926998 cleese_stim-2.3.0/cleese_stim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 17:52:54.000000 cleese_stim-2.3.0/cleese_stim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.914998 cleese_stim-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.914998 cleese_stim-2.3.0/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/about.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.914998 cleese_stim-2.3.0/docs/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.914998 cleese_stim-2.3.0/docs/docs/api/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/api/configs/cleese-face-warp.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/api/configs/cleese-phase-vocoder.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/api/face-warp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/api/general.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/api/phase-vocoder.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.918998 cleese_stim-2.3.0/docs/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   748751 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/canonical_face_model_uv_visualization.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77898 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/dlib_68_landmarks.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/ramps_n.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/ramps_s.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28202 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/shift.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/silly-walk.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    24936 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20884 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_5.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22172 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_6.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33383 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_7.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33556 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/speech_tutorial_8.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/square_n.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/images/square_s.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.918998 cleese_stim-2.3.0/docs/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/javascripts/katex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.918998 cleese_stim-2.3.0/docs/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.918998 cleese_stim-2.3.0/docs/docs/tutorials/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/configs/chained_pitch_stretch.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/configs/random_lips.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/configs/random_pitch_profile.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/configs/random_speed_profile.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.922998 cleese_stim-2.3.0/docs/docs/tutorials/dfm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/dfm/monalisa.landmarks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/dfm/monalisa.random.dfmxy
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/dfm/smile.dfm
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/face.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.922998 cleese_stim-2.3.0/docs/docs/tutorials/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)   150729 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/pics/monalisa.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   121239 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/pics/monalisa_transformed.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/pics/monalisa_transformed_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   115052 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/pics/monalisa_transformed_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   125112 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/pics/monalisa_transformed_4.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 17:52:54.926998 cleese_stim-2.3.0/docs/docs/tutorials/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)   283584 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/female_anniversaire_isochrone.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   399404 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/female_anniversaire_isochrone_transformed.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   348204 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/female_anniversaire_isochrone_transformed_2.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_1.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_2.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_3.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37640 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_4.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    56364 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_5.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    52268 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_6.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    40492 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_7.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    50732 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_flattened_transformed_8.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    37932 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/male_vraiment_original.wav
+-rw-r--r--   0 runner    (1001) docker     (127)  1103516 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/sounds/variation_pitch.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/docs/tutorials/speech.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-05 17:52:54.930997 cleese_stim-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 17:52:49.000000 cleese_stim-2.3.0/setup.py
```

### Comparing `cleese_stim-2.1.0/LICENSE` & `cleese_stim-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/PKG-INFO` & `cleese_stim-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleese_stim
-Version: 2.1.0
+Version: 2.3.0
 Summary: Audio and visual stimuli generation tool
 Home-page: https://github.com/neuro-team-femto/cleese
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/neuro-team-femto/cleese/issues
 Keywords: sound manipulation,phase vocoder
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 License-File: LICENSE
 Requires-Dist: mediapipe
 Requires-Dist: msvc-runtime; platform_system == "Windows"
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tomli
 
-![cleese](tutorial/pics/silly-walk.jpg)
+![cleese](docs/docs/images/silly-walk.jpg)
 
 CLEESE ("Ministry of Silly Speech") is a sound and image manipulation tool
 designed to generate an infinite number of possible stimuli; be it
 natural-sounding expressive variations around an original speech recording, or
 variations on the expression of a human face.
 
 More precisely, CLEESE is currently composed of two engines: `PhaseVocoder` and
```

### Comparing `cleese_stim-2.1.0/README.md` & `cleese_stim-2.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![cleese](tutorial/pics/silly-walk.jpg)
+![cleese](docs/docs/images/silly-walk.jpg)
 
 CLEESE ("Ministry of Silly Speech") is a sound and image manipulation tool
 designed to generate an infinite number of possible stimuli; be it
 natural-sounding expressive variations around an original speech recording, or
 variations on the expression of a human face.
 
 More precisely, CLEESE is currently composed of two engines: `PhaseVocoder` and
```

### Comparing `cleese_stim-2.1.0/cleese_stim/cleese.py` & `cleese_stim-2.3.0/cleese_stim/cleese.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/engines/engine.py` & `cleese_stim-2.3.0/cleese_stim/engines/engine.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/audio_engine.py` & `cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/audio_engine.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/bpf.py` & `cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/bpf.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,30 @@
             BPF[i, 0] = BPFtime[i]
             BPF[i, 1] = config["eq"]["band"]["count"]
             BPF[i, 2::2] = eqFreqVec
             BPF[i, 3::2] = BPFval[:, i]
 
     return BPF
 
+def create_BPF_header(tr, config): 
+    ''' 
+        returns a str that's the header for the file destined to store BPF values
+    '''
+
+    # for pitch, stretch and gain, BPF file is two-columned in the form time,value
+    if tr in ["pitch", "stretch", "gain"]:
+        header = "time,%s"%tr
+    # for eq, BPF file is in the form: time numBands freq1 ampl1 freq2 ampl2 ...
+    elif tr == "eq":
+        num_bands = config["eq"]["band"]["count"] + 1 # one more cutoff frequency than bands
+        header = "time,n_channels"
+        for band in range(0, num_bands):
+            header += ",freq_%d,ampl_%d"%(band,band)
+    return header
+
 
 def createBPFtimeVec(duration, local_pars, timeVec=None):
 
     BPFtime = np.array([0])
     numPoints = 1
     endOnTrans = 0
```

### Comparing `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py` & `cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/phase_vocoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 import scipy.signal as sig
 import time
 import shutil
 
 from .bpf import (
         createBPFtimeVec,
         createBPFfreqs,
-        createBPF,)
+        createBPF,
+        create_BPF_header)
 from .audio_engine import (
         stft,
         istft,
         istft_resamp,
         phaseVocoder_varHop,)
 from ..engine import Engine
 from ...cleese import log, load_config
@@ -46,14 +47,20 @@
                 sample_format=None, timeVec=None,
                 file_output=False):
 
         doCreateBPF = False
         if BPF is None:
             doCreateBPF = True
 
+        try:
+            BPF_EXT = config["main"]["param_ext"]
+        except KeyError as e:
+            BPF_EXT = '.txt' # default bpf extension
+  
+
         if not sample_rate:
             log("ERROR: missing sample rate")
             return
 
         if file_output:
             if not sample_rate or not sample_format:
                 log("ERROR: missing sample format")
@@ -142,16 +149,18 @@
                     BPF = createBPF(tr, config, BPFtime, numPoints,
                                     endOnTrans, eqFreqVec)
 
                 # export BPF as text file
                 if file_output:
                     currBPFfile = os.path.join(
                             config["main"]['currOutPath'],
-                            inFileNoExt+'.'+currFileNo+'.'+currTrString+'_BPF.txt')
-                    np.savetxt(currBPFfile, BPF, '%.8f')
+                            inFileNoExt+'.'+currFileNo+'.'+currTrString+BPF_EXT)
+                    BPF_header = create_BPF_header(tr, config)
+
+                    np.savetxt(currBPFfile, BPF, '%.8f', delimiter = ',', header = BPF_header, comments='')
 
                     if t == 0:
                         currOutFile.append(os.path.join(
                                 config["main"]['currOutPath'],
                                 inFileNoExt+'.'+currFileNo+'.'+currTrString+'.wav'))
                     else:
                         currOutFile[i] = os.path.join(
```

### Comparing `cleese_stim-2.1.0/cleese_stim/engines/phase_vocoder/utils.py` & `cleese_stim-2.3.0/cleese_stim/engines/phase_vocoder/utils.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/audio_processing.py` & `cleese_stim-2.3.0/cleese_stim/third_party/audio_processing.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/mls/demo.py` & `cleese_stim-2.3.0/cleese_stim/third_party/mls/demo.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils.py` & `cleese_stim-2.3.0/cleese_stim/third_party/mls/img_utils.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/mls/img_utils_pytorch.py` & `cleese_stim-2.3.0/cleese_stim/third_party/mls/img_utils_pytorch.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/mls/interp_torch.py` & `cleese_stim-2.3.0/cleese_stim/third_party/mls/interp_torch.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim/third_party/yin.py` & `cleese_stim-2.3.0/cleese_stim/third_party/yin.py`

 * *Files identical despite different names*

### Comparing `cleese_stim-2.1.0/cleese_stim.egg-info/PKG-INFO` & `cleese_stim-2.3.0/cleese_stim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleese_stim
-Version: 2.1.0
+Version: 2.3.0
 Summary: Audio and visual stimuli generation tool
 Home-page: https://github.com/neuro-team-femto/cleese
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/neuro-team-femto/cleese/issues
 Keywords: sound manipulation,phase vocoder
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 License-File: LICENSE
 Requires-Dist: mediapipe
 Requires-Dist: msvc-runtime; platform_system == "Windows"
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tomli
 
-![cleese](tutorial/pics/silly-walk.jpg)
+![cleese](docs/docs/images/silly-walk.jpg)
 
 CLEESE ("Ministry of Silly Speech") is a sound and image manipulation tool
 designed to generate an infinite number of possible stimuli; be it
 natural-sounding expressive variations around an original speech recording, or
 variations on the expression of a human face.
 
 More precisely, CLEESE is currently composed of two engines: `PhaseVocoder` and
```

### Comparing `cleese_stim-2.1.0/setup.cfg` & `cleese_stim-2.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = cleese_stim
-version = 2.1.0
 description = Audio and visual stimuli generation tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sound manipulation, phase vocoder
 license = MIT License
 url = https://github.com/neuro-team-femto/cleese
 project_urls =
```

