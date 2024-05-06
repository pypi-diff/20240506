# Comparing `tmp/nagatoai_core-0.7.0.tar.gz` & `tmp/nagatoai_core-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagatoai_core-0.7.0.tar", max compression
+gzip compressed data, was "nagatoai_core-0.8.0.tar", max compression
```

## Comparing `nagatoai_core-0.7.0.tar` & `nagatoai_core-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.7.0/LICENSE
--rw-r--r--   0        0        0     8094 2024-04-29 06:24:03.515213 nagatoai_core-0.7.0/README.md
--rw-r--r--   0        0        0     3007 2024-04-11 04:55:58.042433 nagatoai_core-0.7.0/nagatoai_core/agent/agent.py
--rw-r--r--   0        0        0    10086 2024-04-16 03:58:07.727447 nagatoai_core-0.7.0/nagatoai_core/agent/anthropic.py
--rw-r--r--   0        0        0     8372 2024-04-29 06:24:03.515970 nagatoai_core-0.7.0/nagatoai_core/agent/groq.py
--rw-r--r--   0        0        0     1128 2024-04-11 04:55:58.043642 nagatoai_core-0.7.0/nagatoai_core/agent/message.py
--rw-r--r--   0        0        0     8515 2024-04-18 05:28:06.141468 nagatoai_core-0.7.0/nagatoai_core/agent/openai.py
--rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.7.0/nagatoai_core/mission/mission.py
--rw-r--r--   0        0        0     2280 2024-04-11 04:55:58.044144 nagatoai_core-0.7.0/nagatoai_core/mission/task.py
--rw-r--r--   0        0        0    29235 2024-04-16 03:58:07.728448 nagatoai_core-0.7.0/nagatoai_core/prompt/templates.py
--rw-r--r--   0        0        0     1007 2024-04-11 04:55:58.044929 nagatoai_core-0.7.0/nagatoai_core/tool/abstract_tool.py
--rw-r--r--   0        0        0     1330 2024-04-18 05:28:06.141811 nagatoai_core-0.7.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py
--rw-r--r--   0        0        0     1280 2024-04-16 03:58:07.728840 nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/confirm.py
--rw-r--r--   0        0        0     1138 2024-04-16 03:58:07.729054 nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/input.py
--rw-r--r--   0        0        0      443 2024-04-16 03:58:07.729329 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/base_config.py
--rw-r--r--   0        0        0     3264 2024-04-16 03:58:07.729584 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_finder.py
--rw-r--r--   0        0        0     2550 2024-04-16 03:58:07.729869 nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py
--rw-r--r--   0        0        0     2150 2024-04-18 05:28:06.142322 nagatoai_core-0.7.0/nagatoai_core/tool/lib/web/page_scraper.py
--rw-r--r--   0        0        0     1441 2024-04-11 04:55:58.046686 nagatoai_core-0.7.0/nagatoai_core/tool/provider/abstract_tool_provider.py
--rw-r--r--   0        0        0     1755 2024-04-11 04:55:58.046901 nagatoai_core-0.7.0/nagatoai_core/tool/provider/anthropic.py
--rw-r--r--   0        0        0     1869 2024-04-16 03:58:07.730257 nagatoai_core-0.7.0/nagatoai_core/tool/provider/openai.py
--rw-r--r--   0        0        0     1247 2024-04-11 04:55:58.047121 nagatoai_core-0.7.0/nagatoai_core/tool/registry.py
--rw-r--r--   0        0        0     2574 2024-04-11 04:55:58.047983 nagatoai_core-0.7.0/nagatoai_core/tool/schema.py
--rw-r--r--   0        0        0      663 2024-04-29 06:24:03.516380 nagatoai_core-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8921 1970-01-01 00:00:00.000000 nagatoai_core-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-31 11:58:01.266545 nagatoai_core-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8021 2024-05-06 13:49:33.332054 nagatoai_core-0.8.0/README.md
+-rw-r--r--   0        0        0     3007 2024-05-02 15:43:56.742277 nagatoai_core-0.8.0/nagatoai_core/agent/agent.py
+-rw-r--r--   0        0        0    10086 2024-04-16 03:58:07.727447 nagatoai_core-0.8.0/nagatoai_core/agent/anthropic.py
+-rw-r--r--   0        0        0     1252 2024-05-06 13:49:33.332749 nagatoai_core-0.8.0/nagatoai_core/agent/factory.py
+-rw-r--r--   0        0        0     8372 2024-04-29 06:24:03.515970 nagatoai_core-0.8.0/nagatoai_core/agent/groq.py
+-rw-r--r--   0        0        0     1128 2024-04-11 04:55:58.043642 nagatoai_core-0.8.0/nagatoai_core/agent/message.py
+-rw-r--r--   0        0        0     8515 2024-04-18 05:28:06.141468 nagatoai_core-0.8.0/nagatoai_core/agent/openai.py
+-rw-r--r--   0        0        0     1009 2024-04-01 06:39:30.733021 nagatoai_core-0.8.0/nagatoai_core/mission/mission.py
+-rw-r--r--   0        0        0     2280 2024-04-11 04:55:58.044144 nagatoai_core-0.8.0/nagatoai_core/mission/task.py
+-rw-r--r--   0        0        0    29235 2024-04-16 03:58:07.728448 nagatoai_core-0.8.0/nagatoai_core/prompt/templates.py
+-rw-r--r--   0        0        0     1007 2024-04-11 04:55:58.044929 nagatoai_core-0.8.0/nagatoai_core/tool/abstract_tool.py
+-rw-r--r--   0        0        0     1330 2024-04-18 05:28:06.141811 nagatoai_core-0.8.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py
+-rw-r--r--   0        0        0     1280 2024-04-16 03:58:07.728840 nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/confirm.py
+-rw-r--r--   0        0        0     1138 2024-04-16 03:58:07.729054 nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/input.py
+-rw-r--r--   0        0        0      443 2024-04-16 03:58:07.729329 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/base_config.py
+-rw-r--r--   0        0        0     3264 2024-04-16 03:58:07.729584 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_finder.py
+-rw-r--r--   0        0        0     2550 2024-04-16 03:58:07.729869 nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py
+-rw-r--r--   0        0        0     2150 2024-04-18 05:28:06.142322 nagatoai_core-0.8.0/nagatoai_core/tool/lib/web/page_scraper.py
+-rw-r--r--   0        0        0     1441 2024-04-11 04:55:58.046686 nagatoai_core-0.8.0/nagatoai_core/tool/provider/abstract_tool_provider.py
+-rw-r--r--   0        0        0     1755 2024-04-11 04:55:58.046901 nagatoai_core-0.8.0/nagatoai_core/tool/provider/anthropic.py
+-rw-r--r--   0        0        0     1869 2024-04-16 03:58:07.730257 nagatoai_core-0.8.0/nagatoai_core/tool/provider/openai.py
+-rw-r--r--   0        0        0     1247 2024-04-11 04:55:58.047121 nagatoai_core-0.8.0/nagatoai_core/tool/registry.py
+-rw-r--r--   0        0        0     2574 2024-04-11 04:55:58.047983 nagatoai_core-0.8.0/nagatoai_core/tool/schema.py
+-rw-r--r--   0        0        0      663 2024-05-06 13:49:33.333011 nagatoai_core-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 nagatoai_core-0.8.0/PKG-INFO
```

### Comparing `nagatoai_core-0.7.0/LICENSE` & `nagatoai_core-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/README.md` & `nagatoai_core-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -44,54 +44,52 @@
 * GPT-3 to GPT-4 (OpenAI)
 * Groq (which gives you access to Llama 3) 🔥
 
 ## Examples of AI Agent configuration
 
 Nagato is built with flexibility at its core, so you could program it using your paradigm of choice. However these are some of the ways I've seen people use Nagato so far.
 
+By default Nagato expects all LLM API keys to be set as environment variables. Nagato may load the keys from the following variables:
+
+```
+OPENAI_API_KEY=<api-key>
+ANTHROPIC_API_KEY=<api-key>
+READWISE_API_KEY=<api-key>
+```
+
 ### Coordinator, worker, and critic agents
 
 In this configuration we have the following:
 
 * 🎯 Coordinator: breaks down a problem statement (from stdin) into an objective and suggests tasks
 * 📚 Researcher: works on a task by performing research
 * ✅ Critic: evaluates whether the task was completed
 
 Example setup for this configuration could look like this:
 
 ```python
-openai_client = OpenAI(
-    organization="<org-id>",
-    api_key="<api-key>",
-)
-
-anthropic_api_key = "<api-key>"
-anthropic_client = Anthropic(api_key=anthropic_api_key)
-
-groq_client = Groq(api_key="<api-key>")
-
-coordinator_agent: Agent = AnthropicAgent(
-    anthropic_client,
+coordinator_agent: Agent = create_agent(
+    anthropic_api_key,
     "claude-3-opus-20240229",
     "Coordinator",
     COORDINATOR_SYSTEM_PROMPT,
     "Coordinator Agent",
 )
 
-researcher_agent: Agent = OpenAIAgent(
-    openai_client,
+researcher_agent = create_agent(
+    anthropic_api_key,
     "gpt-4-turbo-2024-04-09",
     "Researcher",
     RESEARCHER_SYSTEM_PROMPT,
     "Researcher Agent",
 )
 
-critic_agent: Agent = GroqAgent(
-    groq_client,
-    "llama3-70b-8192",
+critic_agent = create_agent(
+    anthropic_api_key,
+    "claude-3-haiku-20240307",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
 ...
 ```
 
@@ -109,28 +107,25 @@
         goal="Fetch last 100 user tweets",
         description="Fetch the tweets from the user using the Twitter API. Limit the number of tweets fetched to 100 only."),
     Task(
         goal="Perform sentiment analysis on the tweets",
         description="Feed the tweets to the AI Agent to analyze sentiment per overall sentiment acoss tweets. Range of values for sentiment can be: Positive, Negative, or Neutral"
     )]
 
-anthropic_api_key = "<api-key>"
-anthropic_client = Anthropic(api_key=anthropic_api_key)
-
-researcher_agent: Agent = AnthropicAgent(
-    anthropic_client,
+coordinator_agent: Agent = create_agent(
+    anthropic_api_key,
     "claude-3-sonnet-20240229",
-    "Researcher",
-    RESEARCHER_SYSTEM_PROMPT,
-    "Researcher Agent",
+    "Coordinator",
+    COORDINATOR_SYSTEM_PROMPT,
+    "Coordinator Agent",
 )
 
-critic_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-opus-20240229",
+critic_agent = create_agent(
+    anthropic_api_key,
+    "claude-3-haiku-20240307",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
 
 for task in task_list:
     # Insert the task into the prompt
```

### Comparing `nagatoai_core-0.7.0/nagatoai_core/agent/agent.py` & `nagatoai_core-0.8.0/nagatoai_core/agent/agent.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/agent/anthropic.py` & `nagatoai_core-0.8.0/nagatoai_core/agent/anthropic.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/agent/groq.py` & `nagatoai_core-0.8.0/nagatoai_core/agent/groq.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/agent/message.py` & `nagatoai_core-0.8.0/nagatoai_core/agent/message.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/agent/openai.py` & `nagatoai_core-0.8.0/nagatoai_core/agent/openai.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/mission/mission.py` & `nagatoai_core-0.8.0/nagatoai_core/mission/mission.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/mission/task.py` & `nagatoai_core-0.8.0/nagatoai_core/mission/task.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/prompt/templates.py` & `nagatoai_core-0.8.0/nagatoai_core/prompt/templates.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/abstract_tool.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/abstract_tool.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/filesystem/text_file_reader.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/confirm.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/confirm.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/human/input.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/human/input.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_finder.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_finder.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/readwise/book_highlights_lister.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/lib/web/page_scraper.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/lib/web/page_scraper.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/provider/abstract_tool_provider.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/provider/abstract_tool_provider.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/provider/anthropic.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/provider/anthropic.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/provider/openai.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/provider/openai.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/registry.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/registry.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/nagatoai_core/tool/schema.py` & `nagatoai_core-0.8.0/nagatoai_core/tool/schema.py`

 * *Files identical despite different names*

### Comparing `nagatoai_core-0.7.0/pyproject.toml` & `nagatoai_core-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nagatoai_core"
-version = "0.7.0"
+version = "0.8.0"
 description = "Nagato-AI is an intuitive AI Agent library that works across multiple LLMs"
 authors = ["Eddie Forson <eddie@edforson.me>"]
 readme = "README.md"
 package-mode = true
 exclude = [
     ".env",
     ".env.*",
```

### Comparing `nagatoai_core-0.7.0/PKG-INFO` & `nagatoai_core-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagatoai_core
-Version: 0.7.0
+Version: 0.8.0
 Summary: Nagato-AI is an intuitive AI Agent library that works across multiple LLMs
 Author: Eddie Forson
 Author-email: eddie@edforson.me
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.1,<0.24.0)
@@ -66,54 +66,52 @@
 * GPT-3 to GPT-4 (OpenAI)
 * Groq (which gives you access to Llama 3) 🔥
 
 ## Examples of AI Agent configuration
 
 Nagato is built with flexibility at its core, so you could program it using your paradigm of choice. However these are some of the ways I've seen people use Nagato so far.
 
+By default Nagato expects all LLM API keys to be set as environment variables. Nagato may load the keys from the following variables:
+
+```
+OPENAI_API_KEY=<api-key>
+ANTHROPIC_API_KEY=<api-key>
+READWISE_API_KEY=<api-key>
+```
+
 ### Coordinator, worker, and critic agents
 
 In this configuration we have the following:
 
 * 🎯 Coordinator: breaks down a problem statement (from stdin) into an objective and suggests tasks
 * 📚 Researcher: works on a task by performing research
 * ✅ Critic: evaluates whether the task was completed
 
 Example setup for this configuration could look like this:
 
 ```python
-openai_client = OpenAI(
-    organization="<org-id>",
-    api_key="<api-key>",
-)
-
-anthropic_api_key = "<api-key>"
-anthropic_client = Anthropic(api_key=anthropic_api_key)
-
-groq_client = Groq(api_key="<api-key>")
-
-coordinator_agent: Agent = AnthropicAgent(
-    anthropic_client,
+coordinator_agent: Agent = create_agent(
+    anthropic_api_key,
     "claude-3-opus-20240229",
     "Coordinator",
     COORDINATOR_SYSTEM_PROMPT,
     "Coordinator Agent",
 )
 
-researcher_agent: Agent = OpenAIAgent(
-    openai_client,
+researcher_agent = create_agent(
+    anthropic_api_key,
     "gpt-4-turbo-2024-04-09",
     "Researcher",
     RESEARCHER_SYSTEM_PROMPT,
     "Researcher Agent",
 )
 
-critic_agent: Agent = GroqAgent(
-    groq_client,
-    "llama3-70b-8192",
+critic_agent = create_agent(
+    anthropic_api_key,
+    "claude-3-haiku-20240307",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
 ...
 ```
 
@@ -131,28 +129,25 @@
         goal="Fetch last 100 user tweets",
         description="Fetch the tweets from the user using the Twitter API. Limit the number of tweets fetched to 100 only."),
     Task(
         goal="Perform sentiment analysis on the tweets",
         description="Feed the tweets to the AI Agent to analyze sentiment per overall sentiment acoss tweets. Range of values for sentiment can be: Positive, Negative, or Neutral"
     )]
 
-anthropic_api_key = "<api-key>"
-anthropic_client = Anthropic(api_key=anthropic_api_key)
-
-researcher_agent: Agent = AnthropicAgent(
-    anthropic_client,
+coordinator_agent: Agent = create_agent(
+    anthropic_api_key,
     "claude-3-sonnet-20240229",
-    "Researcher",
-    RESEARCHER_SYSTEM_PROMPT,
-    "Researcher Agent",
+    "Coordinator",
+    COORDINATOR_SYSTEM_PROMPT,
+    "Coordinator Agent",
 )
 
-critic_agent: Agent = AnthropicAgent(
-    anthropic_client,
-    "claude-3-opus-20240229",
+critic_agent = create_agent(
+    anthropic_api_key,
+    "claude-3-haiku-20240307",
     "Critic",
     CRITIC_SYSTEM_PROMPT,
     "Critic Agent",
 )
 
 for task in task_list:
     # Insert the task into the prompt
```

