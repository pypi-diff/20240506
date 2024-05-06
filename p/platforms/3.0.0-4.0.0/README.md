# Comparing `tmp/platforms-3.0.0.tar.gz` & `tmp/platforms-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platforms-3.0.0.tar", last modified: Sun May  5 22:26:22 2024, max compression
+gzip compressed data, was "platforms-4.0.0.tar", last modified: Sun May  5 23:15:50 2024, max compression
```

## Comparing `platforms-3.0.0.tar` & `platforms-4.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.544894 platforms-3.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      994 2024-05-05 22:26:22.541894 platforms-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.478890 platforms-3.0.0/platforms/
--rw-rw-rw-   0        0        0     3577 2024-05-05 22:24:43.000000 platforms-3.0.0/platforms/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-05 22:25:00.000000 platforms-3.0.0/platforms/version.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.535893 platforms-3.0.0/platforms.egg-info/
--rw-rw-rw-   0        0        0      994 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-05 22:26:22.545894 platforms-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.291702 platforms-4.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0      994 2024-05-05 23:15:50.288702 platforms-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.190696 platforms-4.0.0/platforms/
+-rw-rw-rw-   0        0        0     3611 2024-05-05 23:14:19.000000 platforms-4.0.0/platforms/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 23:15:06.000000 platforms-4.0.0/platforms/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.280701 platforms-4.0.0/platforms.egg-info/
+-rw-rw-rw-   0        0        0      994 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-05 23:15:48.000000 platforms-4.0.0/platforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-05 23:15:50.293702 platforms-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-4.0.0/setup.py
```

### Comparing `platforms-3.0.0/LICENSE` & `platforms-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platforms-3.0.0/PKG-INFO` & `platforms-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 3.0.0
+Version: 4.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-3.0.0/README.md` & `platforms-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `platforms-3.0.0/platforms/__init__.py` & `platforms-4.0.0/platforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pyrogram import Client , filters, errors
 from pyrogram.types import ChatMemberUpdated, Message, ChatPermissions, InlineKeyboardButton, InlineKeyboardMarkup, ReplyKeyboardMarkup, CallbackQuery, InputMediaDocument, InputMediaPhoto, InlineQueryResultArticle, InputTextMessageContent, InlineQueryResultPhoto, InlineQueryResultCachedPhoto
 from pyrogram.errors import MessageNotModified, PeerIdInvalid
 from datetime import datetime, timedelta
 from random import randint
 import requests
 import platform
+from colorama import Fore , init
 sistema_operativo = platform.system()
 session = requests.session()
 
 if sistema_operativo == "Windows":
 	cmd = "cls"
 elif sistema_operativo == "Linux":
 	cmd = "clear"
```

### Comparing `platforms-3.0.0/platforms.egg-info/PKG-INFO` & `platforms-4.0.0/platforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 3.0.0
+Version: 4.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-3.0.0/setup.py` & `platforms-4.0.0/setup.py`

 * *Files identical despite different names*

