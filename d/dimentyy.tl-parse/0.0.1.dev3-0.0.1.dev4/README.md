# Comparing `tmp/dimentyy_tl_parse-0.0.1.dev3.tar.gz` & `tmp/dimentyy_tl_parse-0.0.1.dev4.tar.gz`

## Comparing `dimentyy_tl_parse-0.0.1.dev3.tar` & `dimentyy_tl_parse-0.0.1.dev4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/__init__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/container.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/new_html.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/LICENSE.md
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/pyproject.toml
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/container.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/new_html.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/LICENSE.md
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/pyproject.toml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 dimentyy_tl_parse-0.0.1.dev4/PKG-INFO
```

### Comparing `dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/__init__.py` & `dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Better parsing modes for telethon.TelegramClient"""
+import html
 
 from telethon import TelegramClient
 from telethon.tl.types import TypeMessageEntity
 
 from .new_html import HTMLParser, OnUnknownTag
 
 
@@ -12,15 +13,15 @@
     only by telethon.TelegramClient as it
     automatically parses and unparses messages
     making it easier to work with messages.
 
     **Setup**:
 
     >>> client = TelegramClient(...)
-    >>> client.parse_mode = HTML()
+    >>> parser = HTML.applied_to(client)
     """
 
     def __init__(self, client: TelegramClient, on_unknown_tag: OnUnknownTag = "ignore"):
         self.client = client
         self.on_unknown_tag = on_unknown_tag
 
     @classmethod
@@ -33,21 +34,27 @@
         return self
 
     def parse(self, text: str) -> tuple[str, list[TypeMessageEntity]]:
         """
         **This method is called by** ``telethon.TelegramClient``.
         """
 
-        return HTMLParser.immediate(text, self.on_unknown_tag)
+        return HTMLParser.immediate(text, self.client, self.on_unknown_tag)
 
     def unparse(self, raw_text: str, entities: list[TypeMessageEntity]):
         """
         **This method is called by** ``telethon.TelegramClient``.
 
-        Unparsing occurs when you want to concatenate two messages
+        Unparsing occurs when you want to concatenate two messages.
         """
         raise NotImplementedError
 
+    @staticmethod
+    def mention(user_id: int, content: str, escape: bool = True):
+        """:returns: Mention tag as str."""
+
+        return f"<mention user_id={user_id}>{html.escape(content) if escape else content}</mention>"
+
 
 __all__ = [
     'HTML'
 ]
```

### Comparing `dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/container.py` & `dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/container.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
         # If not all arguments were fulfilled
         # TODO: mode to pass this?
         if None in args.values():
             raise ValueError("Argument has no default value and no value was passed.")
 
         # TODO: mode for handling not opened entities (ignore / raise / full-fill)
-
         current_offset, breaks = self._unclosed_entities.pop(entity, (0, set()))
+
         end_offset = self.raw_text_tl_len
 
         # what?
         for break_offset in sorted(breaks | {end_offset} - {current_offset}):
             self._entities.append(entity(
                 offset=current_offset,
                 length=break_offset - current_offset,
```

### Comparing `dimentyy_tl_parse-0.0.1.dev3/.fake-src/dimentyy/tl/parse/new_html.py` & `dimentyy_tl_parse-0.0.1.dev4/.fake-src/dimentyy/tl/parse/new_html.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from html.parser import HTMLParser as PythonsHTMLParser
-from typing import TypeAlias, Literal, Any, Self
+from typing import TypeAlias, Literal, Any, Self, Optional
 
+from telethon import TelegramClient
 from telethon.tl.types import (MessageEntityBold, MessageEntityItalic, MessageEntityCode,
                                MessageEntityStrike, MessageEntityUnderline, MessageEntityBlockquote,
                                MessageEntitySpoiler, MessageEntityTextUrl, MessageEntityPre,
                                MessageEntityMentionName, MessageEntityCustomEmoji,
                                TypeMessageEntity, InputMessageEntityMentionName)
 
 from .container import ParsingContainer, PlainEntities
 
-OnUnknownTag: TypeAlias = Literal["ignore", "raise"]
+IgnoreUnknownTag: TypeAlias = Literal["ignore"]
+OnUnknownTag: TypeAlias = Literal[IgnoreUnknownTag, "raise"]
 
 
 class HTMLParser(PythonsHTMLParser):
-    def __init__(self, on_unknown_tag: OnUnknownTag):
+    def __init__(self, client: TelegramClient = None, on_unknown_tag: OnUnknownTag = None):
         super().__init__()
 
-        self.on_unknown_tag = on_unknown_tag
+        self.client = client
+
+        self.on_unknown_tag: OnUnknownTag = on_unknown_tag or IgnoreUnknownTag
         self.container = ParsingContainer()
 
     entity_tags = {
         # tag: cls
         "b": MessageEntityBold,
         "i": MessageEntityItalic,
         "u": MessageEntityUnderline,
@@ -97,23 +101,23 @@
         else:
             raise ValueError(f"Unknown '{self.on_unknown_tag}' action on unknown tag.")
 
     def handle_data(self, data: str):  #
         self.container.feed_text(data)
 
     @classmethod
-    def immediate(cls, data: str, unknown_tag: OnUnknownTag) -> tuple[str, list[TypeMessageEntity]]:
+    def immediate(cls, data: str, client: Optional[TelegramClient] = None, unknown_tag: Optional[OnUnknownTag] = None) -> tuple[str, list[TypeMessageEntity]]:
         """
         Just a shorthand:
          - Initialize self;
          - Feed data;
          - Return text & entities.
         """
 
-        self: Self = cls(unknown_tag)
+        self: Self = cls(client, unknown_tag)
         self.feed(data)
         return self.container.bundle
 
 
 __all__ = [
     'HTMLParser', 'OnUnknownTag'
 ]
```

### Comparing `dimentyy_tl_parse-0.0.1.dev3/LICENSE.md` & `dimentyy_tl_parse-0.0.1.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dimentyy_tl_parse-0.0.1.dev3/README.md` & `dimentyy_tl_parse-0.0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dimentyy_tl_parse-0.0.1.dev3/pyproject.toml` & `dimentyy_tl_parse-0.0.1.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.hatch.build.targets.sdist]
 only-include = [".fake-src/dimentyy"]
 
 [project]
 name = "dimentyy.tl-parse"
 description = "Better parsing modes for telethon.TelegramClient"
-version = "0.0.1dev3"
+version = "0.0.1dev4"
 readme = "README.md"
 #requires-python = ">=3.10" #currently unknown
 license = "MIT"
 authors = [
   { name = "dimentyy" },
 ]
 classifiers = [
```

### Comparing `dimentyy_tl_parse-0.0.1.dev3/PKG-INFO` & `dimentyy_tl_parse-0.0.1.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dimentyy.tl-parse
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Better parsing modes for telethon.TelegramClient
 Project-URL: Source, https://github.com/dimentyy/tl-parse.py
 Project-URL: Author, https://t.me/dimentyy
 Author: dimentyy
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: dimentyy.tl-parse Version: 0.0.1.dev3 Summary:
+Metadata-Version: 2.3 Name: dimentyy.tl-parse Version: 0.0.1.dev4 Summary:
 Better parsing modes for telethon.TelegramClient Project-URL: Source, https://
 github.com/dimentyy/tl-parse.py Project-URL: Author, https://t.me/dimentyy
 Author: dimentyy License-Expression: MIT License-File: LICENSE.md Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Requires-Dist: telethon Description-Content-Type: text/markdown #
 Parsing library ### Absolute bloatware. ð ```python from telethon import
 TelegramClient from dimentyy.tl.parse import HTML client: TelegramClient = ...
```

