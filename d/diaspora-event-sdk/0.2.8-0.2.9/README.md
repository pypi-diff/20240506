# Comparing `tmp/diaspora-event-sdk-0.2.8.tar.gz` & `tmp/diaspora-event-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.8.tar", last modified: Sun May  5 03:31:00 2024, max compression
+gzip compressed data, was "diaspora-event-sdk-0.2.9.tar", last modified: Mon May  6 18:03:09 2024, max compression
```

## Comparing `diaspora-event-sdk-0.2.8.tar` & `diaspora-event-sdk-0.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.270716 diaspora-event-sdk-0.2.8/
--rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/LICENSE
--rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/MANIFEST.in
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:31:00.270560 diaspora-event-sdk-0.2.8/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.8/README.md
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.264942 diaspora-event-sdk-0.2.8/diaspora_event_sdk/
--rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.266359 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/_environments.py
--rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-05 02:43:38.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/aws_iam_msk.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.267264 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-05-05 03:13:17.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)    18699 2024-05-05 02:53:21.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/auth.py
--rw-r--r--   0 haochen    (501) staff       (20)     9344 2024-05-05 02:54:55.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/awsrequest.py
--rw-r--r--   0 haochen    (501) staff       (20)    11093 2024-05-05 03:30:05.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/compat.py
--rw-r--r--   0 haochen    (501) staff       (20)     2455 2024-05-05 02:55:47.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/credentials.py
--rw-r--r--   0 haochen    (501) staff       (20)     2002 2024-05-05 02:55:55.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/exceptions.py
--rw-r--r--   0 haochen    (501) staff       (20)     5370 2024-05-05 02:57:08.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/utils.py
--rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/client.py
--rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-05 02:43:19.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/kafka_client.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.268800 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/
--rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/tokenstore.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.269390 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/utils/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/utils/__init__.py
--rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/web_client.py
--rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-05 03:30:48.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk/version.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.265483 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/
--rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-05 03:31:00.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haochen    (501) staff       (20)     1412 2024-05-05 03:31:00.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-05 03:31:00.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haochen    (501) staff       (20)      110 2024-05-05 03:31:00.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/requires.txt
--rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-05 03:31:00.000000 diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/top_level.txt
--rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-05 03:31:00.270774 diaspora-event-sdk-0.2.8/setup.cfg
--rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-05 03:05:11.000000 diaspora-event-sdk-0.2.8/setup.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.269693 diaspora-event-sdk-0.2.8/tests/
--rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.8/tests/__init__.py
-drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-05 03:31:00.270003 diaspora-event-sdk-0.2.8/tests/unit/
--rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.8/tests/unit/test_client.py
--rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.8/tox.ini
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.715973 diaspora-event-sdk-0.2.9/
+-rw-r--r--   0 haochen    (501) staff       (20)    11357 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/LICENSE
+-rw-r--r--   0 haochen    (501) staff       (20)       58 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/MANIFEST.in
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-06 18:03:09.715847 diaspora-event-sdk-0.2.9/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1735 2024-05-03 15:59:19.000000 diaspora-event-sdk-0.2.9/README.md
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.709321 diaspora-event-sdk-0.2.9/diaspora_event_sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)      457 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.711345 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      204 2024-04-07 17:27:11.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/_environments.py
+-rw-r--r--   0 haochen    (501) staff       (20)     3942 2024-05-05 02:43:38.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/aws_iam_msk.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.713039 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-05-05 03:13:17.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)    18699 2024-05-05 02:53:21.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)     9344 2024-05-05 02:54:55.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/awsrequest.py
+-rw-r--r--   0 haochen    (501) staff       (20)    11197 2024-05-05 03:39:37.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/compat.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2455 2024-05-05 02:55:47.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/credentials.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2002 2024-05-05 02:55:55.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/exceptions.py
+-rw-r--r--   0 haochen    (501) staff       (20)     5370 2024-05-05 02:57:08.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/utils.py
+-rw-r--r--   0 haochen    (501) staff       (20)     8541 2024-05-03 15:08:27.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      884 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4286 2024-05-05 02:43:19.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/kafka_client.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.714819 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/
+-rw-r--r--   0 haochen    (501) staff       (20)      239 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1835 2024-04-08 03:36:21.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 haochen    (501) staff       (20)     1047 2024-04-08 03:39:08.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 haochen    (501) staff       (20)      430 2024-04-08 03:40:29.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 haochen    (501) staff       (20)      977 2024-04-08 03:45:19.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 haochen    (501) staff       (20)     7040 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 haochen    (501) staff       (20)      710 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 haochen    (501) staff       (20)     2094 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/tokenstore.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.715109 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/utils/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 haochen    (501) staff       (20)      470 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 haochen    (501) staff       (20)     4770 2024-05-03 14:59:36.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/web_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)       22 2024-05-05 03:41:17.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk/version.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.709846 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/
+-rw-r--r--   0 haochen    (501) staff       (20)     2108 2024-05-06 18:03:09.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haochen    (501) staff       (20)     1412 2024-05-06 18:03:09.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haochen    (501) staff       (20)        1 2024-05-06 18:03:09.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haochen    (501) staff       (20)      110 2024-05-06 18:03:09.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/requires.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       25 2024-05-06 18:03:09.000000 diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/top_level.txt
+-rw-r--r--   0 haochen    (501) staff       (20)       38 2024-05-06 18:03:09.716014 diaspora-event-sdk-0.2.9/setup.cfg
+-rw-r--r--   0 haochen    (501) staff       (20)     1358 2024-05-05 03:05:11.000000 diaspora-event-sdk-0.2.9/setup.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.715459 diaspora-event-sdk-0.2.9/tests/
+-rw-r--r--   0 haochen    (501) staff       (20)        0 2024-04-05 13:13:01.000000 diaspora-event-sdk-0.2.9/tests/__init__.py
+drwxr-xr-x   0 haochen    (501) staff       (20)        0 2024-05-06 18:03:09.715555 diaspora-event-sdk-0.2.9/tests/unit/
+-rw-r--r--   0 haochen    (501) staff       (20)     3019 2024-04-08 02:07:35.000000 diaspora-event-sdk-0.2.9/tests/unit/test_client.py
+-rw-r--r--   0 haochen    (501) staff       (20)      241 2024-04-08 03:50:13.000000 diaspora-event-sdk-0.2.9/tox.ini
```

### Comparing `diaspora-event-sdk-0.2.8/LICENSE` & `diaspora-event-sdk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/PKG-INFO` & `diaspora-event-sdk-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.8/README.md` & `diaspora-event-sdk-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/aws_iam_msk.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/aws_iam_msk.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/auth.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/auth.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/awsrequest.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/compat.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,46 +92,46 @@
     raise ValueError(f"Expected str or bytes, received {type(s)}.")
 
 
 try:
     import xml.etree.cElementTree as ETree
 except ImportError:
     # cElementTree does not exist from Python3.9+
-    import xml.etree.ElementTree as ETree
+    import xml.etree.ElementTree as ETree  # type: ignore
 XMLParseError = ETree.ParseError
 
 
 # def filter_ssl_warnings():
 #     # Ignore warnings related to SNI as it is not being used in validations.
 #     warnings.filterwarnings(
 #         'ignore',
 #         message="A true SSLContext object is not available.*",
 #         category=exceptions.InsecurePlatformWarning,
 #         module=r".*urllib3\.util\.ssl_",
 #     )
 
 
-@classmethod
+@classmethod  # type: ignore
 def from_dict(cls, d):
     new_instance = cls()
     for key, value in d.items():
         new_instance[key] = value
     return new_instance
 
 
-@classmethod
+@classmethod  # type: ignore
 def from_pairs(cls, pairs):
     new_instance = cls()
     for key, value in pairs:
         new_instance[key] = value
     return new_instance
 
 
-HTTPHeaders.from_dict = from_dict
-HTTPHeaders.from_pairs = from_pairs
+HTTPHeaders.from_dict = from_dict  # type: ignore
+HTTPHeaders.from_pairs = from_pairs  # type: ignore
 
 
 def copy_kwargs(kwargs):
     """
     This used to be a compat shim for 2.6 but is now just an alias.
     """
     copy_kwargs = copy.copy(kwargs)
@@ -288,15 +288,15 @@
 #         return (tzlocal, tzwinlocal)
 #     else:
 #         return (tzlocal,)
 
 
 # Detect if CRT is available for use
 try:
-    import awscrt.auth
+    import awscrt.auth  # type: ignore[import]
 
     # Allow user opt-out if needed
     disabled = os.environ.get('BOTO_DISABLE_CRT', "false")
     HAS_CRT = not disabled.lower() == 'true'
 except ImportError:
     HAS_CRT = False
```

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/credentials.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/credentials.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/exceptions.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/exceptions.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/botocore/utils.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/client.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/decorators.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/kafka_client.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/kafka_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/client_login.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/decorators.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/login_flow.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/manager.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/protocol.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/login_manager/tokenstore.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk/sdk/web_client.py` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/PKG-INFO` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diaspora-event-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: SDK of Diaspora Event Fabric: Resilience-enabling services for science from HPC to edge
 Home-page: https://github.com/globus-labs/diaspora-event-sdk
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: kafka-python
 Provides-Extra: test
```

### Comparing `diaspora-event-sdk-0.2.8/diaspora_event_sdk.egg-info/SOURCES.txt` & `diaspora-event-sdk-0.2.9/diaspora_event_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/setup.py` & `diaspora-event-sdk-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `diaspora-event-sdk-0.2.8/tests/unit/test_client.py` & `diaspora-event-sdk-0.2.9/tests/unit/test_client.py`

 * *Files identical despite different names*

