# Comparing `tmp/whisper-ctranslate2-0.4.2.tar.gz` & `tmp/whisper-ctranslate2-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.4.2.tar", last modified: Sun Apr  7 16:36:12 2024, max compression
+gzip compressed data, was "whisper-ctranslate2-0.4.3.tar", last modified: Mon May  6 20:34:45 2024, max compression
```

## Comparing `whisper-ctranslate2-0.4.2.tar` & `whisper-ctranslate2-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.4.2/LICENSE
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.2/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-04-07 16:35:05.000000 whisper-ctranslate2-0.4.2/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.125792 whisper-ctranslate2-0.4.2/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.125792 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14776 2024-02-23 21:48:18.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/commandline.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3567 2024-04-07 16:26:12.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/diarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live_old.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6772 2024-04-07 16:09:16.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-02-23 22:08:01.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8977 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10130 2024-04-07 16:09:16.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.126792 whisper-ctranslate2-0.4.2/tests/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.2/tests/testdiarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper-ctranslate2-0.4.2/tests/testlive.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper-ctranslate2-0.4.2/tests/testwriters.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.126792 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.4.3/LICENSE
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.3/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-05-04 18:06:24.000000 whisper-ctranslate2-0.4.3/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.064273 whisper-ctranslate2-0.4.3/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.065273 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14799 2024-04-10 13:52:29.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/commandline.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3567 2024-04-07 16:26:12.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/diarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live_old.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6776 2024-05-06 20:17:31.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-04-07 16:42:56.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8977 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10210 2024-04-07 17:57:01.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.066273 whisper-ctranslate2-0.4.3/tests/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.3/tests/testdiarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper-ctranslate2-0.4.3/tests/testlive.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper-ctranslate2-0.4.3/tests/testwriters.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.4.2/LICENSE` & `whisper-ctranslate2-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/PKG-INFO` & `whisper-ctranslate2-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: faster-whisper>=1.0.0
+Requires-Dist: faster-whisper>=1.0.2
 Requires-Dist: ctranslate2
 Requires-Dist: tqdm
 Requires-Dist: sounddevice
 Requires-Dist: numpy
 Provides-Extra: dev
-Requires-Dist: flake8==6.*; extra == "dev"
-Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: flake8==7.*; extra == "dev"
+Requires-Dist: black==24.*; extra == "dev"
 Requires-Dist: nose2; extra == "dev"
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
```

### Comparing `whisper-ctranslate2-0.4.2/README.md` & `whisper-ctranslate2-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/setup.py` & `whisper-ctranslate2-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     install_requires=[
         str(r)
         for r in pkg_resources.parse_requirements(
             open(os.path.join(os.path.dirname(__file__), "requirements.txt"))
         )
     ],
     extras_require={
-        "dev": ["flake8==6.*", "black==23.*", "nose2"],
+        "dev": ["flake8==7.*", "black==24.*", "nose2"],
     },
     entry_points={
         "console_scripts": [
             "whisper-ctranslate2=src.whisper_ctranslate2.whisper_ctranslate2:main",
         ]
     },
 )
```

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/commandline.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/commandline.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "small.en",
     "medium",
     "medium.en",
     "large-v1",
     "large-v2",
     "large-v3",
     "distil-large-v2",
+    "distil-large-v3",
     "distil-medium.en",
     "distil-small.en",
 ]
 
 
 class CommandLine:
     @staticmethod
```

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/diarization.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/diarization.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live_old.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live_old.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/transcribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,25 +79,25 @@
     def _get_vad_parameters_dictionary(self, options):
         vad_parameters = {}
 
         if options.vad_threshold:
             vad_parameters["threshold"] = options.vad_threshold
 
         if options.vad_min_speech_duration_ms:
-            vad_parameters[
-                "min_speech_duration_ms"
-            ] = options.vad_min_speech_duration_ms
+            vad_parameters["min_speech_duration_ms"] = (
+                options.vad_min_speech_duration_ms
+            )
 
         if options.vad_max_speech_duration_s:
             vad_parameters["max_speech_duration_s"] = options.vad_max_speech_duration_s
 
         if options.vad_min_silence_duration_ms:
-            vad_parameters[
-                "min_silence_duration_ms"
-            ] = options.vad_min_silence_duration_ms
+            vad_parameters["min_silence_duration_ms"] = (
+                options.vad_min_silence_duration_ms
+            )
 
         return vad_parameters
 
     def __init__(
         self,
         model_path: str,
         device: str,
@@ -197,9 +197,9 @@
                 accumated_inc += increment
                 last_pos = segment.end
                 pbar.update(increment)
 
         return dict(
             text=all_text,
             segments=list_segments,
-            language=language_name,
+            language=info.language,
         )
```

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,17 +141,19 @@
                         start = self.format_timestamp(this_word["start"])
                         end = self.format_timestamp(this_word["end"])
                         if last != start:
                             yield last, start, subtitle_text
 
                         yield start, end, "".join(
                             [
-                                re.sub(r"^(\s*)(.*)$", r"\1<u>\2</u>", word)
-                                if j == i
-                                else word
+                                (
+                                    re.sub(r"^(\s*)(.*)$", r"\1<u>\2</u>", word)
+                                    if j == i
+                                    else word
+                                )
                                 for j, word in enumerate(all_words)
                             ]
                         )
                         last = end
                 else:
                     yield subtitle_start, subtitle_end, subtitle_text
         else:
```

### Comparing `whisper-ctranslate2-0.4.2/tests/testdiarization.py` & `whisper-ctranslate2-0.4.3/tests/testdiarization.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/tests/testlive.py` & `whisper-ctranslate2-0.4.3/tests/testlive.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/tests/testwriters.py` & `whisper-ctranslate2-0.4.3/tests/testwriters.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: faster-whisper>=1.0.0
+Requires-Dist: faster-whisper>=1.0.2
 Requires-Dist: ctranslate2
 Requires-Dist: tqdm
 Requires-Dist: sounddevice
 Requires-Dist: numpy
 Provides-Extra: dev
-Requires-Dist: flake8==6.*; extra == "dev"
-Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: flake8==7.*; extra == "dev"
+Requires-Dist: black==24.*; extra == "dev"
 Requires-Dist: nose2; extra == "dev"
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
```

### Comparing `whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

