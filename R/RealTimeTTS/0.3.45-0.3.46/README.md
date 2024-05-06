# Comparing `tmp/RealTimeTTS-0.3.45.tar.gz` & `tmp/RealTimeTTS-0.3.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.3.45.tar", last modified: Sat May  4 20:20:11 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.3.46.tar", last modified: Mon May  6 13:47:38 2024, max compression
```

## Comparing `RealTimeTTS-0.3.45.tar` & `RealTimeTTS-0.3.46.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.892651 RealTimeTTS-0.3.45/
--rw-rw-rw-   0        0        0    19619 2024-05-04 20:20:11.890650 RealTimeTTS-0.3.45/PKG-INFO
--rw-rw-rw-   0        0        0    18500 2024-04-21 08:30:40.000000 RealTimeTTS-0.3.45/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.889649 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    19619 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-04 20:20:11.000000 RealTimeTTS-0.3.45/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.789644 RealTimeTTS-0.3.45/RealtimeTTS/
--rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.45/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.856701 RealTimeTTS-0.3.45/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9455 2024-04-12 11:47:00.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    47582 2024-04-22 12:17:29.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10595 2024-04-28 18:45:00.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     5340 2024-04-11 20:41:30.000000 RealTimeTTS-0.3.45/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0    10373 2024-05-04 20:11:35.000000 RealTimeTTS-0.3.45/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    29553 2024-05-04 20:09:08.000000 RealTimeTTS-0.3.45/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.45/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-05-04 20:20:11.892651 RealTimeTTS-0.3.45/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-05-04 20:19:49.000000 RealTimeTTS-0.3.45/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:20:11.888647 RealTimeTTS-0.3.45/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.45/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.45/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.257563 RealTimeTTS-0.3.46/
+-rw-rw-rw-   0        0        0    19946 2024-05-06 13:47:38.256563 RealTimeTTS-0.3.46/PKG-INFO
+-rw-rw-rw-   0        0        0    18827 2024-05-06 13:46:11.000000 RealTimeTTS-0.3.46/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.255562 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    19946 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 13:47:37.000000 RealTimeTTS-0.3.46/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 13:47:37.600018 RealTimeTTS-0.3.46/RealtimeTTS/
+-rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.46/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.251558 RealTimeTTS-0.3.46/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0     9455 2024-04-12 11:47:00.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    47582 2024-04-22 12:17:29.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10595 2024-04-28 18:45:00.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     5340 2024-04-11 20:41:30.000000 RealTimeTTS-0.3.46/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10657 2024-05-06 13:40:39.000000 RealTimeTTS-0.3.46/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    30141 2024-05-06 13:37:11.000000 RealTimeTTS-0.3.46/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.46/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:47:38.257563 RealTimeTTS-0.3.46/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2024-05-06 13:47:32.000000 RealTimeTTS-0.3.46/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:47:38.253560 RealTimeTTS-0.3.46/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.46/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.46/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.45/PKG-INFO` & `RealTimeTTS-0.3.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.45
+Version: 0.3.46
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,15 +52,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.44
+Latest Version: v0.3.46
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -328,14 +328,20 @@
 
 #### `language` (string)
 - **Type**: String
 - **Required**: No
 - **Default**: en
 - **Description**: Language to use for sentence splitting.
 
+#### `muted` (bool)
+- **Type**: Bool
+- **Required**: No
+- **Default**: False
+- **Description**: Global muted parameter. If True, no pyAudio stream will be opened. Disables audio playback via local speakers (in case you want to synthesize to file or process audio chunks) and overrides the play parameters muted setting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.45/README.md` & `RealTimeTTS-0.3.46/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.44
+Latest Version: v0.3.46
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -304,14 +304,20 @@
 
 #### `language` (string)
 - **Type**: String
 - **Required**: No
 - **Default**: en
 - **Description**: Language to use for sentence splitting.
 
+#### `muted` (bool)
+- **Type**: Bool
+- **Required**: No
+- **Default**: False
+- **Description**: Global muted parameter. If True, no pyAudio stream will be opened. Disables audio playback via local speakers (in case you want to synthesize to file or process audio chunks) and overrides the play parameters muted setting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.45/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.3.46/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.45
+Version: 0.3.46
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,15 +52,15 @@
 
 ## FAQ
 
 Check the [FAQ page](./FAQ.md) for answers to a lot of questions around the usage of RealtimeTTS.
 
 ## Updates
 
-Latest Version: v0.3.44
+Latest Version: v0.3.46
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -328,14 +328,20 @@
 
 #### `language` (string)
 - **Type**: String
 - **Required**: No
 - **Default**: en
 - **Description**: Language to use for sentence splitting.
 
+#### `muted` (bool)
+- **Type**: Bool
+- **Required**: No
+- **Default**: False
+- **Description**: Global muted parameter. If True, no pyAudio stream will be opened. Disables audio playback via local speakers (in case you want to synthesize to file or process audio chunks) and overrides the play parameters muted setting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.45/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.3.46/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/azure_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/coqui_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.3.46/RealtimeTTS/engines/system_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.3.46/RealtimeTTS/stream_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,28 @@
     """
 
     def __init__(
             self,
             format: int = pyaudio.paInt16,
             channels: int = 1,
             rate: int = 16000,
-            output_device_index=None):
+            output_device_index=None,
+            muted: bool = False):
         """
         Args:
             format (int): Audio format, defaults to pyaudio.paInt16
             channels (int): Number of channels, defaults to 1 (mono)
             rate (int): Sample rate, defaults to 16000
             output_device_index (int): Output device index, defaults to None
         """
         self.format = format
         self.channels = channels
         self.rate = rate
         self.output_device_index = output_device_index
+        self.muted = muted
 
 
 class AudioStream:
     """
     Handles audio stream operations
     - opening, starting, stopping, and closing
     """
@@ -54,35 +56,41 @@
         """Opens an audio stream."""
 
         # check for mpeg format
         pyChannels = self.config.channels
         pySampleRate = self.config.rate
         pyOutput_device_index = self.config.output_device_index
 
-        if self.config.format == pyaudio.paCustomFormat:
-            pyFormat = self.pyaudio_instance.get_format_from_width(2)
-            logging.debug("Opening stream for mpeg audio chunks, "
-                          f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
-                          f"pySampleRate: {pySampleRate}")
+        if self.config.muted:
+            print("Muted mode, no opening stream")
+            logging.debug("Muted mode, no opening stream")
+
         else:
-            pyFormat = self.config.format
-            logging.debug("Opening stream for wave audio chunks, "
-                          f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
-                          f"pySampleRate: {pySampleRate}")
+            print("Opening stream")
+            if self.config.format == pyaudio.paCustomFormat:
+                pyFormat = self.pyaudio_instance.get_format_from_width(2)
+                logging.debug("Opening stream for mpeg audio chunks, "
+                            f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
+                            f"pySampleRate: {pySampleRate}")
+            else:
+                pyFormat = self.config.format
+                logging.debug("Opening stream for wave audio chunks, "
+                            f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
+                            f"pySampleRate: {pySampleRate}")
 
-        try:
-            self.stream = self.pyaudio_instance.open(
-                format=pyFormat,
-                channels=pyChannels,
-                rate=pySampleRate,
-                output_device_index=pyOutput_device_index,
-                output=True)
-        except Exception as e:
-            print(f"Error opening stream: {e}")
-            exit(0)
+            try:
+                self.stream = self.pyaudio_instance.open(
+                    format=pyFormat,
+                    channels=pyChannels,
+                    rate=pySampleRate,
+                    output_device_index=pyOutput_device_index,
+                    output=True)
+            except Exception as e:
+                print(f"Error opening stream: {e}")
+                exit(0)
 
     def start_stream(self):
         """Starts the audio stream."""
         if self.stream and not self.stream.is_active():
             self.stream.start_stream()
 
     def stop_stream(self):
@@ -220,15 +228,14 @@
             chunk = segment.raw_data
 
         sub_chunk_size = 1024
 
         for i in range(0, len(chunk), sub_chunk_size):
             sub_chunk = chunk[i:i + sub_chunk_size]
 
-            # print("Playing/yielding chunk")
             if not self.first_chunk_played and self.on_playback_start:
                 self.on_playback_start()
                 self.first_chunk_played = True
 
             if not self.muted:
                 self.audio_stream.stream.write(sub_chunk)
```

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.3.46/RealtimeTTS/text_to_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                  on_text_stream_stop=None,
                  on_audio_stream_start=None,
                  on_audio_stream_stop=None,
                  on_character=None,
                  output_device_index=None,
                  tokenizer: str = "nltk",
                  language: str = "en",
+                 muted: bool = False,
                  level=logging.WARNING,
                  ):
         """
         Initializes the TextToAudioStream.
 
         Args:
             engine (BaseEngine): The engine used for text to audio synthesis.
@@ -49,28 +50,34 @@
             on_character (callable, optional): Callback function that gets
               called when a single character is processed.
             output_device_index (int, optional): The index of the output device
                 to use for audio playback.
             tokenizer (str, optional): Tokenizer to use for sentence splitting
                 (currently "nltk" and "stanza" are supported).
             language (str, optional): Language to use for sentence splitting.
+            muted (bool, optional): If True, disables audio playback via local
+                speakers (in case you want to synthesize to file or process
+                audio chunks). Default is False.
+                If set to True it will override the play parameters muted
+                setting.
             level (int, optional): Logging level. Defaults to logging.WARNING.
         """
         self.log_characters = log_characters
         self.on_text_stream_start = on_text_stream_start
         self.on_text_stream_stop = on_text_stream_stop
         self.on_audio_stream_start = on_audio_stream_start
         self.on_audio_stream_stop = on_audio_stream_stop
         self.output_device_index = output_device_index
         self.output_wavfile = None
         self.chunk_callback = None
         self.wf = None
         self.abort_events = []
         self.tokenizer = tokenizer
         self.language = language
+        self.global_muted = muted
         self.player = None
         self.play_lock = threading.Lock()
         self.is_playing_flag = False
 
         self._create_iterators()
 
         logging.info(f"Initializing tokenizer {tokenizer} "
@@ -114,21 +121,24 @@
         self.engine = engine
 
         # Extract stream information (format, channels, rate) from the engine
         format, channels, rate = self.engine.get_stream_info()
 
         # Check if the engine doesn't support consuming generators directly
         if not self.engine.can_consume_generators:
+            config = AudioConfiguration(
+                format,
+                channels,
+                rate,
+                self.output_device_index,
+                muted=self.global_muted)
+
             self.player = StreamPlayer(
                 self.engine.queue,
-                AudioConfiguration(
-                    format,
-                    channels,
-                    rate,
-                    self.output_device_index),
+                config,
                 on_playback_start=self._on_audio_stream_start)
         else:
             self.engine.on_playback_start = self._on_audio_stream_start
             self.player = None
 
         logging.info(f"loaded engine {self.engine.engine_name}")
 
@@ -227,14 +237,16 @@
         - muted: If True, disables audio playback via local speakers (in case you want to synthesize to file or process audio chunks). Default is False.
         - sentence_fragment_delimiters (str): A string of characters that are
             considered sentence delimiters. Default is ".?!;:,\n…)]}。-".
         - force_first_fragment_after_words (int): The number of words after
             which the first sentence fragment is forced to be yielded.
             Default is 15 words.
         """
+        if self.global_muted:
+            muted = True
 
         if is_external_call:
             if not self.play_lock.acquire(blocking=False):
                 logging.warning("play() called while already playing audio, skipping")
                 return
 
         self.is_playing_flag = True
@@ -291,15 +303,19 @@
                 self.stream_running = False
                 logging.info("stream stop")
 
                 # Accumulate the generated text and reset the character iterators
                 self.generated_text += self.char_iter.iterated_text
 
                 self._create_iterators()
-                self.is_playing_flag = False
+
+                if is_external_call:
+
+                    self.is_playing_flag = False
+                    self.play_lock.release()
         else:
             try:
                 # Start the audio player to handle playback
                 self.player.start()
                 self.player.on_audio_chunk = self._on_audio_chunk
 
                 # Generate sentences from the characters
```

### Comparing `RealTimeTTS-0.3.45/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.3.46/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/setup.py` & `RealTimeTTS-0.3.46/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.3.45",
+    version="0.3.46",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.3.45/tests/test_callbacks.py` & `RealTimeTTS-0.3.46/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.45/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.3.46/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

