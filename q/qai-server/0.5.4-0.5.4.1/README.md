# Comparing `tmp/qai_server-0.5.4.tar.gz` & `tmp/qai_server-0.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_server-0.5.4.tar", max compression
+gzip compressed data, was "qai_server-0.5.4.1.tar", max compression
```

## Comparing `qai_server-0.5.4.tar` & `qai_server-0.5.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1575 2024-05-02 22:14:37.360384 qai_server-0.5.4/README.md
--rw-r--r--   0        0        0     1217 2024-05-03 03:47:46.459844 qai_server-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1168 2024-05-02 06:52:44.104059 qai_server-0.5.4/src/qai/server/__init__.py
--rw-r--r--   0        0        0       60 2024-05-02 21:39:36.863227 qai_server-0.5.4/src/qai/server/config.py
--rw-r--r--   0        0        0       46 2024-05-02 21:15:14.308413 qai_server-0.5.4/src/qai/server/mock/__init__.py
--rw-r--r--   0        0        0      769 2024-05-02 21:40:51.512429 qai_server-0.5.4/src/qai/server/mock/mock_functions.py
--rw-r--r--   0        0        0     2249 2024-05-02 20:49:56.058745 qai_server-0.5.4/src/qai/server/mock/mock_responses.py
--rw-r--r--   0        0        0      781 2024-05-02 21:26:23.357307 qai_server-0.5.4/src/qai/server/mock/mockable.py
--rw-r--r--   0        0        0     3064 2024-05-02 06:52:44.103836 qai_server-0.5.4/src/qai/server/models.py
--rw-r--r--   0        0        0     5029 2024-05-03 03:45:31.299847 qai_server-0.5.4/src/qai/server/serve.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.102448 qai_server-0.5.4/src/qai/server/tools/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-02 21:43:22.021661 qai_server-0.5.4/src/qai/server/tools/security.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 qai_server-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     2365 2024-05-03 04:27:28.235618 qai_server-0.5.4.1/README.md
+-rw-r--r--   0        0        0     1242 2024-05-06 04:00:56.878045 qai_server-0.5.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1168 2024-05-02 06:52:44.104059 qai_server-0.5.4.1/src/qai/server/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-02 21:39:36.863227 qai_server-0.5.4.1/src/qai/server/config.py
+-rw-r--r--   0        0        0       46 2024-05-02 21:15:14.308413 qai_server-0.5.4.1/src/qai/server/mock/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-02 21:40:51.512429 qai_server-0.5.4.1/src/qai/server/mock/mock_functions.py
+-rw-r--r--   0        0        0     2249 2024-05-02 20:49:56.058745 qai_server-0.5.4.1/src/qai/server/mock/mock_responses.py
+-rw-r--r--   0        0        0      781 2024-05-02 21:26:23.357307 qai_server-0.5.4.1/src/qai/server/mock/mockable.py
+-rw-r--r--   0        0        0     3064 2024-05-02 06:52:44.103836 qai_server-0.5.4.1/src/qai/server/models.py
+-rw-r--r--   0        0        0     5045 2024-05-06 03:58:29.798361 qai_server-0.5.4.1/src/qai/server/serve.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.102448 qai_server-0.5.4.1/src/qai/server/tools/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-02 21:43:22.021661 qai_server-0.5.4.1/src/qai/server/tools/security.py
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 qai_server-0.5.4.1/PKG-INFO
```

### Comparing `qai_server-0.5.4/pyproject.toml` & `qai_server-0.5.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = ""
 name = "qai-server"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.4"
+version = "0.5.4.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 beautifulsoup4 = "^4.12.2"
 dataclasses-json = "^0.6.4"
 flask = "^3.0.3"
 flask-pydantic = "^0.12.0"
 ftfy = "^6.1.1"
 gunicorn = "^22.0.0"
 html2text = "^2020.1.16"
 llama-index = "^0.10.33"
 mysql-connector-python = "^8.4.0"
-qai-agent = "^0.5.2.4"
+qai-agent = "^0.5.2.5"
 qai-chat = "^0.5.1"
 torch = [
   {markers = "sys_platform == 'darwin' and platform_machine == 'arm64'", source = "pypi", version = "^2.3.0"},
   {platform = "darwin", source = "pypi", version = "^2.3.0"},
   {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
   {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"}
 ]
 
 [tool.poetry.group.dev.dependencies]
+ecs-deploy = "^1.14.0"
 toml-sort = "^0.23.1"
 
 [[tool.poetry.source]]
 name = "pytorch-cpu-src"
 priority = "explicit"
 url = "https://download.pytorch.org/whl/cpu"
```

### Comparing `qai_server-0.5.4/src/qai/server/__init__.py` & `qai_server-0.5.4.1/src/qai/server/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/src/qai/server/mock/mock_functions.py` & `qai_server-0.5.4.1/src/qai/server/mock/mock_functions.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/src/qai/server/mock/mock_responses.py` & `qai_server-0.5.4.1/src/qai/server/mock/mock_responses.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/src/qai/server/mock/mockable.py` & `qai_server-0.5.4.1/src/qai/server/mock/mockable.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/src/qai/server/models.py` & `qai_server-0.5.4.1/src/qai/server/models.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/src/qai/server/serve.py` & `qai_server-0.5.4.1/src/qai/server/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     if model.user_id in chat_session:
         agent = chat_session[model.user_id]
     else:
         agent = CampaignAgent.create(**model.to_params())
 
     if model.uploaded_data:
         ## convert list of dict to dict of dict
-        uploaded_data = {d["name"]: d for d in model.uploaded_data}
+        uploaded_data = {d.get("id", uuid.uuid4()): d for d in model.uploaded_data}
         agent.people = uploaded_data
     response: CampaignResponse = agent.chat(model.query)
     js = {}
     js["actions"] = [
         {
             "action": "text",
             "response": response.response,
```

### Comparing `qai_server-0.5.4/src/qai/server/tools/security.py` & `qai_server-0.5.4.1/src/qai/server/tools/security.py`

 * *Files identical despite different names*

### Comparing `qai_server-0.5.4/PKG-INFO` & `qai_server-0.5.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-server
-Version: 0.5.4
+Version: 0.5.4.1
 Summary: 
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
@@ -12,15 +12,15 @@
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: flask-pydantic (>=0.12.0,<0.13.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
 Requires-Dist: gunicorn (>=22.0.0,<23.0.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: llama-index (>=0.10.33,<0.11.0)
 Requires-Dist: mysql-connector-python (>=8.4.0,<9.0.0)
-Requires-Dist: qai-agent (>=0.5.2.4,<0.6.0.0)
+Requires-Dist: qai-agent (>=0.5.2.5,<0.6.0.0)
 Requires-Dist: qai-chat (>=0.5.1,<0.6.0)
 Requires-Dist: torch (==2.3.0+cpu) ; sys_platform == "linux"
 Requires-Dist: torch (==2.3.0+cpu) ; sys_platform == "win32"
 Requires-Dist: torch (>=2.3.0,<3.0.0) ; sys_platform == "darwin"
 Requires-Dist: torch (>=2.3.0,<3.0.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Description-Content-Type: text/markdown
 
@@ -30,15 +30,25 @@
 
 ## Features
 
 - Dockerized application for consistency and portability
 - Campaign management
 - Provides RESTful API endpoints for various tasks
 
-## Requirements
+## 🚀 Tech Stack
+
+- ✅ **Connection to the App Server Database**: [MongoDB](https://www.mongodb.com/).
+- ✅ **Vector Database**: [ChromaDB](https://www.trychroma.com/).
+- ✅ **SQL Relational Database**: MySQL, MariaDB, SQLite3, anything that works with [SQLAlchemy](https://www.sqlalchemy.org/).
+
+
+## Prerequisites
+- All of the above tech stack set up.
+
+## Code Requirements
 
 - Python 3.11
 - Docker
 - Poetry
 
 ## Getting Started
 
@@ -51,15 +61,22 @@
 Go to the project folder
 
 ```bash
 cd qrev/ai/projects/server
 ```
 
 ## Setting up the .env file and config.toml file
-For the .env file you can see the example placed in `examples/example.env`
+For the .env file you can see the example placed in [`examples/example.env`](https://github.com/qrev-ai/qrev/tree/main/ai/projects/server/examples/example.env)
+The `config.toml` configuration file is placed in your application directory under the name `qai`. Linux example `~/.config/qai/config.toml`. An example [config.toml](https://github.com/qrev-ai/qrev/tree/main/ai/examples/config.toml)
+
+### Run locally
+From the server project folder. `ai/projects/server`
+```bash
+sh scripts/run_server.sh
+```
 
 ### Build and Run with Docker
 
 Ensure that Docker is installed and running. Then, use the provided Makefile to build and run the project:
 
 1. **Build the Docker Image**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

