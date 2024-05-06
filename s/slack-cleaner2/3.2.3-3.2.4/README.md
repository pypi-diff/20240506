# Comparing `tmp/slack_cleaner2-3.2.3.tar.gz` & `tmp/slack_cleaner2-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_cleaner2-3.2.3.tar", last modified: Sat Oct 21 01:18:31 2023, max compression
+gzip compressed data, was "slack_cleaner2-3.2.4.tar", last modified: Mon May  6 01:53:22 2024, max compression
```

## Comparing `slack_cleaner2-3.2.3.tar` & `slack_cleaner2-3.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-10-21 01:18:31.025615 slack_cleaner2-3.2.3/
--rw-rw-rw-   0        0        0     1094 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.3/LICENSE
--rw-rw-rw-   0        0        0      238 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5658 2023-10-21 01:18:31.025615 slack_cleaner2-3.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2022-07-21 13:17:11.000000 slack_cleaner2-3.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-10-21 01:18:31.005137 slack_cleaner2-3.2.3/docs/
--rw-rw-rw-   0        0        0      487 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.3/docs/api.rst
--rw-rw-rw-   0        0        0     6156 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.3/docs/conf.py
--rw-rw-rw-   0        0        0      303 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.3/docs/develop-install.rst
--rw-rw-rw-   0        0        0      495 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.3/docs/index.rst
--rw-rw-rw-   0        0        0      146 2023-03-21 00:30:21.000000 slack_cleaner2-3.2.3/docs/installing.rst
--rw-rw-rw-   0        0        0      116 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.3/docs/introduction.rst
--rw-rw-rw-   0        0        0      121 2023-03-21 00:02:41.000000 slack_cleaner2-3.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       78 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.3/requirements.txt
--rw-rw-rw-   0        0        0      447 2023-10-21 01:18:31.028565 slack_cleaner2-3.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-10-21 01:17:41.000000 slack_cleaner2-3.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-21 01:18:31.012990 slack_cleaner2-3.2.3/slack_cleaner2/
--rw-rw-rw-   0        0        0      670 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.3/slack_cleaner2/__init__.py
--rw-rw-rw-   0        0        0      128 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.3/slack_cleaner2/__main__.py
--rw-rw-rw-   0        0        0      167 2023-10-21 01:17:41.000000 slack_cleaner2-3.2.3/slack_cleaner2/_info.py
--rw-rw-rw-   0        0        0     7411 2023-10-21 01:17:32.000000 slack_cleaner2-3.2.3/slack_cleaner2/cli.py
--rw-rw-rw-   0        0        0     3277 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.3/slack_cleaner2/logger.py
--rw-rw-rw-   0        0        0    46774 2023-04-08 16:44:42.000000 slack_cleaner2-3.2.3/slack_cleaner2/model.py
--rw-rw-rw-   0        0        0     6023 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.3/slack_cleaner2/predicates.py
--rw-rw-rw-   0        0        0      618 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.3/slack_cleaner2/util.py
-drwxrwxrwx   0        0        0        0 2023-10-21 01:18:31.020955 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/
--rw-rw-rw-   0        0        0     5658 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       74 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-10-21 01:18:30.000000 slack_cleaner2-3.2.3/slack_cleaner2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-21 01:18:31.023515 slack_cleaner2-3.2.3/tests/
--rw-rw-rw-   0        0        0       18 2019-09-15 21:36:28.000000 slack_cleaner2-3.2.3/tests/__init__.py
--rw-rw-rw-   0        0        0      734 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.3/tests/test_slack_cleaner2.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:53:22.643495 slack_cleaner2-3.2.4/
+-rw-rw-rw-   0        0        0     1094 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.4/LICENSE
+-rw-rw-rw-   0        0        0      238 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5658 2024-05-06 01:53:22.643495 slack_cleaner2-3.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4914 2022-07-21 13:17:11.000000 slack_cleaner2-3.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 01:53:22.619859 slack_cleaner2-3.2.4/docs/
+-rw-rw-rw-   0        0        0      487 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.4/docs/api.rst
+-rw-rw-rw-   0        0        0     6156 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.4/docs/conf.py
+-rw-rw-rw-   0        0        0      303 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.4/docs/develop-install.rst
+-rw-rw-rw-   0        0        0      495 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.4/docs/index.rst
+-rw-rw-rw-   0        0        0      146 2023-03-21 00:30:21.000000 slack_cleaner2-3.2.4/docs/installing.rst
+-rw-rw-rw-   0        0        0      116 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.4/docs/introduction.rst
+-rw-rw-rw-   0        0        0      121 2023-03-21 00:02:41.000000 slack_cleaner2-3.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       78 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.4/requirements.txt
+-rw-rw-rw-   0        0        0      447 2024-05-06 01:53:22.647494 slack_cleaner2-3.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-05-06 01:44:22.000000 slack_cleaner2-3.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:53:22.632644 slack_cleaner2-3.2.4/slack_cleaner2/
+-rw-rw-rw-   0        0        0      670 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.4/slack_cleaner2/__init__.py
+-rw-rw-rw-   0        0        0      128 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.4/slack_cleaner2/__main__.py
+-rw-rw-rw-   0        0        0      167 2024-05-06 01:44:22.000000 slack_cleaner2-3.2.4/slack_cleaner2/_info.py
+-rw-rw-rw-   0        0        0     7411 2023-10-21 01:18:55.000000 slack_cleaner2-3.2.4/slack_cleaner2/cli.py
+-rw-rw-rw-   0        0        0     3277 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.4/slack_cleaner2/logger.py
+-rw-rw-rw-   0        0        0    46700 2024-05-06 01:34:29.000000 slack_cleaner2-3.2.4/slack_cleaner2/model.py
+-rw-rw-rw-   0        0        0     6023 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.4/slack_cleaner2/predicates.py
+-rw-rw-rw-   0        0        0      618 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.4/slack_cleaner2/util.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:53:22.641111 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/
+-rw-rw-rw-   0        0        0     5658 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       74 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-06 01:53:22.000000 slack_cleaner2-3.2.4/slack_cleaner2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 01:53:22.643495 slack_cleaner2-3.2.4/tests/
+-rw-rw-rw-   0        0        0       18 2019-09-15 21:36:28.000000 slack_cleaner2-3.2.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      734 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.4/tests/test_slack_cleaner2.py
```

### Comparing `slack_cleaner2-3.2.3/LICENSE` & `slack_cleaner2-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/PKG-INFO` & `slack_cleaner2-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_cleaner2
-Version: 3.2.3
+Version: 3.2.4
 Summary: Slack Cleaner2 is an improved slack cleaner version using a python first approach
 Home-page: https://github.com/sgratzl/slack_cleaner2
 Author: Samuel Gratzl
 Author-email: sam@sgratzl.com
 License: MIT license
 Keywords: slack_cleaner2 slack slack-cleaner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `slack_cleaner2-3.2.3/README.md` & `slack_cleaner2-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/docs/conf.py` & `slack_cleaner2-3.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/setup.py` & `slack_cleaner2-3.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup_requirements = ["pytest-runner"]
 test_requirements = ["pytest"]
 
 setup(
     name="slack_cleaner2",
     description="Slack Cleaner2 is an improved slack cleaner version using a python first approach",
-    version="3.2.3",
+    version="3.2.4",
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="slack_cleaner2 slack slack-cleaner",
     author="Samuel Gratzl",
     author_email="sam@sgratzl.com",
     url="https://github.com/sgratzl/slack_cleaner2",
```

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/__init__.py` & `slack_cleaner2-3.2.4/slack_cleaner2/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/cli.py` & `slack_cleaner2-3.2.4/slack_cleaner2/cli.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/logger.py` & `slack_cleaner2-3.2.4/slack_cleaner2/logger.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/model.py` & `slack_cleaner2-3.2.4/slack_cleaner2/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import requests
 from requests import Response
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 from .logger import SlackLogger
 
-
 JSONDict = Dict[str, Any]
 TimeIsh = Union[None, int, str, float]
 
 
 class SlackUser:
     """
     internal model of a slack user
@@ -247,15 +246,15 @@
         for msg in reversed(list(messages)) if asc else messages:
             # Delete user messages
             if msg["type"] == "message":
                 s_msg = SlackMessage(msg, self, self._slack)
                 yield s_msg
 
                 if with_replies and s_msg.has_replies:
-                    yield from self.replies_to(s_msg, after=after_time, before=before_time, asc=asc)
+                    yield from self.replies_to(s_msg, after=after, before=before, asc=asc)
 
     def replies_to(self, base_msg: "SlackMessage", after: TimeIsh = None, before: TimeIsh = None, asc=False) -> Iterator["SlackMessage"]:
         """
         returns the replies to a given SlackMessage instance
 
         :param base_msg: message instance to find replies to
         :type base_msg: SlackMessage
@@ -622,15 +621,15 @@
         super().__init__(entry, slack)
         self.msg = msg
 
     def _context(self) -> str:
         return str(self.msg)
 
     def _delete_impl(self):
-        return self._slack.call_rate_limited(lambda: self._slack.client.reactions_remove(self.name, channel=self.msg.channel.id, timestamp=self.msg.ts))
+        return self._slack.call_rate_limited(lambda: self._slack.client.reactions_remove(name=self.name, channel=self.msg.channel.id, timestamp=self.msg.ts))
 
 
 class SlackFile:
     """
     internal representation of a slack file
     """
 
@@ -896,15 +895,15 @@
         if len(time_str) == 8:
             time_d = time.strptime(time_str, "%Y%m%d")
         else:
             time_d = time.strptime(time_str, "%Y%m%d%H%M")
         sec = time.mktime(time_d)
         return str(int(round(sec)))
     except ValueError:
-        log.exception("error parsing date %s", time_str)
+        log.exception("error parsing date %s (%s)", time_str, type(time_str))
         return None
 
 
 ByKey = TypeVar("ByKey")
 
 
 class ByKeyLookup(Generic[ByKey]):
@@ -1321,16 +1320,15 @@
             if not next_page:
                 # initial call
                 return fun({"count": limit})
             return fun({"page": next_page, "count": limit})
 
         while True:
             page, meta = self.safe_api(list_paging_page, [attr, "paging"], [[], {}], scopes, method)
-            for elem in page:
-                yield elem
+            yield from page
             if not meta:
                 return
             total = meta.get("total", 1)
             current = meta.get("page", 1)
             if current >= total:
                 break
             next_page = current + 1
@@ -1355,16 +1353,15 @@
             if not next_cursor:
                 # initial call
                 return fun({"limit": limit})
             return fun({"cursor": next_cursor, "limit": limit})
 
         while True:
             page, meta = self.safe_api(list_cursor_page, [attr, "response_metadata"], [[], {}], scopes, method)
-            for elem in page:
-                yield elem
+            yield from page
             if not meta or not meta.get("next_cursor"):
                 break
             next_cursor = meta["next_cursor"]
 
     def post_delete(self, obj: Union[SlackMessage, SlackFile, ASlackReaction], error: Optional[SlackApiError] = None):
         """
         log a deleted file or message with optional error
@@ -1425,9 +1422,8 @@
         :return: generator of SlackMessage objects
         :return: generator of SlackMessage objects
         :rtype: SlackMessage
         """
         if not channels:
             channels = self.conversations
         for channel in channels:
-            for msg in channel.msgs(after=after, before=before, with_replies=with_replies):
-                yield msg
+            yield from channel.msgs(after=after, before=before, with_replies=with_replies)
```

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/predicates.py` & `slack_cleaner2-3.2.4/slack_cleaner2/predicates.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2/util.py` & `slack_cleaner2-3.2.4/slack_cleaner2/util.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2.egg-info/PKG-INFO` & `slack_cleaner2-3.2.4/slack_cleaner2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-cleaner2
-Version: 3.2.3
+Version: 3.2.4
 Summary: Slack Cleaner2 is an improved slack cleaner version using a python first approach
 Home-page: https://github.com/sgratzl/slack_cleaner2
 Author: Samuel Gratzl
 Author-email: sam@sgratzl.com
 License: MIT license
 Keywords: slack_cleaner2 slack slack-cleaner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `slack_cleaner2-3.2.3/slack_cleaner2.egg-info/SOURCES.txt` & `slack_cleaner2-3.2.4/slack_cleaner2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.3/tests/test_slack_cleaner2.py` & `slack_cleaner2-3.2.4/tests/test_slack_cleaner2.py`

 * *Files identical despite different names*

