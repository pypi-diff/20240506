# Comparing `tmp/agentkit-llm-0.1.6.post2.tar.gz` & `tmp/agentkit-llm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentkit-llm-0.1.6.post2.tar", last modified: Wed May  1 19:52:12 2024, max compression
+gzip compressed data, was "agentkit-llm-0.1.7.tar", last modified: Mon May  6 21:48:06 2024, max compression
```

## Comparing `agentkit-llm-0.1.6.post2.tar` & `agentkit-llm-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.6.post2/LICENSE
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8525 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     8035 2024-04-26 20:02:45.000000 agentkit-llm-0.1.6.post2/README.md
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/setup.cfg
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1001 2024-05-01 19:52:07.000000 agentkit-llm-0.1.6.post2/setup.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.248815 agentkit-llm-0.1.6.post2/src/
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.6.post2/src/agentkit/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.6.post2/src/agentkit/after_query.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-04-14 12:48:55.000000 agentkit-llm-0.1.6.post2/src/agentkit/base_node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.6.post2/src/agentkit/compose_prompt.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.6.post2/src/agentkit/exceptions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.6.post2/src/agentkit/graph.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-01 19:51:25.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/GPT.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1479 2024-04-08 11:11:53.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/__init__.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     3992 2024-04-24 17:36:07.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/base.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/claude.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     1473 2024-04-22 15:26:27.000000 agentkit-llm-0.1.6.post2/src/agentkit/llm_api/utils.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.6.post2/src/agentkit/node.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.6.post2/src/agentkit/node_functions.py
--rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.6.post2/src/agentkit/utils.py
-drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-01 19:52:12.252815 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/
--rw-r--r--   0 holmes    (1000) holmes    (1000)     8525 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/PKG-INFO
--rw-rw-r--   0 holmes    (1000) holmes    (1000)      652 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/entry_points.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)       71 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/requires.txt
--rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-01 19:52:12.000000 agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/top_level.txt
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    18656 2024-04-10 02:29:46.000000 agentkit-llm-0.1.7/LICENSE
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9016 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     8505 2024-05-06 21:46:13.000000 agentkit-llm-0.1.7/README.md
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       38 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/setup.cfg
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1068 2024-05-06 21:33:58.000000 agentkit-llm-0.1.7/setup.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.237146 agentkit-llm-0.1.7/src/
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      191 2024-04-14 12:48:14.000000 agentkit-llm-0.1.7/src/agentkit/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2951 2024-04-29 05:28:17.000000 agentkit-llm-0.1.7/src/agentkit/after_query.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     9580 2024-05-06 21:44:02.000000 agentkit-llm-0.1.7/src/agentkit/base_node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     6649 2024-04-08 08:17:28.000000 agentkit-llm-0.1.7/src/agentkit/compose_prompt.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      621 2024-04-08 07:53:38.000000 agentkit-llm-0.1.7/src/agentkit/exceptions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)    14727 2024-04-08 11:31:02.000000 agentkit-llm-0.1.7/src/agentkit/graph.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit/llm_api/
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4799 2024-05-06 21:41:05.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/GPT.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1726 2024-05-06 21:26:12.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/__init__.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4226 2024-05-06 21:20:24.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/base.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     4615 2024-04-24 17:43:52.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/claude.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     3782 2024-05-06 21:32:28.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/ollama.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     1613 2024-05-06 21:24:37.000000 agentkit-llm-0.1.7/src/agentkit/llm_api/utils.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2319 2024-04-14 12:49:05.000000 agentkit-llm-0.1.7/src/agentkit/node.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      488 2024-04-08 07:54:08.000000 agentkit-llm-0.1.7/src/agentkit/node_functions.py
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)     2213 2024-04-14 12:47:12.000000 agentkit-llm-0.1.7/src/agentkit/utils.py
+drwxrwxr-x   0 holmes    (1000) holmes    (1000)        0 2024-05-06 21:48:06.241146 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/
+-rw-r--r--   0 holmes    (1000) holmes    (1000)     9016 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/PKG-INFO
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      683 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/SOURCES.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        1 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/dependency_links.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)       51 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/entry_points.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)      124 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/requires.txt
+-rw-rw-r--   0 holmes    (1000) holmes    (1000)        9 2024-05-06 21:48:06.000000 agentkit-llm-0.1.7/src/agentkit_llm.egg-info/top_level.txt
```

### Comparing `agentkit-llm-0.1.6.post2/LICENSE` & `agentkit-llm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/PKG-INFO` & `agentkit-llm-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6.post2
+Version: 0.1.7
 Summary: A LLM prompting framework for LLM agents
-Home-page: https://github.com/Holmeswww/AgentKit
+Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: logging
+Provides-Extra: proprietary
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
@@ -59,15 +60,21 @@
 
 To install AgentKit with wandb:
 
 ```bash
 pip install agentkit-llm[logging]
 ```
 
-To install AgentKit with built-in LLM-API support:
+To install AgentKit with OpenAI and Claude LLM-API support:
+
+```bash
+pip install agentkit-llm[proprietary]
+```
+
+To install AgentKit with full built-in LLM-API support (including llama):
 
 ```bash
 pip install agentkit-llm[all]
 ```
 
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
@@ -122,24 +129,30 @@
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
 # Built-in LLM-API
 
-The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+The built-in `agentkit.llm_api` functions require installing with `[proprietary]` or `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
 To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
 
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
+To use Ollama models, see https://github.com/ollama/ollama for installation instructions. Then set `OLLAMA_URL` and `OLLAMA_TOKENIZER_PATH`, or store `OLLAMA_TOKENIZER_PATH`, `OLLAMA_URL` in the first 2 lines of `~/.ollama/ollama_model.info`.
+
+```
+LLM_API_FUNCTION = agentkit.llm_api.get_query("ollama-llama3")
+```
+
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
 
 Finally, run the following to evoke the command line interface (CLI):
```

### Comparing `agentkit-llm-0.1.6.post2/README.md` & `agentkit-llm-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,21 @@
 
 To install AgentKit with wandb:
 
 ```bash
 pip install agentkit-llm[logging]
 ```
 
-To install AgentKit with built-in LLM-API support:
+To install AgentKit with OpenAI and Claude LLM-API support:
+
+```bash
+pip install agentkit-llm[proprietary]
+```
+
+To install AgentKit with full built-in LLM-API support (including llama):
 
 ```bash
 pip install agentkit-llm[all]
 ```
 
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
@@ -107,24 +113,30 @@
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
 # Built-in LLM-API
 
-The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+The built-in `agentkit.llm_api` functions require installing with `[proprietary]` or `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
 To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
 
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
+To use Ollama models, see https://github.com/ollama/ollama for installation instructions. Then set `OLLAMA_URL` and `OLLAMA_TOKENIZER_PATH`, or store `OLLAMA_TOKENIZER_PATH`, `OLLAMA_URL` in the first 2 lines of `~/.ollama/ollama_model.info`.
+
+```
+LLM_API_FUNCTION = agentkit.llm_api.get_query("ollama-llama3")
+```
+
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
 
 Finally, run the following to evoke the command line interface (CLI):
```

### Comparing `agentkit-llm-0.1.6.post2/setup.py` & `agentkit-llm-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 import pkg_resources
 import pathlib
 
 PKG_NAME = "agentkit-llm"
-VERSION = "0.1.6.post2"
+VERSION = "0.1.7"
 EXTRAS = {
     "logging": ["wandb"],
-    "all": ["wandb", "openai", "anthropic", "tiktoken"],
+    "proprietary": ["wandb", "openai", "anthropic", "tiktoken"],
+    "all": ["wandb", "openai", "anthropic", "tiktoken", "llama"],
 }
 
 setuptools.setup(
     name=PKG_NAME,
     version=VERSION,
     author="AgentKit Team",
     description='A LLM prompting framework for LLM agents',
-    url="https://github.com/Holmeswww/AgentKit",
+    url="https://github.com/rhyswynn/AgentKit",
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=setuptools.find_namespace_packages('src'),
     package_dir={'': 'src'},
     entry_points={'console_scripts': ['agentkit=agentkit.run_gui:main']},
     install_requires = ['colorama', 'numpy'],
     extras_require=EXTRAS,
```

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/after_query.py` & `agentkit-llm-0.1.7/src/agentkit/after_query.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/base_node.py` & `agentkit-llm-0.1.7/src/agentkit/base_node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/compose_prompt.py` & `agentkit-llm-0.1.7/src/agentkit/compose_prompt.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/exceptions.py` & `agentkit-llm-0.1.7/src/agentkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/graph.py` & `agentkit-llm-0.1.7/src/agentkit/graph.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/GPT.py` & `agentkit-llm-0.1.7/src/agentkit/llm_api/GPT.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/base.py` & `agentkit-llm-0.1.7/src/agentkit/llm_api/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
     def __init__(self, model_name, global_conter=None, model_type = "chat"):
         self.name = model_name
         assert model_type in ["chat", "completion"], "type should be either 'chat' or 'completion'"
         self.type = model_type
         self.global_counter = global_conter
         self.debug = False
+        if self.global_counter is not None:
+            self.global_counter["token_completion"][self.name] = 0
+            self.global_counter["token_prompt"][self.name] = 0
+            self.global_counter["api_calls"][self.name] = 0
     
     def query_chat(self, messages, shrink_idx, model, max_gen=1024, temp=0.):
         raise NotImplementedError
     
     def query_completion(self, messages, shrink_idx, model, max_gen=1024, temp=0.):
         raise NotImplementedError
```

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/claude.py` & `agentkit-llm-0.1.7/src/agentkit/llm_api/claude.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/llm_api/utils.py` & `agentkit-llm-0.1.7/src/agentkit/llm_api/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,37 @@
     "gpt-4-1106-preview":tiktoken.encoding_for_model("gpt-4"),
     "gpt-4-32k-0613":tiktoken.encoding_for_model("gpt-4"),
     "gpt-3.5-turbo":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "gpt-3.5-turbo-1106":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "gpt-3.5-turbo-0125":tiktoken.encoding_for_model("gpt-3.5-turbo"),
     "claude-3": None,
     "claude-2.1": None,
+    "ollama": None,
 }
 model_maxes = {
     "gpt-4":8192,
     "gpt-4-turbo":128000,
     "gpt-4-1106-preview":128000,
     "gpt-4-32k-0613":32768,
     "gpt-3.5-turbo":16385,
     "gpt-3.5-turbo-1106":16385,
     "gpt-3.5-turbo-0125":16385,
     "claude-3":50000,
     "claude-2.1":50000,
+    "ollama":8192,
 }
 
 def match_model(model_name):
 
     # match model name to the closest string in enc_fns.keys()
     model_name = model_name.lower()
     matches = difflib.get_close_matches(model_name, enc_fns.keys())
-    print("Matched model name to: ", matches)
     matches += [model for model in model_maxes.keys() if model_name.startswith(model)]
     if len(matches) == 0:
         raise ValueError("Model name {} not found!".format(model_name))
     else:
         model = matches[0]
-    
+    print("Matched model_name {} to: {}. If this match is not accurate, then the token counter will not function properly.".format(model_name, model))
+
     model_max = model_maxes[model]
     enc_fn = enc_fns[model]
     return model_max, enc_fn
```

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/node.py` & `agentkit-llm-0.1.7/src/agentkit/node.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit/utils.py` & `agentkit-llm-0.1.7/src/agentkit/utils.py`

 * *Files identical despite different names*

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/PKG-INFO` & `agentkit-llm-0.1.7/src/agentkit_llm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: agentkit-llm
-Version: 0.1.6.post2
+Version: 0.1.7
 Summary: A LLM prompting framework for LLM agents
-Home-page: https://github.com/Holmeswww/AgentKit
+Home-page: https://github.com/rhyswynn/AgentKit
 Author: AgentKit Team
 License: CC-BY-4.0-Attribution
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: logging
+Provides-Extra: proprietary
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="center">
 <img src="https://github.com/Holmeswww/AgentKit/raw/main/imgs/AgentKit.png" width="350px">
 
 **AgentKit: Flow Engineering with Graphs, not Coding**
@@ -59,15 +60,21 @@
 
 To install AgentKit with wandb:
 
 ```bash
 pip install agentkit-llm[logging]
 ```
 
-To install AgentKit with built-in LLM-API support:
+To install AgentKit with OpenAI and Claude LLM-API support:
+
+```bash
+pip install agentkit-llm[proprietary]
+```
+
+To install AgentKit with full built-in LLM-API support (including llama):
 
 ```bash
 pip install agentkit-llm[all]
 ```
 
 Otherwise, to install the cutting edge version from the main branch of this repo, run:
 
@@ -122,24 +129,30 @@
     'prompt': $prompt token counts,
     'completion': $completion token counts,
 }
 ```
 
 # Built-in LLM-API
 
-The built-in `agentkit.llm_api` functions require installing with `[all]` setting. See [the installation guide](#Installation) for details.
+The built-in `agentkit.llm_api` functions require installing with `[proprietary]` or `[all]` setting. See [the installation guide](#Installation) for details.
 
 Currently, the built-in API supports OpenAI and Anthropic, see https://pypi.org/project/openai/ and https://pypi.org/project/anthropic/ for details.
 
 To use the OpenAI models, set environment variables `OPENAI_KEY` and `OPENAI_ORG`. Alternatively, you can put the openai 'key' and 'organization' in the first 2 lines of `~/.openai/openai.key`.
 
 To use the Azure OpenAI models, set environment variables `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_API_VERSION`, `AZURE_OPENAI_ENDPOINT`, and `AZURE_DEPLOYMENT_NAME`. Alternatively, you can store the Azure OpenAI API key, API version, Azure endpoint, and deployment name in the first 4 lines of `~/.openai/azure_openai.key`.
 
 To use the Anthropic models, set environment variable `ANTHROPIC_KEY`. Alternatively, you can put the anthropic 'key' in 3rd line of `~/.openai/openai.key`.
 
+To use Ollama models, see https://github.com/ollama/ollama for installation instructions. Then set `OLLAMA_URL` and `OLLAMA_TOKENIZER_PATH`, or store `OLLAMA_TOKENIZER_PATH`, `OLLAMA_URL` in the first 2 lines of `~/.ollama/ollama_model.info`.
+
+```
+LLM_API_FUNCTION = agentkit.llm_api.get_query("ollama-llama3")
+```
+
 # Using AgentKit without Programming Experience
 
 First, follow [the installation guide](#Installation) to install AgentKit with `[all]` setting.
 
 Then, set environment variables `OPENAI_KEY` and `OPENAI_ORG` to be your OpenAI key and org_key.
 
 Finally, run the following to evoke the command line interface (CLI):
```

### Comparing `agentkit-llm-0.1.6.post2/src/agentkit_llm.egg-info/SOURCES.txt` & `agentkit-llm-0.1.7/src/agentkit_llm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/agentkit/node.py
 src/agentkit/node_functions.py
 src/agentkit/utils.py
 src/agentkit/llm_api/GPT.py
 src/agentkit/llm_api/__init__.py
 src/agentkit/llm_api/base.py
 src/agentkit/llm_api/claude.py
+src/agentkit/llm_api/ollama.py
 src/agentkit/llm_api/utils.py
 src/agentkit_llm.egg-info/PKG-INFO
 src/agentkit_llm.egg-info/SOURCES.txt
 src/agentkit_llm.egg-info/dependency_links.txt
 src/agentkit_llm.egg-info/entry_points.txt
 src/agentkit_llm.egg-info/requires.txt
 src/agentkit_llm.egg-info/top_level.txt
```

