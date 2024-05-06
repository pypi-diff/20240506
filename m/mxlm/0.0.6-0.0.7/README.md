# Comparing `tmp/mxlm-0.0.6.tar.gz` & `tmp/mxlm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.6.tar", last modified: Tue Apr 23 14:00:02 2024, max compression
+gzip compressed data, was "mxlm-0.0.7.tar", last modified: Mon May  6 03:19:46 2024, max compression
```

## Comparing `mxlm-0.0.6.tar` & `mxlm-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.6/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-23 14:00:02.320421 mxlm-0.0.6/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.6/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-23 13:59:46.000000 mxlm-0.0.6/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.6/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     5941 2024-04-23 13:57:15.000000 mxlm-0.0.6/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.6/mxlm/chatmd_utils.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2265 2024-04-23 13:57:54.000000 mxlm-0.0.6/mxlm/dialog_format_conversion.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      291 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.6/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-23 14:00:02.320421 mxlm-0.0.6/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.6/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-06 03:19:46.695691 mxlm-0.0.7/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.7/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-06 03:19:46.695691 mxlm-0.0.7/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.7/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-06 03:19:46.691691 mxlm-0.0.7/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-05-06 03:19:03.000000 mxlm-0.0.7/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      206 2024-04-30 08:00:37.000000 mxlm-0.0.7/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     6134 2024-04-30 07:49:05.000000 mxlm-0.0.7/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.7/mxlm/chatmd_utils.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2266 2024-04-30 07:52:39.000000 mxlm-0.0.7/mxlm/dialog_format_conversion.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      554 2024-05-06 03:17:22.000000 mxlm-0.0.7/mxlm/mxlm_utils.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-05-06 03:19:46.695691 mxlm-0.0.7/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-05-06 03:19:46.000000 mxlm-0.0.7/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      310 2024-05-06 03:19:46.000000 mxlm-0.0.7/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-05-06 03:19:46.000000 mxlm-0.0.7/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-05-06 03:19:46.000000 mxlm-0.0.7/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-05-06 03:19:46.000000 mxlm-0.0.7/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.7/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-05-06 03:19:46.695691 mxlm-0.0.7/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.7/setup.py
```

### Comparing `mxlm-0.0.6/README.md` & `mxlm-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.6/mxlm/__info__.py` & `mxlm-0.0.7/mxlm/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.6/mxlm/chat_api.py` & `mxlm-0.0.7/mxlm/chat_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,17 @@
         temperature=0.5,
         max_tokens=1024,
         top_p=0.9,
         **default_kwargs,
     ):
         from openai import OpenAI
 
-        self.base_url = base_url or self.default_base_url or os.environ.get("OPENAI_BASE_URL")
+        self.base_url = (
+            base_url or self.default_base_url or os.environ.get("OPENAI_BASE_URL")
+        )
         self.api_key = api_key or os.environ.get("OPENAI_API_KEY", "sk-NoneKey")
 
         # split kwargs to client's kwargs and call kwargs
         client_kwargs = {
             k: default_kwargs.pop(k)
             for k in list(default_kwargs)
             if k in OpenAI.__init__.__code__.co_varnames
@@ -126,17 +128,21 @@
         >>> client(
             {
                 "system": "you are a helpful assistant.",
                 "user": "Tell me a joke."
                 }
             )
         Returns new message.content by default
+
+        Support old completions API when set `completions=True`
         """
         messages = messages or self.default_messages
         messages = self.convert_to_messages(messages)
+        for message in messages:
+            assert "role" in message and "content" in message, message
         kwargs = self.default_kwargs.copy()
         kwargs.update(kwargs_)
         if "stream" in kwargs:
             kwargs["stream"] = bool(kwargs["stream"])
         is_completions = kwargs.pop("completions") if "completions" in kwargs else False
         if is_completions:
             d = self.get_dict_by_completions(messages, **kwargs)
```

### Comparing `mxlm-0.0.6/mxlm/chatmd_utils.py` & `mxlm-0.0.7/mxlm/chatmd_utils.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.6/mxlm/dialog_format_conversion.py` & `mxlm-0.0.7/mxlm/dialog_format_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             + f" {(messages[-1]['content'])}"
         )
     else:
         template += f"<s>{B_INST} {(messages[-1]['content']).strip()} {E_INST}"
     template = template[3:]
     return template
 
+
 if __name__ == "__main__":
     from mxlm import ChatAPI
 
     c = ChatAPI()
     msgs = c(dict(system="Helpful assistant", user="Repeat Yes"), return_messages=True)
     msgs = c(msgs + [{"role": "user", "content": "Repeat No!!!"}], return_messages=True)
```

### Comparing `mxlm-0.0.6/setup.py` & `mxlm-0.0.7/setup.py`

 * *Files identical despite different names*

