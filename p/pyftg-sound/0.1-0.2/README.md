# Comparing `tmp/pyftg_sound-0.1.tar.gz` & `tmp/pyftg_sound-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftg_sound-0.1.tar", last modified: Sat May  4 15:50:50 2024, max compression
+gzip compressed data, was "pyftg_sound-0.2.tar", last modified: Mon May  6 07:35:30 2024, max compression
```

## Comparing `pyftg_sound-0.1.tar` & `pyftg_sound-0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.344387 pyftg_sound-0.1/
--rw-r--r--   0 staciiaz   (501) staff       (20)      897 2024-05-04 15:50:50.344221 pyftg_sound-0.1/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)      374 2024-05-04 15:36:05.000000 pyftg_sound-0.1/README.md
--rw-r--r--   0 staciiaz   (501) staff       (20)      531 2024-05-04 15:50:44.000000 pyftg_sound-0.1/pyproject.toml
--rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-05-04 15:50:50.344421 pyftg_sound-0.1/setup.cfg
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.341719 pyftg_sound-0.1/src/
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.342441 pyftg_sound-0.1/src/pyftg_sound/
--rw-r--r--   0 staciiaz   (501) staff       (20)       52 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/config.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.343301 pyftg_sound-0.1/src/pyftg_sound/models/
--rw-r--r--   0 staciiaz   (501) staff       (20)      743 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/models/audio_buffer.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      598 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/models/audio_source.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     5584 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/models/sound_renderer.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.343919 pyftg_sound-0.1/src/pyftg_sound/openal/
--rw-r--r--   0 staciiaz   (501) staff       (20)     3225 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/openal/__init__.py
--rw-r--r--   0 staciiaz   (501) staff       (20)    11330 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/openal/al.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     7082 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/openal/alc.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      126 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/openal/constants.py
--rw-r--r--   0 staciiaz   (501) staff       (20)       51 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/openal/log.py
--rw-r--r--   0 staciiaz   (501) staff       (20)     6014 2024-05-04 15:48:56.000000 pyftg_sound-0.1/src/pyftg_sound/sound_manager.py
--rw-r--r--   0 staciiaz   (501) staff       (20)      640 2024-05-04 15:36:05.000000 pyftg_sound-0.1/src/pyftg_sound/utils.py
-drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-04 15:50:50.344068 pyftg_sound-0.1/src/pyftg_sound.egg-info/
--rw-r--r--   0 staciiaz   (501) staff       (20)      897 2024-05-04 15:50:50.000000 pyftg_sound-0.1/src/pyftg_sound.egg-info/PKG-INFO
--rw-r--r--   0 staciiaz   (501) staff       (20)      581 2024-05-04 15:50:50.000000 pyftg_sound-0.1/src/pyftg_sound.egg-info/SOURCES.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-05-04 15:50:50.000000 pyftg_sound-0.1/src/pyftg_sound.egg-info/dependency_links.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)       14 2024-05-04 15:50:50.000000 pyftg_sound-0.1/src/pyftg_sound.egg-info/requires.txt
--rw-r--r--   0 staciiaz   (501) staff       (20)       12 2024-05-04 15:50:50.000000 pyftg_sound-0.1/src/pyftg_sound.egg-info/top_level.txt
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.018906 pyftg_sound-0.2/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      901 2024-05-06 07:35:30.018741 pyftg_sound-0.2/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)      374 2024-05-04 15:36:05.000000 pyftg_sound-0.2/README.md
+-rw-r--r--   0 staciiaz   (501) staff       (20)      535 2024-05-06 07:34:28.000000 pyftg_sound-0.2/pyproject.toml
+-rw-r--r--   0 staciiaz   (501) staff       (20)       38 2024-05-06 07:35:30.018939 pyftg_sound-0.2/setup.cfg
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.016242 pyftg_sound-0.2/src/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.016738 pyftg_sound-0.2/src/pyftg_sound/
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.017579 pyftg_sound-0.2/src/pyftg_sound/models/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      748 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/models/audio_buffer.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      598 2024-05-04 15:36:05.000000 pyftg_sound-0.2/src/pyftg_sound/models/audio_source.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     4767 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/models/sound_renderer.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.018117 pyftg_sound-0.2/src/pyftg_sound/openal/
+-rw-r--r--   0 staciiaz   (501) staff       (20)     3225 2024-05-04 15:36:05.000000 pyftg_sound-0.2/src/pyftg_sound/openal/__init__.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)    11332 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/openal/al.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6202 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/openal/alc.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)       51 2024-05-04 15:36:05.000000 pyftg_sound-0.2/src/pyftg_sound/openal/log.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1431 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/openal/soft.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     6229 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/sound_manager.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.018437 pyftg_sound-0.2/src/pyftg_sound/utils/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      282 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/utils/dtype.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)     1239 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/utils/openal.py
+-rw-r--r--   0 staciiaz   (501) staff       (20)      640 2024-05-06 07:34:28.000000 pyftg_sound-0.2/src/pyftg_sound/utils/wave.py
+drwxr-xr-x   0 staciiaz   (501) staff       (20)        0 2024-05-06 07:35:30.018582 pyftg_sound-0.2/src/pyftg_sound.egg-info/
+-rw-r--r--   0 staciiaz   (501) staff       (20)      901 2024-05-06 07:35:30.000000 pyftg_sound-0.2/src/pyftg_sound.egg-info/PKG-INFO
+-rw-r--r--   0 staciiaz   (501) staff       (20)      618 2024-05-06 07:35:30.000000 pyftg_sound-0.2/src/pyftg_sound.egg-info/SOURCES.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)        1 2024-05-06 07:35:30.000000 pyftg_sound-0.2/src/pyftg_sound.egg-info/dependency_links.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)       14 2024-05-06 07:35:30.000000 pyftg_sound-0.2/src/pyftg_sound.egg-info/requires.txt
+-rw-r--r--   0 staciiaz   (501) staff       (20)       12 2024-05-06 07:35:30.000000 pyftg_sound-0.2/src/pyftg_sound.egg-info/top_level.txt
```

### Comparing `pyftg_sound-0.1/PKG-INFO` & `pyftg_sound-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyftg-sound
-Version: 0.1
-Summary: A sound library for sound design in DareFightingICE
+Version: 0.2
+Summary: A sound library for DareFightingICE with OpenAL backend
 Author: TeamFightingICE
 Project-URL: Homepage, https://github.com/TeamFightingICE/pyftg-sound
 Project-URL: Issues, https://github.com/TeamFightingICE/pyftg-sound/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pyftg_sound-0.1/pyproject.toml` & `pyftg_sound-0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pyftg-sound"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="TeamFightingICE" },
 ]
-description = "A sound library for sound design in DareFightingICE"
+description = "A sound library for DareFightingICE with OpenAL backend"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/models/audio_buffer.py` & `pyftg_sound-0.2/src/pyftg_sound/models/audio_buffer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from typing import List
 
 from pyftg_sound.openal import al, alc
-from pyftg_sound.utils import load_sound
+from pyftg_sound.utils.wave import load_sound
 
 
 class AudioBuffer:
     contexts: List[alc.ALCcontext]
     buffers: List[int]
 
     def __init__(self, contexts: List[alc.ALCcontext], buffers: List[int]) -> None:
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/models/audio_source.py` & `pyftg_sound-0.2/src/pyftg_sound/models/audio_source.py`

 * *Files identical despite different names*

### Comparing `pyftg_sound-0.1/src/pyftg_sound/models/sound_renderer.py` & `pyftg_sound-0.2/src/pyftg_sound/models/sound_renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import ctypes
 from typing import List
 
 import numpy as np
 
-from pyftg_sound.config import SOUND_RENDER_SIZE, SOUND_SAMPLING_RATE
-from pyftg_sound.openal import al, alc
-from pyftg_sound.openal.constants import (ALC_FLOAT_SOFT,
-                                          ALC_FORMAT_CHANNELS_SOFT,
-                                          ALC_FORMAT_TYPE_SOFT, ALC_FREQUENCY,
-                                          ALC_STEREO_SOFT)
+from pyftg_sound.openal import al, alc, soft
+from pyftg_sound.utils.dtype import dtype_map
+from pyftg_sound.utils.openal import set_source_attribute
 
 
 class SoundRenderer:
     device = None
     context = None
 
     def __init__(self, device, context) -> None:
@@ -22,132 +19,111 @@
     @staticmethod
     def create_default_renderer():
         device = alc.alcOpenDevice(None)
         context = alc.alcCreateContext(device, None)
         return SoundRenderer(device, context)
 
     @staticmethod
-    def create_virtual_renderer():
-        device = alc.alcLoopbackOpenDeviceSOFT(None)
-        attrs = [ALC_FORMAT_TYPE_SOFT, ALC_FLOAT_SOFT, ALC_FORMAT_CHANNELS_SOFT,
-                 ALC_STEREO_SOFT, ALC_FREQUENCY, SOUND_SAMPLING_RATE, 0]
-        attrs_c = al.ALint * len(attrs)
-        attrs_c = attrs_c(*attrs)
+    def create_virtual_renderer(format: int = soft.ALC_FLOAT_SOFT, channel: int = soft.ALC_STEREO_SOFT, sample_rate: int = 48000):
+        device = soft.alcLoopbackOpenDeviceSOFT(None)
+        attrs = [
+            soft.ALC_FORMAT_TYPE_SOFT, format, soft.ALC_FORMAT_CHANNELS_SOFT,
+            channel, alc.ALC_FREQUENCY, sample_rate, 0
+        ]
+        attrs_c = (al.ALint * len(attrs))(*attrs)
         context = alc.alcCreateContext(device, attrs_c)
         return SoundRenderer(device, context)
 
     def set(self) -> None:
         alc.alcMakeContextCurrent(self.context)
 
-    def set_listener_data(self) -> None:
+    def create_source(self, attrs: dict) -> int:
         self.set()
-        al.alListener3f(al.AL_POSITION, 0, 0, 0)
-        al.alListener3f(al.AL_VELOCITY, 0, 0, 0)
-
-    def play(self, source_id: int, buffer_id: int) -> None:
+        source = al.ALuint(0)
+        al.alGenSources(1, source)
+        for attr, value in attrs.items():
+            set_source_attribute(source, attr, value)
+        return source.value
+        
+    def create_buffer(self) -> int:
         self.set()
-        al.alSourcei(source_id, al.AL_BUFFER, buffer_id)
-        al.alSourcePlay(source_id)
+        buffer = al.ALuint(0)
+        al.alGenBuffers(1, buffer)
+        return buffer.value
 
-    def stop(self, source_id: int) -> None:
+    def al_listener_fv(self, param: int, values: List[float]) -> None:
         self.set()
-        if self.is_playing(source_id):
-            al.alSourceStop(source_id)
+        values_arr = (al.ALfloat * len(values))(*values)
+        al.alListenerfv(param, values_arr)
 
-    def play(self, source_id: int, buffer_id: int, x: int, y: int, loop: bool) -> None:
+    def play(self, source_id: int) -> None:
         self.set()
-        if self.is_playing(source_id):
-            self.stop(source_id)
-        al.alSourcei(source_id, al.AL_BUFFER, buffer_id)
-        al.alSource3f(source_id, al.AL_POSITION, x, 0, 4)
-        al.alSourcei(source_id, al.AL_LOOPING, int(loop))
         al.alSourcePlay(source_id)
 
-    def get_source_gain(self, source_id: int) -> float:
+    def is_playing(self, source_id: int) -> bool:
         self.set()
-        return al.alGetSourcef(source_id, al.AL_GAIN)
+        state = al.ALint(0)
+        al.alGetSourcei(source_id, al.AL_SOURCE_STATE, state)
+        return state.value == al.AL_PLAYING
 
-    def set_source_gain(self, source_id: int, gain: float) -> None:
+    def stop(self, source_id: int) -> None:
         self.set()
-        al.alSourcef(source_id, al.AL_GAIN, gain)
+        if self.is_playing(source_id):
+            al.alSourceStop(source_id)
 
-    def set_source_3f(self, source_id: int, param: int, x: int, y: int, z: int) -> None:
+    def play2(self, source_id: int, buffer_id: int, x: float, y: float, z: float, loop: bool) -> None:
         self.set()
-        al.alSource3f(source_id, param, x, y, z)
+        if self.is_playing(source_id):
+            self.stop(source_id)
+        set_source_attribute(source_id, al.AL_BUFFER, buffer_id)
+        set_source_attribute(source_id, al.AL_POSITION, [x, y, z])
+        set_source_attribute(source_id, al.AL_LOOPING, al.AL_TRUE if loop else al.AL_FALSE)
+        self.play(source_id)
 
     def delete_source(self, source_id: int) -> None:
         self.set()
         al.alDeleteSources(1, al.ALuint(source_id))
 
     def delete_buffer(self, buffer_id: int) -> None:
         self.set()
         al.alDeleteBuffers(1, al.ALuint(buffer_id))
 
     def close(self) -> None:
         self.set()
         alc.alcDestroyContext(self.context)
         alc.alcCloseDevice(self.device)
 
-    def is_playing(self, source_id: int) -> bool:
-        self.set()
-        state = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_SOURCE_STATE, state)
-        return state.value == al.AL_PLAYING
-
-    def al_listener_fv(self, param: int, values: List[float]) -> None:
+    def sample_audio(self, dtype: type, render_size: int, nchannels: int) -> np.ndarray:
         self.set()
-        values_arr = (al.ALfloat * len(values))(*values)
-        al.alListenerfv(param, values_arr)
-
-    def sample_audio(self) -> np.ndarray[np.float32]:
-        self.set()
-        audio_data_type = al.ALfloat * SOUND_RENDER_SIZE * 2
-        audio_sample = audio_data_type()
-        audio_sample_pointer = ctypes.cast(audio_sample, ctypes.c_void_p)
-
-        alc.alcRenderSamplesSOFT(self.device, audio_sample_pointer, al.ALsizei(SOUND_RENDER_SIZE))
-        sampled_audio = ctypes.cast(audio_sample_pointer, ctypes.POINTER(audio_data_type)).contents
-
-        separated_channel_audio = np.zeros((2, SOUND_RENDER_SIZE), dtype=np.float32)
-        separated_channel_audio[0, :] = sampled_audio[0]
-        separated_channel_audio[1, :] = sampled_audio[1]
+        audio_sample_type = dtype * render_size * nchannels
+        audio_sample_ptr = ctypes.cast(audio_sample_type(), ctypes.c_void_p)
+        soft.alcRenderSamplesSOFT(self.device, audio_sample_ptr, al.ALsizei(render_size))
+        separated_channel_audio = np.zeros((nchannels, render_size), dtype=dtype_map[dtype])
+        separated_channel_audio[:, :] = ctypes.cast(audio_sample_ptr, ctypes.POINTER(audio_sample_type)).contents
         return separated_channel_audio
     
-    def playback(self, source_id: int, audio_sample: bytes) -> None:
+    def get_processed_buffers(self, source_id: int) -> int:
         self.set()
-        
-        queuedBuffers = al.ALint(0)
-        processedBuffers = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_BUFFERS_QUEUED, queuedBuffers)
-        al.alGetSourcei(source_id, al.AL_BUFFERS_PROCESSED, processedBuffers)
-
-        if processedBuffers.value > 0:
-            buffer = al.ALuint(0)
+        processed_buffers = al.ALint(0)
+        al.alGetSourcei(source_id, al.AL_BUFFERS_PROCESSED, processed_buffers)
+        return processed_buffers.value
+    
+    def playback(self, source_id: int, format: int, audio_sample: bytes, sample_rate: int) -> None:
+        self.set()
+        buffer = al.ALuint(0)
+        if self.get_processed_buffers(source_id) > 0:
             al.alSourceUnqueueBuffers(source_id, 1, buffer)
         else:
-            buffer = al.ALuint(0)
             al.alGenBuffers(1, buffer)
-
-        al.alBufferData(buffer, al.AL_FORMAT_STEREO16, audio_sample, len(audio_sample), SOUND_SAMPLING_RATE)
+        al.alBufferData(buffer, format, audio_sample, len(audio_sample), sample_rate)
         al.alSourceQueueBuffers(source_id, 1, buffer)
-        state = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_SOURCE_STATE, state)
-        if state.value != al.AL_PLAYING:
-            al.alSourcePlay(source_id)
+        if not self.is_playing(source_id):
+            self.play(source_id)
 
     def stop_playback(self, source_id: int) -> None:
         self.set()
-
-        queuedBuffers = al.ALint(0)
-        processedBuffers = al.ALint(0)
-        al.alGetSourcei(source_id, al.AL_BUFFERS_QUEUED, queuedBuffers)
-        al.alGetSourcei(source_id, al.AL_BUFFERS_PROCESSED, processedBuffers)
-
-        bufferCount = queuedBuffers.value + processedBuffers.value
-
         buffer = al.ALuint(0)
-        for _ in range(bufferCount):
+        for _ in range(self.get_processed_buffers(source_id)):
             al.alSourceUnqueueBuffers(source_id, 1, buffer)
             al.alDeleteBuffers(1, buffer)
-        
-        al.alSourceStop(source_id)
-        al.alSourcei(source_id, al.AL_BUFFER, al.AL_NONE)
+        self.stop(source_id)
+        self.al_source_i(source_id, al.AL_BUFFER, al.AL_NONE)
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/openal/__init__.py` & `pyftg_sound-0.2/src/pyftg_sound/openal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftg_sound-0.1/src/pyftg_sound/openal/al.py` & `pyftg_sound-0.2/src/pyftg_sound/openal/al.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,16 +142,18 @@
 ALint = ctypes.c_int
 ALuint = ctypes.c_uint
 ALsizei = ctypes.c_int
 ALenum = ctypes.c_int
 ALfloat = ctypes.c_float
 ALdouble = ctypes.c_double
 ALvoid = None
+
 class ALCCapabilities(ctypes.Structure):
     pass
+
 _bind = dll.bind_function
 
 alEnable = _bind("alEnable", [ALenum])
 alDisable = _bind("alDisable", [ALenum])
 alIsEnabled = _bind("alIsEnabled", [ALenum], ALboolean)
 alGetString = _bind("alGetString", [ALenum], ctypes.POINTER(ALchar))
 alGetBooleanv = _bind("alGetBooleanv", [ALenum, ctypes.POINTER(ALboolean)])
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/openal/alc.py` & `pyftg_sound-0.2/src/pyftg_sound/openal/alc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import ctypes
 
 from . import dll
-from .log import logger
 
 __all__ = ["ALC_FALSE", "ALC_TRUE", "ALC_INVALID", "ALC_FREQUENCY",
            "ALC_REFRESH", "ALC_SYNC", "ALC_MONO_SOURCES", "ALC_STEREO_SOURCES",
            "ALC_NO_ERROR", "ALC_INVALID_DEVICE", "ALC_INVALID_CONTEXT",
            "ALC_INVALID_ENUM", "ALC_INVALID_VALUE", "ALC_OUT_OF_MEMORY",
            "ALC_DEFAULT_DEVICE_SPECIFIER", "ALC_DEVICE_SPECIFIER",
            "ALC_EXTENSIONS", "ALC_MAJOR_VERSION", "ALC_MINOR_VERSION",
@@ -147,20 +146,7 @@
 alcCaptureCloseDevice = _bind("alcCaptureCloseDevice",
                               [ctypes.POINTER(ALCdevice)])
 alcCaptureStart = _bind("alcCaptureStart", [ctypes.POINTER(ALCdevice)])
 alcCaptureStop = _bind("alcCaptureStop", [ctypes.POINTER(ALCdevice)])
 alcCaptureSamples = _bind("alcCaptureSamples", [ctypes.POINTER(ALCdevice),
                                                 ctypes.POINTER(ALCvoid),
                                                 ALCsizei])
-
-try:
-    alcLoopbackOpenDeviceSOFT = _bind("alcLoopbackOpenDeviceSOFT", [ctypes.POINTER(ALCchar)], ctypes.POINTER(ALCdevice))
-    alcGetStringiSOFT = _bind("alcGetStringiSOFT", [ctypes.POINTER(ALCdevice),
-                                                      ctypes.POINTER(ALCenum),
-                                                      ctypes.POINTER(ALCsizei)])
-    alcResetDeviceSOFT = _bind("alcResetDeviceSOFT", [ctypes.POINTER(ALCdevice),
-                                                      ctypes.POINTER(ALCint)])
-    alcRenderSamplesSOFT = _bind("alcRenderSamplesSOFT", [ctypes.POINTER(ALCdevice), ctypes.POINTER(ALCvoid), ALCsizei])
-except AttributeError:
-    logger.warning("OpenAL-Soft functions could not be bound")
-else:
-    __all__.extend(("alcLoopbackOpenDeviceSOFT", "alcGetStringiSOFT", "alcResetDeviceSOFT", "alcRenderSamplesSOFT"))
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/sound_manager.py` & `pyftg_sound-0.2/src/pyftg_sound/sound_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 import numpy as np
 
 from pyftg_sound.models.audio_buffer import AudioBuffer
 from pyftg_sound.models.audio_source import AudioSource
 from pyftg_sound.models.sound_renderer import SoundRenderer
 from pyftg_sound.openal import al
+from pyftg_sound.utils.openal import set_source_attribute
 
 
 class SoundManager:
     sound_renderers: List[SoundRenderer] = []
     audio_sources: List[AudioSource] = []
     audio_buffers: List[AudioBuffer] = []
     sound_buffers: Dict[str, AudioBuffer] = {}
     virtual_renderer: SoundRenderer = None
 
-    def __init__(self, use_default_renderer: bool = True) -> None:
-        if use_default_renderer:
-            self.register_sound_renderer(SoundRenderer.create_default_renderer())
-        self.virtual_renderer = SoundRenderer.create_virtual_renderer()
-        self.register_sound_renderer(self.virtual_renderer)
+    def __init__(self) -> None:
+        pass
 
-    def register_sound_renderer(self, sound_renderer: SoundRenderer) -> None:
+    def set_default_renderer(self, sound_renderer: SoundRenderer) -> None:
         self.sound_renderers.append(sound_renderer)
 
+    def set_virtual_renderer(self, virtual_renderer: SoundRenderer) -> None:
+        self.virtual_renderer = virtual_renderer
+        self.sound_renderers.append(virtual_renderer)
+
     def set_listener_position(self, x: float, y: float, z: float) -> None:
         listener_pos = [x, y, z]
         for sound_renderer in self.sound_renderers:
             sound_renderer.al_listener_fv(al.AL_POSITION, listener_pos)
 
     def set_listener_velocity(self, x: float, y: float, z: float) -> None:
         listener_vel = [x, y, z]
@@ -36,92 +38,87 @@
             sound_renderer.al_listener_fv(al.AL_VELOCITY, listener_vel)
 
     def set_listener_orientation(self, x: float, y: float, z: float, x_up: float, y_up: float, z_up: float) -> None:
         listener_ori = [x, y, z, x_up, y_up, z_up]
         for sound_renderer in self.sound_renderers:
             sound_renderer.al_listener_fv(al.AL_ORIENTATION, listener_ori)
     
-    def create_source(self) -> int:
-        source = al.ALuint(0)
-        al.alGenSources(1, source)
-        al.alSourcef(source, al.AL_ROLLOFF_FACTOR, 0.01)
-        return source.value
-        
-    def create_buffer(self) -> int:
-        buffer = al.ALuint(0)
-        al.alGenBuffers(1, buffer)
-        return buffer.value
-    
-    def create_audio_source(self) -> AudioSource:
+    def create_audio_source(self, attrs: dict = {}) -> AudioSource:
         contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
         source_ids = [0] * len(self.sound_renderers)
         for i, sound_renderer in enumerate(self.sound_renderers):
-            sound_renderer.set()
-            source_ids[i] = self.create_source()
+            source_ids[i] = sound_renderer.create_source(attrs)
         audio_source = AudioSource(contexts, source_ids)
         self.audio_sources.append(audio_source)
         return audio_source
 
     def create_audio_buffer(self, file_path: Path = None) -> AudioBuffer:
         contexts = [sound_renderer.context for sound_renderer in self.sound_renderers]
         buffer_ids = [0] * len(self.sound_renderers)
         for i, sound_renderer in enumerate(self.sound_renderers):
-            sound_renderer.set()
-            buffer_ids[i] = self.create_buffer()
+            buffer_ids[i] = sound_renderer.create_buffer()
         audio_buffer = AudioBuffer(contexts, buffer_ids)
         if file_path is not None:
             audio_buffer.register_sound(file_path)
             self.sound_buffers[file_path.name] = audio_buffer
         self.audio_buffers.append(audio_buffer)
         return audio_buffer
 
-    def play(self, source: AudioSource, buffer: AudioBuffer, x: int, y: int, loop: bool) -> None:
-        for i, sound_renderer in enumerate(self.sound_renderers):
-            source_id = source.get_source_ids()[i]
-            buffer_id = buffer.get_buffers()[i]
-            sound_renderer.play(source_id, buffer_id, x, y, loop)
-
-    def get_sound_buffer(self, sound_name: str) -> AudioBuffer:
-        return self.sound_buffers.get(sound_name)
-
     def is_playing(self, source: AudioSource) -> bool:
         ans = False
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
             ans = ans or sound_renderer.is_playing(source_id)
         return ans
+    
+    def play(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, loop: bool) -> None:
+        self.play3d(source, buffer, x, 0, y, loop)
+
+    def play3d(self, source: AudioSource, buffer: AudioBuffer, x: float, y: float, z: float, loop: bool) -> None:
+        for i, sound_renderer in enumerate(self.sound_renderers):
+            source_id = source.get_source_ids()[i]
+            buffer_id = buffer.get_buffers()[i]
+            sound_renderer.play2(source_id, buffer_id, x, y, z, loop)
 
     def stop(self, source: AudioSource) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
             sound_renderer.stop(source_id)
 
-    def set_source_pos(self, source: AudioSource, x: int, y: int) -> None:
+    def set_source_pos(self, source: AudioSource, x: float, y: float) -> None:
+        self.set_source_pos3d(source, x, 0, y)
+
+    def set_source_pos3d(self, source: AudioSource, x: float, y: float, z: float) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
-            sound_renderer.set_source_3f(source_id, al.AL_POSITION, x, 0, 4)
+            set_source_attribute(source_id, al.AL_POSITION, [x, y, z], context=sound_renderer.context)
 
     def set_source_gain(self, source: AudioSource, gain: float) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
-            sound_renderer.set_source_gain(source_id, np.clip(gain, 0, 1))
+            set_source_attribute(source_id, al.AL_GAIN, gain, context=sound_renderer.context)
+
+    def get_sound_buffer(self, sound_name: str) -> AudioBuffer:
+        return self.sound_buffers.get(sound_name)
 
-    def sample_audio(self) -> np.ndarray[np.float32]:
-        return self.virtual_renderer.sample_audio()
+    def sample_audio(self, dtype: type = al.ALfloat, render_size: int = 800, nchannels: int = 2) -> np.ndarray:
+        if not self.virtual_renderer:
+            raise ValueError("Virtual renderer not set")
+        return self.virtual_renderer.sample_audio(dtype, render_size, nchannels)
     
     def remove_source(self, source: AudioSource) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
             sound_renderer.delete_source(source_id)
         self.audio_sources.remove(source)
 
-    def playback(self, source: AudioSource, audio_sample: bytes) -> None:
+    def playback(self, source: AudioSource, format: int, audio_sample: bytes, sample_rate: int) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
-            sound_renderer.playback(source_id, audio_sample)
+            sound_renderer.playback(source_id, format, audio_sample, sample_rate)
 
     def stop_playback(self, source: AudioSource) -> None:
         for i, sound_renderer in enumerate(self.sound_renderers):
             source_id = source.get_source_ids()[i]
             sound_renderer.stop_playback(source_id)
 
     def stop_all(self) -> None:
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound/utils.py` & `pyftg_sound-0.2/src/pyftg_sound/utils/wave.py`

 * *Files identical despite different names*

### Comparing `pyftg_sound-0.1/src/pyftg_sound.egg-info/PKG-INFO` & `pyftg_sound-0.2/src/pyftg_sound.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyftg-sound
-Version: 0.1
-Summary: A sound library for sound design in DareFightingICE
+Version: 0.2
+Summary: A sound library for DareFightingICE with OpenAL backend
 Author: TeamFightingICE
 Project-URL: Homepage, https://github.com/TeamFightingICE/pyftg-sound
 Project-URL: Issues, https://github.com/TeamFightingICE/pyftg-sound/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `pyftg_sound-0.1/src/pyftg_sound.egg-info/SOURCES.txt` & `pyftg_sound-0.2/src/pyftg_sound.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 README.md
 pyproject.toml
-src/pyftg_sound/config.py
 src/pyftg_sound/sound_manager.py
-src/pyftg_sound/utils.py
 src/pyftg_sound.egg-info/PKG-INFO
 src/pyftg_sound.egg-info/SOURCES.txt
 src/pyftg_sound.egg-info/dependency_links.txt
 src/pyftg_sound.egg-info/requires.txt
 src/pyftg_sound.egg-info/top_level.txt
 src/pyftg_sound/models/audio_buffer.py
 src/pyftg_sound/models/audio_source.py
 src/pyftg_sound/models/sound_renderer.py
 src/pyftg_sound/openal/__init__.py
 src/pyftg_sound/openal/al.py
 src/pyftg_sound/openal/alc.py
-src/pyftg_sound/openal/constants.py
-src/pyftg_sound/openal/log.py
+src/pyftg_sound/openal/log.py
+src/pyftg_sound/openal/soft.py
+src/pyftg_sound/utils/dtype.py
+src/pyftg_sound/utils/openal.py
+src/pyftg_sound/utils/wave.py
```

