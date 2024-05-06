# Comparing `tmp/telegram_notifier_client-1.1.0.tar.gz` & `tmp/telegram_notifier_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_notifier_client-1.1.0.tar", last modified: Sun Apr 28 14:57:21 2024, max compression
+gzip compressed data, was "telegram_notifier_client-1.2.0.tar", last modified: Mon May  6 06:38:59 2024, max compression
```

## Comparing `telegram_notifier_client-1.1.0.tar` & `telegram_notifier_client-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.1.0/README.md
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-04-28 14:56:42.000000 telegram_notifier_client-1.1.0/pyproject.toml
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/setup.cfg
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-04-28 14:56:42.000000 telegram_notifier_client-1.1.0/setup.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.471851 telegram_notifier_client-1.1.0/src/
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.471851 telegram_notifier_client-1.1.0/src/notifier_client/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.1.0/src/notifier_client/__init__.py
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    19776 2024-04-28 07:31:16.000000 telegram_notifier_client-1.1.0/src/notifier_client/web_app_notifier_client.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-04-28 14:57:21.475851 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/requires.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-04-28 14:57:21.000000 telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/top_level.txt
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.0/README.md
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-05-06 06:32:49.000000 telegram_notifier_client-1.2.0/pyproject.toml
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/setup.cfg
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-05-06 06:32:49.000000 telegram_notifier_client-1.2.0/setup.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.344550 telegram_notifier_client-1.2.0/src/
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.344550 telegram_notifier_client-1.2.0/src/notifier_client/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.0/src/notifier_client/__init__.py
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    20057 2024-05-05 11:18:50.000000 telegram_notifier_client-1.2.0/src/notifier_client/web_app_notifier_client.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/requires.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/top_level.txt
```

### Comparing `telegram_notifier_client-1.1.0/PKG-INFO` & `telegram_notifier_client-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_notifier_client
-Version: 1.1.0
+Version: 1.2.0
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

### Comparing `telegram_notifier_client-1.1.0/src/notifier_client/web_app_notifier_client.py` & `telegram_notifier_client-1.2.0/src/notifier_client/web_app_notifier_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import secrets
 from dataclasses import dataclass
 from logging import Logger
 from typing import Tuple, Optional, Union, List
 
 import requests
 
 logger = logging.getLogger('telegram')
@@ -13,23 +14,25 @@
     return message.replace("<", "&lt;").replace(">", "&gt;")
 
 
 @dataclass
 class Message:
     page: int
     content: str
+    message_tag: str
     emergency: str = ''
     amend: dict = None
 
     def message(self) -> str:
         if self.emergency:
             self.emergency = prepare_for_html(self.emergency)
         self.content = prepare_for_html(self.content)
         emergency = f"<b>Emergency Message</b><blockquote>{self.emergency}</blockquote>\n" if self.emergency else ""
-        return f"<blockquote>{self.content}</blockquote>\n{emergency}<b>Page: {self.page}</b>\n"
+        page = f"<b>Page: {self.page}</b>\n" if self.page > 1 else ""
+        return f"<blockquote>{self.content}</blockquote>\n{emergency}{page}{self.message_tag}"
 
 
 @dataclass
 class PrettifiedMessage:
     title: str
     apm_reference: str
     body: str = None
@@ -366,17 +369,17 @@
         """
         mandatory_msg = f"\nemergency_msg: {emergency_msg}\namend: {amend}"
         first_message_size = self.max_msg_size - len(mandatory_msg)
         if first_message_size < 0:
             raise Exception("Max size is to low")
         first_message = message[:first_message_size]
         rest_of_message = message[first_message_size:]
-
-        return [Message(1, first_message, emergency_msg, amend)] + [
-            Message(page + 2, rest_of_message[i:i + self.max_msg_size])
+        message_tag = f"#{secrets.token_hex(5)}\n" if rest_of_message else ""
+        return [Message(1, first_message, message_tag, emergency_msg, amend)] + [
+            Message(page + 2, rest_of_message[i:i + self.max_msg_size], message_tag)
             for page, i in enumerate(range(0, len(rest_of_message), self.max_msg_size))
         ]
 
     def __send_message_pagination(
             self, message: str, send_func: callable, amend: dict = None, emergency_msg: str = ''
     ) -> Union[int, Optional[Tuple[int, bool]]]:
         """
@@ -434,19 +437,21 @@
             - retrying (int): The number of times to retry sending the message.
         Returns:
             - None
         """
         for _ in range(retrying):
             logger.info(f'{message}, {self.receiver_id}')
             url = f'https://api.telegram.org/bot{self.telegram_bot_token}/sendMessage'
-            amend = prepare_for_html(json.dumps(amend, default=str, indent=4))
+            amend = (f'<b>Amend</b>\n<pre><code class="language-python">'
+                     f'{prepare_for_html(json.dumps(amend, default=str, indent=4))}'
+                     f'</code></pre>\n\n') if amend else ""
             data = {
                 'chat_id': self.receiver_id,
                 'text': f'<b>Message </b>\n{message}\n'
-                        f'<b>Amend</b>\n<pre><code class="language-python">{amend}</code></pre>\n\n'
+                        f'{amend}'
                         f'<b>#emergency</b>',
                 'disable_web_page_preview': True,
                 "parse_mode": "HTML"
             }
             if self.topic_id:
                 data['reply_to_message_id'] = self.topic_id
             if requests.post(url=url, data=data, timeout=15).status_code == 200:
```

### Comparing `telegram_notifier_client-1.1.0/src/telegram_notifier_client.egg-info/PKG-INFO` & `telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-notifier-client
-Version: 1.1.0
+Version: 1.2.0
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

