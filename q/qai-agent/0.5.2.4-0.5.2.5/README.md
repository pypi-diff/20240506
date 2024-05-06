# Comparing `tmp/qai_agent-0.5.2.4.tar.gz` & `tmp/qai_agent-0.5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_agent-0.5.2.4.tar", max compression
+gzip compressed data, was "qai_agent-0.5.2.5.tar", max compression
```

## Comparing `qai_agent-0.5.2.4.tar` & `qai_agent-0.5.2.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       13 2024-05-02 06:52:44.114033 qai_agent-0.5.2.4/README.md
--rw-r--r--   0        0        0     1922 2024-05-03 03:44:01.122525 qai_agent-0.5.2.4/pyproject.toml
--rw-r--r--   0        0        0     1227 2024-05-02 06:52:44.117744 qai_agent-0.5.2.4/src/qai/agent/__init__.py
--rw-r--r--   0        0        0    10266 2024-05-03 01:58:29.958742 qai_agent-0.5.2.4/src/qai/agent/agents/campaign_agent.py
--rw-r--r--   0        0        0     2332 2024-05-03 02:00:00.798354 qai_agent-0.5.2.4/src/qai/agent/agents/conversation_agent.py
--rw-r--r--   0        0        0    13254 2024-05-02 17:42:04.131721 qai_agent-0.5.2.4/src/qai/agent/agents/email_agent.py
--rw-r--r--   0        0        0     3389 2024-05-02 06:52:44.120375 qai_agent-0.5.2.4/src/qai/agent/agents/example_agent.py
--rw-r--r--   0        0        0     3505 2024-05-03 01:56:35.020021 qai_agent-0.5.2.4/src/qai/agent/agents/find_agent.py
--rw-r--r--   0        0        0    10827 2024-05-03 01:59:12.545583 qai_agent-0.5.2.4/src/qai/agent/agents/sqlquery_agent.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.118819 qai_agent-0.5.2.4/src/qai/agent/agents/tools/__init__.py
--rw-r--r--   0        0        0     1399 2024-05-02 06:52:44.118768 qai_agent-0.5.2.4/src/qai/agent/agents/tools/outreach.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.124088 qai_agent-0.5.2.4/src/qai/agent/agents/worker/__init__.py
--rw-r--r--   0        0        0     3166 2024-05-02 06:52:44.131675 qai_agent-0.5.2.4/src/qai/agent/basic.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.132044 qai_agent-0.5.2.4/src/qai/agent/data/__init__.py
--rw-r--r--   0        0        0     1284 2024-05-02 06:52:44.131968 qai_agent-0.5.2.4/src/qai/agent/data/state_codes.py
--rw-r--r--   0        0        0     1322 2024-05-02 06:52:44.117542 qai_agent-0.5.2.4/src/qai/agent/llama_index/llm_program.py
--rw-r--r--   0        0        0      170 2024-05-02 06:52:44.116688 qai_agent-0.5.2.4/src/qai/agent/models.py
--rw-r--r--   0        0        0     3312 2024-05-02 06:52:44.116889 qai_agent-0.5.2.4/src/qai/agent/qaibot.py
--rw-r--r--   0        0        0     3403 2024-05-02 06:52:44.117981 qai_agent-0.5.2.4/src/qai/agent/serve.py
--rw-r--r--   0        0        0     1270 2024-05-02 06:52:44.130644 qai_agent-0.5.2.4/src/qai/agent/sessions/qai_session.py
--rw-r--r--   0        0        0        0 2024-05-02 06:52:44.115489 qai_agent-0.5.2.4/src/qai/agent/tools/__init__.py
--rw-r--r--   0        0        0      423 2024-05-02 06:52:44.115702 qai_agent-0.5.2.4/src/qai/agent/tools/types.py
--rw-r--r--   0        0        0     4497 2024-05-02 06:52:44.117132 qai_agent-0.5.2.4/src/qai/agent/tools.py
--rw-r--r--   0        0        0       56 2024-05-02 06:52:44.126120 qai_agent-0.5.2.4/src/qai/agent/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-05-02 06:52:44.128007 qai_agent-0.5.2.4/src/qai/agent/utils/db_utils.py
--rw-r--r--   0        0        0     8321 2024-05-03 02:13:36.174980 qai_agent-0.5.2.4/src/qai/agent/utils/distribute.py
--rw-r--r--   0        0        0     3636 2024-05-02 06:52:44.127769 qai_agent-0.5.2.4/src/qai/agent/utils/utils.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 qai_agent-0.5.2.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-05-02 06:52:44.114033 qai_agent-0.5.2.5/README.md
+-rw-r--r--   0        0        0     1922 2024-05-06 03:49:43.112083 qai_agent-0.5.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-05-02 06:52:44.117744 qai_agent-0.5.2.5/src/qai/agent/__init__.py
+-rw-r--r--   0        0        0    10266 2024-05-03 01:58:29.958742 qai_agent-0.5.2.5/src/qai/agent/agents/campaign_agent.py
+-rw-r--r--   0        0        0     2332 2024-05-03 02:00:00.798354 qai_agent-0.5.2.5/src/qai/agent/agents/conversation_agent.py
+-rw-r--r--   0        0        0    12756 2024-05-06 03:49:18.505943 qai_agent-0.5.2.5/src/qai/agent/agents/email_agent.py
+-rw-r--r--   0        0        0     3389 2024-05-02 06:52:44.120375 qai_agent-0.5.2.5/src/qai/agent/agents/example_agent.py
+-rw-r--r--   0        0        0     3505 2024-05-03 01:56:35.020021 qai_agent-0.5.2.5/src/qai/agent/agents/find_agent.py
+-rw-r--r--   0        0        0    10827 2024-05-03 01:59:12.545583 qai_agent-0.5.2.5/src/qai/agent/agents/sqlquery_agent.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.118819 qai_agent-0.5.2.5/src/qai/agent/agents/tools/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 06:52:44.118768 qai_agent-0.5.2.5/src/qai/agent/agents/tools/outreach.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.124088 qai_agent-0.5.2.5/src/qai/agent/agents/worker/__init__.py
+-rw-r--r--   0        0        0     3166 2024-05-02 06:52:44.131675 qai_agent-0.5.2.5/src/qai/agent/basic.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.132044 qai_agent-0.5.2.5/src/qai/agent/data/__init__.py
+-rw-r--r--   0        0        0     1284 2024-05-02 06:52:44.131968 qai_agent-0.5.2.5/src/qai/agent/data/state_codes.py
+-rw-r--r--   0        0        0     1322 2024-05-02 06:52:44.117542 qai_agent-0.5.2.5/src/qai/agent/llama_index/llm_program.py
+-rw-r--r--   0        0        0      170 2024-05-02 06:52:44.116688 qai_agent-0.5.2.5/src/qai/agent/models.py
+-rw-r--r--   0        0        0     3312 2024-05-02 06:52:44.116889 qai_agent-0.5.2.5/src/qai/agent/qaibot.py
+-rw-r--r--   0        0        0     3403 2024-05-02 06:52:44.117981 qai_agent-0.5.2.5/src/qai/agent/serve.py
+-rw-r--r--   0        0        0     1270 2024-05-02 06:52:44.130644 qai_agent-0.5.2.5/src/qai/agent/sessions/qai_session.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:52:44.115489 qai_agent-0.5.2.5/src/qai/agent/tools/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-02 06:52:44.115702 qai_agent-0.5.2.5/src/qai/agent/tools/types.py
+-rw-r--r--   0        0        0     4497 2024-05-02 06:52:44.117132 qai_agent-0.5.2.5/src/qai/agent/tools.py
+-rw-r--r--   0        0        0       56 2024-05-02 06:52:44.126120 qai_agent-0.5.2.5/src/qai/agent/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-05-02 06:52:44.128007 qai_agent-0.5.2.5/src/qai/agent/utils/db_utils.py
+-rw-r--r--   0        0        0     8321 2024-05-03 02:13:36.174980 qai_agent-0.5.2.5/src/qai/agent/utils/distribute.py
+-rw-r--r--   0        0        0      471 2024-05-06 03:42:15.747389 qai_agent-0.5.2.5/src/qai/agent/utils/schema_utils.py
+-rw-r--r--   0        0        0     3636 2024-05-02 06:52:44.127769 qai_agent-0.5.2.5/src/qai/agent/utils/utils.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 qai_agent-0.5.2.5/PKG-INFO
```

### Comparing `qai_agent-0.5.2.4/pyproject.toml` & `qai_agent-0.5.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = "Qai Agents for the Qai AI Platform"
 name = "qai-agent"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.2.4"
+version = "0.5.2.5"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 install = "^1.3.5"
 llama-index-agent-openai = "^0.2.3"
 llama-index-core = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
```

### Comparing `qai_agent-0.5.2.4/src/qai/agent/__init__.py` & `qai_agent-0.5.2.5/src/qai/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/campaign_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/campaign_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/conversation_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/conversation_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/email_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/email_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from llama_index.core.tools.tool_spec.base import BaseToolSpec
 from llama_index.core.tools.types import BaseTool
 from pydantic import BaseModel, Field
 from pymongo import MongoClient
 
 from qai.agent import ROOT_DIR, cfg
 from qai.agent.utils.distribute import adistribute
+from qai.agent.utils.schema_utils import get_name
 
 log = getLogger(__name__)
 PROJ_DIR = os.path.dirname(os.path.dirname(os.path.dirname(ROOT_DIR)))
 
 example_template = """"""
 job_title_template = """, who holds the job title {job_title}"""
 industry_template = """Industry of {company_name} is {industry}"""
@@ -101,16 +102,16 @@
         Args:
             from_person (dict): The person sending the email.
             from_company (dict): The company sending the email.
             to_person (dict): The person receiving the email.
             to_company (dict): The company receiving the email.
 
         """
-        from_name = self.get_name(from_person)
-        to_name = self.get_name(to_person)
+        from_name = get_name(from_person)
+        to_name = get_name(to_person)
 
         from_company_name = self.get_cname(from_company)
         to_company_name = self.get_cname(to_company)
 
         from_job_title = from_person.get("job_title")
         to_job_title = to_person.get("job_title")
         from_job_title_template = (
@@ -153,30 +154,14 @@
         cname = company.get("company_name")
         if not cname:
             cname = company.get("name")
         if not cname:
             raise ValueError(f"Company must have a name. values={company}")
         return cname
 
-    def get_name(self, person: dict) -> str:
-        """
-        Get the name from the person dict.
-        """
-        name = person.get("name")
-        if not name:
-            first_name = person.get("first_name")
-            last_name = person.get("last_name")
-            if first_name and last_name:
-                name = f"{first_name} {last_name}"
-            else:
-                name = first_name or last_name
-        if not name:
-            raise ValueError(f"Person must have a name. values={person}")
-        return name
-
     def draft_email(
         self,
         to_person: dict,
         to_company: dict,
         prompt: Optional[str] = None,
         callback: Optional[Callable] = None,
     ) -> EmailModel:
```

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/example_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/example_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/find_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/find_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/sqlquery_agent.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/sqlquery_agent.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/agents/tools/outreach.py` & `qai_agent-0.5.2.5/src/qai/agent/agents/tools/outreach.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/basic.py` & `qai_agent-0.5.2.5/src/qai/agent/basic.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/data/state_codes.py` & `qai_agent-0.5.2.5/src/qai/agent/data/state_codes.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/llama_index/llm_program.py` & `qai_agent-0.5.2.5/src/qai/agent/llama_index/llm_program.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/qaibot.py` & `qai_agent-0.5.2.5/src/qai/agent/qaibot.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/serve.py` & `qai_agent-0.5.2.5/src/qai/agent/serve.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/sessions/qai_session.py` & `qai_agent-0.5.2.5/src/qai/agent/sessions/qai_session.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/tools.py` & `qai_agent-0.5.2.5/src/qai/agent/tools.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/utils/distribute.py` & `qai_agent-0.5.2.5/src/qai/agent/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/src/qai/agent/utils/utils.py` & `qai_agent-0.5.2.5/src/qai/agent/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qai_agent-0.5.2.4/PKG-INFO` & `qai_agent-0.5.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qai-agent
-Version: 0.5.2.4
+Version: 0.5.2.5
 Summary: Qai Agents for the Qai AI Platform
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: install (>=1.3.5,<2.0.0)
```

