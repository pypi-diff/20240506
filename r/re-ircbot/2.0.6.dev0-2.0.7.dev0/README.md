# Comparing `tmp/re_ircbot-2.0.6.dev0.tar.gz` & `tmp/re_ircbot-2.0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.6.dev0.tar", last modified: Sun May  5 22:01:30 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.7.dev0.tar", last modified: Mon May  6 16:08:14 2024, max compression
```

## Comparing `re_ircbot-2.0.6.dev0.tar` & `re_ircbot-2.0.7.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-05 22:01:22.000000 re_ircbot-2.0.6.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-05 22:01:22.000000 re_ircbot-2.0.6.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54808 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5594 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/format.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18286 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-05 22:01:30.000000 re_ircbot-2.0.6.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-05 22:01:30.235484 re_ircbot-2.0.6.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-05 22:01:23.000000 re_ircbot-2.0.6.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:08:14.853106 re_ircbot-2.0.7.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-06 16:08:14.853106 re_ircbot-2.0.7.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:08:14.849106 re_ircbot-2.0.7.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54808 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5594 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18634 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-06 16:08:14.853106 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-06 16:08:14.000000 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-06 16:08:14.000000 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-06 16:08:14.000000 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-06 16:08:14.000000 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-06 16:08:14.000000 re_ircbot-2.0.7.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-06 16:08:14.853106 re_ircbot-2.0.7.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-06 16:08:05.000000 re_ircbot-2.0.7.dev0/setup.py
```

### Comparing `re_ircbot-2.0.6.dev0/LICENSE` & `re_ircbot-2.0.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/PKG-INFO` & `re_ircbot-2.0.7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.6.dev0
+Version: 2.0.7.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.6.dev0/README.md` & `re_ircbot-2.0.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/client.py` & `re_ircbot-2.0.7.dev0/ircbot/client.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/dcc.py` & `re_ircbot-2.0.7.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/format.py` & `re_ircbot-2.0.7.dev0/ircbot/format.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/hooks.py` & `re_ircbot-2.0.7.dev0/ircbot/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,23 @@
 
     help_msg_header: list[str] = []
     help_msg: dict[str, str] = {}
     help_msg_bottom: list[str] = []
     commands_help = {}
     help_menu_separator: str = "\n"
     help_on_private: bool = False
+    enable_help: bool = True
+
+    def set_auto_help(self, enable: bool) -> Self:
+        """setAutoHelp. Enables or disables the automatic help command.
+
+        :param enable: bool. Enable or disable the automatic help command.
+        """
+        self.enable_help = enable
+        return self
 
     def set_help_menu_separator(self, sep: str) -> Self:
         """Sets the separator string between the help commands. If can contain a
         '\n'.
 
         :param sep: separator
         :type sep: str
@@ -355,14 +364,17 @@
                     self.commands_help[cmd] = cb["help"]
 
             elif isinstance(cb, Callable):
                 self.re_command(expression)(cb)
             else:
                 raise BaseException(f"Invalid command definition for {cmd}")
 
+        if not self.enable_help:
+            return
+
         self._defined_command_dict = command_dict
         if self.help_msg or self.commands_help:
             _commands = find_shortest_prefix([c for c in command_dict.keys() if not not_regex(c)] + ["help"])
 
             def help_menu(args, message):
                 channel = message.channel
                 if self.help_on_private:
```

### Comparing `re_ircbot-2.0.6.dev0/ircbot/message.py` & `re_ircbot-2.0.7.dev0/ircbot/message.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.7.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.7.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/ircbot/utils.py` & `re_ircbot-2.0.7.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.6.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.7.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.6.dev0
+Version: 2.0.7.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.6.dev0/setup.py` & `re_ircbot-2.0.7.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.6-dev"
+VERSION = "2.0.7-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

