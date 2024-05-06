# Comparing `tmp/reverse-engineering-assistant-1.0.3.tar.gz` & `tmp/reverse_engineering_assistant-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse-engineering-assistant-1.0.3.tar", last modified: Sun Mar 24 07:12:04 2024, max compression
+gzip compressed data, was "reverse_engineering_assistant-2.9.1.tar", last modified: Mon May  6 02:46:43 2024, max compression
```

## Comparing `reverse-engineering-assistant-1.0.3.tar` & `reverse_engineering_assistant-2.9.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/api_server_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/api_server_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/api_server_tools/llm_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/api_server_tools/re_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16251 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/assistant_api_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/reva_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-03-24 07:11:59.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/tool_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-24 07:12:04.000000 reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 07:12:04.250523 reverse-engineering-assistant-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.558109 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/llm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/re_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/chat_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/reva_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-06 02:46:37.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 02:46:43.000000 reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:46:43.562110 reverse_engineering_assistant-2.9.1/setup.cfg
```

### Comparing `reverse-engineering-assistant-1.0.3/PKG-INFO` & `reverse_engineering_assistant-2.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: reverse-engineering-assistant
-Version: 1.0.3
+Version: 2.9.1
 Summary: An AI assistant for reverse engineering tasks
 Author: サイバーカイダ (cyberkaida)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: langchain
 Requires-Dist: langchain-core
 Requires-Dist: langchain-openai
-Requires-Dist: llama-cpp-python
 Requires-Dist: prompt_toolkit
 Requires-Dist: sentence_transformers
 Requires-Dist: PyYAML
 Requires-Dist: pydantic
 Requires-Dist: rich
-Requires-Dist: Flask
+Requires-Dist: grpcio
+Requires-Dist: protobuf
 
 # ReVA - Reverse Engineering Assistant
 
-[✨ An (old) quick demo! ✨](https://asciinema.org/a/626197)
+> Updated demo coming soon!
 
 The reverse engineering assistant (ReVA) is a project to build a disassembler agnostic AI assistant for
 reverse engineering tasks. This includes both _offline_ and online inference and a simple architecture.
 
 ReVa is different from other efforts at building AI assistants for RE tasks because it uses a _tool driven approach_.
 ReVa aims to provide a variety of small tools to the LLM, just as your RE environment provides a set of small tools
 to you. ReVa combines this approach with chain-of-reasoning techniques to empower the LLM to complete complex tasks.
@@ -64,24 +64,21 @@
 RevA is based on [langchain](https://langchain.com),
 which supports a number of models.
 
 Built in support is provided for:
 - [OpenAI](https://platform.openai.com/overview) for online inference and easy setup (Needs an OpenAI API key)
 - [Ollama](https://ollama.ai) and any model it supports for local on-device inference or connecting to a self hosted remote inference server.
 
-Limited support is provided for:
-- [llama-cpp](https://llama-cpp-python.readthedocs.io/en/latest/) and any model it supports for local on-device inference
-- [text-generation-webui](https://github.com/oobabooga/text-generation-webui) and any model it supports for self-hosted remote inference
-
 Adding additional inference servers is easy if it is supported by langchain.
 
-See the configuration section for more information about setting the model.
-
 ## Configuration
 
+> This is currently being moved to the Ghidra GUI
+> See Edit -> Tool Options -> ReVa in the Codebrowser Tool
+
 Configuration for the reverse engineering assistant is stored at
 `~/.config/reverse-engineering-assistant/config.yaml`. If this
 is not present on first start, a default configuration using
 OpenAI for inference and the `OPENAI_API_TOKEN` environment
 variable will be used.
 
 The most important setting is the `type` top level setting.
@@ -102,90 +99,69 @@
 ## Workflow
 
 RevA has a two step workflow.
 1. Open your RE tool and the program you want to examine
 2. Open the chat session.
 
 ReVa uses an extension for your RE tool to perform analysis.
-See [Ghidra Support](#ghidra-support) and [BinaryNinja Support](#binary-ninja-support) below.
-
-Once open the RE tool will try to connect to ReVa's REST API on localhost.
-
-A project cache is created in `~/.cache/reverse-engineering-assistant/projects`. This contains your chat log and other
-cache data. This can be deleted at any time and ReVa will re-generate the data as needed.
+See [Ghidra Support](#ghidra-support) below.
 
-To ask questions and run the inference a command line tool is provided. Run `revassistant --project ${NAME_OF_YOUR_FILE}` to begin the chat session.
+To ask questions and run the inference a command line tool is provided. Run `reva-chat` to begin the chat session. This command will find your open Ghidra
+and connect to it. To open a new chat, run the command again in another terminal.
 
-> Note: In the future `--project` will refer to a _project_ in Ghidra and allow inference across multiple files.
-> I am waiting for BinaryNinja's project feature to make this change, if this takes too long I will rework this argument.
-
-`revassistant` provides a chat window and runs the command API to talk with the RE tool.
-
-> Note: Right now only one `revassistant` can run at a time (as we start a server on a well known port)
-> In the future we will share the server between chat clients and RE tool connections.
+If you have more than one Ghidra open, you can select the right one with
+`reva-chat --project ${project-name}`, if it is not set, `reva-chat` will
+ask you which project you want to connect to.
 
 ## Installation
 
+First install the python component, I like to use `pipx`. It is best to make
+sure that `reva-server` and `reva-chat` are on your path.
+The Ghidra extension will need to start `reva-server`, and you will need to
+run `reva-chat`.
+
 To install the particular extension for your disassembler see:
 - [Ghidra Support](#ghidra-support)
-- [Binary Ninja Support](#binary-ninja-support)
-
-To install the chat component you can do the following:
-
-```sh
-python3 -m pip install ./reverse-engineering-assistant
-```
 
 The chat can be started with:
 
 ```sh
-revassistant --project ${NAME_OF_YOUR_PROJECT}
+reva-chat
 ```
 
+> You can also configure the path to `reva-server` in `Edit -> Tool Options -> ReVa`
+> if it is not on your path. But you really should put it on your path!
+
 # Ghidra Support
 
 ## Usage
 
-The [ghidra-assistant](ghidra-assistant/README.md) plugin must be installed first. 
+> The Python package must be installed for the Ghidra extension to work!
+
+Follow the instructions in the [ghidra-assistant](ghidra-assistant/README.md) plugin.
 
 After installation, enable the `ReVaPlugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
 
 If you want ReVa enabled by default, click File -> Save Tool to save the configuration.
 
-To start the inference side, open Help -> About ${program name}. In this popup you will see details about your open file.
-The `Program Name:` field is the name you need to pass to `revassistant --project` to start the inference server. In some
-cases this is different to the name in the project view.
+If everything is working correctly you will see a ReVa menu on your menu bar.
 
 ## Undo
 
 Whenever ReVa performs an action it will create an undo point for each action. If ReVa renames 5 variables, this will be
 one undo.
 
 ## Menus
 
+> These are being added in the next release
+
 ReVa adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
 "Examine the variable usage in `main` in detail, rename the variables with more descriptive names.",
 or use the menu system.
 
 For example you can right click a variable in the decompilation, select Reva -> Rename variable and ReVa
 will perform the action.
 
-Note this uses the same system as chatting with ReVa, this means you can monitor ReVas thoughts in the chat
-window while the action is performed.
-
-# Binary Ninja Support
-
-> Note: Binary Ninja support is currently on hold while the basic functions are implemented in the Ghidra plugin.
-> This is because plugin development for Binary Ninja is easier as we have Python3. I will resume development soon!
-
-Install the ReVA BinaryNinja plugin by opening your BinaryNinja plugin directory (Plugins -> Open Plugin Folder)
-and copying or symbolic linking the [binary-ninja-assistant](./binary-ninja-assistant) directory into the plugin
-directory.
-
-Restart Binary Ninja and "ReVA Push" will be available in the Plugin menu.
-Press this to push data from BinaryNinja to ReVA, then follow the instructions in the [Workflow section](#workflow).
-The project name will be the name of the current open file.
-
 # Support
 
 Do you like my work? Want to support this project and others? Interested in how this project was designed and built?
 This project and many others are built live on my stream at https://twitch.tv/cyberkaida !
```

### Comparing `reverse-engineering-assistant-1.0.3/pyproject.toml` & `reverse_engineering_assistant-2.9.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reverse-engineering-assistant"
 readme = "README.md"
-version = "1.0.3"
+version = "2.9.1"
 authors = [
     {name="サイバーカイダ (cyberkaida)"},
 ]
 description = "An AI assistant for reverse engineering tasks"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dependencies = [
     "langchain",
     "langchain-core",
     "langchain-openai",
-    "llama-cpp-python",
     "prompt_toolkit",
     "sentence_transformers",
     "PyYAML",
     "pydantic",
     "rich",
-    "Flask",
+    "grpcio",
+    "protobuf",
 ]
 
 [project.scripts]
-revassistant = "reverse_engineering_assistant.assistant:main"
-reva-serve = "reverse_engineering_assistant.assistant_api_server:main"
 reva-server = "reverse_engineering_assistant.assistant_api_server:main"
-
+reva-chat = "reverse_engineering_assistant.chat_client:main"
```

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/assistant.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,16 @@
 
     llm: BaseLLM | BaseChatModel
 
     model_memory: BaseMemory
 
     chat_history: List[str]
 
+    langchain_callbacks: List[BaseCallbackHandler]
+
     def __repr__(self) -> str:
         return f"<ReverseEngineeringAssistant for {self.project}>"
 
     @classmethod
     def get_projects(cls) -> List[str]:
         """
         Gets the names of the projects.
@@ -211,28 +213,30 @@
         This method is passed to the LLM as a callback when the LLM encounters an exception
         from one of the Reva tools. We then return output to the LLM to help it fix its problem.
         """
         if isinstance(e, RevaToolException):
             return f"RevaToolException: {e}"
         raise e
 
-    def __init__(self, project: str | AssistantProject, model_type: Optional[ModelType] = None) -> None:
+    def __init__(self, project: str | AssistantProject, model_type: Optional[ModelType] = None, langchain_callbacks: Optional[List[BaseCallbackHandler]] = None) -> None:
         """
         Initializes a new instance of the ReverseEngineeringAssistant class.
 
         Args:
             project (str | AssistantProject): The reverse engineering project to query.
             model_type (Optional[ModelType], optional): The model type for the reverse engineering assistant. Defaults to None.
         """
         self.chat_history = []
         if isinstance(project, str):
             self.project = AssistantProject(project)
         else:
             self.project = project
 
+        self.langchain_callbacks = langchain_callbacks or []
+
         self.llm = get_model(model_type)
 
         # Let's take the tools that have been decorated with @register_tool and turn them into
         # tools the LLM can use.
         self.tools = [ tool_type(self.project, self.llm) for tool_type in _reva_tool_list]
         logger.debug(f"Loaded tools: {[ x for x in self.tools]}")
 
@@ -251,14 +255,15 @@
                 base_tools.append(function)
 
         #self.model_memory = ConversationTokenBufferMemory(
         #    llm=self.llm
         #)
         self.model_memory = ConversationBufferMemory()
         callbacks: List[BaseCallbackHandler] = [RevaActionLogger()]
+        callbacks.extend(self.langchain_callbacks)
         callback_manager = RevaActionLoggerManager(handlers=callbacks, inheritable_handlers=callbacks)
 
         agent =  StructuredChatAgent.from_llm_and_tools(
             llm=self.llm,
             tools=base_tools,
             system_message=configuration.prompt_template.system_prompt,
             verbose=False,
```

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/configuration.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/configuration.py`

 * *Files identical despite different names*

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/documents.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/documents.py`

 * *Files identical despite different names*

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/model.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/model.py`

 * *Files identical despite different names*

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/tool.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/tool.py`

 * *Files identical despite different names*

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant/tool_protocol.py` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant/api_server_tools/re_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,509 +1,354 @@
-#!/usr/bin/env python3
-
-"""
-This file contains the communications protocol for interacting between
-the ReVa inference side and the reverse engineering tool.
-
-This file is python3, but it should not interact with the inference
-side directly. While BinaryNinja can use this directly, Ghidra will
-reimplement this protocol in Java.
-
-We will have integration tests that generate messages and attempt to
-parse on both sides to make sure these do not diverge.
-
-Some design notes:
-- We need to include extra information in each response that could lead
-  to new discoveries or links. This is to make sure the inference side
-  stays curious.
-- Every field needs docstrings to help the LLM reason about messages.
-  In general these will be wrapped by methods in assistant.py when a
-  tool is exposed to the LLM, if we need to send a response
-  directly to the LLM, we need to make sure it can reason about the
-  fields.
-"""
-
 from __future__ import annotations
-from typing import List, Optional, Union, Dict, Any, Type, Annotated
 
-from abc import ABC, abstractproperty, abstractmethod
-from datetime import datetime
 
-from uuid import UUID, uuid4
-import json
 from pathlib import Path
-import logging
+from typing import Dict, List, Optional
 
-from click import Option
-from pydantic import BaseModel, Field
-import pydantic
-import pydantic_core
+from langchain.chat_models.base import BaseChatModel
+from langchain.llms.base import BaseLLM
+from numpy import add
 
-try:
-    from pydantic import validator
-except ImportError:
-    # Depending on the version we might have validator in another place
-    from pydantic.functional_validators import function_validator as validator # type: ignore
+from ..tool import AssistantProject
+from ..assistant import AssistantProject, RevaTool, BaseLLM, register_tool
+from ..assistant_api_server import get_channel
 
-from pydantic.dataclasses import dataclass
+from ..reva_exceptions import RevaToolException
 
-import tempfile
-
-_reva_message_types: Dict[str, Type[RevaMessage]] = {}
-
-def register_message(cls: Type[RevaMessage]) -> Type[RevaMessage]:
-    """
-    Register a message type
-    """
-    logging.getLogger("reverse_engineering_assistant.tool_protocol.register_message").debug(f"Registering message type {cls.__name__}")
-    _reva_message_types[cls.__name__] = cls
-    return cls
-
-
-logger = logging.getLogger("reverse_engineering_assistant.tool_protocol")
-class RevaMessage(BaseModel, ABC):
-    """
-    Base class for all messages sent between the inference side and the
-    reverse engineering tool.
-    """
-
-    message_type: str = Field()
-    """
-    The type of this message. This is used to determine which class to
-    deserialise the message into.
-
-    Must be one of the subclasses of RevaMessage.
-    """
-
-    @validator("message_type")
-    def validate_message_type(cls, value: str) -> str:
+import logging
 
+# TODO: I think the word tool is used too much in the project... It's a bit confusing...
+class RevaRemoteTool(RevaTool):
+    @property
+    def channel(self):
+        return get_channel()
+
+
+@register_tool
+class RevaDecompilationIndex(RevaRemoteTool):
+    """
+    An index of decompiled functions available to the
+    reverse engineering assistant.
+    """
+    index_name = "decompilation"
+    description = "Used for retrieving decompiled functions"
+    logger = logging.getLogger("reverse_engineering_assistant.RevaDecompilationIndex")
+
+    def __init__(self, project: AssistantProject, llm: BaseLLM) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for retrieveing decompiled functions"
+        self.tool_functions = [
+            self.get_decompilation_for_function,
+            # TODO: Implement these functions
+            #self.get_defined_function_list_paginated,
+            #self.get_defined_function_count,
+        ]
 
-        assert value in _reva_message_types, f"Unknown message type {value}, check the logs to make sure the `register_message` was called for this message type. Registered message types are {_reva_message_types.keys()}"
-        return value
+    def get_decompilation_for_function(self, function_name_or_address: str | int) -> Dict[str, str]:
+        """
+        Return the decompilation for the given function. The function can be specified by name or address.
+        Hint: It is too slow to decompile _all_ functions, so use get_defined_function_list_paginated to get a list of functions
+        and be sure to specify the function name or address exactly.
+        """
 
+        # First normalise the argument
+        address: Optional[int] = None
+        name: Optional[str] = None
+        if isinstance(function_name_or_address, int):
+                address = function_name_or_address
+        elif isinstance(function_name_or_address, str):
+            name = function_name_or_address
+
+        if address is None and name is None:
+            raise RevaToolException("function_name_or_address must be an address or function name")
+
+        if address and address <= 0:
+            raise RevaToolException("function_name_or_address must be a positive integer or a function name")
+
+        # Now we can create the message and call over the RPC
+        from ..protocol import RevaGetDecompilation_pb2_grpc, RevaGetDecompilation_pb2
+        stub = RevaGetDecompilation_pb2_grpc.RevaDecompilationServiceStub(self.channel)
+
+        request = RevaGetDecompilation_pb2.RevaGetDecompilationRequest()
+
+        if name:
+            request.function = name
+        if address:
+            request.address = address
+
+        response: RevaGetDecompilation_pb2.RevaGetDecompilationResponse = stub.GetDecompilation(request)
+
+        # Finally we can return the response
+        return {
+            "function": response.function,
+            "function_signature": response.function_signature,
+            "address": hex(response.address),
+            "decompilation": response.decompilation,
+            "listing": response.listing,
+            "variables": response.variables, #type: ignore # We can ignore this because it can be serialised to a dict
+            "incoming_calls": response.incoming_calls,
+            "outgoing_calls": response.outgoing_calls,
+        }
 
-    message_id: UUID = Field(default_factory=uuid4)
-    """
-    Unique identifier for this message
-    """
 
-    @classmethod
-    def to_specific_message(cls, thing: Dict) -> RevaMessage:
+    def get_defined_function_list_paginated(self, page: int, page_size: int = 20) -> List[str]:
         """
-        Convert this message to the specific message type
+        Return a paginated list of functions in the index. Use get_defined_function_count to get the total number of functions.
+        page is 1 indexed. To get the first page, set page to 1. Do not set page to 0.
         """
-        # First validate it is a ReVa message
-        RevaMessage.model_validate(thing)
-        try:
-            logger.debug(f"Converting message to specific type {thing['message_type']}")
-            logger.debug(f"Checking for message type {thing['message_type']} in {_reva_message_types}")
-            message_class = _reva_message_types[thing["message_type"]]
-            logger.debug(f"Message class is {message_class}")
-            try:
-                return message_class.model_validate(thing)
-            except pydantic_core.ValidationError:
-                # If we fail to turn it into a specific type, make it a generic type
-                # This allows us to extract things like error messages.
-                if issubclass(message_class, RevaMessageResponse):
-                    return RevaMessageResponse.model_validate(thing)
-                else:
-                    logger.exception(f"Failed to parse {thing} as {message_class}")
-                return RevaMessage.model_validate(thing)
-        except KeyError:
-            raise ValueError(f"No message type in message, is this a ReVa message?")
+        raise NotImplementedError("This function is not implemented yet")
+        return response.function_list
 
-    def send(self) -> None:
+    def get_defined_function_count(self) -> int:
         """
-        Send this message
+        Return the total number of defined functions in the program.
         """
-        raise NotImplementedError()
 
-class RevaMessageResponse(RevaMessage, ABC):
+        raise NotImplementedError("This function is not implemented yet")
+        return response.function_count
+
+# TODO: This tool is not implemented yet
+#@register_tool
+class RevaRenameFunctionVariable(RevaRemoteTool):
     """
-    Base class for all messages sent in response to a RevaMessage
+    A tool for renaming variables used in functions
     """
-    response_to: UUID = Field()
-    error_message: Optional[str] = Field(default=None)
 
+    description = "Used for renaming variables used in functions"
+    logger = logging.getLogger("reverse_engineering_assistant.RevaRenameFunctionVariable")
 
-class RevaMessageToTool(RevaMessage):
-    """
-    Base class for messages sent to the tool
-    """
+    def __init__(self, project: AssistantProject, llm: BaseLLM | BaseChatModel) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for renaming variables used in functions"
+        self.tool_functions = [
+            self.rename_multiple_variables_in_function,
+            self.rename_variable_in_function
+        ]
 
-    def send(self) -> None:
+    def rename_multiple_variables_in_function(self, new_names: Dict[str, str], containing_function: str) -> List[str]:
         """
-        Send this message
-        """
-        raise NotImplementedError()
-
+        Change the names of multiple variables in the function `containing_function` to the new names specified in `new_names`.
+        `new_names` is a dictionary where the keys are the old names and the values are the new names.
 
-class RevaMessageToReva(RevaMessage):
-    """
-    Base class for messages sent to the inference side
-    """
+        If there are many variables to rename in a function, use this. It is more efficient than calling rename_variable_in_function multiple times.
+        After calling this, you can confirm the changes by decompiling the function again.
+        If there is a failure, retrying the operation will not help.
+        """
+        outputs: List[str] = []
+        for old_name, new_name in new_names.items():
+            outputs.append(self.rename_variable_in_function(new_name, old_name, containing_function))
+        return outputs
 
-    def send(self) -> None:
+    def rename_variable_in_function(self, new_name: str, old_name: str, containing_function: str):
         """
-        Send this message
+        Change the name of the variable with the name `old_name` in `containing_function` to `new_name`.
+        If the thing you want to rename is not in a function, you should use rename symbol instead,
         """
-        raise NotImplementedError()
-
-# MARK: - Heartbeats
-
-@register_message
-class RevaHeartbeat(RevaMessageToReva):
-    """
-    A heartbeat message is sent periodically to ensure the connection
-    is still alive.
-    """
-    message_type: str = "RevaHeartbeat"
+        raise NotImplementedError("This function is not implemented yet")
+        return f"Renamed {old_name} to {new_name} in {containing_function}"
 
-@register_message
-class RevaHeartbeatResponse(RevaMessageToTool, RevaMessageResponse):
+#TODO: This tool is not implemented yet
+#@register_tool
+class RevaCrossReferenceTool(RevaRemoteTool):
     """
-    A heartbeat response is sent in response to a heartbeat message.
+    An tool to retrieve cross references, to and from, addresses.
     """
-    message_type: str = "RevaHeartbeatResponse"
-
-# MARK: Simple state messages
+    index_directory: Path
+    def __init__(self, project: AssistantProject, llm: BaseLLM) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for retrieving cross references to and from addresses"
 
-class RevaGetCursor(RevaMessageToTool):
-    """
-    Request the current cursor position
-    """
-    pass
+        self.tool_functions = [
+            self.get_references,
+        ]
 
-class RevaGetCursorResponse(RevaMessageToReva):
-    """
-    Response to a RevaGetCursor message
-    """
-    cursor_address: int = Field()
-    """
-    The current cursor position
-    """
-    symbol: Optional[str] = None
-    """
-    If the cursor is at a symbol, this is the name of the symbol
-    """
-    function: Optional[str] = None
-    """
-    If the cursor is in a function, this is the name of the function
-    """
-    # TODO: Add data type
+    def get_references(self, address_or_symbol: str) -> Optional[Dict[str, List[str]]]:
+        """
+        Return a list of references to and from the given address or symbol.
+        These might be calls from/to other functions, or data references from/to this address.
+        """
+        from ..protocol import RevaGetReferences_pb2_grpc, RevaGetReferences_pb2
 
-# MARK: Memory related messages
+        stub = RevaGetReferences_pb2_grpc.RevaGetReferencesServiceStub(self.channel)
 
-@register_message
-class RevaGetDataAtAddress(RevaMessageToTool):
-    """
-    Request the data at a given address
-    """
-    message_type: str = "RevaGetDataAtAddress"
+        request = RevaGetReferences_pb2.RevaGetReferencesRequest()
+        request.address_or_symbol = address_or_symbol
 
-    address_or_symbol: str = Field()
-    """
-    The address to retrieve data from
-    """
-    size: int = Field()
-    """
-    The number of bytes to retrieve
-    """
+        response: RevaGetReferences_pb2.RevaGetReferencesResponse = stub.GetReferences(request)
 
-@register_message
-class RevaGetDataAtAddressResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaGetDataAtAddress message
-    """
-    message_type: str = "RevaGetDataAtAddressResponse"
+        return {
+            "references_to": response.references_to,
+            "references_from": response.references_from,
+        }
 
-    address: int = Field()
-    """
-    The address this data is at
-    """
-    data: bytes = Field()
+@register_tool
+class RevaGetSymbols(RevaRemoteTool):
     """
-    The data at the given address
-    """
-    symbol: Optional[str] = None
-    """
-    If the address is a symbol, this is the name of the symbol
+    A tool for listing symbols in a program.
+    These could be functions, global variables, or other named entities.
     """
+    logger = logging.getLogger("reverse_engineering_assistant.RevaGetSymbols")
 
-# MARK: Decompilation and functions
 
-@register_message
-class RevaGetDecompilation(RevaMessageToTool):
-    """
-    Request the decompilation of a given address
-    """
-    message_type: str = "RevaGetDecompilation"
-    address: Optional[int] = Field()
-    """
-    The address to decompile
-    """
-    function: Optional[str] = None
-    """
-    The function to decompile. If None, the function at the given
-    address will be decompiled.
-    """
+    def __init__(self, project: AssistantProject, llm: BaseLLM) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for retrieving symbols in the program"
 
-class RevaVariable(BaseModel):
-    name: str = Field()
-    storage: Optional[str] = Field(default=None)
-    data_type: Optional[str] = Field(default=None)
-    size: Optional[int] = Field(default=None)
+        self.tool_functions = [
+            self.get_symbol_count,
+            self.get_symbols,
+            self.get_symbol,
+            self.get_function_count,
+            self.get_functions,
+        ]
 
-@register_message
-class RevaGetDecompilationResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaGetDecompilation message
-    """
-    message_type: str = "RevaGetDecompilationResponse"
-    address: int = Field()
-    """
-    The address this decompilation is at
-    """
-    decompilation: str = Field()
-    """
-    The decompilation of the given address
-    """
-    listing: Optional[str] = Field(default=None)
-    """
-    The disassebly listing of the function
-    """
-    function: str = Field()
-    """
-    The function this decompilation is for
-    """
-    function_signature: str = Field()
-    """
-    The signature of the function
-    """
-    incoming_calls: List[str] = Field()
-    """
-    The functions that call this function
-    """
-    outgoing_calls: List[str] = Field()
-    """
-    The functions that this function calls
-    """
-    variables: List[RevaVariable] = Field()
-    """
-    The variables in this function
-    """
+    def _get_symbol_list(self) -> List[str]:
+        from ..protocol import RevaGetSymbols_pb2_grpc, RevaGetSymbols_pb2
+        stub = RevaGetSymbols_pb2_grpc.RevaToolSymbolServiceStub(self.channel)
 
-@register_message
-class RevaGetFunctionCount(RevaMessageToTool):
-    """
-    Request the number of functions in the program
-    """
-    message_type: str  = "RevaGetFunctionCount"
-    pass
+        request = RevaGetSymbols_pb2.RevaGetSymbolsRequest()
 
-@register_message
-class RevaGetFunctionCountResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaGetFunctionCount message
-    """
-    message_type: str  = "RevaGetFunctionCountResponse"
-    function_count: int = Field()
-    """
-    The number of functions in the program
-    """
+        response: RevaGetSymbols_pb2.RevaGetSymbolsResponse = stub.GetSymbols(request)
 
-@register_message
-class RevaGetDefinedFunctionList(RevaMessageToTool):
-    """
-    Request a list of defined functions
-    """
-    message_type: str  = "RevaGetDefinedFunctionList"
-    page: int = Field()
-    """
-    The page number to retrieve. 1 indexed.
-    """
-    page_size: int = Field()
-    """
-    The number of functions to retrieve per page
-    """
+        return response.symbols
 
-@register_message
-class RevaGetDefinedFunctionListResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaGetDefinedFunctionList message
-    """
-    message_type: str  = "RevaGetDefinedFunctionListResponse"
-    function_list: List[str] = Field()
-    """
-    A list of defined functions
-    """
+    def _get_function_list(self) -> List[str]:
+        function_list: List[str] = []
+        for symbol_name in self._get_symbol_list():
+            symbol = self.get_symbol(symbol_name)
+            if symbol["type"] == "FUNCTION":
+                function_list.append(symbol_name)
+        return function_list
 
-@register_message
-class RevaGetReferences(RevaMessageToTool):
-    """
-    Request a list of references to a given address
-    """
-    message_type: str  = "RevaGetReferences"
-    address_or_symbol: str = Field()
-    """
-    The address to retrieve references to
-    """
+    def get_function_count(self) -> int:
+        """
+        Return the total number of functions in the program.
+        Useful before calling get_functions.
+        """
+        return len(self._get_function_list())
 
-@register_message
-class RevaGetReferencesResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaGetReferences message
-    """
-    message_type: str  = "RevaGetReferencesResponse"
-    references_to: List[str] = Field()
-    """
-    A list of references to the given address
-    """
-    references_from: List[str] = Field()
-    """
-    A list of references from the given address
-    """
+    def get_functions(self, page: int = 0, page_size: int = 20) -> List[Dict[str, str]]:
+        """
+        Return a list of functions in the program.
+        Please check the total number of functions with get_function_count before calling this.
+        The page is 0 indexed. To get the first page, set page to 0.
+        Pick a page_size that is reasonable for your context size.
+        """
+        if page < 0:
+            raise RevaToolException("page must be 0 or a positive integer")
+        if page_size <= 0:
+            raise RevaToolException("page_size must be a positive integer")
+
+        function_list = self._get_function_list()
+        start = (page - 1) * page_size
+        end = page * page_size
+
+        function_details: List[Dict[str, str]] = []
+        for function in function_list[start:end]:
+            # TODO: Replace with get_function
+            function_details.append(self.get_symbol(function))
+        return function_details
 
-@register_message
-class RevaGetSymbols(RevaMessageToTool):
-    """
-    Request a list of symbols
-    """
-    message_type: str  = "RevaGetSymbols"
-    page: int = Field()
-    """
-    The page number to retrieve. 1 indexed.
-    """
-    page_size: int = Field()
-    """
-    The number of symbols to retrieve per page
-    """
+    def get_symbol_count(self) -> int:
+        """
+        Return the total number of symbols in the program.
+        Useful before calling get_symbols.
+        """
+        return len(self._get_symbol_list())
 
-@register_message
-class RevaSetSymbolName(RevaMessageToTool):
-    """
-    Set the name for a function or symbol,
-    or create a label for an address.
+    def get_symbols(self, page: int = 0, page_size: int = 20) -> List[Dict[str, str]]:
+        """
+        Return a list of symbols in the program.
+        Please check the total number of symbols with get_symbol_count before calling this.
+        The page is 0 indexed. To get the first page, set page to 0.
+        Pick a page_size that is reasonable for your context size.
+        """
+        if page < 0:
+            raise RevaToolException("page must be 0 or a positive integer")
+        if page_size <= 0:
+            raise RevaToolException("page_size must be a positive integer")
+
+        symbol_list = self._get_symbol_list()
+        start = (page - 1) * page_size
+        end = page * page_size
+
+        symbol_details: List[Dict[str, str]] = []
+        for symbol in symbol_list[start:end]:
+            symbol_details.append(self.get_symbol(symbol))
+        return symbol_details
 
-    When setting the name for a variable in a functions
-    please use RevaRenameVariable.
-    """
-    message_type: str = "RevaSetSymbolName"
-    old_name_or_address: str = Field()
-    new_name: str = Field()
+    def get_symbol(self, address_or_name: str) -> Dict[str, str]:
+        """
+        Return information about the symbol at the given address or with the given name.
+        Returns a dictionary with the keys "name", "address", and "type".
+        """
+        from ..protocol import RevaGetSymbols_pb2_grpc, RevaGetSymbols_pb2
+        stub = RevaGetSymbols_pb2_grpc.RevaToolSymbolServiceStub(self.channel)
 
-@register_message
-class RevaGetNewSymbolName(RevaMessageToReva):
-    """
-    Ask the modek for a better name
-    """
-    message_type: str = "RevaGetNewSymbolName"
-    symbol_name: str = Field()
-    """
-    The symbol to rename
-    """
+        request = RevaGetSymbols_pb2.RevaSymbolRequest()
+        request.address_or_name = address_or_name
+        self.logger.debug(f"Getting symbol {address_or_name} request: {request}")
+        response: RevaGetSymbols_pb2.RevaSymbolResponse = stub.GetSymbol(request)
+        self.logger.debug(f"Got symbol {address_or_name} response: {response}")
+        return {
+            "name": response.name,
+            "address": response.address,
+            "type": RevaGetSymbols_pb2.SymbolType.Name(response.type),
+        }
 
-@register_message
-class RevaGetNewSymbolNameResponse(RevaMessageToTool, RevaMessageResponse):
-    """
-    Response to a RevaGetNewSymbolName message.
-    """
-    message_type: str = "RevaGetNewSymbolNameResponse"
 
-@register_message
-class RevaSetSymbolNameResponse(RevaMessageToTool, RevaMessageResponse):
+@register_tool
+class RevaSetSymbolName(RevaRemoteTool):
     """
-    Response to a RevaSetSymbolName message
+    A tool for creating or changing the name for a global symbol.
+    This could be a function name, or a global variable name.
     """
-    message_type: str = "RevaSetSymbolNameResponse"
 
-@register_message
-class RevaGetNewVariableName(RevaMessageToReva):
-    """
-    Ask the model for a better name
-    """
-    message_type: str= "RevaGetNewVariableName"
-    variable: RevaVariable = Field()
-    """
-    The variable to rename
-    """
-    function_name: str = Field()
-    """
-    The function this variable is in
-    """
+    def __init__(self, project: AssistantProject, llm: BaseLLM) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for retrieving cross references to and from addresses"
 
-@register_message
-class RevaGetNewVariableNameResponse(RevaMessageToTool, RevaMessageResponse):
-    """
-    Response to a RevaGetNewVariableName message.
-    """
-    message_type: str = "RevaGetNewVariableNameResponse"
+        self.tool_functions = [
+            self.set_symbol_name,
+        ]
 
-@register_message
-class RevaRenameVariable(RevaMessageToTool):
-    """
-    Tell the tool to rename a variable
-    """
-    message_type: str = "RevaRenameVariable"
-    variable: RevaVariable = Field()
-    """
-    The variable to rename
-    """
-    new_name: str = Field()
-    """
-    The new name to give the variable
-    """
-    function_name: str = Field()
-    """
-    The function this variable is in
-    """
+    def set_symbol_name(self, new_name: str, old_name_or_address: str) -> Dict[str, str]:
+        """
+        Set the name of the symbol at the given address to `new_name`. If an old name is
+        provided, rename the symbol to `new_name`.
+        """
+        from ..protocol import RevaGetSymbols_pb2_grpc, RevaGetSymbols_pb2
+        stub = RevaGetSymbols_pb2_grpc.RevaToolSymbolServiceStub(self.channel)
 
-@register_message
-class RevaRenameVariableResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaRenameVariable message.
+        request = RevaGetSymbols_pb2.RevaSetSymbolNameRequest()
+        request.new_name = new_name
+        request.old_name_or_address = old_name_or_address
 
-    A simple yes/no, not much to respond with.
-    """
-    message_type: str = "RevaRenameVariableResponse"
+        response: RevaGetSymbols_pb2.RevaSetSymbolNameResponse = stub.SetSymbolName(request)
 
-class RevaLocation(BaseModel):
-    cursor_address: Optional[str] = Field(default=None)
-    function_name: Optional[str] = Field(default=None)
-    start_address: Optional[str] = Field(default=None)
-    end_address: Optional[str] = Field(default=None)
-    content: Optional[str] = Field(default=None)
+        return {
+            "old_name": old_name_or_address,
+            "new_name": new_name,
+        }
 
-@register_message
-class RevaExplain(RevaMessageToReva):
+@register_tool
+class RevaSetComment(RevaRemoteTool):
     """
-    Ask the model to explain something
-    """
-    message_type: str = "RevaExplain"
-    location: RevaLocation = Field()
-    """
-    The location to explain
+    A tool for setting comments on addresses, functions and symbols.
     """
 
-@register_message
-class RevaExplainResponse(RevaMessageToTool, RevaMessageResponse):
-    """
-    Response to a RevaExplain message
-    """
-    message_type: str = "RevaExplainResponse"
+    def __init__(self, project: AssistantProject, llm: BaseLLM) -> None:
+        super().__init__(project, llm)
+        self.description = "Used for setting comments on addresses, functions and symbols"
 
-@register_message
-class RevaSetComment(RevaMessageToTool):
-    """
-    Set a comment at a given address
-    """
-    message_type: str = "RevaSetComment"
-    address_or_symbol: str = Field()
-    comment: str = Field()
+        self.tool_functions = [
+            self.set_comment,
+        ]
 
-@register_message
-class RevaSetCommentResponse(RevaMessageToReva, RevaMessageResponse):
-    """
-    Response to a RevaSetComment message
-    """
-    message_type: str = "RevaSetCommentResponse"
+    def set_comment(self, comment: str, address_or_symbol: str) -> Dict[str, str]:
+        """
+        Set the comment at the given address, function or symbol to `comment`.
+        Use this when you want to add an explanation or note to a specific part
+        of the code.
+        """
+        raise NotImplementedError("This function is not implemented yet")
+        return response.model_dump()
```

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/PKG-INFO` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: reverse-engineering-assistant
-Version: 1.0.3
+Version: 2.9.1
 Summary: An AI assistant for reverse engineering tasks
 Author: サイバーカイダ (cyberkaida)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: langchain
 Requires-Dist: langchain-core
 Requires-Dist: langchain-openai
-Requires-Dist: llama-cpp-python
 Requires-Dist: prompt_toolkit
 Requires-Dist: sentence_transformers
 Requires-Dist: PyYAML
 Requires-Dist: pydantic
 Requires-Dist: rich
-Requires-Dist: Flask
+Requires-Dist: grpcio
+Requires-Dist: protobuf
 
 # ReVA - Reverse Engineering Assistant
 
-[✨ An (old) quick demo! ✨](https://asciinema.org/a/626197)
+> Updated demo coming soon!
 
 The reverse engineering assistant (ReVA) is a project to build a disassembler agnostic AI assistant for
 reverse engineering tasks. This includes both _offline_ and online inference and a simple architecture.
 
 ReVa is different from other efforts at building AI assistants for RE tasks because it uses a _tool driven approach_.
 ReVa aims to provide a variety of small tools to the LLM, just as your RE environment provides a set of small tools
 to you. ReVa combines this approach with chain-of-reasoning techniques to empower the LLM to complete complex tasks.
@@ -64,24 +64,21 @@
 RevA is based on [langchain](https://langchain.com),
 which supports a number of models.
 
 Built in support is provided for:
 - [OpenAI](https://platform.openai.com/overview) for online inference and easy setup (Needs an OpenAI API key)
 - [Ollama](https://ollama.ai) and any model it supports for local on-device inference or connecting to a self hosted remote inference server.
 
-Limited support is provided for:
-- [llama-cpp](https://llama-cpp-python.readthedocs.io/en/latest/) and any model it supports for local on-device inference
-- [text-generation-webui](https://github.com/oobabooga/text-generation-webui) and any model it supports for self-hosted remote inference
-
 Adding additional inference servers is easy if it is supported by langchain.
 
-See the configuration section for more information about setting the model.
-
 ## Configuration
 
+> This is currently being moved to the Ghidra GUI
+> See Edit -> Tool Options -> ReVa in the Codebrowser Tool
+
 Configuration for the reverse engineering assistant is stored at
 `~/.config/reverse-engineering-assistant/config.yaml`. If this
 is not present on first start, a default configuration using
 OpenAI for inference and the `OPENAI_API_TOKEN` environment
 variable will be used.
 
 The most important setting is the `type` top level setting.
@@ -102,90 +99,69 @@
 ## Workflow
 
 RevA has a two step workflow.
 1. Open your RE tool and the program you want to examine
 2. Open the chat session.
 
 ReVa uses an extension for your RE tool to perform analysis.
-See [Ghidra Support](#ghidra-support) and [BinaryNinja Support](#binary-ninja-support) below.
-
-Once open the RE tool will try to connect to ReVa's REST API on localhost.
-
-A project cache is created in `~/.cache/reverse-engineering-assistant/projects`. This contains your chat log and other
-cache data. This can be deleted at any time and ReVa will re-generate the data as needed.
+See [Ghidra Support](#ghidra-support) below.
 
-To ask questions and run the inference a command line tool is provided. Run `revassistant --project ${NAME_OF_YOUR_FILE}` to begin the chat session.
+To ask questions and run the inference a command line tool is provided. Run `reva-chat` to begin the chat session. This command will find your open Ghidra
+and connect to it. To open a new chat, run the command again in another terminal.
 
-> Note: In the future `--project` will refer to a _project_ in Ghidra and allow inference across multiple files.
-> I am waiting for BinaryNinja's project feature to make this change, if this takes too long I will rework this argument.
-
-`revassistant` provides a chat window and runs the command API to talk with the RE tool.
-
-> Note: Right now only one `revassistant` can run at a time (as we start a server on a well known port)
-> In the future we will share the server between chat clients and RE tool connections.
+If you have more than one Ghidra open, you can select the right one with
+`reva-chat --project ${project-name}`, if it is not set, `reva-chat` will
+ask you which project you want to connect to.
 
 ## Installation
 
+First install the python component, I like to use `pipx`. It is best to make
+sure that `reva-server` and `reva-chat` are on your path.
+The Ghidra extension will need to start `reva-server`, and you will need to
+run `reva-chat`.
+
 To install the particular extension for your disassembler see:
 - [Ghidra Support](#ghidra-support)
-- [Binary Ninja Support](#binary-ninja-support)
-
-To install the chat component you can do the following:
-
-```sh
-python3 -m pip install ./reverse-engineering-assistant
-```
 
 The chat can be started with:
 
 ```sh
-revassistant --project ${NAME_OF_YOUR_PROJECT}
+reva-chat
 ```
 
+> You can also configure the path to `reva-server` in `Edit -> Tool Options -> ReVa`
+> if it is not on your path. But you really should put it on your path!
+
 # Ghidra Support
 
 ## Usage
 
-The [ghidra-assistant](ghidra-assistant/README.md) plugin must be installed first. 
+> The Python package must be installed for the Ghidra extension to work!
+
+Follow the instructions in the [ghidra-assistant](ghidra-assistant/README.md) plugin.
 
 After installation, enable the `ReVaPlugin` extension in the CodeBrowser tool (Open a file and click: File -> Configure -> Miscellaneous).
 
 If you want ReVa enabled by default, click File -> Save Tool to save the configuration.
 
-To start the inference side, open Help -> About ${program name}. In this popup you will see details about your open file.
-The `Program Name:` field is the name you need to pass to `revassistant --project` to start the inference server. In some
-cases this is different to the name in the project view.
+If everything is working correctly you will see a ReVa menu on your menu bar.
 
 ## Undo
 
 Whenever ReVa performs an action it will create an undo point for each action. If ReVa renames 5 variables, this will be
 one undo.
 
 ## Menus
 
+> These are being added in the next release
+
 ReVa adds some elements to the Ghidra UI. You can either ask ReVa to do something in the chat window,
 "Examine the variable usage in `main` in detail, rename the variables with more descriptive names.",
 or use the menu system.
 
 For example you can right click a variable in the decompilation, select Reva -> Rename variable and ReVa
 will perform the action.
 
-Note this uses the same system as chatting with ReVa, this means you can monitor ReVas thoughts in the chat
-window while the action is performed.
-
-# Binary Ninja Support
-
-> Note: Binary Ninja support is currently on hold while the basic functions are implemented in the Ghidra plugin.
-> This is because plugin development for Binary Ninja is easier as we have Python3. I will resume development soon!
-
-Install the ReVA BinaryNinja plugin by opening your BinaryNinja plugin directory (Plugins -> Open Plugin Folder)
-and copying or symbolic linking the [binary-ninja-assistant](./binary-ninja-assistant) directory into the plugin
-directory.
-
-Restart Binary Ninja and "ReVA Push" will be available in the Plugin menu.
-Press this to push data from BinaryNinja to ReVA, then follow the instructions in the [Workflow section](#workflow).
-The project name will be the name of the current open file.
-
 # Support
 
 Do you like my work? Want to support this project and others? Interested in how this project was designed and built?
 This project and many others are built live on my stream at https://twitch.tv/cyberkaida !
```

### Comparing `reverse-engineering-assistant-1.0.3/reverse_engineering_assistant.egg-info/SOURCES.txt` & `reverse_engineering_assistant-2.9.1/reverse_engineering_assistant.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 README.md
 pyproject.toml
+reverse_engineering_assistant/.gitignore
 reverse_engineering_assistant/__init__.py
 reverse_engineering_assistant/assistant.py
 reverse_engineering_assistant/assistant_api_server.py
+reverse_engineering_assistant/chat_client.py
 reverse_engineering_assistant/configuration.py
 reverse_engineering_assistant/documents.py
 reverse_engineering_assistant/model.py
 reverse_engineering_assistant/reva_exceptions.py
 reverse_engineering_assistant/tool.py
-reverse_engineering_assistant/tool_protocol.py
 reverse_engineering_assistant.egg-info/PKG-INFO
 reverse_engineering_assistant.egg-info/SOURCES.txt
 reverse_engineering_assistant.egg-info/dependency_links.txt
 reverse_engineering_assistant.egg-info/entry_points.txt
 reverse_engineering_assistant.egg-info/requires.txt
 reverse_engineering_assistant.egg-info/top_level.txt
 reverse_engineering_assistant/api_server_tools/__init__.py
+reverse_engineering_assistant/api_server_tools/connection.py
 reverse_engineering_assistant/api_server_tools/llm_tools.py
 reverse_engineering_assistant/api_server_tools/re_tools.py
```

