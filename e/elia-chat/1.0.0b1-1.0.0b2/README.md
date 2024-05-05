# Comparing `tmp/elia_chat-1.0.0b1.tar.gz` & `tmp/elia_chat-1.0.0b2.tar.gz`

## Comparing `elia_chat-1.0.0b1.tar` & `elia_chat-1.0.0b2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.python-version
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/requirements-dev.lock
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/app.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/config.py
--rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/locations.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/models.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/database/models.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 elia_chat-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/.python-version
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/requirements-dev.lock
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/app.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/config.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/locations.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/models.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 elia_chat-1.0.0b2/PKG-INFO
```

### Comparing `elia_chat-1.0.0b1/.pre-commit-config.yaml` & `elia_chat-1.0.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/requirements-dev.lock` & `elia_chat-1.0.0b2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/requirements.lock` & `elia_chat-1.0.0b2/requirements.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/__main__.py` & `elia_chat-1.0.0b2/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/app.py` & `elia_chat-1.0.0b2/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/chats_manager.py` & `elia_chat-1.0.0b2/elia_chat/chats_manager.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/config.py` & `elia_chat-1.0.0b2/elia_chat/config.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/elia.scss` & `elia_chat-1.0.0b2/elia_chat/elia.scss`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/locations.py` & `elia_chat-1.0.0b2/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/models.py` & `elia_chat-1.0.0b2/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/time_display.py` & `elia_chat-1.0.0b2/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/database/converters.py` & `elia_chat-1.0.0b2/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/database/database.py` & `elia_chat-1.0.0b2/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/database/import_chatgpt.py` & `elia_chat-1.0.0b2/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/database/models.py` & `elia_chat-1.0.0b2/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/screens/chat_details.py` & `elia_chat-1.0.0b2/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/screens/chat_screen.py` & `elia_chat-1.0.0b2/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/screens/help_screen.py` & `elia_chat-1.0.0b2/elia_chat/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/screens/home_screen.py` & `elia_chat-1.0.0b2/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/app_header.py` & `elia_chat-1.0.0b2/elia_chat/widgets/app_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         with Horizontal():
             with Vertical(id="cl-header-container"):
                 yield Label(
                     Text.assemble(
                         ("elia ", title_style + Style(bold=True)),
                         ("///", subtitle_style),
-                        (f" {version('elia')}", title_style),
+                        (f" {version('elia_chat')}", title_style),
                     )
                 )
             model_name = self.elia.runtime_config.selected_model
             model = get_model_by_name(model_name, self.elia.launch_config)
             yield Label(self._get_selected_model_link_text(model), id="model-label")
 
     def _get_selected_model_link_text(self, model: EliaChatModel) -> str:
```

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/chat.py` & `elia_chat-1.0.0b2/elia_chat/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/chat_header.py` & `elia_chat-1.0.0b2/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/chat_list.py` & `elia_chat-1.0.0b2/elia_chat/widgets/chat_list.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/chat_options.py` & `elia_chat-1.0.0b2/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/chatbox.py` & `elia_chat-1.0.0b2/elia_chat/widgets/chatbox.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/prompt_input.py` & `elia_chat-1.0.0b2/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/elia_chat/widgets/token_analysis.py` & `elia_chat-1.0.0b2/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/.gitignore` & `elia_chat-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/README.md` & `elia_chat-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `elia_chat-1.0.0b1/pyproject.toml` & `elia_chat-1.0.0b2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "A terminal interface to ChatGPT."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.0.0b1/PKG-INFO` & `elia_chat-1.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A terminal interface to ChatGPT.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: humanize>=4.6.0
```

