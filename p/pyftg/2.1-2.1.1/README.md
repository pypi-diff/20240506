# Comparing `tmp/pyftg-2.1.tar.gz` & `tmp/pyftg-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftg-2.1.tar", last modified: Sat May  4 15:51:26 2024, max compression
+gzip compressed data, was "pyftg-2.1.1.tar", last modified: Mon May  6 07:36:32 2024, max compression
```

## Comparing `pyftg-2.1.tar` & `pyftg-2.1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.508325 pyftg-2.1/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1072 2024-02-18 17:20:43.000000 pyftg-2.1/LICENSE
--rw-r--r--   0 staciiaz   (501) staff       (20)     1634 2024-05-04 15:51:26.508158 pyftg-2.1/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)     1031 2024-04-24 09:41:02.000000 pyftg-2.1/README.md
--rw-r--r--   0 staciiaz   (501) staff       (20)      573 2024-05-04 15:51:19.000000 pyftg-2.1/pyproject.toml
--rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-05-04 15:51:26.508359 pyftg-2.1/setup.cfg
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.502121 pyftg-2.1/src/
--rw-r--r--   0 staciiaz   (501) staff       (20)     3407 2024-04-13 17:15:22.000000 pyftg-2.1/src/DisplayInfo.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1858 2024-04-10 19:07:27.000000 pyftg-2.1/src/KickAI.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1525 2023-10-08 11:53:34.000000 pyftg-2.1/src/Main_Capture.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     3230 2023-10-08 07:42:51.000000 pyftg-2.1/src/Main_Collector.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1643 2023-10-17 07:13:15.000000 pyftg-2.1/src/Main_FDG.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1175 2024-04-11 13:38:52.000000 pyftg-2.1/src/Main_PyAIvsPyAI.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1134 2024-04-11 13:51:53.000000 pyftg-2.1/src/Main_SinglePyAI.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      864 2024-04-24 09:42:13.000000 pyftg-2.1/src/Main_SoundAI.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      765 2024-04-24 09:42:13.000000 pyftg-2.1/src/TestSoundAI.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.502230 pyftg-2.1/src/pyftg/
--rw-r--r--   0 staciiaz   (501) staff       (20)      381 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/__init__.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503151 pyftg-2.1/src/pyftg/aiinterface/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1237 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/aiinterface/ai_interface.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     6231 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/aiinterface/command_center.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      757 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/aiinterface/soundgenai_interface.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.500249 pyftg-2.1/src/pyftg/grpc/
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503364 pyftg-2.1/src/pyftg/grpc/asyncio/
--rw-r--r--   0 staciiaz   (501) staff       (20)     2805 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/grpc/asyncio/ai_controller.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2568 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/asyncio/gateway.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503834 pyftg-2.1/src/pyftg/grpc/threading/
--rw-r--r--   0 staciiaz   (501) staff       (20)     2742 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/grpc/threading/ai_controller.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2348 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2508 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/observer_gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      603 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/grpc/threading/observer_handler.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.503946 pyftg-2.1/src/pyftg/interfaces/
--rw-r--r--   0 staciiaz   (501) staff       (20)      541 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/interfaces/async_gateway.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.505140 pyftg-2.1/src/pyftg/models/
--rw-r--r--   0 staciiaz   (501) staff       (20)     5349 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/attack_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1346 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/audio_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/models/base_model.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     4873 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/character_data.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.505958 pyftg-2.1/src/pyftg/models/enums/
--rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1847 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/action.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      121 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/data_flag.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      153 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/enums/flag.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1111 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/int_action.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      105 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/int_state.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/enums/state.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      100 2024-04-11 13:33:38.000000 pyftg-2.1/src/pyftg/models/enums/status_code.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      953 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/fft_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2849 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/models/frame_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1482 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/game_data.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      990 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/hit_area.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1427 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/key.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     1136 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/models/round_result.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      851 2024-04-13 17:13:16.000000 pyftg-2.1/src/pyftg/models/screen_data.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.506730 pyftg-2.1/src/pyftg/protoc/
--rw-r--r--   0 staciiaz   (501) staff       (20)        0 2023-04-11 11:53:26.000000 pyftg-2.1/src/pyftg/protoc/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/__init__.pyi
--rw-r--r--   0 staciiaz   (501) staff       (20)     3286 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/enum_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/enum_pb2_grpc.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     5662 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/message_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/message_pb2_grpc.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     4602 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/service_pb2.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     6775 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/protoc/service_pb2_grpc.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.500735 pyftg-2.1/src/pyftg/socket/
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507053 pyftg-2.1/src/pyftg/socket/asyncio/
--rw-r--r--   0 staciiaz   (501) staff       (20)     3144 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/socket/asyncio/ai_controller.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2872 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/asyncio/gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2649 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/socket/asyncio/generative_sound_gateway.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507251 pyftg-2.1/src/pyftg/socket/threading/
--rw-r--r--   0 staciiaz   (501) staff       (20)     3133 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/socket/threading/ai_controller.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     2763 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/threading/gateway.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507456 pyftg-2.1/src/pyftg/socket/utils/
--rw-r--r--   0 staciiaz   (501) staff       (20)      642 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/utils/asyncio.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      508 2024-04-12 17:24:08.000000 pyftg-2.1/src/pyftg/socket/utils/threading.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507854 pyftg-2.1/src/pyftg/utils/
--rw-r--r--   0 staciiaz   (501) staff       (20)      417 2024-05-04 15:41:21.000000 pyftg-2.1/src/pyftg/utils/gateway.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      430 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/utils/logging.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      258 2024-04-24 09:41:02.000000 pyftg-2.1/src/pyftg/utils/protobuf.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      252 2024-04-10 19:05:46.000000 pyftg-2.1/src/pyftg/utils/resource_loader.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:51:26.507995 pyftg-2.1/src/pyftg.egg-info/
--rw-r--r--   0 staciiaz   (501) staff       (20)     1634 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)     2073 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/SOURCES.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/dependency_links.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)       53 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/requires.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)      119 2024-05-04 15:51:26.000000 pyftg-2.1/src/pyftg.egg-info/top_level.txt
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.679302 pyftg-2.1.1/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1072 2024-02-18 17:20:43.000000 pyftg-2.1.1/LICENSE
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1378 2024-05-06 07:36:32.679102 pyftg-2.1.1/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)      773 2024-05-06 07:36:19.000000 pyftg-2.1.1/README.md
+-rw-r--r--   0 staciiaz   (501) staff       (20)      575 2024-05-06 07:36:12.000000 pyftg-2.1.1/pyproject.toml
+-rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-05-06 07:36:32.679337 pyftg-2.1.1/setup.cfg
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.672346 pyftg-2.1.1/src/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3407 2024-04-13 17:15:22.000000 pyftg-2.1.1/src/DisplayInfo.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1858 2024-04-10 19:07:27.000000 pyftg-2.1.1/src/KickAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1525 2023-10-08 11:53:34.000000 pyftg-2.1.1/src/Main_Capture.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3230 2023-10-08 07:42:51.000000 pyftg-2.1.1/src/Main_Collector.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1643 2023-10-17 07:13:15.000000 pyftg-2.1.1/src/Main_FDG.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1175 2024-04-11 13:38:52.000000 pyftg-2.1.1/src/Main_PyAIvsPyAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1134 2024-04-11 13:51:53.000000 pyftg-2.1.1/src/Main_SinglePyAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      864 2024-04-24 09:42:13.000000 pyftg-2.1.1/src/Main_SoundAI.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      765 2024-04-24 09:42:13.000000 pyftg-2.1.1/src/TestSoundAI.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.672474 pyftg-2.1.1/src/pyftg/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      381 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/__init__.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.673482 pyftg-2.1.1/src/pyftg/aiinterface/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1237 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/aiinterface/ai_interface.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6231 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/aiinterface/command_center.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      757 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/aiinterface/soundgenai_interface.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.670228 pyftg-2.1.1/src/pyftg/grpc/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.673740 pyftg-2.1.1/src/pyftg/grpc/asyncio/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2805 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/asyncio/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2568 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/asyncio/gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.674215 pyftg-2.1.1/src/pyftg/grpc/threading/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2742 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/threading/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2348 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/threading/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2508 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/threading/observer_gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      603 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/grpc/threading/observer_handler.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.674344 pyftg-2.1.1/src/pyftg/interfaces/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      541 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/interfaces/async_gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.675664 pyftg-2.1.1/src/pyftg/models/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     5349 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/attack_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1346 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/audio_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/base_model.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     4873 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/character_data.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.676629 pyftg-2.1.1/src/pyftg/models/enums/
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/__init__.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1847 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/action.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      121 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/data_flag.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      153 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/flag.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1111 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/int_action.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      105 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/int_state.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      346 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/state.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      100 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/enums/status_code.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      953 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/fft_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2849 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/frame_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1482 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/game_data.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      990 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/hit_area.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1427 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/key.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1136 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/round_result.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      851 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/models/screen_data.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.677512 pyftg-2.1.1/src/pyftg/protoc/
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2023-04-11 11:53:26.000000 pyftg-2.1.1/src/pyftg/protoc/__init__.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)        0 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/__init__.pyi
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3286 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/enum_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/enum_pb2_grpc.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     5662 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/message_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)       87 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/message_pb2_grpc.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     4602 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/service_pb2.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6775 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/protoc/service_pb2_grpc.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.670705 pyftg-2.1.1/src/pyftg/socket/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.677852 pyftg-2.1.1/src/pyftg/socket/asyncio/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3144 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/asyncio/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2872 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/asyncio/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2649 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/asyncio/generative_sound_gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.678071 pyftg-2.1.1/src/pyftg/socket/threading/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3133 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/threading/ai_controller.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2763 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/threading/gateway.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.678315 pyftg-2.1.1/src/pyftg/socket/utils/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      642 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/utils/asyncio.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      508 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/socket/utils/threading.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.678760 pyftg-2.1.1/src/pyftg/utils/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      417 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/utils/gateway.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      430 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/utils/logging.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      258 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/utils/protobuf.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      252 2024-05-04 17:46:05.000000 pyftg-2.1.1/src/pyftg/utils/resource_loader.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:36:32.678920 pyftg-2.1.1/src/pyftg.egg-info/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1378 2024-05-06 07:36:32.000000 pyftg-2.1.1/src/pyftg.egg-info/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)     2073 2024-05-06 07:36:32.000000 pyftg-2.1.1/src/pyftg.egg-info/SOURCES.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-05-06 07:36:32.000000 pyftg-2.1.1/src/pyftg.egg-info/dependency_links.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)       53 2024-05-06 07:36:32.000000 pyftg-2.1.1/src/pyftg.egg-info/requires.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)      119 2024-05-06 07:36:32.000000 pyftg-2.1.1/src/pyftg.egg-info/top_level.txt
```

### Comparing `pyftg-2.1/LICENSE` & `pyftg-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/PKG-INFO` & `pyftg-2.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftg
-Version: 2.1
+Version: 2.1.1
 Summary: An interface for implementing python AI in DareFightingICE
 Author: TeamFightingICE
 Project-URL: Homepage, https://github.com/TeamFightingICE/pyftg
 Project-URL: Issues, https://github.com/TeamFightingICE/pyftg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,14 @@
 Requires-Dist: grpcio-tools~=1.62.1
 Requires-Dist: protobuf~=4.25.3
 
 # pyftg
 
 An interface for implementing python AI in DareFightingICE
 
-**Note:** Version 2.0 is the latest version compatible with the legacy [FightingICE](https://github.com/TeamFightingICE/FightingICE). Version 2.1 and later will only support [DareFightingICE-Unity](https://github.com/TeamFightingICE/DareFightingICE-Unity).
-
 First, install `pyftg` with pip.
 ```
 pip install pyftg
 ```
 
 Initiate `Gateway` for connecting to DareFightingICE platform.
 ```
```

### Comparing `pyftg-2.1/README.md` & `pyftg-2.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # pyftg
 
 An interface for implementing python AI in DareFightingICE
 
-**Note:** Version 2.0 is the latest version compatible with the legacy [FightingICE](https://github.com/TeamFightingICE/FightingICE). Version 2.1 and later will only support [DareFightingICE-Unity](https://github.com/TeamFightingICE/DareFightingICE-Unity).
-
 First, install `pyftg` with pip.
 ```
 pip install pyftg
 ```
 
 Initiate `Gateway` for connecting to DareFightingICE platform.
 ```
```

### Comparing `pyftg-2.1/pyproject.toml` & `pyftg-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyftg"
-version = "2.1"
+version = "2.1.1"
 authors = [
   { name="TeamFightingICE" },
 ]
 description = "An interface for implementing python AI in DareFightingICE"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyftg-2.1/src/DisplayInfo.py` & `pyftg-2.1.1/src/DisplayInfo.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/KickAI.py` & `pyftg-2.1.1/src/KickAI.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_Capture.py` & `pyftg-2.1.1/src/Main_Capture.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_Collector.py` & `pyftg-2.1.1/src/Main_Collector.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_FDG.py` & `pyftg-2.1.1/src/Main_FDG.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_PyAIvsPyAI.py` & `pyftg-2.1.1/src/Main_PyAIvsPyAI.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_SinglePyAI.py` & `pyftg-2.1.1/src/Main_SinglePyAI.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/Main_SoundAI.py` & `pyftg-2.1.1/src/Main_SoundAI.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/TestSoundAI.py` & `pyftg-2.1.1/src/TestSoundAI.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/aiinterface/ai_interface.py` & `pyftg-2.1.1/src/pyftg/aiinterface/ai_interface.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/aiinterface/command_center.py` & `pyftg-2.1.1/src/pyftg/aiinterface/command_center.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/aiinterface/soundgenai_interface.py` & `pyftg-2.1.1/src/pyftg/aiinterface/soundgenai_interface.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/asyncio/ai_controller.py` & `pyftg-2.1.1/src/pyftg/grpc/asyncio/ai_controller.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/asyncio/gateway.py` & `pyftg-2.1.1/src/pyftg/grpc/asyncio/gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/threading/ai_controller.py` & `pyftg-2.1.1/src/pyftg/grpc/threading/ai_controller.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/threading/gateway.py` & `pyftg-2.1.1/src/pyftg/grpc/threading/gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/threading/observer_gateway.py` & `pyftg-2.1.1/src/pyftg/grpc/threading/observer_gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/grpc/threading/observer_handler.py` & `pyftg-2.1.1/src/pyftg/grpc/threading/observer_handler.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/interfaces/async_gateway.py` & `pyftg-2.1.1/src/pyftg/interfaces/async_gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/attack_data.py` & `pyftg-2.1.1/src/pyftg/models/attack_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/audio_data.py` & `pyftg-2.1.1/src/pyftg/models/audio_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/character_data.py` & `pyftg-2.1.1/src/pyftg/models/character_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/enums/action.py` & `pyftg-2.1.1/src/pyftg/models/enums/action.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/enums/int_action.py` & `pyftg-2.1.1/src/pyftg/models/enums/int_action.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/fft_data.py` & `pyftg-2.1.1/src/pyftg/models/fft_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/frame_data.py` & `pyftg-2.1.1/src/pyftg/models/frame_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/game_data.py` & `pyftg-2.1.1/src/pyftg/models/game_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/hit_area.py` & `pyftg-2.1.1/src/pyftg/models/hit_area.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/key.py` & `pyftg-2.1.1/src/pyftg/models/key.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/round_result.py` & `pyftg-2.1.1/src/pyftg/models/round_result.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/models/screen_data.py` & `pyftg-2.1.1/src/pyftg/models/screen_data.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/protoc/enum_pb2.py` & `pyftg-2.1.1/src/pyftg/protoc/enum_pb2.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/protoc/message_pb2.py` & `pyftg-2.1.1/src/pyftg/protoc/message_pb2.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/protoc/service_pb2.py` & `pyftg-2.1.1/src/pyftg/protoc/service_pb2.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/protoc/service_pb2_grpc.py` & `pyftg-2.1.1/src/pyftg/protoc/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/asyncio/ai_controller.py` & `pyftg-2.1.1/src/pyftg/socket/asyncio/ai_controller.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/asyncio/gateway.py` & `pyftg-2.1.1/src/pyftg/socket/asyncio/gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/asyncio/generative_sound_gateway.py` & `pyftg-2.1.1/src/pyftg/socket/asyncio/generative_sound_gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/threading/ai_controller.py` & `pyftg-2.1.1/src/pyftg/socket/threading/ai_controller.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/threading/gateway.py` & `pyftg-2.1.1/src/pyftg/socket/threading/gateway.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg/socket/utils/asyncio.py` & `pyftg-2.1.1/src/pyftg/socket/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyftg-2.1/src/pyftg.egg-info/PKG-INFO` & `pyftg-2.1.1/src/pyftg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftg
-Version: 2.1
+Version: 2.1.1
 Summary: An interface for implementing python AI in DareFightingICE
 Author: TeamFightingICE
 Project-URL: Homepage, https://github.com/TeamFightingICE/pyftg
 Project-URL: Issues, https://github.com/TeamFightingICE/pyftg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,14 @@
 Requires-Dist: grpcio-tools~=1.62.1
 Requires-Dist: protobuf~=4.25.3
 
 # pyftg
 
 An interface for implementing python AI in DareFightingICE
 
-**Note:** Version 2.0 is the latest version compatible with the legacy [FightingICE](https://github.com/TeamFightingICE/FightingICE). Version 2.1 and later will only support [DareFightingICE-Unity](https://github.com/TeamFightingICE/DareFightingICE-Unity).
-
 First, install `pyftg` with pip.
 ```
 pip install pyftg
 ```
 
 Initiate `Gateway` for connecting to DareFightingICE platform.
 ```
```

### Comparing `pyftg-2.1/src/pyftg.egg-info/SOURCES.txt` & `pyftg-2.1.1/src/pyftg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

