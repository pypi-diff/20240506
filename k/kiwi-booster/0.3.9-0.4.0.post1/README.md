# Comparing `tmp/kiwi_booster-0.3.9.tar.gz` & `tmp/kiwi_booster-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_booster-0.3.9.tar", max compression
+gzip compressed data, was "kiwi_booster-0.4.0.post1.tar", max compression
```

## Comparing `kiwi_booster-0.3.9.tar` & `kiwi_booster-0.4.0.post1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.3.9/LICENSE
--rw-r--r--   0        0        0     9196 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/README.md
--rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.3.9/kiwi_booster/__init__.py
--rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.3.9/kiwi_booster/common_utils/__init__.py
--rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/common_utils/geographic.py
--rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/common_utils/json.py
--rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.3.9/kiwi_booster/common_utils/loggers.py
--rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.3.9/kiwi_booster/common_utils/requests.py
--rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.3.9/kiwi_booster/common_utils/time.py
--rw-r--r--   0        0        0     3207 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/common_utils/video.py
--rw-r--r--   0        0        0     1794 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/decorators.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/__init__.py
--rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/bigquery.py
--rw-r--r--   0        0        0     1312 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/kfp.py
--rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/secrets.py
--rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.3.9/kiwi_booster/gcp_utils/storage.py
--rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/mcap_utils/__init__.py
--rw-r--r--   0        0        0    11933 2024-04-09 14:19:56.284992 kiwi_booster-0.3.9/kiwi_booster/mcap_utils/decode.py
--rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.3.9/kiwi_booster/ml_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.3.9/kiwi_booster/ml_utils/benchmarks.py
--rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.3.9/kiwi_booster/ml_utils/prediction.py
--rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.3.9/kiwi_booster/slack_utils.py
--rw-r--r--   0        0        0     3095 2024-04-09 14:19:56.288992 kiwi_booster-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    10758 1970-01-01 00:00:00.000000 kiwi_booster-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 16:09:22.014857 kiwi_booster-0.4.0.post1/LICENSE
+-rw-r--r--   0        0        0     9196 2024-04-09 14:19:56.284992 kiwi_booster-0.4.0.post1/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 15:53:32.721294 kiwi_booster-0.4.0.post1/kiwi_booster/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 16:06:23.304697 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/__init__.py
+-rw-r--r--   0        0        0     1199 2024-03-01 18:03:31.363100 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/geographic.py
+-rw-r--r--   0        0        0      578 2024-03-01 18:03:31.363100 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/json.py
+-rw-r--r--   0        0        0     1748 2023-05-14 16:09:16.985180 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/loggers.py
+-rw-r--r--   0        0        0        0 2023-05-11 22:59:08.795321 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/requests.py
+-rw-r--r--   0        0        0     3444 2024-03-01 18:04:06.915726 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/time.py
+-rw-r--r--   0        0        0     3207 2024-04-09 14:19:56.284992 kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/video.py
+-rw-r--r--   0        0        0     2391 2024-04-14 17:15:17.594958 kiwi_booster-0.4.0.post1/kiwi_booster/decorators.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/__init__.py
+-rw-r--r--   0        0        0      569 2024-02-22 20:14:01.692745 kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/bigquery.py
+-rw-r--r--   0        0        0     1312 2024-04-09 14:19:56.284992 kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/kfp.py
+-rw-r--r--   0        0        0     2070 2024-02-23 17:29:39.403328 kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/secrets.py
+-rw-r--r--   0        0        0     3995 2024-03-01 18:04:06.915726 kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/storage.py
+-rw-r--r--   0        0        0        0 2024-03-01 18:03:31.363100 kiwi_booster-0.4.0.post1/kiwi_booster/mcap_utils/__init__.py
+-rw-r--r--   0        0        0    11933 2024-04-09 14:19:56.284992 kiwi_booster-0.4.0.post1/kiwi_booster/mcap_utils/decode.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:46:25.109610 kiwi_booster-0.4.0.post1/kiwi_booster/ml_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:22.783840 kiwi_booster-0.4.0.post1/kiwi_booster/ml_utils/benchmarks.py
+-rw-r--r--   0        0        0        0 2023-05-11 23:00:10.175752 kiwi_booster-0.4.0.post1/kiwi_booster/ml_utils/prediction.py
+-rw-r--r--   0        0        0     4110 2024-03-01 18:03:31.363100 kiwi_booster-0.4.0.post1/kiwi_booster/slack_utils.py
+-rw-r--r--   0        0        0     3079 2024-05-06 20:20:59.688630 kiwi_booster-0.4.0.post1/pyproject.toml
+-rw-r--r--   0        0        0    10715 1970-01-01 00:00:00.000000 kiwi_booster-0.4.0.post1/PKG-INFO
```

### Comparing `kiwi_booster-0.3.9/LICENSE` & `kiwi_booster-0.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/README.md` & `kiwi_booster-0.4.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/common_utils/geographic.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/geographic.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/common_utils/json.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/json.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/common_utils/loggers.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/common_utils/time.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/time.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/common_utils/video.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/common_utils/video.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/decorators.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Module with all the decorators commonly used
 """
 
 import os
 import sys
 import traceback
-from typing import Callable, Union
+from typing import Any, Callable, Optional, Union
+
+from .slack_utils import SlackBot
 
 
 def try_catch_log(function: Callable) -> Callable:
     """
         Decorator to catch and log exceptions.
 
     Args:
@@ -28,35 +30,48 @@
             print(f"[ERROR] args: {args}")
             print(f"[ERROR] kwargs: {kwargs}")
             return None
 
     return wrapper_fun
 
 
-def try_catch(function: Callable) -> None:
+def try_catch(bot: Optional[SlackBot] = None) -> Callable[..., Any]:
     """
     Decorator to run a function within a try-catch block and
-    print the result in case of an error.
+    print the result in case of an error. If a Slack bot is provided,
+    it will send the error message to a Slack channel.
 
     Args:
-        function (Callable): Function to run
+        bot (SlackBot, optional): Slack bot for sending error messages. Defaults to None.
     """
 
-    def wrapper_fun(*args, **kwargs) -> Union[Callable, None]:
-        try:
-            return function(*args, **kwargs)
-        except Exception as e:
-            exc_type, exc_obj, exc_tb = sys.exc_info()
-            # Get next traceback because this one belongs to this wrapper
-            exc_tb = exc_tb.tb_next
-
-            fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-            file = os.path.splitext(fname)[0]
-
-            error_summary = (
-                f"Exception error on file '{file}.py' function '{function.__name__}':"
-                f" {e}, {exc_type}, {fname}, {exc_tb.tb_lineno}"
-            )
-            print(error_summary)
-            traceback.print_exc()
-            full_traceback = traceback.format_exception(type(e), e, e.__traceback__)
-            full_traceback = "".join(full_traceback)
+    def decorator(function: Callable[..., Any]) -> Callable[..., Any]:
+        def wrapper_fun(*args: Any, **kwargs: Any) -> Any:
+            try:
+                return function(*args, **kwargs)
+            except Exception as e:
+                exc_type, exc_obj, exc_tb = sys.exc_info()
+                # Get next traceback because this one belongs to this wrapper
+                exc_tb = exc_tb.tb_next
+
+                fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
+                file = os.path.splitext(fname)[0]
+
+                error_summary = (
+                    f"Exception error on file '{file}.py' function '{function.__name__}':"
+                    f" {e}, {exc_type}, {fname}, {exc_tb.tb_lineno}"
+                )
+                print(error_summary)
+                traceback.print_exc()
+                full_traceback = traceback.format_exception(type(e), e, e.__traceback__)
+                full_traceback = "".join(full_traceback)
+
+                if bot is not None:
+                    bot.send_message(
+                        type="error", summary=error_summary, traceback=full_traceback
+                    )
+
+                return None
+
+        return wrapper_fun
+
+    return decorator
```

### Comparing `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/bigquery.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/bigquery.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/kfp.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/kfp.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/secrets.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/gcp_utils/storage.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/gcp_utils/storage.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/mcap_utils/decode.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/mcap_utils/decode.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/kiwi_booster/slack_utils.py` & `kiwi_booster-0.4.0.post1/kiwi_booster/slack_utils.py`

 * *Files identical despite different names*

### Comparing `kiwi_booster-0.3.9/pyproject.toml` & `kiwi_booster-0.4.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiwi-booster"
-version = "0.3.9"
+version = "0.4.0.post1"
 description = "Python utility functions and classes for KiwiBot AI&Robotics team"
 authors = ["Sebastian Hernandez <juan.hernandez@kiwibot.con>"]
 readme = "README.md"
 packages = [{include = "kiwi_booster"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13.0"
@@ -21,16 +21,15 @@
 google-auth = "^2.18.0"
 timezonefinder = "4.4.1"
 tzlocal = "^5.2"
 mcap = "^1.1.1"
 mcap-ros2-support = "^0.5.3"
 ipregistry = "^3.2.0"
 pillow = "^10.2.0"
-protobuf = "^3.20.0"
-kfp = "^2.4.0"
+kfp = "2.7.0"
 python-path = "^0.1.3"
 opencv-python = { version = "^4.9.0.80", optional = true }
 moviepy = { version = "^1.0.3", optional = true } 
 
 [tool.poetry.extras]
 video = ["opencv-python", "moviepy"]
```

### Comparing `kiwi_booster-0.3.9/PKG-INFO` & `kiwi_booster-0.4.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi-booster
-Version: 0.3.9
+Version: 0.4.0.post1
 Summary: Python utility functions and classes for KiwiBot AI&Robotics team
 Author: Sebastian Hernandez
 Author-email: juan.hernandez@kiwibot.con
 Requires-Python: >=3.8,<3.13.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,23 +14,22 @@
 Provides-Extra: video
 Requires-Dist: google-auth (>=2.18.0,<3.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0)
 Requires-Dist: google-cloud-secret-manager (>=2.16.1,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
 Requires-Dist: google-crc32c (>=1.5.0,<2.0.0)
 Requires-Dist: ipregistry (>=3.2.0,<4.0.0)
-Requires-Dist: kfp (>=2.4.0,<3.0.0)
+Requires-Dist: kfp (==2.7.0)
 Requires-Dist: mcap (>=1.1.1,<2.0.0)
 Requires-Dist: mcap-ros2-support (>=0.5.3,<0.6.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0) ; extra == "video"
 Requires-Dist: numpy (>=1.19,<2.0) ; python_version < "3.9"
 Requires-Dist: numpy (>=1.23,<2.0) ; python_version >= "3.9"
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0) ; extra == "video"
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
-Requires-Dist: protobuf (>=3.20.0,<4.0.0)
 Requires-Dist: python-path (>=0.1.3,<0.2.0)
 Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Requires-Dist: timezonefinder (==4.4.1)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: kiwi-booster Version: 0.3.9 Summary: Python utility
-functions and classes for KiwiBot AI&Robotics team Author: Sebastian Hernandez
-Author-email: juan.hernandez@kiwibot.con Requires-Python: >=3.8,<3.13.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: video Requires-Dist: google-auth (>=2.18.0,<3.0.0) Requires-
-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0) Requires-Dist: google-cloud-
-secret-manager (>=2.16.1,<3.0.0) Requires-Dist: google-cloud-storage
-(>=2.9.0,<3.0.0) Requires-Dist: google-crc32c (>=1.5.0,<2.0.0) Requires-Dist:
-ipregistry (>=3.2.0,<4.0.0) Requires-Dist: kfp (>=2.4.0,<3.0.0) Requires-Dist:
-mcap (>=1.1.1,<2.0.0) Requires-Dist: mcap-ros2-support (>=0.5.3,<0.6.0)
-Requires-Dist: moviepy (>=1.0.3,<2.0.0) ; extra == "video" Requires-Dist: numpy
-(>=1.19,<2.0) ; python_version < "3.9" Requires-Dist: numpy (>=1.23,<2.0) ;
-python_version >= "3.9" Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0) ;
-extra == "video" Requires-Dist: pillow (>=10.2.0,<11.0.0) Requires-Dist:
-protobuf (>=3.20.0,<4.0.0) Requires-Dist: python-path (>=0.1.3,<0.2.0)
-Requires-Dist: slack-sdk (>=3.21.3,<4.0.0) Requires-Dist: structlog
-(>=23.1.0,<24.0.0) Requires-Dist: timezonefinder (==4.4.1) Requires-Dist:
-tzlocal (>=5.2,<6.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: kiwi-booster Version: 0.4.0.post1 Summary: Python
+utility functions and classes for KiwiBot AI&Robotics team Author: Sebastian
+Hernandez Author-email: juan.hernandez@kiwibot.con Requires-Python:
+>=3.8,<3.13.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Provides-Extra: video Requires-Dist: google-auth
+(>=2.18.0,<3.0.0) Requires-Dist: google-cloud-bigquery (>=3.10.0,<4.0.0)
+Requires-Dist: google-cloud-secret-manager (>=2.16.1,<3.0.0) Requires-Dist:
+google-cloud-storage (>=2.9.0,<3.0.0) Requires-Dist: google-crc32c
+(>=1.5.0,<2.0.0) Requires-Dist: ipregistry (>=3.2.0,<4.0.0) Requires-Dist: kfp
+(==2.7.0) Requires-Dist: mcap (>=1.1.1,<2.0.0) Requires-Dist: mcap-ros2-support
+(>=0.5.3,<0.6.0) Requires-Dist: moviepy (>=1.0.3,<2.0.0) ; extra == "video"
+Requires-Dist: numpy (>=1.19,<2.0) ; python_version < "3.9" Requires-Dist:
+numpy (>=1.23,<2.0) ; python_version >= "3.9" Requires-Dist: opencv-python
+(>=4.9.0.80,<5.0.0.0) ; extra == "video" Requires-Dist: pillow
+(>=10.2.0,<11.0.0) Requires-Dist: python-path (>=0.1.3,<0.2.0) Requires-Dist:
+slack-sdk (>=3.21.3,<4.0.0) Requires-Dist: structlog (>=23.1.0,<24.0.0)
+Requires-Dist: timezonefinder (==4.4.1) Requires-Dist: tzlocal (>=5.2,<6.0)
+Description-Content-Type: text/markdown
 
                                     _[_L_o_g_o_]
                             ******** KKiiwwii BBoooosstteerr ********
              Python utils and classes for KiwiBot AI&Robotics team
              _M_a_k_e_ _a_ _P_u_l_l_ _R_e_q_u_e_s_t Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 --- ### Table of contents - [About The Project](#about-the-project) - [MCAP
 ROSBag Decoder](#mcap-rosbag-decoder) - [Getting started](#getting-started) -
```

