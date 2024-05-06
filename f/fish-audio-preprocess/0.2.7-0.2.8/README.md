# Comparing `tmp/fish_audio_preprocess-0.2.7.tar.gz` & `tmp/fish_audio_preprocess-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_audio_preprocess-0.2.7.tar", last modified: Tue Apr 16 07:01:58 2024, max compression
+gzip compressed data, was "fish_audio_preprocess-0.2.8.tar", last modified: Mon May  6 00:52:39 2024, max compression
```

## Comparing `fish_audio_preprocess-0.2.7.tar` & `fish_audio_preprocess-0.2.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.096560 fish_audio_preprocess-0.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.096560 fish_audio_preprocess-0.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/README.zh.md
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fap-complete.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.100560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.100560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/convert_to_wav.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/loudness_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/merge_short.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/separate_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/slice_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/loudness_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/separate_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 07:01:58.000000 fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:01:58.104560 fish_audio_preprocess-0.2.7/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-16 06:57:45.000000 fish_audio_preprocess-0.2.7/tools/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.824476 fish_audio_preprocess-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.828476 fish_audio_preprocess-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/README.zh.md
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fap-complete.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.828476 fish_audio_preprocess-0.2.8/fish_audio_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/convert_to_wav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/loudness_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/merge_short.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/separate_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/slice_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/loudness_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/separate_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/slice_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9832 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/slice_audio_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 00:52:39.000000 fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:52:39.832476 fish_audio_preprocess-0.2.8/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 00:50:25.000000 fish_audio_preprocess-0.2.8/tools/lint.py
```

### Comparing `fish_audio_preprocess-0.2.7/.github/workflows/ci.yml` & `fish_audio_preprocess-0.2.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/.gitignore` & `fish_audio_preprocess-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/LICENSE` & `fish_audio_preprocess-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/PKG-INFO` & `fish_audio_preprocess-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.2.7
+Version: 0.2.8
 Summary: Preprocess audio data
 Author-email: Lengyue <lengyue@lengyue.me>
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
```

### Comparing `fish_audio_preprocess-0.2.7/README.md` & `fish_audio_preprocess-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/README.zh.md` & `fish_audio_preprocess-0.2.8/README.zh.md`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fap-complete.zsh` & `fish_audio_preprocess-0.2.8/fap-complete.zsh`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/__main__.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/convert_to_wav.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/convert_to_wav.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/frequency.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/frequency.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/length.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/length.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,108 @@
-from concurrent.futures import ProcessPoolExecutor
+from functools import partial
+from multiprocessing import Pool
 from pathlib import Path
 from typing import Optional
 
 import click
 from loguru import logger
 from tqdm import tqdm
 
 from fish_audio_preprocess.utils.file import AUDIO_EXTENSIONS, list_files
 
 
 def process_one(file, input_dir):
     import soundfile as sf
 
-    sound = sf.SoundFile(str(file))
+    try:
+        sound = sf.SoundFile(str(file))
+    except Exception as e:
+        logger.warning(f"Error reading {file}: {e}")
+        return None
+
     return (
         len(sound),
         sound.samplerate,
         len(sound) / sound.samplerate,
         file.relative_to(input_dir),
     )
 
 
+def process_one_accurate(file, input_dir):
+    import torchaudio
+
+    try:
+        y, sr = torchaudio.load(str(file), backend="sox")
+        return y.size(-1), sr, y.size(-1) / sr, file.relative_to(input_dir)
+    except Exception as e:
+        logger.warning(f"Error reading {file}: {e}")
+        return None
+
+
 @click.command()
 @click.argument("input_dir", type=click.Path(exists=True, file_okay=False))
 @click.option("--recursive/--no-recursive", default=True, help="Search recursively")
 @click.option(
     "--visualize/--no-visualize", default=False, help="Visualize the distribution"
 )
 @click.option(
+    "--accurate/--no-accurate",
+    default=False,
+    help="Use accurate mode for duration calculation",
+)
+@click.option(
     "-l", "--long-threshold", default=None, type=float, help="Threshold for long files"
 )
 @click.option(
     "-s",
     "--short-threshold",
     default=None,
     type=float,
     help="Threshold for short files",
 )
+@click.option(
+    "-w",
+    "--num-workers",
+    default=10,
+    type=int,
+    help="Number of workers for parallel processing",
+)
 def length(
     input_dir: str,
     recursive: bool,
     visualize: bool,
+    accurate: bool,
     long_threshold: Optional[float],
     short_threshold: Optional[float],
+    num_workers: int,
 ):
     """
     Get the length of all audio files in a directory
     """
-    import soundfile as sf
     from matplotlib import pyplot as plt
 
     input_dir = Path(input_dir)
     files = list_files(input_dir, AUDIO_EXTENSIONS, recursive=recursive)
     logger.info(f"Found {len(files)} files, calculating length")
 
     infos = []
+    process_one_partial = partial(
+        process_one_accurate if accurate else process_one, input_dir=input_dir
+    )
+
+    with Pool(processes=num_workers) as executor:
+        for res in tqdm(
+            executor.imap_unordered(process_one_partial, files),
+            total=len(files),
+            desc="Processing",
+        ):
+            if res is None:
+                continue
 
-    with ProcessPoolExecutor(max_workers=10) as executor:
-        tasks = []
-        for file in tqdm(files, desc="Preparing"):
-            tasks.append(executor.submit(process_one, file, input_dir))
-        for task in tqdm(tasks, desc="Processing"):
-            infos.append(task.result())
+            infos.append(res)
 
     # Duration
     total_duration = sum(i[2] for i in infos)
     avg_duration = total_duration / len(infos)
     logger.info(f"Total duration: {total_duration / 3600:.2f} hours")
     logger.info(f"Average duration: {avg_duration:.2f} seconds")
     logger.info(f"Max duration: {max(i[2] for i in infos):.2f} seconds")
```

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/loudness_norm.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/merge_short.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/merge_short.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/resample.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/resample.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/separate_audio.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/slice_audio.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/slice_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/cli/transcribe.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/cli/transcribe.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/file.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/file.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/loudness_norm.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/loudness_norm.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/separate_audio.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/separate_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/slice_audio.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/slice_audio_v2.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/slice_audio_v2.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess/utils/transcribe.py` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess/utils/transcribe.py`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/PKG-INFO` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fish-audio-preprocess
-Version: 0.2.7
+Version: 0.2.8
 Summary: Preprocess audio data
 Author-email: Lengyue <lengyue@lengyue.me>
 License: Apache
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm>=4.64.1
```

### Comparing `fish_audio_preprocess-0.2.7/fish_audio_preprocess.egg-info/SOURCES.txt` & `fish_audio_preprocess-0.2.8/fish_audio_preprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fish_audio_preprocess-0.2.7/pyproject.toml` & `fish_audio_preprocess-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "openai-whisper",
 ]
 description = "Preprocess audio data"
 license = {text = "Apache"}
 name = "fish-audio-preprocess"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.2.7"
+version = "0.2.8"
 
 [project.scripts]
 fap = "fish_audio_preprocess.cli.__main__:cli"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

