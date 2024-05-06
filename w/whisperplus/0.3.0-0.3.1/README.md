# Comparing `tmp/whisperplus-0.3.0.tar.gz` & `tmp/whisperplus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisperplus-0.3.0.tar", last modified: Sat May  4 15:26:15 2024, max compression
+gzip compressed data, was "whisperplus-0.3.1.tar", last modified: Sun May  5 21:41:23 2024, max compression
```

## Comparing `whisperplus-0.3.0.tar` & `whisperplus-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 15:26:15.432433 whisperplus-0.3.0/
--rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.3.0/LICENSE
--rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.3.0/MANIFEST.in
--rw-r--r--   0 kadirnar   (501) staff       (20)     6135 2024-05-04 15:26:15.432595 whisperplus-0.3.0/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)     5825 2024-05-04 15:18:34.000000 whisperplus-0.3.0/README.md
--rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 11:16:41.000000 whisperplus-0.3.0/requirements.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-04 15:26:15.432904 whisperplus-0.3.0/setup.cfg
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.3.0/setup.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 15:26:15.428460 whisperplus-0.3.0/whisperplus/
--rw-r--r--   0 kadirnar   (501) staff       (20)      658 2024-05-04 15:11:08.000000 whisperplus-0.3.0/whisperplus/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/app.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 15:26:15.431712 whisperplus-0.3.0/whisperplus/pipelines/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/autollm_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/lancedb_chatbot.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/long_text_summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/summarization.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.3.0/whisperplus/pipelines/text2speech.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     2753 2024-05-04 13:38:51.000000 whisperplus-0.3.0/whisperplus/pipelines/whisper.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/whisper_autocaption.py
--rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/pipelines/whisper_diarize.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1276 2024-05-04 13:38:51.000000 whisperplus-0.3.0/whisperplus/test.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 15:26:15.432308 whisperplus-0.3.0/whisperplus/utils/
--rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/utils/__init__.py
--rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/utils/download_utils.py
--rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.3.0/whisperplus/utils/text_utils.py
-drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-04 15:26:15.429365 whisperplus-0.3.0/whisperplus.egg-info/
--rw-r--r--   0 kadirnar   (501) staff       (20)     6135 2024-05-04 15:26:15.000000 whisperplus-0.3.0/whisperplus.egg-info/PKG-INFO
--rw-r--r--   0 kadirnar   (501) staff       (20)      760 2024-05-04 15:26:15.000000 whisperplus-0.3.0/whisperplus.egg-info/SOURCES.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-04 15:26:15.000000 whisperplus-0.3.0/whisperplus.egg-info/dependency_links.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 15:26:15.000000 whisperplus-0.3.0/whisperplus.egg-info/requires.txt
--rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-04 15:26:15.000000 whisperplus-0.3.0/whisperplus.egg-info/top_level.txt
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-05 21:41:23.501818 whisperplus-0.3.1/
+-rw-r--r--   0 kadirnar   (501) staff       (20)    11357 2024-04-29 20:18:01.000000 whisperplus-0.3.1/LICENSE
+-rw-r--r--   0 kadirnar   (501) staff       (20)       25 2024-04-29 20:18:01.000000 whisperplus-0.3.1/MANIFEST.in
+-rw-r--r--   0 kadirnar   (501) staff       (20)     6165 2024-05-05 21:41:23.501986 whisperplus-0.3.1/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5855 2024-05-05 21:41:11.000000 whisperplus-0.3.1/README.md
+-rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-04 11:16:41.000000 whisperplus-0.3.1/requirements.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      748 2024-05-05 21:41:23.502290 whisperplus-0.3.1/setup.cfg
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-29 20:18:01.000000 whisperplus-0.3.1/setup.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-05 21:41:23.498812 whisperplus-0.3.1/whisperplus/
+-rw-r--r--   0 kadirnar   (501) staff       (20)      736 2024-05-05 21:41:11.000000 whisperplus-0.3.1/whisperplus/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     7729 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/app.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2136 2024-05-05 21:41:11.000000 whisperplus-0.3.1/whisperplus/audio_eval.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-05 21:41:23.501341 whisperplus-0.3.1/whisperplus/pipelines/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3123 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/autollm_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     5543 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/lancedb_chatbot.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     2487 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/long_text_summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1380 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/summarization.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1751 2024-04-30 23:17:02.000000 whisperplus-0.3.1/whisperplus/pipelines/text2speech.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3208 2024-05-05 21:41:11.000000 whisperplus-0.3.1/whisperplus/pipelines/whisper.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     3492 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/whisper_autocaption.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)    10897 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/pipelines/whisper_diarize.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1276 2024-05-05 21:41:08.000000 whisperplus-0.3.1/whisperplus/test.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-05 21:41:23.501723 whisperplus-0.3.1/whisperplus/utils/
+-rw-r--r--   0 kadirnar   (501) staff       (20)        0 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/utils/__init__.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)     1403 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/utils/download_utils.py
+-rw-r--r--   0 kadirnar   (501) staff       (20)      532 2024-04-29 20:18:01.000000 whisperplus-0.3.1/whisperplus/utils/text_utils.py
+drwxr-xr-x   0 kadirnar   (501) staff       (20)        0 2024-05-05 21:41:23.499905 whisperplus-0.3.1/whisperplus.egg-info/
+-rw-r--r--   0 kadirnar   (501) staff       (20)     6165 2024-05-05 21:41:23.000000 whisperplus-0.3.1/whisperplus.egg-info/PKG-INFO
+-rw-r--r--   0 kadirnar   (501) staff       (20)      786 2024-05-05 21:41:23.000000 whisperplus-0.3.1/whisperplus.egg-info/SOURCES.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)        1 2024-05-05 21:41:23.000000 whisperplus-0.3.1/whisperplus.egg-info/dependency_links.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)      378 2024-05-05 21:41:23.000000 whisperplus-0.3.1/whisperplus.egg-info/requires.txt
+-rw-r--r--   0 kadirnar   (501) staff       (20)       12 2024-05-05 21:41:23.000000 whisperplus-0.3.1/whisperplus.egg-info/top_level.txt
```

### Comparing `whisperplus-0.3.0/LICENSE` & `whisperplus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/PKG-INFO` & `whisperplus-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.3.0
+Version: 0.3.1
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
+    WhisperPlus: Faster, Smarter, and More Capable 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -41,15 +41,15 @@
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
-
+import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
 
 hqq_config = HqqConfig(
     nbits=1,
     group_size=64,
@@ -63,16 +63,19 @@
     load_in_4bit=True,
     bnb_4bit_quant_type="nf4",
     bnb_4bit_compute_dtype=torch.bfloat16,
     bnb_4bit_use_double_quant=True,
 )
 
 pipeline = SpeechToTextPipeline(
-    model_id="distil-whisper/distil-large-v3", quant_config=hqq_config
-)  # or bnb_config
+    model_id="distil-whisper/distil-large-v3",
+    quant_config=hqq_config,
+    hqq=True,
+    flash_attention_2=True,
+)
 
 transcript = pipeline(
     audio_path=audio_path,
     chunk_length_s=30,
     stride_length_s=5,
     max_new_tokens=128,
     batch_size=100,
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.3.0 Summary: WhisperPlus: A
+Metadata-Version: 2.1 Name: whisperplus Version: 0.3.1 Summary: WhisperPlus: A
 Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
-  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
+        ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
 ## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
 huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
 ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
 huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
 library, follow the steps below for different tasks: ### ðµ Youtube URL to
 Audio ```python from whisperplus import SpeechToTextPipeline,
 download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
+audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
-quant_config=hqq_config ) # or bnb_config transcript = pipeline
-( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
+quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
+pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
 ```python from whisperplus import TextSummarizationPipeline summarizer =
 TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
 summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
 Long Text Support Summarization ```python from whisperplus import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
```

### Comparing `whisperplus-0.3.0/README.md` & `whisperplus-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
+    WhisperPlus: Faster, Smarter, and More Capable 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -30,15 +30,15 @@
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
-
+import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
 
 hqq_config = HqqConfig(
     nbits=1,
     group_size=64,
@@ -52,16 +52,19 @@
     load_in_4bit=True,
     bnb_4bit_quant_type="nf4",
     bnb_4bit_compute_dtype=torch.bfloat16,
     bnb_4bit_use_double_quant=True,
 )
 
 pipeline = SpeechToTextPipeline(
-    model_id="distil-whisper/distil-large-v3", quant_config=hqq_config
-)  # or bnb_config
+    model_id="distil-whisper/distil-large-v3",
+    quant_config=hqq_config,
+    hqq=True,
+    flash_attention_2=True,
+)
 
 transcript = pipeline(
     audio_path=audio_path,
     chunk_length_s=30,
     stride_length_s=5,
     max_new_tokens=128,
     batch_size=100,
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
+        ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
 ## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
 huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
 ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
 huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
 library, follow the steps below for different tasks: ### ðµ Youtube URL to
 Audio ```python from whisperplus import SpeechToTextPipeline,
 download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
+audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
-quant_config=hqq_config ) # or bnb_config transcript = pipeline
-( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
+quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
+pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
 ```python from whisperplus import TextSummarizationPipeline summarizer =
 TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
 summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
 Long Text Support Summarization ```python from whisperplus import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
```

### Comparing `whisperplus-0.3.0/setup.cfg` & `whisperplus-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/setup.py` & `whisperplus-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/__init__.py` & `whisperplus-0.3.1/whisperplus/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from whisper.pipelines.whisper_autocaption import WhisperAutoCaptionPipeline
+
 from whisperplus.pipelines.autollm_chatbot import AutoLLMChatWithVideo
 from whisperplus.pipelines.long_text_summarization import LongTextSummarizationPipeline
 from whisperplus.pipelines.summarization import TextSummarizationPipeline
 from whisperplus.pipelines.text2speech import TextToSpeechPipeline
 from whisperplus.pipelines.whisper import SpeechToTextPipeline
 from whisperplus.pipelines.whisper_diarize import ASRDiarizationPipeline
 from whisperplus.utils.download_utils import download_and_convert_to_mp3
 from whisperplus.utils.text_utils import format_speech_to_dialogue
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 __author__ = 'kadirnar'
 __license__ = 'Apache License 2.0'
```

### Comparing `whisperplus-0.3.0/whisperplus/app.py` & `whisperplus-0.3.1/whisperplus/app.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/autollm_chatbot.py` & `whisperplus-0.3.1/whisperplus/pipelines/autollm_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/lancedb_chatbot.py` & `whisperplus-0.3.1/whisperplus/pipelines/lancedb_chatbot.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/long_text_summarization.py` & `whisperplus-0.3.1/whisperplus/pipelines/long_text_summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/summarization.py` & `whisperplus-0.3.1/whisperplus/pipelines/summarization.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/text2speech.py` & `whisperplus-0.3.1/whisperplus/pipelines/text2speech.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/whisper.py` & `whisperplus-0.3.1/whisperplus/pipelines/whisper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 import logging
+from typing import Optional
 
 import torch
-from hqq.core.quantize import HQQBackend, HQQLinear
 from transformers import AutoModelForSpeechSeq2Seq, AutoProcessor, pipeline
 
-HQQLinear.set_backend(HQQBackend.PYTORCH)  # Pytorch backend
-HQQLinear.set_backend(HQQBackend.PYTORCH_COMPILE)  # Compiled Pytorch via dynamo
-HQQLinear.set_backend(HQQBackend.ATEN)  # C++ Aten/CUDA backend (set automatically by default if available)
-
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 class SpeechToTextPipeline:
     """Class for converting audio to text using a pre-trained speech recognition model."""
 
-    def __init__(self, model_id: str = "distil-whisper/distil-large-v3", quant_config=None):
+    def __init__(
+            self,
+            model_id: str = "distil-whisper/distil-large-v3",
+            quant_config=None,
+            hqq: Optional[bool] = True,
+            flash_attention_2: Optional[bool] = True):
         self.model = None
         self.device = None
+        self.hqq = hqq
+        self.flash_attention_2 = flash_attention_2
 
         if self.model is None:
             self.load_model(model_id)
         else:
             logging.info("Model already loaded.")
 
     def load_model(self, model_id: str = "distil-whisper/distil-large-v3", quant_config=None):
+        if self.hqq:
+            from hqq.core.quantize import HQQBackend, HQQLinear
+            HQQLinear.set_backend(HQQBackend.PYTORCH)  # Pytorch backend
+            HQQLinear.set_backend(HQQBackend.PYTORCH_COMPILE)  # Compiled Pytorch via dynamo
+            HQQLinear.set_backend(
+                HQQBackend.ATEN)  # C++ Aten/CUDA backend (set automatically by default if available)
+
+        if self.flash_attention_2:
+            attn_implementation = "flash_attention_2"
+        else:
+            attn_implementation = "sdpa"
+
         model = AutoModelForSpeechSeq2Seq.from_pretrained(
             model_id,
             quantization_config=quant_config,
             low_cpu_mem_usage=True,
             use_safetensors=True,
-            attn_implementation="flash_attention_2",
+            attn_implementation=attn_implementation,
             torch_dtype=torch.bfloat16,
             device_map='auto',
-            max_memory={0: "24GiB"})
+        )
         logging.info("Model loaded successfully.")
 
         processor = AutoProcessor.from_pretrained(model_id)
 
         self.processor = processor
         self.model = model
 
@@ -65,13 +80,13 @@
             chunk_length_s=chunk_length_s,
             stride_length_s=stride_length_s,
             max_new_tokens=max_new_tokens,
             batch_size=batch_size,
             return_timestamps=return_timestamps,
             tokenizer=self.processor.tokenizer,
             feature_extractor=self.processor.feature_extractor,
-            model_kwargs={"use_flash_attention_2": True},
+            model_kwargs={"use_flash_attention_2": self.flash_attention_2},
             generate_kwargs={"language": language},
         )
         logging.info("Transcribing audio...")
         result = pipe(audio_path)
         return result
```

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/whisper_autocaption.py` & `whisperplus-0.3.1/whisperplus/pipelines/whisper_autocaption.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/pipelines/whisper_diarize.py` & `whisperplus-0.3.1/whisperplus/pipelines/whisper_diarize.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/test.py` & `whisperplus-0.3.1/whisperplus/test.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/utils/download_utils.py` & `whisperplus-0.3.1/whisperplus/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus/utils/text_utils.py` & `whisperplus-0.3.1/whisperplus/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `whisperplus-0.3.0/whisperplus.egg-info/PKG-INFO` & `whisperplus-0.3.1/whisperplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: whisperplus
-Version: 0.3.0
+Version: 0.3.1
 Summary: WhisperPlus: A Python library for WhisperPlus API.
 Home-page: https://github.com/kadirnar/whisperplus
 Author: kadirnar
 Author-email: kadir.nar@hotmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h2>
-    WhisperPlus: Advancing Speech2Text and Text2Speech Feature 🚀
+    WhisperPlus: Faster, Smarter, and More Capable 🚀
 </h2>
 <div>
     <img width="500" alt="teaser" src="doc\openai-whisper.jpg">
 </div>
 <div>
     <a href="https://pypi.org/project/whisperplus" target="_blank">
         <img src="https://img.shields.io/pypi/pyversions/whisperplus.svg?color=%2334D058" alt="Supported Python versions">
@@ -41,15 +41,15 @@
 To use the whisperplus library, follow the steps below for different tasks:
 
 ### 🎵 Youtube URL to Audio
 
 ```python
 from whisperplus import SpeechToTextPipeline, download_and_convert_to_mp3
 from transformers import BitsAndBytesConfig, HqqConfig
-
+import torch
 
 url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
 audio_path = download_and_convert_to_mp3(url)
 
 hqq_config = HqqConfig(
     nbits=1,
     group_size=64,
@@ -63,16 +63,19 @@
     load_in_4bit=True,
     bnb_4bit_quant_type="nf4",
     bnb_4bit_compute_dtype=torch.bfloat16,
     bnb_4bit_use_double_quant=True,
 )
 
 pipeline = SpeechToTextPipeline(
-    model_id="distil-whisper/distil-large-v3", quant_config=hqq_config
-)  # or bnb_config
+    model_id="distil-whisper/distil-large-v3",
+    quant_config=hqq_config,
+    hqq=True,
+    flash_attention_2=True,
+)
 
 transcript = pipeline(
     audio_path=audio_path,
     chunk_length_s=30,
     stride_length_s=5,
     max_new_tokens=128,
     batch_size=100,
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: whisperplus Version: 0.3.0 Summary: WhisperPlus: A
+Metadata-Version: 2.1 Name: whisperplus Version: 0.3.1 Summary: WhisperPlus: A
 Python library for WhisperPlus API. Home-page: https://github.com/kadirnar/
 whisperplus Author: kadirnar Author-email: kadir.nar@hotmail.com License:
 Apache License 2.0 Description-Content-Type: text/markdown License-File:
 LICENSE
-  ********** WWhhiissppeerrPPlluuss:: AAddvvaanncciinngg SSppeeeecchh22TTeexxtt aanndd TTeexxtt22SSppeeeecchh FFeeaattuurree ?ð??? **********
+        ********** WWhhiissppeerrPPlluuss:: FFaasstteerr,, SSmmaarrtteerr,, aanndd MMoorree CCaappaabbllee ?ð??? **********
                                    [teaser]
          _[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_p_y_p_i_ _v_e_r_s_i_o_n_]_[_H_u_g_g_i_n_g_F_a_c_e_ _S_p_a_c_e_s_]
 ## ð ï¸ Installation ```bash pip install whisperplus git+https://github.com/
 huggingface/transformers pip install flash-attn --no-build-isolation ``` ##
 ð¤ Model Hub You can find the models on the [HuggingFace Model Hub](https://
 huggingface.co/models?search=whisper) ## ðï¸ Usage To use the whisperplus
 library, follow the steps below for different tasks: ### ðµ Youtube URL to
 Audio ```python from whisperplus import SpeechToTextPipeline,
 download_and_convert_to_mp3 from transformers import BitsAndBytesConfig,
-HqqConfig url = "https://www.youtube.com/watch?v=di3rHkEZuUw" audio_path =
-download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
+HqqConfig import torch url = "https://www.youtube.com/watch?v=di3rHkEZuUw"
+audio_path = download_and_convert_to_mp3(url) hqq_config = HqqConfig( nbits=1,
 group_size=64, quant_zero=False, quant_scale=False, axis=0, offload_meta=False,
 ) # axis=0 is used by default bnb_config = BitsAndBytesConfig
 ( load_in_4bit=True, bnb_4bit_quant_type="nf4",
 bnb_4bit_compute_dtype=torch.bfloat16, bnb_4bit_use_double_quant=True, )
 pipeline = SpeechToTextPipeline( model_id="distil-whisper/distil-large-v3",
-quant_config=hqq_config ) # or bnb_config transcript = pipeline
-( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
+quant_config=hqq_config, hqq=True, flash_attention_2=True, ) transcript =
+pipeline( audio_path=audio_path, chunk_length_s=30, stride_length_s=5,
 max_new_tokens=128, batch_size=100, language="english",
 return_timestamps=False, ) print(transcript) ``` ### ð° Summarization
 ```python from whisperplus import TextSummarizationPipeline summarizer =
 TextSummarizationPipeline(model_id="facebook/bart-large-cnn") summary =
 summarizer.summarize(transcript) print(summary[0]["summary_text"]) ``` ### ð°
 Long Text Support Summarization ```python from whisperplus import
 LongTextSummarizationPipeline summarizer = LongTextSummarizationPipeline
```

### Comparing `whisperplus-0.3.0/whisperplus.egg-info/SOURCES.txt` & `whisperplus-0.3.1/whisperplus.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 whisperplus/__init__.py
 whisperplus/app.py
+whisperplus/audio_eval.py
 whisperplus/test.py
 whisperplus.egg-info/PKG-INFO
 whisperplus.egg-info/SOURCES.txt
 whisperplus.egg-info/dependency_links.txt
 whisperplus.egg-info/requires.txt
 whisperplus.egg-info/top_level.txt
 whisperplus/pipelines/__init__.py
```

