# Comparing `tmp/kwldn_bot-1.2.2.tar.gz` & `tmp/kwldn_bot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwldn_bot-1.2.2.tar", last modified: Sun Mar  3 01:01:00 2024, max compression
+gzip compressed data, was "kwldn_bot-1.3.0.tar", last modified: Mon May  6 21:34:41 2024, max compression
```

## Comparing `kwldn_bot-1.2.2.tar` & `kwldn_bot-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.799738 kwldn_bot-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-03 01:01:00.799738 kwldn_bot-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 01:01:00.799738 kwldn_bot-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.791738 kwldn_bot-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.795738 kwldn_bot-1.2.2/src/kwldn_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.795738 kwldn_bot-1.2.2/src/kwldn_bot/database/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/database/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.795738 kwldn_bot-1.2.2/src/kwldn_bot/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/modules/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/modules/state_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-03 01:00:52.000000 kwldn_bot-1.2.2/src/kwldn_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:01:00.795738 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-03 01:01:00.000000 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-03 01:01:00.000000 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 01:01:00.000000 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 01:01:00.000000 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-03 01:01:00.000000 kwldn_bot-1.2.2/src/kwldn_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.308267 kwldn_bot-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.308267 kwldn_bot-1.3.0/src/kwldn_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/src/kwldn_bot/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/database/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/src/kwldn_bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/modules/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/modules/state_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 21:34:36.000000 kwldn_bot-1.3.0/src/kwldn_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:34:41.312267 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 21:34:41.000000 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 21:34:41.000000 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:34:41.000000 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:34:41.000000 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 21:34:41.000000 kwldn_bot-1.3.0/src/kwldn_bot.egg-info/top_level.txt
```

### Comparing `kwldn_bot-1.2.2/PKG-INFO` & `kwldn_bot-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwldn_bot
-Version: 1.2.2
+Version: 1.3.0
 Summary: Universal aiogram bot library
 Author-email: kewldan <kewldanil1@gmail.com>
 Project-URL: Homepage, https://github.com/kewldan/xbot
 Keywords: bot,telegram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kwldn_bot-1.2.2/pyproject.toml` & `kwldn_bot-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kwldn_bot"
-version = "1.2.2"
+version = "1.3.0"
 description = "Universal aiogram bot library"
 readme = "README.md"
 authors = [{ name = "kewldan", email = "kewldanil1@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot/bot.py` & `kwldn_bot-1.3.0/src/kwldn_bot/bot.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot/config.py` & `kwldn_bot-1.3.0/src/kwldn_bot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if not os.path.exists('data'):
     os.mkdir('data')
 
 
 class BotSettings(BaseModel):
     token: str = ''
-    owners: list[int] = []
+    owners: list[str] = []
     mongo: str = ''
     debug: bool = True
     database: str = ''
 
 
 class BasicBotConfig(BaseModel):
     bot: BotSettings = BotSettings()
```

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot/modules/error_handler.py` & `kwldn_bot-1.3.0/src/kwldn_bot/modules/error_handler.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot/modules/state_clear.py` & `kwldn_bot-1.3.0/src/kwldn_bot/modules/state_clear.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot/utils.py` & `kwldn_bot-1.3.0/src/kwldn_bot/utils.py`

 * *Files identical despite different names*

### Comparing `kwldn_bot-1.2.2/src/kwldn_bot.egg-info/PKG-INFO` & `kwldn_bot-1.3.0/src/kwldn_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwldn_bot
-Version: 1.2.2
+Version: 1.3.0
 Summary: Universal aiogram bot library
 Author-email: kewldan <kewldanil1@gmail.com>
 Project-URL: Homepage, https://github.com/kewldan/xbot
 Keywords: bot,telegram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

