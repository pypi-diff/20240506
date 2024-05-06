# Comparing `tmp/mypy-boto3-medialive-1.34.83.tar.gz` & `tmp/mypy_boto3_medialive-1.34.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.34.83.tar", last modified: Thu Apr 11 19:18:07 2024, max compression
+gzip compressed data, was "mypy_boto3_medialive-1.34.99.tar", last modified: Mon May  6 19:32:25 2024, max compression
```

## Comparing `mypy-boto3-medialive-1.34.83.tar` & `mypy_boto3_medialive-1.34.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77865 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    77862 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    46713 2024-04-11 19:17:32.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    46713 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18536 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   186555 2024-04-11 19:17:35.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   186555 2024-04-11 19:17:34.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-04-11 19:17:31.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 19:18:07.000000 mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:07.415372 mypy-boto3-medialive-1.34.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-11 19:17:30.000000 mypy-boto3-medialive-1.34.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:25.481575 mypy_boto3_medialive-1.34.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-05-06 19:32:25.481575 mypy_boto3_medialive-1.34.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15669 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:25.481575 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77915 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77912 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    46862 2024-05-06 19:32:10.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46862 2024-05-06 19:32:10.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18500 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   211708 2024-05-06 19:32:14.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211708 2024-05-06 19:32:13.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-05-06 19:32:09.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:32:25.481575 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 19:32:25.000000 mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:32:25.481575 mypy_boto3_medialive-1.34.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-06 19:32:08.000000 mypy_boto3_medialive-1.34.99/setup.py
```

### Comparing `mypy-boto3-medialive-1.34.83/LICENSE` & `mypy_boto3_medialive-1.34.99/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/PKG-INFO` & `mypy_boto3_medialive-1.34.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.83
-Summary: Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.99
+Summary: Type annotations for boto3.MediaLive 1.34.99 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.34.83/README.md` & `mypy_boto3_medialive-1.34.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__init__.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/__main__.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.34.83\n"
-        "Version:         1.34.83\n"
-        "Builder version: 7.23.2\n"
+        "Type annotations for boto3.MediaLive 1.34.99\n"
+        "Version:         1.34.99\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.83")
+    print("1.34.99")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,22 +81,22 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsTypeDef,
+    EncoderSettingsUnionTypeDef,
     EventBridgeRuleTemplateTargetTypeDef,
     GetCloudWatchAlarmTemplateGroupResponseTypeDef,
     GetCloudWatchAlarmTemplateResponseTypeDef,
     GetEventBridgeRuleTemplateGroupResponseTypeDef,
     GetEventBridgeRuleTemplateResponseTypeDef,
     GetSignalMapResponseTypeDef,
-    InputAttachmentTypeDef,
+    InputAttachmentUnionTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -117,15 +117,15 @@
     ListSignalMapsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationTypeDef,
+    OutputDestinationUnionTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     RestartChannelPipelinesResponseTypeDef,
     StartChannelResponseTypeDef,
     StartDeleteMonitorDeploymentResponseTypeDef,
     StartMonitorDeploymentResponseTypeDef,
     StartMultiplexResponseTypeDef,
@@ -306,17 +306,17 @@
         """
 
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -1163,17 +1163,17 @@
         """
 
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -1184,15 +1184,15 @@
         """
 
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/client.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -81,22 +81,22 @@
     DescribeMultiplexProgramResponseTypeDef,
     DescribeMultiplexResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     DescribeReservationResponseTypeDef,
     DescribeScheduleResponseTypeDef,
     DescribeThumbnailsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EncoderSettingsTypeDef,
+    EncoderSettingsUnionTypeDef,
     EventBridgeRuleTemplateTargetTypeDef,
     GetCloudWatchAlarmTemplateGroupResponseTypeDef,
     GetCloudWatchAlarmTemplateResponseTypeDef,
     GetEventBridgeRuleTemplateGroupResponseTypeDef,
     GetEventBridgeRuleTemplateResponseTypeDef,
     GetSignalMapResponseTypeDef,
-    InputAttachmentTypeDef,
+    InputAttachmentUnionTypeDef,
     InputDestinationRequestTypeDef,
     InputDeviceConfigurableSettingsTypeDef,
     InputDeviceRequestTypeDef,
     InputDeviceSettingsTypeDef,
     InputSourceRequestTypeDef,
     InputSpecificationTypeDef,
     InputVpcRequestTypeDef,
@@ -117,15 +117,15 @@
     ListSignalMapsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MaintenanceCreateSettingsTypeDef,
     MaintenanceUpdateSettingsTypeDef,
     MediaConnectFlowRequestTypeDef,
     MultiplexProgramSettingsTypeDef,
     MultiplexSettingsTypeDef,
-    OutputDestinationTypeDef,
+    OutputDestinationUnionTypeDef,
     PurchaseOfferingResponseTypeDef,
     RenewalSettingsTypeDef,
     RestartChannelPipelinesResponseTypeDef,
     StartChannelResponseTypeDef,
     StartDeleteMonitorDeploymentResponseTypeDef,
     StartMonitorDeploymentResponseTypeDef,
     StartMultiplexResponseTypeDef,
@@ -303,17 +303,17 @@
         """
 
     def create_channel(
         self,
         *,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
         ChannelClass: ChannelClassType = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceCreateSettingsTypeDef = ...,
         Name: str = ...,
         RequestId: str = ...,
         Reserved: str = ...,
         RoleArn: str = ...,
@@ -1160,17 +1160,17 @@
         """
 
     def update_channel(
         self,
         *,
         ChannelId: str,
         CdiInputSpecification: CdiInputSpecificationTypeDef = ...,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
-        EncoderSettings: EncoderSettingsTypeDef = ...,
-        InputAttachments: Sequence[InputAttachmentTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
+        EncoderSettings: EncoderSettingsUnionTypeDef = ...,
+        InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,
         InputSpecification: InputSpecificationTypeDef = ...,
         LogLevel: LogLevelType = ...,
         Maintenance: MaintenanceUpdateSettingsTypeDef = ...,
         Name: str = ...,
         RoleArn: str = ...,
     ) -> UpdateChannelResponseTypeDef:
         """
@@ -1181,15 +1181,15 @@
         """
 
     def update_channel_class(
         self,
         *,
         ChannelClass: ChannelClassType,
         ChannelId: str,
-        Destinations: Sequence[OutputDestinationTypeDef] = ...,
+        Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,
     ) -> UpdateChannelClassResponseTypeDef:
         """
         Changes the class of the channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client.update_channel_class)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/client/#update_channel_class)
         """
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     "Scte35AposNoRegionalBlackoutBehaviorType",
     "Scte35AposWebDeliveryAllowedBehaviorType",
     "Scte35ArchiveAllowedFlagType",
     "Scte35DeviceRestrictionsType",
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
+    "Scte35SegmentationScopeType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
     "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
     "SignalMapCreatedWaiterName",
     "SignalMapMonitorDeletedWaiterName",
     "SignalMapMonitorDeployedWaiterName",
@@ -865,14 +866,15 @@
     "NONE", "RESTRICT_GROUP0", "RESTRICT_GROUP1", "RESTRICT_GROUP2"
 ]
 Scte35InputModeType = Literal["FIXED", "FOLLOW_ACTIVE"]
 Scte35NoRegionalBlackoutFlagType = Literal["NO_REGIONAL_BLACKOUT", "REGIONAL_BLACKOUT"]
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
+Scte35SegmentationScopeType = Literal["ALL_OUTPUT_GROUPS", "SCTE35_ENABLED_OUTPUT_GROUPS"]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
 SignalMapCreatedWaiterName = Literal["signal_map_created"]
 SignalMapMonitorDeletedWaiterName = Literal["signal_map_monitor_deleted"]
 SignalMapMonitorDeployedWaiterName = Literal["signal_map_monitor_deployed"]
@@ -1259,14 +1261,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/literals.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     "Scte35AposNoRegionalBlackoutBehaviorType",
     "Scte35AposWebDeliveryAllowedBehaviorType",
     "Scte35ArchiveAllowedFlagType",
     "Scte35DeviceRestrictionsType",
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
+    "Scte35SegmentationScopeType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
     "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
     "SignalMapCreatedWaiterName",
     "SignalMapMonitorDeletedWaiterName",
     "SignalMapMonitorDeployedWaiterName",
@@ -865,14 +866,15 @@
     "NONE", "RESTRICT_GROUP0", "RESTRICT_GROUP1", "RESTRICT_GROUP2"
 ]
 Scte35InputModeType = Literal["FIXED", "FOLLOW_ACTIVE"]
 Scte35NoRegionalBlackoutFlagType = Literal["NO_REGIONAL_BLACKOUT", "REGIONAL_BLACKOUT"]
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
+Scte35SegmentationScopeType = Literal["ALL_OUTPUT_GROUPS", "SCTE35_ENABLED_OUTPUT_GROUPS"]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
 SignalMapCreatedWaiterName = Literal["signal_map_created"]
 SignalMapMonitorDeletedWaiterName = Literal["signal_map_monitor_deleted"]
 SignalMapMonitorDeployedWaiterName = Literal["signal_map_monitor_deployed"]
@@ -1259,14 +1261,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeScheduleResponsePaginatorTypeDef,
-    ListChannelsResponsePaginatorTypeDef,
+    DescribeScheduleResponseTypeDef,
+    ListChannelsResponseTypeDef,
     ListCloudWatchAlarmTemplateGroupsResponseTypeDef,
     ListCloudWatchAlarmTemplatesResponseTypeDef,
     ListEventBridgeRuleTemplateGroupsResponseTypeDef,
     ListEventBridgeRuleTemplatesResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
@@ -103,30 +103,30 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
         self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeScheduleResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListChannelsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 
 class ListCloudWatchAlarmTemplateGroupsPaginator(Paginator):
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/paginator.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    DescribeScheduleResponsePaginatorTypeDef,
-    ListChannelsResponsePaginatorTypeDef,
+    DescribeScheduleResponseTypeDef,
+    ListChannelsResponseTypeDef,
     ListCloudWatchAlarmTemplateGroupsResponseTypeDef,
     ListCloudWatchAlarmTemplatesResponseTypeDef,
     ListEventBridgeRuleTemplateGroupsResponseTypeDef,
     ListEventBridgeRuleTemplatesResponseTypeDef,
     ListInputDevicesResponseTypeDef,
     ListInputDeviceTransfersResponseTypeDef,
     ListInputSecurityGroupsResponseTypeDef,
@@ -101,29 +101,29 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
     """
 
     def paginate(
         self, *, ChannelId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeScheduleResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeScheduleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#describeschedulepaginator)
         """
 
 class ListChannelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListChannelsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/paginators/#listchannelspaginator)
         """
 
 class ListCloudWatchAlarmTemplateGroupsPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AacSettingsTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -272,14 +272,15 @@
     Scte35AposNoRegionalBlackoutBehaviorType,
     Scte35AposWebDeliveryAllowedBehaviorType,
     Scte35ArchiveAllowedFlagType,
     Scte35DeviceRestrictionsType,
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
+    Scte35SegmentationScopeType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
     SignalMapMonitorDeploymentStatusType,
     SignalMapStatusType,
     SmoothGroupAudioOnlyTimecodeControlType,
@@ -446,14 +447,15 @@
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
     "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
     "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
     "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
     "GetEventBridgeRuleTemplateRequestRequestTypeDef",
     "GetSignalMapRequestRequestTypeDef",
+    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -488,35 +490,38 @@
     "SignalMapSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MediaResourceNeighborTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
+    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
-    "RtmpGroupSettingsTypeDef",
+    "RtmpGroupSettingsOutputTypeDef",
     "UdpGroupSettingsTypeDef",
+    "RtmpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
     "RestartChannelPipelinesRequestRequestTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
-    "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
+    "StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef",
+    "StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartDeleteMonitorDeploymentRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartInputDeviceRequestRequestTypeDef",
     "StartMonitorDeploymentRequestRequestTypeDef",
@@ -535,27 +540,31 @@
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
+    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
-    "StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef",
+    "StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef",
+    "StaticImageOutputActivateScheduleActionSettingsOutputTypeDef",
     "StaticImageOutputActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionPaginatorTypeDef",
+    "AudioTrackSelectionExtraOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
     "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
     "CreateCloudWatchAlarmTemplateResponseTypeDef",
@@ -570,14 +579,15 @@
     "UpdateAccountConfigurationResponseTypeDef",
     "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
     "UpdateCloudWatchAlarmTemplateResponseTypeDef",
     "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
     "ListCloudWatchAlarmTemplatesResponseTypeDef",
+    "ColorCorrectionSettingsOutputTypeDef",
     "ColorCorrectionSettingsTypeDef",
     "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
     "CreateEventBridgeRuleTemplateResponseTypeDef",
     "GetEventBridgeRuleTemplateResponseTypeDef",
     "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
     "UpdateEventBridgeRuleTemplateResponseTypeDef",
     "CreateInputRequestRequestTypeDef",
@@ -621,78 +631,93 @@
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
     "M2tsSettingsTypeDef",
+    "OutputLockingSettingsOutputTypeDef",
     "OutputLockingSettingsTypeDef",
     "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
     "ListEventBridgeRuleTemplatesResponseTypeDef",
     "FailoverConditionSettingsTypeDef",
-    "ScheduleActionStartSettingsPaginatorTypeDef",
+    "ScheduleActionStartSettingsExtraOutputTypeDef",
+    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
+    "H265ColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
     "HlsCdnSettingsTypeDef",
     "NetworkInputSettingsTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
     "ListSignalMapsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
     "MediaResourceTypeDef",
+    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
-    "OutputDestinationPaginatorTypeDef",
+    "OutputDestinationExtraOutputTypeDef",
+    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
-    "PauseStateScheduleActionSettingsPaginatorTypeDef",
+    "PauseStateScheduleActionSettingsExtraOutputTypeDef",
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
     "VideoSelectorSettingsTypeDef",
     "ArchiveGroupSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsPaginatorTypeDef",
+    "AudioSelectorSettingsExtraOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
     "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
-    "CaptionSelectorSettingsPaginatorTypeDef",
+    "CaptionSelectorSettingsExtraOutputTypeDef",
+    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
     "ArchiveContainerSettingsTypeDef",
     "UdpContainerSettingsTypeDef",
+    "GlobalConfigurationOutputTypeDef",
     "GlobalConfigurationTypeDef",
     "FailoverConditionTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "InputPrepareScheduleActionSettingsPaginatorTypeDef",
+    "InputPrepareScheduleActionSettingsExtraOutputTypeDef",
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
-    "InputSwitchScheduleActionSettingsPaginatorTypeDef",
+    "InputSwitchScheduleActionSettingsExtraOutputTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
@@ -706,81 +731,97 @@
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
+    "OutputDestinationUnionTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
+    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorPaginatorTypeDef",
+    "AudioSelectorExtraOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionSelectorPaginatorTypeDef",
+    "CaptionSelectorExtraOutputTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "ArchiveOutputSettingsTypeDef",
     "UdpOutputSettingsTypeDef",
-    "AutomaticInputFailoverSettingsPaginatorTypeDef",
+    "AutomaticInputFailoverSettingsExtraOutputTypeDef",
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
+    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "InputSettingsPaginatorTypeDef",
+    "InputSettingsExtraOutputTypeDef",
+    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
-    "Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
-    "InputAttachmentPaginatorTypeDef",
+    "InputAttachmentExtraOutputTypeDef",
+    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
-    "ScheduleActionSettingsPaginatorTypeDef",
+    "ScheduleActionSettingsExtraOutputTypeDef",
+    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
-    "ChannelSummaryPaginatorTypeDef",
     "ChannelSummaryTypeDef",
+    "InputAttachmentUnionTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "ScheduleActionPaginatorTypeDef",
+    "ScheduleActionExtraOutputTypeDef",
+    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
-    "ListChannelsResponsePaginatorTypeDef",
     "ListChannelsResponseTypeDef",
+    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
-    "DescribeScheduleResponsePaginatorTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
+    "DescribeScheduleResponseTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
-    "DescribeScheduleResponseTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
-    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RestartChannelPipelinesResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
+    "CreateChannelRequestRequestTypeDef",
+    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
+    "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
@@ -1791,14 +1832,22 @@
 )
 GetSignalMapRequestRequestTypeDef = TypedDict(
     "GetSignalMapRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
+H264ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H264ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": NotRequired[Dict[str, Any]],
+        "Rec601Settings": NotRequired[Dict[str, Any]],
+        "Rec709Settings": NotRequired[Dict[str, Any]],
+    },
+)
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
         "Rec709Settings": NotRequired[Mapping[str, Any]],
     },
@@ -2159,14 +2208,20 @@
     {
         "Duration": NotRequired[int],
         "PasswordParam": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
+MotionGraphicsSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsSettingsOutputTypeDef",
+    {
+        "HtmlMotionGraphicsSettings": NotRequired[Dict[str, Any]],
+    },
+)
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": NotRequired[Mapping[str, Any]],
     },
 )
 MsSmoothOutputSettingsTypeDef = TypedDict(
@@ -2231,18 +2286,18 @@
     {
         "PasswordParam": NotRequired[str],
         "StreamName": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
-RtmpGroupSettingsTypeDef = TypedDict(
-    "RtmpGroupSettingsTypeDef",
+RtmpGroupSettingsOutputTypeDef = TypedDict(
+    "RtmpGroupSettingsOutputTypeDef",
     {
-        "AdMarkers": NotRequired[Sequence[Literal["ON_CUE_POINT_SCTE35"]]],
+        "AdMarkers": NotRequired[List[Literal["ON_CUE_POINT_SCTE35"]]],
         "AuthenticationScheme": NotRequired[AuthenticationSchemeType],
         "CacheFullBehavior": NotRequired[RtmpCacheFullBehaviorType],
         "CacheLength": NotRequired[int],
         "CaptionData": NotRequired[RtmpCaptionDataType],
         "InputLossAction": NotRequired[InputLossActionForRtmpOutType],
         "RestartDelay": NotRequired[int],
         "IncludeFillerNalUnits": NotRequired[IncludeFillerNalUnitsType],
@@ -2252,14 +2307,27 @@
     "UdpGroupSettingsTypeDef",
     {
         "InputLossAction": NotRequired[InputLossActionForUdpOutType],
         "TimedMetadataId3Frame": NotRequired[UdpTimedMetadataId3FrameType],
         "TimedMetadataId3Period": NotRequired[int],
     },
 )
+RtmpGroupSettingsTypeDef = TypedDict(
+    "RtmpGroupSettingsTypeDef",
+    {
+        "AdMarkers": NotRequired[Sequence[Literal["ON_CUE_POINT_SCTE35"]]],
+        "AuthenticationScheme": NotRequired[AuthenticationSchemeType],
+        "CacheFullBehavior": NotRequired[RtmpCacheFullBehaviorType],
+        "CacheLength": NotRequired[int],
+        "CaptionData": NotRequired[RtmpCaptionDataType],
+        "InputLossAction": NotRequired[InputLossActionForRtmpOutType],
+        "RestartDelay": NotRequired[int],
+        "IncludeFillerNalUnits": NotRequired[IncludeFillerNalUnitsType],
+    },
+)
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 RebootInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2305,16 +2373,24 @@
 StaticImageDeactivateScheduleActionSettingsTypeDef = TypedDict(
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     {
         "FadeOut": NotRequired[int],
         "Layer": NotRequired[int],
     },
 )
-StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
+StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "OutputNames": List[str],
+        "FadeOut": NotRequired[int],
+        "Layer": NotRequired[int],
+    },
+)
+StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef",
     {
         "OutputNames": List[str],
         "FadeOut": NotRequired[int],
         "Layer": NotRequired[int],
     },
 )
 StaticImageOutputDeactivateScheduleActionSettingsTypeDef = TypedDict(
@@ -2527,21 +2603,40 @@
     {
         "Destination": OutputLocationRefTypeDef,
         "CertificateMode": NotRequired[RtmpOutputCertificateModeType],
         "ConnectionRetryInterval": NotRequired[int],
         "NumRetries": NotRequired[int],
     },
 )
+AudioChannelMappingOutputTypeDef = TypedDict(
+    "AudioChannelMappingOutputTypeDef",
+    {
+        "InputChannelLevels": List[InputChannelLevelTypeDef],
+        "OutputChannel": int,
+    },
+)
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": NotRequired[AacSettingsTypeDef],
+        "Ac3Settings": NotRequired[Ac3SettingsTypeDef],
+        "Eac3AtmosSettings": NotRequired[Eac3AtmosSettingsTypeDef],
+        "Eac3Settings": NotRequired[Eac3SettingsTypeDef],
+        "Mp2Settings": NotRequired[Mp2SettingsTypeDef],
+        "PassThroughSettings": NotRequired[Dict[str, Any]],
+        "WavSettings": NotRequired[WavSettingsTypeDef],
+    },
+)
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": NotRequired[AacSettingsTypeDef],
         "Ac3Settings": NotRequired[Ac3SettingsTypeDef],
         "Eac3AtmosSettings": NotRequired[Eac3AtmosSettingsTypeDef],
         "Eac3Settings": NotRequired[Eac3SettingsTypeDef],
@@ -2641,16 +2736,32 @@
         "ImageX": NotRequired[int],
         "ImageY": NotRequired[int],
         "Layer": NotRequired[int],
         "Opacity": NotRequired[int],
         "Width": NotRequired[int],
     },
 )
-StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef",
+StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Image": InputLocationTypeDef,
+        "OutputNames": List[str],
+        "Duration": NotRequired[int],
+        "FadeIn": NotRequired[int],
+        "FadeOut": NotRequired[int],
+        "Height": NotRequired[int],
+        "ImageX": NotRequired[int],
+        "ImageY": NotRequired[int],
+        "Layer": NotRequired[int],
+        "Opacity": NotRequired[int],
+        "Width": NotRequired[int],
+    },
+)
+StaticImageOutputActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageOutputActivateScheduleActionSettingsOutputTypeDef",
     {
         "Image": InputLocationTypeDef,
         "OutputNames": List[str],
         "Duration": NotRequired[int],
         "FadeIn": NotRequired[int],
         "FadeOut": NotRequired[int],
         "Height": NotRequired[int],
@@ -2680,16 +2791,23 @@
 StaticKeySettingsTypeDef = TypedDict(
     "StaticKeySettingsTypeDef",
     {
         "StaticKeyValue": str,
         "KeyProviderServer": NotRequired[InputLocationTypeDef],
     },
 )
-AudioTrackSelectionPaginatorTypeDef = TypedDict(
-    "AudioTrackSelectionPaginatorTypeDef",
+AudioTrackSelectionExtraOutputTypeDef = TypedDict(
+    "AudioTrackSelectionExtraOutputTypeDef",
+    {
+        "Tracks": List[AudioTrackTypeDef],
+        "DolbyEDecode": NotRequired[AudioDolbyEDecodeTypeDef],
+    },
+)
+AudioTrackSelectionOutputTypeDef = TypedDict(
+    "AudioTrackSelectionOutputTypeDef",
     {
         "Tracks": List[AudioTrackTypeDef],
         "DolbyEDecode": NotRequired[AudioDolbyEDecodeTypeDef],
     },
 )
 AudioTrackSelectionTypeDef = TypedDict(
     "AudioTrackSelectionTypeDef",
@@ -2922,24 +3040,30 @@
         "PageNumber": NotRequired[str],
     },
 )
 ListCloudWatchAlarmTemplateGroupsResponseTypeDef = TypedDict(
     "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
     {
         "CloudWatchAlarmTemplateGroups": List[CloudWatchAlarmTemplateGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListCloudWatchAlarmTemplatesResponseTypeDef = TypedDict(
     "ListCloudWatchAlarmTemplatesResponseTypeDef",
     {
         "CloudWatchAlarmTemplates": List[CloudWatchAlarmTemplateSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ColorCorrectionSettingsOutputTypeDef = TypedDict(
+    "ColorCorrectionSettingsOutputTypeDef",
+    {
+        "GlobalColorCorrections": List[ColorCorrectionTypeDef],
     },
 )
 ColorCorrectionSettingsTypeDef = TypedDict(
     "ColorCorrectionSettingsTypeDef",
     {
         "GlobalColorCorrections": Sequence[ColorCorrectionTypeDef],
     },
@@ -3492,47 +3616,66 @@
         "TimedMetadataBehavior": NotRequired[M2tsTimedMetadataBehaviorType],
         "TimedMetadataPid": NotRequired[str],
         "TransportStreamId": NotRequired[int],
         "VideoPid": NotRequired[str],
         "Scte35PrerollPullupMilliseconds": NotRequired[float],
     },
 )
+OutputLockingSettingsOutputTypeDef = TypedDict(
+    "OutputLockingSettingsOutputTypeDef",
+    {
+        "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
+        "PipelineLockingSettings": NotRequired[Dict[str, Any]],
+    },
+)
 OutputLockingSettingsTypeDef = TypedDict(
     "OutputLockingSettingsTypeDef",
     {
         "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
         "PipelineLockingSettings": NotRequired[Mapping[str, Any]],
     },
 )
 ListEventBridgeRuleTemplateGroupsResponseTypeDef = TypedDict(
     "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
     {
         "EventBridgeRuleTemplateGroups": List[EventBridgeRuleTemplateGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEventBridgeRuleTemplatesResponseTypeDef = TypedDict(
     "ListEventBridgeRuleTemplatesResponseTypeDef",
     {
         "EventBridgeRuleTemplates": List[EventBridgeRuleTemplateSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": NotRequired[AudioSilenceFailoverSettingsTypeDef],
         "InputLossSettings": NotRequired[InputLossFailoverSettingsTypeDef],
         "VideoBlackSettings": NotRequired[VideoBlackFailoverSettingsTypeDef],
     },
 )
-ScheduleActionStartSettingsPaginatorTypeDef = TypedDict(
-    "ScheduleActionStartSettingsPaginatorTypeDef",
+ScheduleActionStartSettingsExtraOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsExtraOutputTypeDef",
+    {
+        "FixedModeScheduleActionStartSettings": NotRequired[
+            FixedModeScheduleActionStartSettingsTypeDef
+        ],
+        "FollowModeScheduleActionStartSettings": NotRequired[
+            FollowModeScheduleActionStartSettingsTypeDef
+        ],
+        "ImmediateModeScheduleActionStartSettings": NotRequired[Dict[str, Any]],
+    },
+)
+ScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsOutputTypeDef",
     {
         "FixedModeScheduleActionStartSettings": NotRequired[
             FixedModeScheduleActionStartSettingsTypeDef
         ],
         "FollowModeScheduleActionStartSettings": NotRequired[
             FollowModeScheduleActionStartSettingsTypeDef
         ],
@@ -3579,14 +3722,24 @@
 )
 Mpeg2FilterSettingsTypeDef = TypedDict(
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": NotRequired[TemporalFilterSettingsTypeDef],
     },
 )
+H265ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H265ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": NotRequired[Dict[str, Any]],
+        "DolbyVision81Settings": NotRequired[Dict[str, Any]],
+        "Hdr10Settings": NotRequired[Hdr10SettingsTypeDef],
+        "Rec601Settings": NotRequired[Dict[str, Any]],
+        "Rec709Settings": NotRequired[Dict[str, Any]],
+    },
+)
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "DolbyVision81Settings": NotRequired[Mapping[str, Any]],
         "Hdr10Settings": NotRequired[Hdr10SettingsTypeDef],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
@@ -3676,32 +3829,32 @@
         "AudioChannelPairs": NotRequired[List[InputDeviceUhdAudioChannelPairConfigTypeDef]],
     },
 )
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSignalMapsResponseTypeDef = TypedDict(
     "ListSignalMapsResponseTypeDef",
     {
-        "NextToken": str,
         "SignalMaps": List[SignalMapSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StandardHlsSettingsTypeDef = TypedDict(
     "StandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
         "AudioRenditionSets": NotRequired[str],
@@ -3711,14 +3864,21 @@
     "MediaResourceTypeDef",
     {
         "Destinations": NotRequired[List[MediaResourceNeighborTypeDef]],
         "Name": NotRequired[str],
         "Sources": NotRequired[List[MediaResourceNeighborTypeDef]],
     },
 )
+MotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "MotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
+        "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
+    },
+)
 MotionGraphicsConfigurationTypeDef = TypedDict(
     "MotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
         "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
     },
 )
@@ -3753,16 +3913,25 @@
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NotRequired[NielsenCBETTypeDef],
         "NielsenDistributionType": NotRequired[NielsenWatermarksDistributionTypesType],
         "NielsenNaesIiNwSettings": NotRequired[NielsenNaesIiNwTypeDef],
     },
 )
-OutputDestinationPaginatorTypeDef = TypedDict(
-    "OutputDestinationPaginatorTypeDef",
+OutputDestinationExtraOutputTypeDef = TypedDict(
+    "OutputDestinationExtraOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "MediaPackageSettings": NotRequired[List[MediaPackageOutputDestinationSettingsTypeDef]],
+        "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
+        "Settings": NotRequired[List[OutputDestinationSettingsTypeDef]],
+    },
+)
+OutputDestinationOutputTypeDef = TypedDict(
+    "OutputDestinationOutputTypeDef",
     {
         "Id": NotRequired[str],
         "MediaPackageSettings": NotRequired[List[MediaPackageOutputDestinationSettingsTypeDef]],
         "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
         "Settings": NotRequired[List[OutputDestinationSettingsTypeDef]],
     },
 )
@@ -3771,16 +3940,22 @@
     {
         "Id": NotRequired[str],
         "MediaPackageSettings": NotRequired[Sequence[MediaPackageOutputDestinationSettingsTypeDef]],
         "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
         "Settings": NotRequired[Sequence[OutputDestinationSettingsTypeDef]],
     },
 )
-PauseStateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "PauseStateScheduleActionSettingsPaginatorTypeDef",
+PauseStateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Pipelines": NotRequired[List[PipelinePauseStateSettingsTypeDef]],
+    },
+)
+PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     {
         "Pipelines": NotRequired[List[PipelinePauseStateSettingsTypeDef]],
     },
 )
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
@@ -3821,22 +3996,48 @@
     "ArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "ArchiveCdnSettings": NotRequired[ArchiveCdnSettingsTypeDef],
         "RolloverInterval": NotRequired[int],
     },
 )
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
+        "ChannelsIn": NotRequired[int],
+        "ChannelsOut": NotRequired[int],
+    },
+)
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
         "ChannelsIn": NotRequired[int],
         "ChannelsOut": NotRequired[int],
     },
 )
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "AribDestinationSettings": NotRequired[Dict[str, Any]],
+        "BurnInDestinationSettings": NotRequired[BurnInDestinationSettingsTypeDef],
+        "DvbSubDestinationSettings": NotRequired[DvbSubDestinationSettingsTypeDef],
+        "EbuTtDDestinationSettings": NotRequired[EbuTtDDestinationSettingsTypeDef],
+        "EmbeddedDestinationSettings": NotRequired[Dict[str, Any]],
+        "EmbeddedPlusScte20DestinationSettings": NotRequired[Dict[str, Any]],
+        "RtmpCaptionInfoDestinationSettings": NotRequired[Dict[str, Any]],
+        "Scte20PlusEmbeddedDestinationSettings": NotRequired[Dict[str, Any]],
+        "Scte27DestinationSettings": NotRequired[Dict[str, Any]],
+        "SmpteTtDestinationSettings": NotRequired[Dict[str, Any]],
+        "TeletextDestinationSettings": NotRequired[Dict[str, Any]],
+        "TtmlDestinationSettings": NotRequired[TtmlDestinationSettingsTypeDef],
+        "WebvttDestinationSettings": NotRequired[WebvttDestinationSettingsTypeDef],
+    },
+)
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": NotRequired[Mapping[str, Any]],
         "BurnInDestinationSettings": NotRequired[BurnInDestinationSettingsTypeDef],
         "DvbSubDestinationSettings": NotRequired[DvbSubDestinationSettingsTypeDef],
         "EbuTtDDestinationSettings": NotRequired[EbuTtDDestinationSettingsTypeDef],
@@ -3853,21 +4054,30 @@
 )
 KeyProviderSettingsTypeDef = TypedDict(
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": NotRequired[StaticKeySettingsTypeDef],
     },
 )
-AudioSelectorSettingsPaginatorTypeDef = TypedDict(
-    "AudioSelectorSettingsPaginatorTypeDef",
+AudioSelectorSettingsExtraOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsExtraOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
+        "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
+        "AudioPidSelection": NotRequired[AudioPidSelectionTypeDef],
+        "AudioTrackSelection": NotRequired[AudioTrackSelectionExtraOutputTypeDef],
+    },
+)
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
     {
         "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
         "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
         "AudioPidSelection": NotRequired[AudioPidSelectionTypeDef],
-        "AudioTrackSelection": NotRequired[AudioTrackSelectionPaginatorTypeDef],
+        "AudioTrackSelection": NotRequired[AudioTrackSelectionOutputTypeDef],
     },
 )
 AudioSelectorSettingsTypeDef = TypedDict(
     "AudioSelectorSettingsTypeDef",
     {
         "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
         "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
@@ -3875,18 +4085,31 @@
         "AudioTrackSelection": NotRequired[AudioTrackSelectionTypeDef],
     },
 )
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": NotRequired[AvailSettingsTypeDef],
+        "Scte35SegmentationScope": NotRequired[Scte35SegmentationScopeType],
     },
 )
-CaptionSelectorSettingsPaginatorTypeDef = TypedDict(
-    "CaptionSelectorSettingsPaginatorTypeDef",
+CaptionSelectorSettingsExtraOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsExtraOutputTypeDef",
+    {
+        "AncillarySourceSettings": NotRequired[AncillarySourceSettingsTypeDef],
+        "AribSourceSettings": NotRequired[Dict[str, Any]],
+        "DvbSubSourceSettings": NotRequired[DvbSubSourceSettingsTypeDef],
+        "EmbeddedSourceSettings": NotRequired[EmbeddedSourceSettingsTypeDef],
+        "Scte20SourceSettings": NotRequired[Scte20SourceSettingsTypeDef],
+        "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
+        "TeletextSourceSettings": NotRequired[TeletextSourceSettingsTypeDef],
+    },
+)
+CaptionSelectorSettingsOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsOutputTypeDef",
     {
         "AncillarySourceSettings": NotRequired[AncillarySourceSettingsTypeDef],
         "AribSourceSettings": NotRequired[Dict[str, Any]],
         "DvbSubSourceSettings": NotRequired[DvbSubSourceSettingsTypeDef],
         "EmbeddedSourceSettings": NotRequired[EmbeddedSourceSettingsTypeDef],
         "Scte20SourceSettings": NotRequired[Scte20SourceSettingsTypeDef],
         "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
@@ -3904,25 +4127,25 @@
         "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
         "TeletextSourceSettings": NotRequired[TeletextSourceSettingsTypeDef],
     },
 )
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
-        "NextToken": str,
         "Offerings": List[OfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
-        "NextToken": str,
         "Reservations": List[ReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3942,16 +4165,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3966,14 +4189,26 @@
 )
 UdpContainerSettingsTypeDef = TypedDict(
     "UdpContainerSettingsTypeDef",
     {
         "M2tsSettings": NotRequired[M2tsSettingsTypeDef],
     },
 )
+GlobalConfigurationOutputTypeDef = TypedDict(
+    "GlobalConfigurationOutputTypeDef",
+    {
+        "InitialAudioGain": NotRequired[int],
+        "InputEndAction": NotRequired[GlobalConfigurationInputEndActionType],
+        "InputLossBehavior": NotRequired[InputLossBehaviorTypeDef],
+        "OutputLockingMode": NotRequired[GlobalConfigurationOutputLockingModeType],
+        "OutputTimingSource": NotRequired[GlobalConfigurationOutputTimingSourceType],
+        "SupportLowFramerateInputs": NotRequired[GlobalConfigurationLowFramerateInputsType],
+        "OutputLockingSettings": NotRequired[OutputLockingSettingsOutputTypeDef],
+    },
+)
 GlobalConfigurationTypeDef = TypedDict(
     "GlobalConfigurationTypeDef",
     {
         "InitialAudioGain": NotRequired[int],
         "InputEndAction": NotRequired[GlobalConfigurationInputEndActionType],
         "InputLossBehavior": NotRequired[InputLossBehaviorTypeDef],
         "OutputLockingMode": NotRequired[GlobalConfigurationOutputLockingModeType],
@@ -3991,14 +4226,61 @@
 FrameCaptureGroupSettingsTypeDef = TypedDict(
     "FrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "FrameCaptureCdnSettings": NotRequired[FrameCaptureCdnSettingsTypeDef],
     },
 )
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": NotRequired[H264AdaptiveQuantizationType],
+        "AfdSignaling": NotRequired[AfdSignalingType],
+        "Bitrate": NotRequired[int],
+        "BufFillPct": NotRequired[int],
+        "BufSize": NotRequired[int],
+        "ColorMetadata": NotRequired[H264ColorMetadataType],
+        "ColorSpaceSettings": NotRequired[H264ColorSpaceSettingsOutputTypeDef],
+        "EntropyEncoding": NotRequired[H264EntropyEncodingType],
+        "FilterSettings": NotRequired[H264FilterSettingsTypeDef],
+        "FixedAfd": NotRequired[FixedAfdType],
+        "FlickerAq": NotRequired[H264FlickerAqType],
+        "ForceFieldPictures": NotRequired[H264ForceFieldPicturesType],
+        "FramerateControl": NotRequired[H264FramerateControlType],
+        "FramerateDenominator": NotRequired[int],
+        "FramerateNumerator": NotRequired[int],
+        "GopBReference": NotRequired[H264GopBReferenceType],
+        "GopClosedCadence": NotRequired[int],
+        "GopNumBFrames": NotRequired[int],
+        "GopSize": NotRequired[float],
+        "GopSizeUnits": NotRequired[H264GopSizeUnitsType],
+        "Level": NotRequired[H264LevelType],
+        "LookAheadRateControl": NotRequired[H264LookAheadRateControlType],
+        "MaxBitrate": NotRequired[int],
+        "MinIInterval": NotRequired[int],
+        "NumRefFrames": NotRequired[int],
+        "ParControl": NotRequired[H264ParControlType],
+        "ParDenominator": NotRequired[int],
+        "ParNumerator": NotRequired[int],
+        "Profile": NotRequired[H264ProfileType],
+        "QualityLevel": NotRequired[H264QualityLevelType],
+        "QvbrQualityLevel": NotRequired[int],
+        "RateControlMode": NotRequired[H264RateControlModeType],
+        "ScanType": NotRequired[H264ScanTypeType],
+        "SceneChangeDetect": NotRequired[H264SceneChangeDetectType],
+        "Slices": NotRequired[int],
+        "Softness": NotRequired[int],
+        "SpatialAq": NotRequired[H264SpatialAqType],
+        "SubgopLength": NotRequired[H264SubGopLengthType],
+        "Syntax": NotRequired[H264SyntaxType],
+        "TemporalAq": NotRequired[H264TemporalAqType],
+        "TimecodeInsertion": NotRequired[H264TimecodeInsertionBehaviorType],
+        "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
+    },
+)
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": NotRequired[H264AdaptiveQuantizationType],
         "AfdSignaling": NotRequired[AfdSignalingType],
         "Bitrate": NotRequired[int],
         "BufFillPct": NotRequired[int],
@@ -4060,14 +4342,55 @@
         "GopSizeUnits": NotRequired[Mpeg2GopSizeUnitsType],
         "ScanType": NotRequired[Mpeg2ScanTypeType],
         "SubgopLength": NotRequired[Mpeg2SubGopLengthType],
         "TimecodeInsertion": NotRequired[Mpeg2TimecodeInsertionBehaviorType],
         "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
     },
 )
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "AdaptiveQuantization": NotRequired[H265AdaptiveQuantizationType],
+        "AfdSignaling": NotRequired[AfdSignalingType],
+        "AlternativeTransferFunction": NotRequired[H265AlternativeTransferFunctionType],
+        "Bitrate": NotRequired[int],
+        "BufSize": NotRequired[int],
+        "ColorMetadata": NotRequired[H265ColorMetadataType],
+        "ColorSpaceSettings": NotRequired[H265ColorSpaceSettingsOutputTypeDef],
+        "FilterSettings": NotRequired[H265FilterSettingsTypeDef],
+        "FixedAfd": NotRequired[FixedAfdType],
+        "FlickerAq": NotRequired[H265FlickerAqType],
+        "GopClosedCadence": NotRequired[int],
+        "GopSize": NotRequired[float],
+        "GopSizeUnits": NotRequired[H265GopSizeUnitsType],
+        "Level": NotRequired[H265LevelType],
+        "LookAheadRateControl": NotRequired[H265LookAheadRateControlType],
+        "MaxBitrate": NotRequired[int],
+        "MinIInterval": NotRequired[int],
+        "ParDenominator": NotRequired[int],
+        "ParNumerator": NotRequired[int],
+        "Profile": NotRequired[H265ProfileType],
+        "QvbrQualityLevel": NotRequired[int],
+        "RateControlMode": NotRequired[H265RateControlModeType],
+        "ScanType": NotRequired[H265ScanTypeType],
+        "SceneChangeDetect": NotRequired[H265SceneChangeDetectType],
+        "Slices": NotRequired[int],
+        "Tier": NotRequired[H265TierType],
+        "TimecodeInsertion": NotRequired[H265TimecodeInsertionBehaviorType],
+        "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
+        "MvOverPictureBoundaries": NotRequired[H265MvOverPictureBoundariesType],
+        "MvTemporalPredictor": NotRequired[H265MvTemporalPredictorType],
+        "TileHeight": NotRequired[int],
+        "TilePadding": NotRequired[H265TilePaddingType],
+        "TileWidth": NotRequired[int],
+        "TreeblockSize": NotRequired[H265TreeblockSizeType],
+    },
+)
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "AdaptiveQuantization": NotRequired[H265AdaptiveQuantizationType],
         "AfdSignaling": NotRequired[AfdSignalingType],
@@ -4101,32 +4424,48 @@
         "MvTemporalPredictor": NotRequired[H265MvTemporalPredictorType],
         "TileHeight": NotRequired[int],
         "TilePadding": NotRequired[H265TilePaddingType],
         "TileWidth": NotRequired[int],
         "TreeblockSize": NotRequired[H265TreeblockSizeType],
     },
 )
-InputPrepareScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsPaginatorTypeDef",
+InputPrepareScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "InputAttachmentNameReference": NotRequired[str],
+        "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
+        "UrlPath": NotRequired[List[str]],
+    },
+)
+InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": NotRequired[str],
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[List[str]],
     },
 )
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": NotRequired[str],
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[Sequence[str]],
     },
 )
-InputSwitchScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "InputSwitchScheduleActionSettingsPaginatorTypeDef",
+InputSwitchScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "InputSwitchScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
+        "UrlPath": NotRequired[List[str]],
+    },
+)
+InputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[List[str]],
     },
 )
 InputSwitchScheduleActionSettingsTypeDef = TypedDict(
@@ -4463,16 +4802,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MultiplexProgramSettingsTypeDef = TypedDict(
     "MultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
         "PreferredChannelPipeline": NotRequired[PreferredChannelPipelineType],
@@ -4482,22 +4821,15 @@
 )
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NotRequired[NielsenWatermarksSettingsTypeDef],
     },
 )
-UpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "UpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
-    },
-)
+OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationExtraOutputTypeDef]
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 DescribeThumbnailsResponseTypeDef = TypedDict(
@@ -4512,27 +4844,88 @@
     {
         "ColorSpace": NotRequired[VideoSelectorColorSpaceType],
         "ColorSpaceSettings": NotRequired[VideoSelectorColorSpaceSettingsTypeDef],
         "ColorSpaceUsage": NotRequired[VideoSelectorColorSpaceUsageType],
         "SelectorSettings": NotRequired[VideoSelectorSettingsTypeDef],
     },
 )
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+        "Accessibility": NotRequired[AccessibilityTypeType],
+        "DestinationSettings": NotRequired[CaptionDestinationSettingsOutputTypeDef],
+        "LanguageCode": NotRequired[str],
+        "LanguageDescription": NotRequired[str],
+        "CaptionDashRoles": NotRequired[List[DashRoleCaptionType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
+    },
+)
 CaptionDescriptionTypeDef = TypedDict(
     "CaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
         "Accessibility": NotRequired[AccessibilityTypeType],
         "DestinationSettings": NotRequired[CaptionDestinationSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageDescription": NotRequired[str],
         "CaptionDashRoles": NotRequired[Sequence[DashRoleCaptionType]],
         "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefTypeDef,
+        "AdMarkers": NotRequired[List[HlsAdMarkersType]],
+        "BaseUrlContent": NotRequired[str],
+        "BaseUrlContent1": NotRequired[str],
+        "BaseUrlManifest": NotRequired[str],
+        "BaseUrlManifest1": NotRequired[str],
+        "CaptionLanguageMappings": NotRequired[List[CaptionLanguageMappingTypeDef]],
+        "CaptionLanguageSetting": NotRequired[HlsCaptionLanguageSettingType],
+        "ClientCache": NotRequired[HlsClientCacheType],
+        "CodecSpecification": NotRequired[HlsCodecSpecificationType],
+        "ConstantIv": NotRequired[str],
+        "DirectoryStructure": NotRequired[HlsDirectoryStructureType],
+        "DiscontinuityTags": NotRequired[HlsDiscontinuityTagsType],
+        "EncryptionType": NotRequired[HlsEncryptionTypeType],
+        "HlsCdnSettings": NotRequired[HlsCdnSettingsTypeDef],
+        "HlsId3SegmentTagging": NotRequired[HlsId3SegmentTaggingStateType],
+        "IFrameOnlyPlaylists": NotRequired[IFrameOnlyPlaylistTypeType],
+        "IncompleteSegmentBehavior": NotRequired[HlsIncompleteSegmentBehaviorType],
+        "IndexNSegments": NotRequired[int],
+        "InputLossAction": NotRequired[InputLossActionForHlsOutType],
+        "IvInManifest": NotRequired[HlsIvInManifestType],
+        "IvSource": NotRequired[HlsIvSourceType],
+        "KeepSegments": NotRequired[int],
+        "KeyFormat": NotRequired[str],
+        "KeyFormatVersions": NotRequired[str],
+        "KeyProviderSettings": NotRequired[KeyProviderSettingsTypeDef],
+        "ManifestCompression": NotRequired[HlsManifestCompressionType],
+        "ManifestDurationFormat": NotRequired[HlsManifestDurationFormatType],
+        "MinSegmentLength": NotRequired[int],
+        "Mode": NotRequired[HlsModeType],
+        "OutputSelection": NotRequired[HlsOutputSelectionType],
+        "ProgramDateTime": NotRequired[HlsProgramDateTimeType],
+        "ProgramDateTimeClock": NotRequired[HlsProgramDateTimeClockType],
+        "ProgramDateTimePeriod": NotRequired[int],
+        "RedundantManifest": NotRequired[HlsRedundantManifestType],
+        "SegmentLength": NotRequired[int],
+        "SegmentationMode": NotRequired[HlsSegmentationModeType],
+        "SegmentsPerSubdirectory": NotRequired[int],
+        "StreamInfResolution": NotRequired[HlsStreamInfResolutionType],
+        "TimedMetadataId3Frame": NotRequired[HlsTimedMetadataId3FrameType],
+        "TimedMetadataId3Period": NotRequired[int],
+        "TimestampDeltaMilliseconds": NotRequired[int],
+        "TsFileMode": NotRequired[HlsTsFileModeType],
+    },
+)
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "AdMarkers": NotRequired[Sequence[HlsAdMarkersType]],
         "BaseUrlContent": NotRequired[str],
         "BaseUrlContent1": NotRequired[str],
@@ -4573,34 +4966,49 @@
         "StreamInfResolution": NotRequired[HlsStreamInfResolutionType],
         "TimedMetadataId3Frame": NotRequired[HlsTimedMetadataId3FrameType],
         "TimedMetadataId3Period": NotRequired[int],
         "TimestampDeltaMilliseconds": NotRequired[int],
         "TsFileMode": NotRequired[HlsTsFileModeType],
     },
 )
-AudioSelectorPaginatorTypeDef = TypedDict(
-    "AudioSelectorPaginatorTypeDef",
+AudioSelectorExtraOutputTypeDef = TypedDict(
+    "AudioSelectorExtraOutputTypeDef",
     {
         "Name": str,
-        "SelectorSettings": NotRequired[AudioSelectorSettingsPaginatorTypeDef],
+        "SelectorSettings": NotRequired[AudioSelectorSettingsExtraOutputTypeDef],
+    },
+)
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+        "SelectorSettings": NotRequired[AudioSelectorSettingsOutputTypeDef],
     },
 )
 AudioSelectorTypeDef = TypedDict(
     "AudioSelectorTypeDef",
     {
         "Name": str,
         "SelectorSettings": NotRequired[AudioSelectorSettingsTypeDef],
     },
 )
-CaptionSelectorPaginatorTypeDef = TypedDict(
-    "CaptionSelectorPaginatorTypeDef",
+CaptionSelectorExtraOutputTypeDef = TypedDict(
+    "CaptionSelectorExtraOutputTypeDef",
+    {
+        "Name": str,
+        "LanguageCode": NotRequired[str],
+        "SelectorSettings": NotRequired[CaptionSelectorSettingsExtraOutputTypeDef],
+    },
+)
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
     {
         "Name": str,
         "LanguageCode": NotRequired[str],
-        "SelectorSettings": NotRequired[CaptionSelectorSettingsPaginatorTypeDef],
+        "SelectorSettings": NotRequired[CaptionSelectorSettingsOutputTypeDef],
     },
 )
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "Name": str,
         "LanguageCode": NotRequired[str],
@@ -4620,16 +5028,25 @@
     {
         "ContainerSettings": UdpContainerSettingsTypeDef,
         "Destination": OutputLocationRefTypeDef,
         "BufferMsec": NotRequired[int],
         "FecOutputSettings": NotRequired[FecOutputSettingsTypeDef],
     },
 )
-AutomaticInputFailoverSettingsPaginatorTypeDef = TypedDict(
-    "AutomaticInputFailoverSettingsPaginatorTypeDef",
+AutomaticInputFailoverSettingsExtraOutputTypeDef = TypedDict(
+    "AutomaticInputFailoverSettingsExtraOutputTypeDef",
+    {
+        "SecondaryInputId": str,
+        "ErrorClearTimeMsec": NotRequired[int],
+        "FailoverConditions": NotRequired[List[FailoverConditionTypeDef]],
+        "InputPreference": NotRequired[InputPreferenceType],
+    },
+)
+AutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     {
         "SecondaryInputId": str,
         "ErrorClearTimeMsec": NotRequired[int],
         "FailoverConditions": NotRequired[List[FailoverConditionTypeDef]],
         "InputPreference": NotRequired[InputPreferenceType],
     },
 )
@@ -4638,14 +5055,23 @@
     {
         "SecondaryInputId": str,
         "ErrorClearTimeMsec": NotRequired[int],
         "FailoverConditions": NotRequired[Sequence[FailoverConditionTypeDef]],
         "InputPreference": NotRequired[InputPreferenceType],
     },
 )
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "FrameCaptureSettings": NotRequired[FrameCaptureSettingsTypeDef],
+        "H264Settings": NotRequired[H264SettingsOutputTypeDef],
+        "H265Settings": NotRequired[H265SettingsOutputTypeDef],
+        "Mpeg2Settings": NotRequired[Mpeg2SettingsTypeDef],
+    },
+)
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": NotRequired[FrameCaptureSettingsTypeDef],
         "H264Settings": NotRequired[H264SettingsTypeDef],
         "H265Settings": NotRequired[H265SettingsTypeDef],
         "Mpeg2Settings": NotRequired[Mpeg2SettingsTypeDef],
@@ -4665,31 +5091,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HlsOutputSettingsTypeDef = TypedDict(
     "HlsOutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
         "H265PackagingType": NotRequired[HlsH265PackagingTypeType],
@@ -4756,14 +5182,32 @@
     "UpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
         "MultiplexProgramSettings": NotRequired[MultiplexProgramSettingsTypeDef],
     },
 )
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+        "Name": str,
+        "AudioNormalizationSettings": NotRequired[AudioNormalizationSettingsTypeDef],
+        "AudioType": NotRequired[AudioTypeType],
+        "AudioTypeControl": NotRequired[AudioDescriptionAudioTypeControlType],
+        "AudioWatermarkingSettings": NotRequired[AudioWatermarkSettingsTypeDef],
+        "CodecSettings": NotRequired[AudioCodecSettingsOutputTypeDef],
+        "LanguageCode": NotRequired[str],
+        "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
+        "RemixSettings": NotRequired[RemixSettingsOutputTypeDef],
+        "StreamName": NotRequired[str],
+        "AudioDashRoles": NotRequired[List[DashRoleAudioType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
+    },
+)
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
         "AudioNormalizationSettings": NotRequired[AudioNormalizationSettingsTypeDef],
         "AudioType": NotRequired[AudioTypeType],
@@ -4774,39 +5218,77 @@
         "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
         "RemixSettings": NotRequired[RemixSettingsTypeDef],
         "StreamName": NotRequired[str],
         "AudioDashRoles": NotRequired[Sequence[DashRoleAudioType]],
         "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
+UpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "UpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
+    },
+)
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "ArchiveGroupSettings": NotRequired[ArchiveGroupSettingsTypeDef],
+        "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
+        "HlsGroupSettings": NotRequired[HlsGroupSettingsOutputTypeDef],
+        "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
+        "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
+        "MultiplexGroupSettings": NotRequired[Dict[str, Any]],
+        "RtmpGroupSettings": NotRequired[RtmpGroupSettingsOutputTypeDef],
+        "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
+        "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
+    },
+)
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": NotRequired[ArchiveGroupSettingsTypeDef],
         "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
         "HlsGroupSettings": NotRequired[HlsGroupSettingsTypeDef],
         "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
         "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
         "MultiplexGroupSettings": NotRequired[Mapping[str, Any]],
         "RtmpGroupSettings": NotRequired[RtmpGroupSettingsTypeDef],
         "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
         "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
     },
 )
-InputSettingsPaginatorTypeDef = TypedDict(
-    "InputSettingsPaginatorTypeDef",
+InputSettingsExtraOutputTypeDef = TypedDict(
+    "InputSettingsExtraOutputTypeDef",
+    {
+        "AudioSelectors": NotRequired[List[AudioSelectorExtraOutputTypeDef]],
+        "CaptionSelectors": NotRequired[List[CaptionSelectorExtraOutputTypeDef]],
+        "DeblockFilter": NotRequired[InputDeblockFilterType],
+        "DenoiseFilter": NotRequired[InputDenoiseFilterType],
+        "FilterStrength": NotRequired[int],
+        "InputFilter": NotRequired[InputFilterType],
+        "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
+        "Scte35Pid": NotRequired[int],
+        "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
+        "SourceEndBehavior": NotRequired[InputSourceEndBehaviorType],
+        "VideoSelector": NotRequired[VideoSelectorTypeDef],
+    },
+)
+InputSettingsOutputTypeDef = TypedDict(
+    "InputSettingsOutputTypeDef",
     {
-        "AudioSelectors": NotRequired[List[AudioSelectorPaginatorTypeDef]],
-        "CaptionSelectors": NotRequired[List[CaptionSelectorPaginatorTypeDef]],
+        "AudioSelectors": NotRequired[List[AudioSelectorOutputTypeDef]],
+        "CaptionSelectors": NotRequired[List[CaptionSelectorOutputTypeDef]],
         "DeblockFilter": NotRequired[InputDeblockFilterType],
         "DenoiseFilter": NotRequired[InputDenoiseFilterType],
         "FilterStrength": NotRequired[int],
         "InputFilter": NotRequired[InputFilterType],
         "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
         "Scte35Pid": NotRequired[int],
         "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
@@ -4826,14 +5308,26 @@
         "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
         "Scte35Pid": NotRequired[int],
         "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
         "SourceEndBehavior": NotRequired[InputSourceEndBehaviorType],
         "VideoSelector": NotRequired[VideoSelectorTypeDef],
     },
 )
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "Name": str,
+        "CodecSettings": NotRequired[VideoCodecSettingsOutputTypeDef],
+        "Height": NotRequired[int],
+        "RespondToAfd": NotRequired[VideoDescriptionRespondToAfdType],
+        "ScalingBehavior": NotRequired[VideoDescriptionScalingBehaviorType],
+        "Sharpness": NotRequired[int],
+        "Width": NotRequired[int],
+    },
+)
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "Name": str,
         "CodecSettings": NotRequired[VideoCodecSettingsTypeDef],
         "Height": NotRequired[int],
         "RespondToAfd": NotRequired[VideoDescriptionRespondToAfdType],
@@ -4866,35 +5360,50 @@
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef",
+Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
+    },
+)
+Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     {
         "Scte35Descriptors": List[Scte35DescriptorTypeDef],
     },
 )
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
-InputAttachmentPaginatorTypeDef = TypedDict(
-    "InputAttachmentPaginatorTypeDef",
+InputAttachmentExtraOutputTypeDef = TypedDict(
+    "InputAttachmentExtraOutputTypeDef",
     {
         "AutomaticInputFailoverSettings": NotRequired[
-            AutomaticInputFailoverSettingsPaginatorTypeDef
+            AutomaticInputFailoverSettingsExtraOutputTypeDef
         ],
         "InputAttachmentName": NotRequired[str],
         "InputId": NotRequired[str],
-        "InputSettings": NotRequired[InputSettingsPaginatorTypeDef],
+        "InputSettings": NotRequired[InputSettingsExtraOutputTypeDef],
+    },
+)
+InputAttachmentOutputTypeDef = TypedDict(
+    "InputAttachmentOutputTypeDef",
+    {
+        "AutomaticInputFailoverSettings": NotRequired[AutomaticInputFailoverSettingsOutputTypeDef],
+        "InputAttachmentName": NotRequired[str],
+        "InputId": NotRequired[str],
+        "InputSettings": NotRequired[InputSettingsOutputTypeDef],
     },
 )
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": NotRequired[AutomaticInputFailoverSettingsTypeDef],
         "InputAttachmentName": NotRequired[str],
@@ -4908,47 +5417,83 @@
         "OutputSettings": OutputSettingsTypeDef,
         "AudioDescriptionNames": NotRequired[Sequence[str]],
         "CaptionDescriptionNames": NotRequired[Sequence[str]],
         "OutputName": NotRequired[str],
         "VideoDescriptionName": NotRequired[str],
     },
 )
-ScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "ScheduleActionSettingsPaginatorTypeDef",
+ScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsExtraOutputTypeDef",
     {
         "HlsId3SegmentTaggingSettings": NotRequired[
             HlsId3SegmentTaggingScheduleActionSettingsTypeDef
         ],
         "HlsTimedMetadataSettings": NotRequired[HlsTimedMetadataScheduleActionSettingsTypeDef],
-        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsPaginatorTypeDef],
-        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsPaginatorTypeDef],
+        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsExtraOutputTypeDef],
+        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsExtraOutputTypeDef],
         "MotionGraphicsImageActivateSettings": NotRequired[
             MotionGraphicsActivateScheduleActionSettingsTypeDef
         ],
         "MotionGraphicsImageDeactivateSettings": NotRequired[Dict[str, Any]],
-        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsPaginatorTypeDef],
+        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsExtraOutputTypeDef],
         "Scte35InputSettings": NotRequired[Scte35InputScheduleActionSettingsTypeDef],
         "Scte35ReturnToNetworkSettings": NotRequired[
             Scte35ReturnToNetworkScheduleActionSettingsTypeDef
         ],
         "Scte35SpliceInsertSettings": NotRequired[Scte35SpliceInsertScheduleActionSettingsTypeDef],
         "Scte35TimeSignalSettings": NotRequired[
-            Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef
+            Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef
         ],
         "StaticImageActivateSettings": NotRequired[
             StaticImageActivateScheduleActionSettingsTypeDef
         ],
         "StaticImageDeactivateSettings": NotRequired[
             StaticImageDeactivateScheduleActionSettingsTypeDef
         ],
         "StaticImageOutputActivateSettings": NotRequired[
-            StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef
+            StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef
         ],
         "StaticImageOutputDeactivateSettings": NotRequired[
-            StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef
+            StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef
+        ],
+    },
+)
+ScheduleActionSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsOutputTypeDef",
+    {
+        "HlsId3SegmentTaggingSettings": NotRequired[
+            HlsId3SegmentTaggingScheduleActionSettingsTypeDef
+        ],
+        "HlsTimedMetadataSettings": NotRequired[HlsTimedMetadataScheduleActionSettingsTypeDef],
+        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsOutputTypeDef],
+        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsOutputTypeDef],
+        "MotionGraphicsImageActivateSettings": NotRequired[
+            MotionGraphicsActivateScheduleActionSettingsTypeDef
+        ],
+        "MotionGraphicsImageDeactivateSettings": NotRequired[Dict[str, Any]],
+        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsOutputTypeDef],
+        "Scte35InputSettings": NotRequired[Scte35InputScheduleActionSettingsTypeDef],
+        "Scte35ReturnToNetworkSettings": NotRequired[
+            Scte35ReturnToNetworkScheduleActionSettingsTypeDef
+        ],
+        "Scte35SpliceInsertSettings": NotRequired[Scte35SpliceInsertScheduleActionSettingsTypeDef],
+        "Scte35TimeSignalSettings": NotRequired[
+            Scte35TimeSignalScheduleActionSettingsOutputTypeDef
+        ],
+        "StaticImageActivateSettings": NotRequired[
+            StaticImageActivateScheduleActionSettingsTypeDef
+        ],
+        "StaticImageDeactivateSettings": NotRequired[
+            StaticImageDeactivateScheduleActionSettingsTypeDef
+        ],
+        "StaticImageOutputActivateSettings": NotRequired[
+            StaticImageOutputActivateScheduleActionSettingsOutputTypeDef
+        ],
+        "StaticImageOutputDeactivateSettings": NotRequired[
+            StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef
         ],
     },
 )
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": NotRequired[
@@ -4978,94 +5523,101 @@
             StaticImageOutputActivateScheduleActionSettingsTypeDef
         ],
         "StaticImageOutputDeactivateSettings": NotRequired[
             StaticImageOutputDeactivateScheduleActionSettingsTypeDef
         ],
     },
 )
-ChannelSummaryPaginatorTypeDef = TypedDict(
-    "ChannelSummaryPaginatorTypeDef",
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
         "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationPaginatorTypeDef]],
+        "Destinations": NotRequired[List[OutputDestinationOutputTypeDef]],
         "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
         "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentPaginatorTypeDef]],
+        "InputAttachments": NotRequired[List[InputAttachmentOutputTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
         "Maintenance": NotRequired[MaintenanceStatusTypeDef],
         "Name": NotRequired[str],
         "PipelinesRunningCount": NotRequired[int],
         "RoleArn": NotRequired[str],
         "State": NotRequired[ChannelStateType],
         "Tags": NotRequired[Dict[str, str]],
         "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentExtraOutputTypeDef]
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
     {
-        "Arn": NotRequired[str],
-        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationTypeDef]],
-        "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
-        "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentTypeDef]],
-        "InputSpecification": NotRequired[InputSpecificationTypeDef],
-        "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceStatusTypeDef],
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
         "Name": NotRequired[str],
-        "PipelinesRunningCount": NotRequired[int],
-        "RoleArn": NotRequired[str],
-        "State": NotRequired[ChannelStateType],
-        "Tags": NotRequired[Dict[str, str]],
-        "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
         "Name": NotRequired[str],
     },
 )
-ScheduleActionPaginatorTypeDef = TypedDict(
-    "ScheduleActionPaginatorTypeDef",
+ScheduleActionExtraOutputTypeDef = TypedDict(
+    "ScheduleActionExtraOutputTypeDef",
+    {
+        "ActionName": str,
+        "ScheduleActionSettings": ScheduleActionSettingsExtraOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsExtraOutputTypeDef,
+    },
+)
+ScheduleActionOutputTypeDef = TypedDict(
+    "ScheduleActionOutputTypeDef",
     {
         "ActionName": str,
-        "ScheduleActionSettings": ScheduleActionSettingsPaginatorTypeDef,
-        "ScheduleActionStartSettings": ScheduleActionStartSettingsPaginatorTypeDef,
+        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
     },
 )
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
 )
-ListChannelsResponsePaginatorTypeDef = TypedDict(
-    "ListChannelsResponsePaginatorTypeDef",
-    {
-        "Channels": List[ChannelSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+EncoderSettingsOutputTypeDef = TypedDict(
+    "EncoderSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
+        "AvailBlanking": NotRequired[AvailBlankingTypeDef],
+        "AvailConfiguration": NotRequired[AvailConfigurationTypeDef],
+        "BlackoutSlate": NotRequired[BlackoutSlateTypeDef],
+        "CaptionDescriptions": NotRequired[List[CaptionDescriptionOutputTypeDef]],
+        "FeatureActivations": NotRequired[FeatureActivationsTypeDef],
+        "GlobalConfiguration": NotRequired[GlobalConfigurationOutputTypeDef],
+        "MotionGraphicsConfiguration": NotRequired[MotionGraphicsConfigurationOutputTypeDef],
+        "NielsenConfiguration": NotRequired[NielsenConfigurationTypeDef],
+        "ThumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
+        "ColorCorrectionSettings": NotRequired[ColorCorrectionSettingsOutputTypeDef],
     },
 )
 EncoderSettingsTypeDef = TypedDict(
     "EncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
@@ -5079,101 +5631,74 @@
         "GlobalConfiguration": NotRequired[GlobalConfigurationTypeDef],
         "MotionGraphicsConfiguration": NotRequired[MotionGraphicsConfigurationTypeDef],
         "NielsenConfiguration": NotRequired[NielsenConfigurationTypeDef],
         "ThumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
         "ColorCorrectionSettings": NotRequired[ColorCorrectionSettingsTypeDef],
     },
 )
-DescribeScheduleResponsePaginatorTypeDef = TypedDict(
-    "DescribeScheduleResponsePaginatorTypeDef",
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
     {
-        "NextToken": str,
-        "ScheduleActions": List[ScheduleActionPaginatorTypeDef],
+        "ScheduleActions": List[ScheduleActionExtraOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
     {
-        "NextToken": str,
-        "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": NotRequired[str],
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
         "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationTypeDef]],
+        "Destinations": NotRequired[List[OutputDestinationOutputTypeDef]],
         "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
-        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
+        "EncoderSettings": NotRequired[EncoderSettingsOutputTypeDef],
         "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentTypeDef]],
+        "InputAttachments": NotRequired[List[InputAttachmentOutputTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
         "Maintenance": NotRequired[MaintenanceStatusTypeDef],
         "Name": NotRequired[str],
         "PipelineDetails": NotRequired[List[PipelineDetailTypeDef]],
         "PipelinesRunningCount": NotRequired[int],
         "RoleArn": NotRequired[str],
         "State": NotRequired[ChannelStateType],
         "Tags": NotRequired[Dict[str, str]],
         "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
-        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
-        "InputAttachments": NotRequired[Sequence[InputAttachmentTypeDef]],
-        "InputSpecification": NotRequired[InputSpecificationTypeDef],
-        "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceCreateSettingsTypeDef],
-        "Name": NotRequired[str],
-        "RequestId": NotRequired[str],
-        "Reserved": NotRequired[str],
-        "RoleArn": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
-        "Vpc": NotRequired[VpcOutputSettingsTypeDef],
-    },
-)
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5185,19 +5710,19 @@
 )
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5209,19 +5734,19 @@
 )
 RestartChannelPipelinesResponseTypeDef = TypedDict(
     "RestartChannelPipelinesResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "MaintenanceStatus": str,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
@@ -5234,19 +5759,19 @@
 )
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5258,63 +5783,83 @@
 )
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChannelRequestRequestTypeDef = TypedDict(
-    "UpdateChannelRequestRequestTypeDef",
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
     {
-        "ChannelId": str,
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
+        "ChannelClass": NotRequired[ChannelClassType],
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
         "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
-        "InputAttachments": NotRequired[Sequence[InputAttachmentTypeDef]],
+        "InputAttachments": NotRequired[Sequence[InputAttachmentUnionTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceUpdateSettingsTypeDef],
+        "Maintenance": NotRequired[MaintenanceCreateSettingsTypeDef],
         "Name": NotRequired[str],
+        "RequestId": NotRequired[str],
+        "Reserved": NotRequired[str],
         "RoleArn": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+        "Vpc": NotRequired[VpcOutputSettingsTypeDef],
     },
 )
-BatchUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "BatchUpdateScheduleRequestRequestTypeDef",
+EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
+UpdateChannelRequestRequestTypeDef = TypedDict(
+    "UpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
-        "Creates": NotRequired[BatchScheduleActionCreateRequestTypeDef],
-        "Deletes": NotRequired[BatchScheduleActionDeleteRequestTypeDef],
+        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
+        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
+        "InputAttachments": NotRequired[Sequence[InputAttachmentUnionTypeDef]],
+        "InputSpecification": NotRequired[InputSpecificationTypeDef],
+        "LogLevel": NotRequired[LogLevelType],
+        "Maintenance": NotRequired[MaintenanceUpdateSettingsTypeDef],
+        "Name": NotRequired[str],
+        "RoleArn": NotRequired[str],
     },
 )
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "BatchUpdateScheduleRequestRequestTypeDef",
+    {
+        "ChannelId": str,
+        "Creates": NotRequired[BatchScheduleActionCreateRequestTypeDef],
+        "Deletes": NotRequired[BatchScheduleActionDeleteRequestTypeDef],
+    },
+)
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/type_defs.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AacSettingsTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AacCodingModeType,
     AacInputTypeType,
     AacProfileType,
@@ -272,14 +272,15 @@
     Scte35AposNoRegionalBlackoutBehaviorType,
     Scte35AposWebDeliveryAllowedBehaviorType,
     Scte35ArchiveAllowedFlagType,
     Scte35DeviceRestrictionsType,
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
+    Scte35SegmentationScopeType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
     Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
     SignalMapMonitorDeploymentStatusType,
     SignalMapStatusType,
     SmoothGroupAudioOnlyTimecodeControlType,
@@ -446,14 +447,15 @@
     "FrameCaptureOutputSettingsTypeDef",
     "TimecodeBurninSettingsTypeDef",
     "GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef",
     "GetCloudWatchAlarmTemplateRequestRequestTypeDef",
     "GetEventBridgeRuleTemplateGroupRequestRequestTypeDef",
     "GetEventBridgeRuleTemplateRequestRequestTypeDef",
     "GetSignalMapRequestRequestTypeDef",
+    "H264ColorSpaceSettingsOutputTypeDef",
     "H264ColorSpaceSettingsTypeDef",
     "TemporalFilterSettingsTypeDef",
     "Hdr10SettingsTypeDef",
     "HlsAkamaiSettingsTypeDef",
     "HlsBasicPutSettingsTypeDef",
     "HlsMediaStoreSettingsTypeDef",
     "HlsS3SettingsTypeDef",
@@ -488,35 +490,38 @@
     "SignalMapSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "M3u8SettingsTypeDef",
     "MaintenanceUpdateSettingsTypeDef",
     "MediaPackageOutputDestinationSettingsTypeDef",
     "MediaResourceNeighborTypeDef",
     "MotionGraphicsActivateScheduleActionSettingsTypeDef",
+    "MotionGraphicsSettingsOutputTypeDef",
     "MotionGraphicsSettingsTypeDef",
     "MsSmoothOutputSettingsTypeDef",
     "MultiplexMediaConnectOutputDestinationSettingsTypeDef",
     "MultiplexProgramChannelDestinationSettingsTypeDef",
     "MultiplexProgramServiceDescriptorTypeDef",
     "MultiplexSettingsSummaryTypeDef",
     "MultiplexStatmuxVideoSettingsTypeDef",
     "NielsenCBETTypeDef",
     "NielsenNaesIiNwTypeDef",
     "OutputDestinationSettingsTypeDef",
-    "RtmpGroupSettingsTypeDef",
+    "RtmpGroupSettingsOutputTypeDef",
     "UdpGroupSettingsTypeDef",
+    "RtmpGroupSettingsTypeDef",
     "PipelinePauseStateSettingsTypeDef",
     "RebootInputDeviceRequestRequestTypeDef",
     "RejectInputDeviceTransferRequestRequestTypeDef",
     "RestartChannelPipelinesRequestRequestTypeDef",
     "Scte35InputScheduleActionSettingsTypeDef",
     "Scte35ReturnToNetworkScheduleActionSettingsTypeDef",
     "Scte35SpliceInsertScheduleActionSettingsTypeDef",
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
-    "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
+    "StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef",
+    "StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef",
     "StaticImageOutputDeactivateScheduleActionSettingsTypeDef",
     "Scte35DeliveryRestrictionsTypeDef",
     "StartChannelRequestRequestTypeDef",
     "StartDeleteMonitorDeploymentRequestRequestTypeDef",
     "StartInputDeviceMaintenanceWindowRequestRequestTypeDef",
     "StartInputDeviceRequestRequestTypeDef",
     "StartMonitorDeploymentRequestRequestTypeDef",
@@ -535,27 +540,31 @@
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
     "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
+    "AudioChannelMappingOutputTypeDef",
     "AudioChannelMappingTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
     "AvailBlankingTypeDef",
     "BlackoutSlateTypeDef",
     "BurnInDestinationSettingsTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "InputLossBehaviorTypeDef",
     "StaticImageActivateScheduleActionSettingsTypeDef",
-    "StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef",
+    "StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef",
+    "StaticImageOutputActivateScheduleActionSettingsOutputTypeDef",
     "StaticImageOutputActivateScheduleActionSettingsTypeDef",
     "StaticKeySettingsTypeDef",
-    "AudioTrackSelectionPaginatorTypeDef",
+    "AudioTrackSelectionExtraOutputTypeDef",
+    "AudioTrackSelectionOutputTypeDef",
     "AudioTrackSelectionTypeDef",
     "AvailSettingsTypeDef",
     "BatchDeleteResponseTypeDef",
     "BatchStartResponseTypeDef",
     "BatchStopResponseTypeDef",
     "CreateCloudWatchAlarmTemplateGroupResponseTypeDef",
     "CreateCloudWatchAlarmTemplateResponseTypeDef",
@@ -570,14 +579,15 @@
     "UpdateAccountConfigurationResponseTypeDef",
     "UpdateCloudWatchAlarmTemplateGroupResponseTypeDef",
     "UpdateCloudWatchAlarmTemplateResponseTypeDef",
     "UpdateEventBridgeRuleTemplateGroupResponseTypeDef",
     "TeletextSourceSettingsTypeDef",
     "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
     "ListCloudWatchAlarmTemplatesResponseTypeDef",
+    "ColorCorrectionSettingsOutputTypeDef",
     "ColorCorrectionSettingsTypeDef",
     "CreateEventBridgeRuleTemplateRequestRequestTypeDef",
     "CreateEventBridgeRuleTemplateResponseTypeDef",
     "GetEventBridgeRuleTemplateResponseTypeDef",
     "UpdateEventBridgeRuleTemplateRequestRequestTypeDef",
     "UpdateEventBridgeRuleTemplateResponseTypeDef",
     "CreateInputRequestRequestTypeDef",
@@ -621,78 +631,93 @@
     "ListInputsRequestListInputsPaginateTypeDef",
     "ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef",
     "ListMultiplexesRequestListMultiplexesPaginateTypeDef",
     "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListSignalMapsRequestListSignalMapsPaginateTypeDef",
     "M2tsSettingsTypeDef",
+    "OutputLockingSettingsOutputTypeDef",
     "OutputLockingSettingsTypeDef",
     "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
     "ListEventBridgeRuleTemplatesResponseTypeDef",
     "FailoverConditionSettingsTypeDef",
-    "ScheduleActionStartSettingsPaginatorTypeDef",
+    "ScheduleActionStartSettingsExtraOutputTypeDef",
+    "ScheduleActionStartSettingsOutputTypeDef",
     "ScheduleActionStartSettingsTypeDef",
     "FrameCaptureCdnSettingsTypeDef",
     "FrameCaptureSettingsTypeDef",
     "H264FilterSettingsTypeDef",
     "H265FilterSettingsTypeDef",
     "Mpeg2FilterSettingsTypeDef",
+    "H265ColorSpaceSettingsOutputTypeDef",
     "H265ColorSpaceSettingsTypeDef",
     "VideoSelectorColorSpaceSettingsTypeDef",
     "HlsCdnSettingsTypeDef",
     "NetworkInputSettingsTypeDef",
     "InputClippingSettingsTypeDef",
     "InputDestinationTypeDef",
     "InputDeviceConfigurableSettingsTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "InputDeviceUhdSettingsTypeDef",
     "ListInputDeviceTransfersResponseTypeDef",
     "ListMultiplexProgramsResponseTypeDef",
     "ListSignalMapsResponseTypeDef",
     "StandardHlsSettingsTypeDef",
     "MediaResourceTypeDef",
+    "MotionGraphicsConfigurationOutputTypeDef",
     "MotionGraphicsConfigurationTypeDef",
     "MultiplexOutputDestinationTypeDef",
     "MultiplexSummaryTypeDef",
     "MultiplexVideoSettingsTypeDef",
     "NielsenWatermarksSettingsTypeDef",
-    "OutputDestinationPaginatorTypeDef",
+    "OutputDestinationExtraOutputTypeDef",
+    "OutputDestinationOutputTypeDef",
     "OutputDestinationTypeDef",
-    "PauseStateScheduleActionSettingsPaginatorTypeDef",
+    "PauseStateScheduleActionSettingsExtraOutputTypeDef",
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     "PauseStateScheduleActionSettingsTypeDef",
     "Scte35SegmentationDescriptorTypeDef",
     "ThumbnailDetailTypeDef",
     "VideoSelectorSettingsTypeDef",
     "ArchiveGroupSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "KeyProviderSettingsTypeDef",
-    "AudioSelectorSettingsPaginatorTypeDef",
+    "AudioSelectorSettingsExtraOutputTypeDef",
+    "AudioSelectorSettingsOutputTypeDef",
     "AudioSelectorSettingsTypeDef",
     "AvailConfigurationTypeDef",
-    "CaptionSelectorSettingsPaginatorTypeDef",
+    "CaptionSelectorSettingsExtraOutputTypeDef",
+    "CaptionSelectorSettingsOutputTypeDef",
     "CaptionSelectorSettingsTypeDef",
     "ListOfferingsResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "UpdateReservationResponseTypeDef",
     "CreateInputSecurityGroupResponseTypeDef",
     "ListInputSecurityGroupsResponseTypeDef",
     "UpdateInputSecurityGroupResponseTypeDef",
     "ArchiveContainerSettingsTypeDef",
     "UdpContainerSettingsTypeDef",
+    "GlobalConfigurationOutputTypeDef",
     "GlobalConfigurationTypeDef",
     "FailoverConditionTypeDef",
     "FrameCaptureGroupSettingsTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
     "Mpeg2SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "InputPrepareScheduleActionSettingsPaginatorTypeDef",
+    "InputPrepareScheduleActionSettingsExtraOutputTypeDef",
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
     "InputPrepareScheduleActionSettingsTypeDef",
-    "InputSwitchScheduleActionSettingsPaginatorTypeDef",
+    "InputSwitchScheduleActionSettingsExtraOutputTypeDef",
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     "InputSwitchScheduleActionSettingsTypeDef",
     "DescribeInputResponseTypeDef",
     "InputTypeDef",
     "UpdateInputDeviceRequestRequestTypeDef",
     "DescribeInputDeviceResponseTypeDef",
     "InputDeviceSummaryTypeDef",
     "UpdateInputDeviceResponseTypeDef",
@@ -706,81 +731,97 @@
     "DescribeMultiplexResponseTypeDef",
     "MultiplexTypeDef",
     "StartMultiplexResponseTypeDef",
     "StopMultiplexResponseTypeDef",
     "ListMultiplexesResponseTypeDef",
     "MultiplexProgramSettingsTypeDef",
     "AudioWatermarkSettingsTypeDef",
-    "UpdateChannelClassRequestRequestTypeDef",
+    "OutputDestinationUnionTypeDef",
     "Scte35DescriptorSettingsTypeDef",
     "DescribeThumbnailsResponseTypeDef",
     "VideoSelectorTypeDef",
+    "CaptionDescriptionOutputTypeDef",
     "CaptionDescriptionTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "AudioSelectorPaginatorTypeDef",
+    "AudioSelectorExtraOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioSelectorTypeDef",
-    "CaptionSelectorPaginatorTypeDef",
+    "CaptionSelectorExtraOutputTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
     "ArchiveOutputSettingsTypeDef",
     "UdpOutputSettingsTypeDef",
-    "AutomaticInputFailoverSettingsPaginatorTypeDef",
+    "AutomaticInputFailoverSettingsExtraOutputTypeDef",
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     "AutomaticInputFailoverSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
     "CreateInputResponseTypeDef",
     "CreatePartnerInputResponseTypeDef",
     "ListInputsResponseTypeDef",
     "UpdateInputResponseTypeDef",
     "ListInputDevicesResponseTypeDef",
     "HlsOutputSettingsTypeDef",
     "CreateMultiplexResponseTypeDef",
     "UpdateMultiplexResponseTypeDef",
     "CreateMultiplexProgramRequestRequestTypeDef",
     "DeleteMultiplexProgramResponseTypeDef",
     "DescribeMultiplexProgramResponseTypeDef",
     "MultiplexProgramTypeDef",
     "UpdateMultiplexProgramRequestRequestTypeDef",
+    "AudioDescriptionOutputTypeDef",
     "AudioDescriptionTypeDef",
+    "UpdateChannelClassRequestRequestTypeDef",
     "Scte35DescriptorTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "InputSettingsPaginatorTypeDef",
+    "InputSettingsExtraOutputTypeDef",
+    "InputSettingsOutputTypeDef",
     "InputSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
     "OutputSettingsTypeDef",
     "CreateMultiplexProgramResponseTypeDef",
     "UpdateMultiplexProgramResponseTypeDef",
-    "Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef",
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
-    "InputAttachmentPaginatorTypeDef",
+    "InputAttachmentExtraOutputTypeDef",
+    "InputAttachmentOutputTypeDef",
     "InputAttachmentTypeDef",
     "OutputTypeDef",
-    "ScheduleActionSettingsPaginatorTypeDef",
+    "ScheduleActionSettingsExtraOutputTypeDef",
+    "ScheduleActionSettingsOutputTypeDef",
     "ScheduleActionSettingsTypeDef",
-    "ChannelSummaryPaginatorTypeDef",
     "ChannelSummaryTypeDef",
+    "InputAttachmentUnionTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "ScheduleActionPaginatorTypeDef",
+    "ScheduleActionExtraOutputTypeDef",
+    "ScheduleActionOutputTypeDef",
     "ScheduleActionTypeDef",
-    "ListChannelsResponsePaginatorTypeDef",
     "ListChannelsResponseTypeDef",
+    "EncoderSettingsOutputTypeDef",
     "EncoderSettingsTypeDef",
-    "DescribeScheduleResponsePaginatorTypeDef",
-    "BatchScheduleActionCreateRequestTypeDef",
+    "DescribeScheduleResponseTypeDef",
     "BatchScheduleActionCreateResultTypeDef",
     "BatchScheduleActionDeleteResultTypeDef",
-    "DescribeScheduleResponseTypeDef",
+    "BatchScheduleActionCreateRequestTypeDef",
     "ChannelTypeDef",
-    "CreateChannelRequestRequestTypeDef",
     "DeleteChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "RestartChannelPipelinesResponseTypeDef",
     "StartChannelResponseTypeDef",
     "StopChannelResponseTypeDef",
+    "CreateChannelRequestRequestTypeDef",
+    "EncoderSettingsUnionTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "BatchUpdateScheduleRequestRequestTypeDef",
     "BatchUpdateScheduleResponseTypeDef",
+    "BatchUpdateScheduleRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelClassResponseTypeDef",
     "UpdateChannelResponseTypeDef",
 )
 
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
@@ -1791,14 +1832,22 @@
 )
 GetSignalMapRequestRequestTypeDef = TypedDict(
     "GetSignalMapRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
+H264ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H264ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": NotRequired[Dict[str, Any]],
+        "Rec601Settings": NotRequired[Dict[str, Any]],
+        "Rec709Settings": NotRequired[Dict[str, Any]],
+    },
+)
 H264ColorSpaceSettingsTypeDef = TypedDict(
     "H264ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
         "Rec709Settings": NotRequired[Mapping[str, Any]],
     },
@@ -2159,14 +2208,20 @@
     {
         "Duration": NotRequired[int],
         "PasswordParam": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
+MotionGraphicsSettingsOutputTypeDef = TypedDict(
+    "MotionGraphicsSettingsOutputTypeDef",
+    {
+        "HtmlMotionGraphicsSettings": NotRequired[Dict[str, Any]],
+    },
+)
 MotionGraphicsSettingsTypeDef = TypedDict(
     "MotionGraphicsSettingsTypeDef",
     {
         "HtmlMotionGraphicsSettings": NotRequired[Mapping[str, Any]],
     },
 )
 MsSmoothOutputSettingsTypeDef = TypedDict(
@@ -2231,18 +2286,18 @@
     {
         "PasswordParam": NotRequired[str],
         "StreamName": NotRequired[str],
         "Url": NotRequired[str],
         "Username": NotRequired[str],
     },
 )
-RtmpGroupSettingsTypeDef = TypedDict(
-    "RtmpGroupSettingsTypeDef",
+RtmpGroupSettingsOutputTypeDef = TypedDict(
+    "RtmpGroupSettingsOutputTypeDef",
     {
-        "AdMarkers": NotRequired[Sequence[Literal["ON_CUE_POINT_SCTE35"]]],
+        "AdMarkers": NotRequired[List[Literal["ON_CUE_POINT_SCTE35"]]],
         "AuthenticationScheme": NotRequired[AuthenticationSchemeType],
         "CacheFullBehavior": NotRequired[RtmpCacheFullBehaviorType],
         "CacheLength": NotRequired[int],
         "CaptionData": NotRequired[RtmpCaptionDataType],
         "InputLossAction": NotRequired[InputLossActionForRtmpOutType],
         "RestartDelay": NotRequired[int],
         "IncludeFillerNalUnits": NotRequired[IncludeFillerNalUnitsType],
@@ -2252,14 +2307,27 @@
     "UdpGroupSettingsTypeDef",
     {
         "InputLossAction": NotRequired[InputLossActionForUdpOutType],
         "TimedMetadataId3Frame": NotRequired[UdpTimedMetadataId3FrameType],
         "TimedMetadataId3Period": NotRequired[int],
     },
 )
+RtmpGroupSettingsTypeDef = TypedDict(
+    "RtmpGroupSettingsTypeDef",
+    {
+        "AdMarkers": NotRequired[Sequence[Literal["ON_CUE_POINT_SCTE35"]]],
+        "AuthenticationScheme": NotRequired[AuthenticationSchemeType],
+        "CacheFullBehavior": NotRequired[RtmpCacheFullBehaviorType],
+        "CacheLength": NotRequired[int],
+        "CaptionData": NotRequired[RtmpCaptionDataType],
+        "InputLossAction": NotRequired[InputLossActionForRtmpOutType],
+        "RestartDelay": NotRequired[int],
+        "IncludeFillerNalUnits": NotRequired[IncludeFillerNalUnitsType],
+    },
+)
 PipelinePauseStateSettingsTypeDef = TypedDict(
     "PipelinePauseStateSettingsTypeDef",
     {
         "PipelineId": PipelineIdType,
     },
 )
 RebootInputDeviceRequestRequestTypeDef = TypedDict(
@@ -2305,16 +2373,24 @@
 StaticImageDeactivateScheduleActionSettingsTypeDef = TypedDict(
     "StaticImageDeactivateScheduleActionSettingsTypeDef",
     {
         "FadeOut": NotRequired[int],
         "Layer": NotRequired[int],
     },
 )
-StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef",
+StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "OutputNames": List[str],
+        "FadeOut": NotRequired[int],
+        "Layer": NotRequired[int],
+    },
+)
+StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef",
     {
         "OutputNames": List[str],
         "FadeOut": NotRequired[int],
         "Layer": NotRequired[int],
     },
 )
 StaticImageOutputDeactivateScheduleActionSettingsTypeDef = TypedDict(
@@ -2527,21 +2603,40 @@
     {
         "Destination": OutputLocationRefTypeDef,
         "CertificateMode": NotRequired[RtmpOutputCertificateModeType],
         "ConnectionRetryInterval": NotRequired[int],
         "NumRetries": NotRequired[int],
     },
 )
+AudioChannelMappingOutputTypeDef = TypedDict(
+    "AudioChannelMappingOutputTypeDef",
+    {
+        "InputChannelLevels": List[InputChannelLevelTypeDef],
+        "OutputChannel": int,
+    },
+)
 AudioChannelMappingTypeDef = TypedDict(
     "AudioChannelMappingTypeDef",
     {
         "InputChannelLevels": Sequence[InputChannelLevelTypeDef],
         "OutputChannel": int,
     },
 )
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": NotRequired[AacSettingsTypeDef],
+        "Ac3Settings": NotRequired[Ac3SettingsTypeDef],
+        "Eac3AtmosSettings": NotRequired[Eac3AtmosSettingsTypeDef],
+        "Eac3Settings": NotRequired[Eac3SettingsTypeDef],
+        "Mp2Settings": NotRequired[Mp2SettingsTypeDef],
+        "PassThroughSettings": NotRequired[Dict[str, Any]],
+        "WavSettings": NotRequired[WavSettingsTypeDef],
+    },
+)
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": NotRequired[AacSettingsTypeDef],
         "Ac3Settings": NotRequired[Ac3SettingsTypeDef],
         "Eac3AtmosSettings": NotRequired[Eac3AtmosSettingsTypeDef],
         "Eac3Settings": NotRequired[Eac3SettingsTypeDef],
@@ -2641,16 +2736,32 @@
         "ImageX": NotRequired[int],
         "ImageY": NotRequired[int],
         "Layer": NotRequired[int],
         "Opacity": NotRequired[int],
         "Width": NotRequired[int],
     },
 )
-StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef",
+StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Image": InputLocationTypeDef,
+        "OutputNames": List[str],
+        "Duration": NotRequired[int],
+        "FadeIn": NotRequired[int],
+        "FadeOut": NotRequired[int],
+        "Height": NotRequired[int],
+        "ImageX": NotRequired[int],
+        "ImageY": NotRequired[int],
+        "Layer": NotRequired[int],
+        "Opacity": NotRequired[int],
+        "Width": NotRequired[int],
+    },
+)
+StaticImageOutputActivateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "StaticImageOutputActivateScheduleActionSettingsOutputTypeDef",
     {
         "Image": InputLocationTypeDef,
         "OutputNames": List[str],
         "Duration": NotRequired[int],
         "FadeIn": NotRequired[int],
         "FadeOut": NotRequired[int],
         "Height": NotRequired[int],
@@ -2680,16 +2791,23 @@
 StaticKeySettingsTypeDef = TypedDict(
     "StaticKeySettingsTypeDef",
     {
         "StaticKeyValue": str,
         "KeyProviderServer": NotRequired[InputLocationTypeDef],
     },
 )
-AudioTrackSelectionPaginatorTypeDef = TypedDict(
-    "AudioTrackSelectionPaginatorTypeDef",
+AudioTrackSelectionExtraOutputTypeDef = TypedDict(
+    "AudioTrackSelectionExtraOutputTypeDef",
+    {
+        "Tracks": List[AudioTrackTypeDef],
+        "DolbyEDecode": NotRequired[AudioDolbyEDecodeTypeDef],
+    },
+)
+AudioTrackSelectionOutputTypeDef = TypedDict(
+    "AudioTrackSelectionOutputTypeDef",
     {
         "Tracks": List[AudioTrackTypeDef],
         "DolbyEDecode": NotRequired[AudioDolbyEDecodeTypeDef],
     },
 )
 AudioTrackSelectionTypeDef = TypedDict(
     "AudioTrackSelectionTypeDef",
@@ -2922,24 +3040,30 @@
         "PageNumber": NotRequired[str],
     },
 )
 ListCloudWatchAlarmTemplateGroupsResponseTypeDef = TypedDict(
     "ListCloudWatchAlarmTemplateGroupsResponseTypeDef",
     {
         "CloudWatchAlarmTemplateGroups": List[CloudWatchAlarmTemplateGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListCloudWatchAlarmTemplatesResponseTypeDef = TypedDict(
     "ListCloudWatchAlarmTemplatesResponseTypeDef",
     {
         "CloudWatchAlarmTemplates": List[CloudWatchAlarmTemplateSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+ColorCorrectionSettingsOutputTypeDef = TypedDict(
+    "ColorCorrectionSettingsOutputTypeDef",
+    {
+        "GlobalColorCorrections": List[ColorCorrectionTypeDef],
     },
 )
 ColorCorrectionSettingsTypeDef = TypedDict(
     "ColorCorrectionSettingsTypeDef",
     {
         "GlobalColorCorrections": Sequence[ColorCorrectionTypeDef],
     },
@@ -3492,47 +3616,66 @@
         "TimedMetadataBehavior": NotRequired[M2tsTimedMetadataBehaviorType],
         "TimedMetadataPid": NotRequired[str],
         "TransportStreamId": NotRequired[int],
         "VideoPid": NotRequired[str],
         "Scte35PrerollPullupMilliseconds": NotRequired[float],
     },
 )
+OutputLockingSettingsOutputTypeDef = TypedDict(
+    "OutputLockingSettingsOutputTypeDef",
+    {
+        "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
+        "PipelineLockingSettings": NotRequired[Dict[str, Any]],
+    },
+)
 OutputLockingSettingsTypeDef = TypedDict(
     "OutputLockingSettingsTypeDef",
     {
         "EpochLockingSettings": NotRequired[EpochLockingSettingsTypeDef],
         "PipelineLockingSettings": NotRequired[Mapping[str, Any]],
     },
 )
 ListEventBridgeRuleTemplateGroupsResponseTypeDef = TypedDict(
     "ListEventBridgeRuleTemplateGroupsResponseTypeDef",
     {
         "EventBridgeRuleTemplateGroups": List[EventBridgeRuleTemplateGroupSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListEventBridgeRuleTemplatesResponseTypeDef = TypedDict(
     "ListEventBridgeRuleTemplatesResponseTypeDef",
     {
         "EventBridgeRuleTemplates": List[EventBridgeRuleTemplateSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FailoverConditionSettingsTypeDef = TypedDict(
     "FailoverConditionSettingsTypeDef",
     {
         "AudioSilenceSettings": NotRequired[AudioSilenceFailoverSettingsTypeDef],
         "InputLossSettings": NotRequired[InputLossFailoverSettingsTypeDef],
         "VideoBlackSettings": NotRequired[VideoBlackFailoverSettingsTypeDef],
     },
 )
-ScheduleActionStartSettingsPaginatorTypeDef = TypedDict(
-    "ScheduleActionStartSettingsPaginatorTypeDef",
+ScheduleActionStartSettingsExtraOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsExtraOutputTypeDef",
+    {
+        "FixedModeScheduleActionStartSettings": NotRequired[
+            FixedModeScheduleActionStartSettingsTypeDef
+        ],
+        "FollowModeScheduleActionStartSettings": NotRequired[
+            FollowModeScheduleActionStartSettingsTypeDef
+        ],
+        "ImmediateModeScheduleActionStartSettings": NotRequired[Dict[str, Any]],
+    },
+)
+ScheduleActionStartSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionStartSettingsOutputTypeDef",
     {
         "FixedModeScheduleActionStartSettings": NotRequired[
             FixedModeScheduleActionStartSettingsTypeDef
         ],
         "FollowModeScheduleActionStartSettings": NotRequired[
             FollowModeScheduleActionStartSettingsTypeDef
         ],
@@ -3579,14 +3722,24 @@
 )
 Mpeg2FilterSettingsTypeDef = TypedDict(
     "Mpeg2FilterSettingsTypeDef",
     {
         "TemporalFilterSettings": NotRequired[TemporalFilterSettingsTypeDef],
     },
 )
+H265ColorSpaceSettingsOutputTypeDef = TypedDict(
+    "H265ColorSpaceSettingsOutputTypeDef",
+    {
+        "ColorSpacePassthroughSettings": NotRequired[Dict[str, Any]],
+        "DolbyVision81Settings": NotRequired[Dict[str, Any]],
+        "Hdr10Settings": NotRequired[Hdr10SettingsTypeDef],
+        "Rec601Settings": NotRequired[Dict[str, Any]],
+        "Rec709Settings": NotRequired[Dict[str, Any]],
+    },
+)
 H265ColorSpaceSettingsTypeDef = TypedDict(
     "H265ColorSpaceSettingsTypeDef",
     {
         "ColorSpacePassthroughSettings": NotRequired[Mapping[str, Any]],
         "DolbyVision81Settings": NotRequired[Mapping[str, Any]],
         "Hdr10Settings": NotRequired[Hdr10SettingsTypeDef],
         "Rec601Settings": NotRequired[Mapping[str, Any]],
@@ -3676,32 +3829,32 @@
         "AudioChannelPairs": NotRequired[List[InputDeviceUhdAudioChannelPairConfigTypeDef]],
     },
 )
 ListInputDeviceTransfersResponseTypeDef = TypedDict(
     "ListInputDeviceTransfersResponseTypeDef",
     {
         "InputDeviceTransfers": List[TransferringInputDeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMultiplexProgramsResponseTypeDef = TypedDict(
     "ListMultiplexProgramsResponseTypeDef",
     {
         "MultiplexPrograms": List[MultiplexProgramSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListSignalMapsResponseTypeDef = TypedDict(
     "ListSignalMapsResponseTypeDef",
     {
-        "NextToken": str,
         "SignalMaps": List[SignalMapSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StandardHlsSettingsTypeDef = TypedDict(
     "StandardHlsSettingsTypeDef",
     {
         "M3u8Settings": M3u8SettingsTypeDef,
         "AudioRenditionSets": NotRequired[str],
@@ -3711,14 +3864,21 @@
     "MediaResourceTypeDef",
     {
         "Destinations": NotRequired[List[MediaResourceNeighborTypeDef]],
         "Name": NotRequired[str],
         "Sources": NotRequired[List[MediaResourceNeighborTypeDef]],
     },
 )
+MotionGraphicsConfigurationOutputTypeDef = TypedDict(
+    "MotionGraphicsConfigurationOutputTypeDef",
+    {
+        "MotionGraphicsSettings": MotionGraphicsSettingsOutputTypeDef,
+        "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
+    },
+)
 MotionGraphicsConfigurationTypeDef = TypedDict(
     "MotionGraphicsConfigurationTypeDef",
     {
         "MotionGraphicsSettings": MotionGraphicsSettingsTypeDef,
         "MotionGraphicsInsertion": NotRequired[MotionGraphicsInsertionType],
     },
 )
@@ -3753,16 +3913,25 @@
     "NielsenWatermarksSettingsTypeDef",
     {
         "NielsenCbetSettings": NotRequired[NielsenCBETTypeDef],
         "NielsenDistributionType": NotRequired[NielsenWatermarksDistributionTypesType],
         "NielsenNaesIiNwSettings": NotRequired[NielsenNaesIiNwTypeDef],
     },
 )
-OutputDestinationPaginatorTypeDef = TypedDict(
-    "OutputDestinationPaginatorTypeDef",
+OutputDestinationExtraOutputTypeDef = TypedDict(
+    "OutputDestinationExtraOutputTypeDef",
+    {
+        "Id": NotRequired[str],
+        "MediaPackageSettings": NotRequired[List[MediaPackageOutputDestinationSettingsTypeDef]],
+        "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
+        "Settings": NotRequired[List[OutputDestinationSettingsTypeDef]],
+    },
+)
+OutputDestinationOutputTypeDef = TypedDict(
+    "OutputDestinationOutputTypeDef",
     {
         "Id": NotRequired[str],
         "MediaPackageSettings": NotRequired[List[MediaPackageOutputDestinationSettingsTypeDef]],
         "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
         "Settings": NotRequired[List[OutputDestinationSettingsTypeDef]],
     },
 )
@@ -3771,16 +3940,22 @@
     {
         "Id": NotRequired[str],
         "MediaPackageSettings": NotRequired[Sequence[MediaPackageOutputDestinationSettingsTypeDef]],
         "MultiplexSettings": NotRequired[MultiplexProgramChannelDestinationSettingsTypeDef],
         "Settings": NotRequired[Sequence[OutputDestinationSettingsTypeDef]],
     },
 )
-PauseStateScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "PauseStateScheduleActionSettingsPaginatorTypeDef",
+PauseStateScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Pipelines": NotRequired[List[PipelinePauseStateSettingsTypeDef]],
+    },
+)
+PauseStateScheduleActionSettingsOutputTypeDef = TypedDict(
+    "PauseStateScheduleActionSettingsOutputTypeDef",
     {
         "Pipelines": NotRequired[List[PipelinePauseStateSettingsTypeDef]],
     },
 )
 PauseStateScheduleActionSettingsTypeDef = TypedDict(
     "PauseStateScheduleActionSettingsTypeDef",
     {
@@ -3821,22 +3996,48 @@
     "ArchiveGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "ArchiveCdnSettings": NotRequired[ArchiveCdnSettingsTypeDef],
         "RolloverInterval": NotRequired[int],
     },
 )
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMappings": List[AudioChannelMappingOutputTypeDef],
+        "ChannelsIn": NotRequired[int],
+        "ChannelsOut": NotRequired[int],
+    },
+)
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMappings": Sequence[AudioChannelMappingTypeDef],
         "ChannelsIn": NotRequired[int],
         "ChannelsOut": NotRequired[int],
     },
 )
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "AribDestinationSettings": NotRequired[Dict[str, Any]],
+        "BurnInDestinationSettings": NotRequired[BurnInDestinationSettingsTypeDef],
+        "DvbSubDestinationSettings": NotRequired[DvbSubDestinationSettingsTypeDef],
+        "EbuTtDDestinationSettings": NotRequired[EbuTtDDestinationSettingsTypeDef],
+        "EmbeddedDestinationSettings": NotRequired[Dict[str, Any]],
+        "EmbeddedPlusScte20DestinationSettings": NotRequired[Dict[str, Any]],
+        "RtmpCaptionInfoDestinationSettings": NotRequired[Dict[str, Any]],
+        "Scte20PlusEmbeddedDestinationSettings": NotRequired[Dict[str, Any]],
+        "Scte27DestinationSettings": NotRequired[Dict[str, Any]],
+        "SmpteTtDestinationSettings": NotRequired[Dict[str, Any]],
+        "TeletextDestinationSettings": NotRequired[Dict[str, Any]],
+        "TtmlDestinationSettings": NotRequired[TtmlDestinationSettingsTypeDef],
+        "WebvttDestinationSettings": NotRequired[WebvttDestinationSettingsTypeDef],
+    },
+)
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "AribDestinationSettings": NotRequired[Mapping[str, Any]],
         "BurnInDestinationSettings": NotRequired[BurnInDestinationSettingsTypeDef],
         "DvbSubDestinationSettings": NotRequired[DvbSubDestinationSettingsTypeDef],
         "EbuTtDDestinationSettings": NotRequired[EbuTtDDestinationSettingsTypeDef],
@@ -3853,21 +4054,30 @@
 )
 KeyProviderSettingsTypeDef = TypedDict(
     "KeyProviderSettingsTypeDef",
     {
         "StaticKeySettings": NotRequired[StaticKeySettingsTypeDef],
     },
 )
-AudioSelectorSettingsPaginatorTypeDef = TypedDict(
-    "AudioSelectorSettingsPaginatorTypeDef",
+AudioSelectorSettingsExtraOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsExtraOutputTypeDef",
+    {
+        "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
+        "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
+        "AudioPidSelection": NotRequired[AudioPidSelectionTypeDef],
+        "AudioTrackSelection": NotRequired[AudioTrackSelectionExtraOutputTypeDef],
+    },
+)
+AudioSelectorSettingsOutputTypeDef = TypedDict(
+    "AudioSelectorSettingsOutputTypeDef",
     {
         "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
         "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
         "AudioPidSelection": NotRequired[AudioPidSelectionTypeDef],
-        "AudioTrackSelection": NotRequired[AudioTrackSelectionPaginatorTypeDef],
+        "AudioTrackSelection": NotRequired[AudioTrackSelectionOutputTypeDef],
     },
 )
 AudioSelectorSettingsTypeDef = TypedDict(
     "AudioSelectorSettingsTypeDef",
     {
         "AudioHlsRenditionSelection": NotRequired[AudioHlsRenditionSelectionTypeDef],
         "AudioLanguageSelection": NotRequired[AudioLanguageSelectionTypeDef],
@@ -3875,18 +4085,31 @@
         "AudioTrackSelection": NotRequired[AudioTrackSelectionTypeDef],
     },
 )
 AvailConfigurationTypeDef = TypedDict(
     "AvailConfigurationTypeDef",
     {
         "AvailSettings": NotRequired[AvailSettingsTypeDef],
+        "Scte35SegmentationScope": NotRequired[Scte35SegmentationScopeType],
     },
 )
-CaptionSelectorSettingsPaginatorTypeDef = TypedDict(
-    "CaptionSelectorSettingsPaginatorTypeDef",
+CaptionSelectorSettingsExtraOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsExtraOutputTypeDef",
+    {
+        "AncillarySourceSettings": NotRequired[AncillarySourceSettingsTypeDef],
+        "AribSourceSettings": NotRequired[Dict[str, Any]],
+        "DvbSubSourceSettings": NotRequired[DvbSubSourceSettingsTypeDef],
+        "EmbeddedSourceSettings": NotRequired[EmbeddedSourceSettingsTypeDef],
+        "Scte20SourceSettings": NotRequired[Scte20SourceSettingsTypeDef],
+        "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
+        "TeletextSourceSettings": NotRequired[TeletextSourceSettingsTypeDef],
+    },
+)
+CaptionSelectorSettingsOutputTypeDef = TypedDict(
+    "CaptionSelectorSettingsOutputTypeDef",
     {
         "AncillarySourceSettings": NotRequired[AncillarySourceSettingsTypeDef],
         "AribSourceSettings": NotRequired[Dict[str, Any]],
         "DvbSubSourceSettings": NotRequired[DvbSubSourceSettingsTypeDef],
         "EmbeddedSourceSettings": NotRequired[EmbeddedSourceSettingsTypeDef],
         "Scte20SourceSettings": NotRequired[Scte20SourceSettingsTypeDef],
         "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
@@ -3904,25 +4127,25 @@
         "Scte27SourceSettings": NotRequired[Scte27SourceSettingsTypeDef],
         "TeletextSourceSettings": NotRequired[TeletextSourceSettingsTypeDef],
     },
 )
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
-        "NextToken": str,
         "Offerings": List[OfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
-        "NextToken": str,
         "Reservations": List[ReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3942,16 +4165,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputSecurityGroupsResponseTypeDef = TypedDict(
     "ListInputSecurityGroupsResponseTypeDef",
     {
         "InputSecurityGroups": List[InputSecurityGroupTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInputSecurityGroupResponseTypeDef = TypedDict(
     "UpdateInputSecurityGroupResponseTypeDef",
     {
         "SecurityGroup": InputSecurityGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3966,14 +4189,26 @@
 )
 UdpContainerSettingsTypeDef = TypedDict(
     "UdpContainerSettingsTypeDef",
     {
         "M2tsSettings": NotRequired[M2tsSettingsTypeDef],
     },
 )
+GlobalConfigurationOutputTypeDef = TypedDict(
+    "GlobalConfigurationOutputTypeDef",
+    {
+        "InitialAudioGain": NotRequired[int],
+        "InputEndAction": NotRequired[GlobalConfigurationInputEndActionType],
+        "InputLossBehavior": NotRequired[InputLossBehaviorTypeDef],
+        "OutputLockingMode": NotRequired[GlobalConfigurationOutputLockingModeType],
+        "OutputTimingSource": NotRequired[GlobalConfigurationOutputTimingSourceType],
+        "SupportLowFramerateInputs": NotRequired[GlobalConfigurationLowFramerateInputsType],
+        "OutputLockingSettings": NotRequired[OutputLockingSettingsOutputTypeDef],
+    },
+)
 GlobalConfigurationTypeDef = TypedDict(
     "GlobalConfigurationTypeDef",
     {
         "InitialAudioGain": NotRequired[int],
         "InputEndAction": NotRequired[GlobalConfigurationInputEndActionType],
         "InputLossBehavior": NotRequired[InputLossBehaviorTypeDef],
         "OutputLockingMode": NotRequired[GlobalConfigurationOutputLockingModeType],
@@ -3991,14 +4226,61 @@
 FrameCaptureGroupSettingsTypeDef = TypedDict(
     "FrameCaptureGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "FrameCaptureCdnSettings": NotRequired[FrameCaptureCdnSettingsTypeDef],
     },
 )
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": NotRequired[H264AdaptiveQuantizationType],
+        "AfdSignaling": NotRequired[AfdSignalingType],
+        "Bitrate": NotRequired[int],
+        "BufFillPct": NotRequired[int],
+        "BufSize": NotRequired[int],
+        "ColorMetadata": NotRequired[H264ColorMetadataType],
+        "ColorSpaceSettings": NotRequired[H264ColorSpaceSettingsOutputTypeDef],
+        "EntropyEncoding": NotRequired[H264EntropyEncodingType],
+        "FilterSettings": NotRequired[H264FilterSettingsTypeDef],
+        "FixedAfd": NotRequired[FixedAfdType],
+        "FlickerAq": NotRequired[H264FlickerAqType],
+        "ForceFieldPictures": NotRequired[H264ForceFieldPicturesType],
+        "FramerateControl": NotRequired[H264FramerateControlType],
+        "FramerateDenominator": NotRequired[int],
+        "FramerateNumerator": NotRequired[int],
+        "GopBReference": NotRequired[H264GopBReferenceType],
+        "GopClosedCadence": NotRequired[int],
+        "GopNumBFrames": NotRequired[int],
+        "GopSize": NotRequired[float],
+        "GopSizeUnits": NotRequired[H264GopSizeUnitsType],
+        "Level": NotRequired[H264LevelType],
+        "LookAheadRateControl": NotRequired[H264LookAheadRateControlType],
+        "MaxBitrate": NotRequired[int],
+        "MinIInterval": NotRequired[int],
+        "NumRefFrames": NotRequired[int],
+        "ParControl": NotRequired[H264ParControlType],
+        "ParDenominator": NotRequired[int],
+        "ParNumerator": NotRequired[int],
+        "Profile": NotRequired[H264ProfileType],
+        "QualityLevel": NotRequired[H264QualityLevelType],
+        "QvbrQualityLevel": NotRequired[int],
+        "RateControlMode": NotRequired[H264RateControlModeType],
+        "ScanType": NotRequired[H264ScanTypeType],
+        "SceneChangeDetect": NotRequired[H264SceneChangeDetectType],
+        "Slices": NotRequired[int],
+        "Softness": NotRequired[int],
+        "SpatialAq": NotRequired[H264SpatialAqType],
+        "SubgopLength": NotRequired[H264SubGopLengthType],
+        "Syntax": NotRequired[H264SyntaxType],
+        "TemporalAq": NotRequired[H264TemporalAqType],
+        "TimecodeInsertion": NotRequired[H264TimecodeInsertionBehaviorType],
+        "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
+    },
+)
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": NotRequired[H264AdaptiveQuantizationType],
         "AfdSignaling": NotRequired[AfdSignalingType],
         "Bitrate": NotRequired[int],
         "BufFillPct": NotRequired[int],
@@ -4060,14 +4342,55 @@
         "GopSizeUnits": NotRequired[Mpeg2GopSizeUnitsType],
         "ScanType": NotRequired[Mpeg2ScanTypeType],
         "SubgopLength": NotRequired[Mpeg2SubGopLengthType],
         "TimecodeInsertion": NotRequired[Mpeg2TimecodeInsertionBehaviorType],
         "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
     },
 )
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "AdaptiveQuantization": NotRequired[H265AdaptiveQuantizationType],
+        "AfdSignaling": NotRequired[AfdSignalingType],
+        "AlternativeTransferFunction": NotRequired[H265AlternativeTransferFunctionType],
+        "Bitrate": NotRequired[int],
+        "BufSize": NotRequired[int],
+        "ColorMetadata": NotRequired[H265ColorMetadataType],
+        "ColorSpaceSettings": NotRequired[H265ColorSpaceSettingsOutputTypeDef],
+        "FilterSettings": NotRequired[H265FilterSettingsTypeDef],
+        "FixedAfd": NotRequired[FixedAfdType],
+        "FlickerAq": NotRequired[H265FlickerAqType],
+        "GopClosedCadence": NotRequired[int],
+        "GopSize": NotRequired[float],
+        "GopSizeUnits": NotRequired[H265GopSizeUnitsType],
+        "Level": NotRequired[H265LevelType],
+        "LookAheadRateControl": NotRequired[H265LookAheadRateControlType],
+        "MaxBitrate": NotRequired[int],
+        "MinIInterval": NotRequired[int],
+        "ParDenominator": NotRequired[int],
+        "ParNumerator": NotRequired[int],
+        "Profile": NotRequired[H265ProfileType],
+        "QvbrQualityLevel": NotRequired[int],
+        "RateControlMode": NotRequired[H265RateControlModeType],
+        "ScanType": NotRequired[H265ScanTypeType],
+        "SceneChangeDetect": NotRequired[H265SceneChangeDetectType],
+        "Slices": NotRequired[int],
+        "Tier": NotRequired[H265TierType],
+        "TimecodeInsertion": NotRequired[H265TimecodeInsertionBehaviorType],
+        "TimecodeBurninSettings": NotRequired[TimecodeBurninSettingsTypeDef],
+        "MvOverPictureBoundaries": NotRequired[H265MvOverPictureBoundariesType],
+        "MvTemporalPredictor": NotRequired[H265MvTemporalPredictorType],
+        "TileHeight": NotRequired[int],
+        "TilePadding": NotRequired[H265TilePaddingType],
+        "TileWidth": NotRequired[int],
+        "TreeblockSize": NotRequired[H265TreeblockSizeType],
+    },
+)
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "AdaptiveQuantization": NotRequired[H265AdaptiveQuantizationType],
         "AfdSignaling": NotRequired[AfdSignalingType],
@@ -4101,32 +4424,48 @@
         "MvTemporalPredictor": NotRequired[H265MvTemporalPredictorType],
         "TileHeight": NotRequired[int],
         "TilePadding": NotRequired[H265TilePaddingType],
         "TileWidth": NotRequired[int],
         "TreeblockSize": NotRequired[H265TreeblockSizeType],
     },
 )
-InputPrepareScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "InputPrepareScheduleActionSettingsPaginatorTypeDef",
+InputPrepareScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "InputAttachmentNameReference": NotRequired[str],
+        "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
+        "UrlPath": NotRequired[List[str]],
+    },
+)
+InputPrepareScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputPrepareScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": NotRequired[str],
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[List[str]],
     },
 )
 InputPrepareScheduleActionSettingsTypeDef = TypedDict(
     "InputPrepareScheduleActionSettingsTypeDef",
     {
         "InputAttachmentNameReference": NotRequired[str],
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[Sequence[str]],
     },
 )
-InputSwitchScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "InputSwitchScheduleActionSettingsPaginatorTypeDef",
+InputSwitchScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "InputSwitchScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "InputAttachmentNameReference": str,
+        "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
+        "UrlPath": NotRequired[List[str]],
+    },
+)
+InputSwitchScheduleActionSettingsOutputTypeDef = TypedDict(
+    "InputSwitchScheduleActionSettingsOutputTypeDef",
     {
         "InputAttachmentNameReference": str,
         "InputClippingSettings": NotRequired[InputClippingSettingsTypeDef],
         "UrlPath": NotRequired[List[str]],
     },
 )
 InputSwitchScheduleActionSettingsTypeDef = TypedDict(
@@ -4463,16 +4802,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMultiplexesResponseTypeDef = TypedDict(
     "ListMultiplexesResponseTypeDef",
     {
         "Multiplexes": List[MultiplexSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 MultiplexProgramSettingsTypeDef = TypedDict(
     "MultiplexProgramSettingsTypeDef",
     {
         "ProgramNumber": int,
         "PreferredChannelPipeline": NotRequired[PreferredChannelPipelineType],
@@ -4482,22 +4821,15 @@
 )
 AudioWatermarkSettingsTypeDef = TypedDict(
     "AudioWatermarkSettingsTypeDef",
     {
         "NielsenWatermarksSettings": NotRequired[NielsenWatermarksSettingsTypeDef],
     },
 )
-UpdateChannelClassRequestRequestTypeDef = TypedDict(
-    "UpdateChannelClassRequestRequestTypeDef",
-    {
-        "ChannelClass": ChannelClassType,
-        "ChannelId": str,
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
-    },
-)
+OutputDestinationUnionTypeDef = Union[OutputDestinationTypeDef, OutputDestinationExtraOutputTypeDef]
 Scte35DescriptorSettingsTypeDef = TypedDict(
     "Scte35DescriptorSettingsTypeDef",
     {
         "SegmentationDescriptorScte35DescriptorSettings": Scte35SegmentationDescriptorTypeDef,
     },
 )
 DescribeThumbnailsResponseTypeDef = TypedDict(
@@ -4512,27 +4844,88 @@
     {
         "ColorSpace": NotRequired[VideoSelectorColorSpaceType],
         "ColorSpaceSettings": NotRequired[VideoSelectorColorSpaceSettingsTypeDef],
         "ColorSpaceUsage": NotRequired[VideoSelectorColorSpaceUsageType],
         "SelectorSettings": NotRequired[VideoSelectorSettingsTypeDef],
     },
 )
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
+    {
+        "CaptionSelectorName": str,
+        "Name": str,
+        "Accessibility": NotRequired[AccessibilityTypeType],
+        "DestinationSettings": NotRequired[CaptionDestinationSettingsOutputTypeDef],
+        "LanguageCode": NotRequired[str],
+        "LanguageDescription": NotRequired[str],
+        "CaptionDashRoles": NotRequired[List[DashRoleCaptionType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
+    },
+)
 CaptionDescriptionTypeDef = TypedDict(
     "CaptionDescriptionTypeDef",
     {
         "CaptionSelectorName": str,
         "Name": str,
         "Accessibility": NotRequired[AccessibilityTypeType],
         "DestinationSettings": NotRequired[CaptionDestinationSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageDescription": NotRequired[str],
         "CaptionDashRoles": NotRequired[Sequence[DashRoleCaptionType]],
         "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "Destination": OutputLocationRefTypeDef,
+        "AdMarkers": NotRequired[List[HlsAdMarkersType]],
+        "BaseUrlContent": NotRequired[str],
+        "BaseUrlContent1": NotRequired[str],
+        "BaseUrlManifest": NotRequired[str],
+        "BaseUrlManifest1": NotRequired[str],
+        "CaptionLanguageMappings": NotRequired[List[CaptionLanguageMappingTypeDef]],
+        "CaptionLanguageSetting": NotRequired[HlsCaptionLanguageSettingType],
+        "ClientCache": NotRequired[HlsClientCacheType],
+        "CodecSpecification": NotRequired[HlsCodecSpecificationType],
+        "ConstantIv": NotRequired[str],
+        "DirectoryStructure": NotRequired[HlsDirectoryStructureType],
+        "DiscontinuityTags": NotRequired[HlsDiscontinuityTagsType],
+        "EncryptionType": NotRequired[HlsEncryptionTypeType],
+        "HlsCdnSettings": NotRequired[HlsCdnSettingsTypeDef],
+        "HlsId3SegmentTagging": NotRequired[HlsId3SegmentTaggingStateType],
+        "IFrameOnlyPlaylists": NotRequired[IFrameOnlyPlaylistTypeType],
+        "IncompleteSegmentBehavior": NotRequired[HlsIncompleteSegmentBehaviorType],
+        "IndexNSegments": NotRequired[int],
+        "InputLossAction": NotRequired[InputLossActionForHlsOutType],
+        "IvInManifest": NotRequired[HlsIvInManifestType],
+        "IvSource": NotRequired[HlsIvSourceType],
+        "KeepSegments": NotRequired[int],
+        "KeyFormat": NotRequired[str],
+        "KeyFormatVersions": NotRequired[str],
+        "KeyProviderSettings": NotRequired[KeyProviderSettingsTypeDef],
+        "ManifestCompression": NotRequired[HlsManifestCompressionType],
+        "ManifestDurationFormat": NotRequired[HlsManifestDurationFormatType],
+        "MinSegmentLength": NotRequired[int],
+        "Mode": NotRequired[HlsModeType],
+        "OutputSelection": NotRequired[HlsOutputSelectionType],
+        "ProgramDateTime": NotRequired[HlsProgramDateTimeType],
+        "ProgramDateTimeClock": NotRequired[HlsProgramDateTimeClockType],
+        "ProgramDateTimePeriod": NotRequired[int],
+        "RedundantManifest": NotRequired[HlsRedundantManifestType],
+        "SegmentLength": NotRequired[int],
+        "SegmentationMode": NotRequired[HlsSegmentationModeType],
+        "SegmentsPerSubdirectory": NotRequired[int],
+        "StreamInfResolution": NotRequired[HlsStreamInfResolutionType],
+        "TimedMetadataId3Frame": NotRequired[HlsTimedMetadataId3FrameType],
+        "TimedMetadataId3Period": NotRequired[int],
+        "TimestampDeltaMilliseconds": NotRequired[int],
+        "TsFileMode": NotRequired[HlsTsFileModeType],
+    },
+)
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "AdMarkers": NotRequired[Sequence[HlsAdMarkersType]],
         "BaseUrlContent": NotRequired[str],
         "BaseUrlContent1": NotRequired[str],
@@ -4573,34 +4966,49 @@
         "StreamInfResolution": NotRequired[HlsStreamInfResolutionType],
         "TimedMetadataId3Frame": NotRequired[HlsTimedMetadataId3FrameType],
         "TimedMetadataId3Period": NotRequired[int],
         "TimestampDeltaMilliseconds": NotRequired[int],
         "TsFileMode": NotRequired[HlsTsFileModeType],
     },
 )
-AudioSelectorPaginatorTypeDef = TypedDict(
-    "AudioSelectorPaginatorTypeDef",
+AudioSelectorExtraOutputTypeDef = TypedDict(
+    "AudioSelectorExtraOutputTypeDef",
     {
         "Name": str,
-        "SelectorSettings": NotRequired[AudioSelectorSettingsPaginatorTypeDef],
+        "SelectorSettings": NotRequired[AudioSelectorSettingsExtraOutputTypeDef],
+    },
+)
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "Name": str,
+        "SelectorSettings": NotRequired[AudioSelectorSettingsOutputTypeDef],
     },
 )
 AudioSelectorTypeDef = TypedDict(
     "AudioSelectorTypeDef",
     {
         "Name": str,
         "SelectorSettings": NotRequired[AudioSelectorSettingsTypeDef],
     },
 )
-CaptionSelectorPaginatorTypeDef = TypedDict(
-    "CaptionSelectorPaginatorTypeDef",
+CaptionSelectorExtraOutputTypeDef = TypedDict(
+    "CaptionSelectorExtraOutputTypeDef",
+    {
+        "Name": str,
+        "LanguageCode": NotRequired[str],
+        "SelectorSettings": NotRequired[CaptionSelectorSettingsExtraOutputTypeDef],
+    },
+)
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
     {
         "Name": str,
         "LanguageCode": NotRequired[str],
-        "SelectorSettings": NotRequired[CaptionSelectorSettingsPaginatorTypeDef],
+        "SelectorSettings": NotRequired[CaptionSelectorSettingsOutputTypeDef],
     },
 )
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "Name": str,
         "LanguageCode": NotRequired[str],
@@ -4620,16 +5028,25 @@
     {
         "ContainerSettings": UdpContainerSettingsTypeDef,
         "Destination": OutputLocationRefTypeDef,
         "BufferMsec": NotRequired[int],
         "FecOutputSettings": NotRequired[FecOutputSettingsTypeDef],
     },
 )
-AutomaticInputFailoverSettingsPaginatorTypeDef = TypedDict(
-    "AutomaticInputFailoverSettingsPaginatorTypeDef",
+AutomaticInputFailoverSettingsExtraOutputTypeDef = TypedDict(
+    "AutomaticInputFailoverSettingsExtraOutputTypeDef",
+    {
+        "SecondaryInputId": str,
+        "ErrorClearTimeMsec": NotRequired[int],
+        "FailoverConditions": NotRequired[List[FailoverConditionTypeDef]],
+        "InputPreference": NotRequired[InputPreferenceType],
+    },
+)
+AutomaticInputFailoverSettingsOutputTypeDef = TypedDict(
+    "AutomaticInputFailoverSettingsOutputTypeDef",
     {
         "SecondaryInputId": str,
         "ErrorClearTimeMsec": NotRequired[int],
         "FailoverConditions": NotRequired[List[FailoverConditionTypeDef]],
         "InputPreference": NotRequired[InputPreferenceType],
     },
 )
@@ -4638,14 +5055,23 @@
     {
         "SecondaryInputId": str,
         "ErrorClearTimeMsec": NotRequired[int],
         "FailoverConditions": NotRequired[Sequence[FailoverConditionTypeDef]],
         "InputPreference": NotRequired[InputPreferenceType],
     },
 )
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "FrameCaptureSettings": NotRequired[FrameCaptureSettingsTypeDef],
+        "H264Settings": NotRequired[H264SettingsOutputTypeDef],
+        "H265Settings": NotRequired[H265SettingsOutputTypeDef],
+        "Mpeg2Settings": NotRequired[Mpeg2SettingsTypeDef],
+    },
+)
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "FrameCaptureSettings": NotRequired[FrameCaptureSettingsTypeDef],
         "H264Settings": NotRequired[H264SettingsTypeDef],
         "H265Settings": NotRequired[H265SettingsTypeDef],
         "Mpeg2Settings": NotRequired[Mpeg2SettingsTypeDef],
@@ -4665,31 +5091,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "Inputs": List[InputTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "Input": InputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListInputDevicesResponseTypeDef = TypedDict(
     "ListInputDevicesResponseTypeDef",
     {
         "InputDevices": List[InputDeviceSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 HlsOutputSettingsTypeDef = TypedDict(
     "HlsOutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
         "H265PackagingType": NotRequired[HlsH265PackagingTypeType],
@@ -4756,14 +5182,32 @@
     "UpdateMultiplexProgramRequestRequestTypeDef",
     {
         "MultiplexId": str,
         "ProgramName": str,
         "MultiplexProgramSettings": NotRequired[MultiplexProgramSettingsTypeDef],
     },
 )
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioSelectorName": str,
+        "Name": str,
+        "AudioNormalizationSettings": NotRequired[AudioNormalizationSettingsTypeDef],
+        "AudioType": NotRequired[AudioTypeType],
+        "AudioTypeControl": NotRequired[AudioDescriptionAudioTypeControlType],
+        "AudioWatermarkingSettings": NotRequired[AudioWatermarkSettingsTypeDef],
+        "CodecSettings": NotRequired[AudioCodecSettingsOutputTypeDef],
+        "LanguageCode": NotRequired[str],
+        "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
+        "RemixSettings": NotRequired[RemixSettingsOutputTypeDef],
+        "StreamName": NotRequired[str],
+        "AudioDashRoles": NotRequired[List[DashRoleAudioType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
+    },
+)
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioSelectorName": str,
         "Name": str,
         "AudioNormalizationSettings": NotRequired[AudioNormalizationSettingsTypeDef],
         "AudioType": NotRequired[AudioTypeType],
@@ -4774,39 +5218,77 @@
         "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
         "RemixSettings": NotRequired[RemixSettingsTypeDef],
         "StreamName": NotRequired[str],
         "AudioDashRoles": NotRequired[Sequence[DashRoleAudioType]],
         "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
+UpdateChannelClassRequestRequestTypeDef = TypedDict(
+    "UpdateChannelClassRequestRequestTypeDef",
+    {
+        "ChannelClass": ChannelClassType,
+        "ChannelId": str,
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
+    },
+)
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
 )
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "ArchiveGroupSettings": NotRequired[ArchiveGroupSettingsTypeDef],
+        "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
+        "HlsGroupSettings": NotRequired[HlsGroupSettingsOutputTypeDef],
+        "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
+        "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
+        "MultiplexGroupSettings": NotRequired[Dict[str, Any]],
+        "RtmpGroupSettings": NotRequired[RtmpGroupSettingsOutputTypeDef],
+        "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
+        "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
+    },
+)
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "ArchiveGroupSettings": NotRequired[ArchiveGroupSettingsTypeDef],
         "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
         "HlsGroupSettings": NotRequired[HlsGroupSettingsTypeDef],
         "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
         "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
         "MultiplexGroupSettings": NotRequired[Mapping[str, Any]],
         "RtmpGroupSettings": NotRequired[RtmpGroupSettingsTypeDef],
         "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
         "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
     },
 )
-InputSettingsPaginatorTypeDef = TypedDict(
-    "InputSettingsPaginatorTypeDef",
+InputSettingsExtraOutputTypeDef = TypedDict(
+    "InputSettingsExtraOutputTypeDef",
+    {
+        "AudioSelectors": NotRequired[List[AudioSelectorExtraOutputTypeDef]],
+        "CaptionSelectors": NotRequired[List[CaptionSelectorExtraOutputTypeDef]],
+        "DeblockFilter": NotRequired[InputDeblockFilterType],
+        "DenoiseFilter": NotRequired[InputDenoiseFilterType],
+        "FilterStrength": NotRequired[int],
+        "InputFilter": NotRequired[InputFilterType],
+        "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
+        "Scte35Pid": NotRequired[int],
+        "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
+        "SourceEndBehavior": NotRequired[InputSourceEndBehaviorType],
+        "VideoSelector": NotRequired[VideoSelectorTypeDef],
+    },
+)
+InputSettingsOutputTypeDef = TypedDict(
+    "InputSettingsOutputTypeDef",
     {
-        "AudioSelectors": NotRequired[List[AudioSelectorPaginatorTypeDef]],
-        "CaptionSelectors": NotRequired[List[CaptionSelectorPaginatorTypeDef]],
+        "AudioSelectors": NotRequired[List[AudioSelectorOutputTypeDef]],
+        "CaptionSelectors": NotRequired[List[CaptionSelectorOutputTypeDef]],
         "DeblockFilter": NotRequired[InputDeblockFilterType],
         "DenoiseFilter": NotRequired[InputDenoiseFilterType],
         "FilterStrength": NotRequired[int],
         "InputFilter": NotRequired[InputFilterType],
         "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
         "Scte35Pid": NotRequired[int],
         "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
@@ -4826,14 +5308,26 @@
         "NetworkInputSettings": NotRequired[NetworkInputSettingsTypeDef],
         "Scte35Pid": NotRequired[int],
         "Smpte2038DataPreference": NotRequired[Smpte2038DataPreferenceType],
         "SourceEndBehavior": NotRequired[InputSourceEndBehaviorType],
         "VideoSelector": NotRequired[VideoSelectorTypeDef],
     },
 )
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "Name": str,
+        "CodecSettings": NotRequired[VideoCodecSettingsOutputTypeDef],
+        "Height": NotRequired[int],
+        "RespondToAfd": NotRequired[VideoDescriptionRespondToAfdType],
+        "ScalingBehavior": NotRequired[VideoDescriptionScalingBehaviorType],
+        "Sharpness": NotRequired[int],
+        "Width": NotRequired[int],
+    },
+)
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "Name": str,
         "CodecSettings": NotRequired[VideoCodecSettingsTypeDef],
         "Height": NotRequired[int],
         "RespondToAfd": NotRequired[VideoDescriptionRespondToAfdType],
@@ -4866,35 +5360,50 @@
 UpdateMultiplexProgramResponseTypeDef = TypedDict(
     "UpdateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef",
+Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef",
+    {
+        "Scte35Descriptors": List[Scte35DescriptorTypeDef],
+    },
+)
+Scte35TimeSignalScheduleActionSettingsOutputTypeDef = TypedDict(
+    "Scte35TimeSignalScheduleActionSettingsOutputTypeDef",
     {
         "Scte35Descriptors": List[Scte35DescriptorTypeDef],
     },
 )
 Scte35TimeSignalScheduleActionSettingsTypeDef = TypedDict(
     "Scte35TimeSignalScheduleActionSettingsTypeDef",
     {
         "Scte35Descriptors": Sequence[Scte35DescriptorTypeDef],
     },
 )
-InputAttachmentPaginatorTypeDef = TypedDict(
-    "InputAttachmentPaginatorTypeDef",
+InputAttachmentExtraOutputTypeDef = TypedDict(
+    "InputAttachmentExtraOutputTypeDef",
     {
         "AutomaticInputFailoverSettings": NotRequired[
-            AutomaticInputFailoverSettingsPaginatorTypeDef
+            AutomaticInputFailoverSettingsExtraOutputTypeDef
         ],
         "InputAttachmentName": NotRequired[str],
         "InputId": NotRequired[str],
-        "InputSettings": NotRequired[InputSettingsPaginatorTypeDef],
+        "InputSettings": NotRequired[InputSettingsExtraOutputTypeDef],
+    },
+)
+InputAttachmentOutputTypeDef = TypedDict(
+    "InputAttachmentOutputTypeDef",
+    {
+        "AutomaticInputFailoverSettings": NotRequired[AutomaticInputFailoverSettingsOutputTypeDef],
+        "InputAttachmentName": NotRequired[str],
+        "InputId": NotRequired[str],
+        "InputSettings": NotRequired[InputSettingsOutputTypeDef],
     },
 )
 InputAttachmentTypeDef = TypedDict(
     "InputAttachmentTypeDef",
     {
         "AutomaticInputFailoverSettings": NotRequired[AutomaticInputFailoverSettingsTypeDef],
         "InputAttachmentName": NotRequired[str],
@@ -4908,47 +5417,83 @@
         "OutputSettings": OutputSettingsTypeDef,
         "AudioDescriptionNames": NotRequired[Sequence[str]],
         "CaptionDescriptionNames": NotRequired[Sequence[str]],
         "OutputName": NotRequired[str],
         "VideoDescriptionName": NotRequired[str],
     },
 )
-ScheduleActionSettingsPaginatorTypeDef = TypedDict(
-    "ScheduleActionSettingsPaginatorTypeDef",
+ScheduleActionSettingsExtraOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsExtraOutputTypeDef",
     {
         "HlsId3SegmentTaggingSettings": NotRequired[
             HlsId3SegmentTaggingScheduleActionSettingsTypeDef
         ],
         "HlsTimedMetadataSettings": NotRequired[HlsTimedMetadataScheduleActionSettingsTypeDef],
-        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsPaginatorTypeDef],
-        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsPaginatorTypeDef],
+        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsExtraOutputTypeDef],
+        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsExtraOutputTypeDef],
         "MotionGraphicsImageActivateSettings": NotRequired[
             MotionGraphicsActivateScheduleActionSettingsTypeDef
         ],
         "MotionGraphicsImageDeactivateSettings": NotRequired[Dict[str, Any]],
-        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsPaginatorTypeDef],
+        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsExtraOutputTypeDef],
         "Scte35InputSettings": NotRequired[Scte35InputScheduleActionSettingsTypeDef],
         "Scte35ReturnToNetworkSettings": NotRequired[
             Scte35ReturnToNetworkScheduleActionSettingsTypeDef
         ],
         "Scte35SpliceInsertSettings": NotRequired[Scte35SpliceInsertScheduleActionSettingsTypeDef],
         "Scte35TimeSignalSettings": NotRequired[
-            Scte35TimeSignalScheduleActionSettingsPaginatorTypeDef
+            Scte35TimeSignalScheduleActionSettingsExtraOutputTypeDef
         ],
         "StaticImageActivateSettings": NotRequired[
             StaticImageActivateScheduleActionSettingsTypeDef
         ],
         "StaticImageDeactivateSettings": NotRequired[
             StaticImageDeactivateScheduleActionSettingsTypeDef
         ],
         "StaticImageOutputActivateSettings": NotRequired[
-            StaticImageOutputActivateScheduleActionSettingsPaginatorTypeDef
+            StaticImageOutputActivateScheduleActionSettingsExtraOutputTypeDef
         ],
         "StaticImageOutputDeactivateSettings": NotRequired[
-            StaticImageOutputDeactivateScheduleActionSettingsPaginatorTypeDef
+            StaticImageOutputDeactivateScheduleActionSettingsExtraOutputTypeDef
+        ],
+    },
+)
+ScheduleActionSettingsOutputTypeDef = TypedDict(
+    "ScheduleActionSettingsOutputTypeDef",
+    {
+        "HlsId3SegmentTaggingSettings": NotRequired[
+            HlsId3SegmentTaggingScheduleActionSettingsTypeDef
+        ],
+        "HlsTimedMetadataSettings": NotRequired[HlsTimedMetadataScheduleActionSettingsTypeDef],
+        "InputPrepareSettings": NotRequired[InputPrepareScheduleActionSettingsOutputTypeDef],
+        "InputSwitchSettings": NotRequired[InputSwitchScheduleActionSettingsOutputTypeDef],
+        "MotionGraphicsImageActivateSettings": NotRequired[
+            MotionGraphicsActivateScheduleActionSettingsTypeDef
+        ],
+        "MotionGraphicsImageDeactivateSettings": NotRequired[Dict[str, Any]],
+        "PauseStateSettings": NotRequired[PauseStateScheduleActionSettingsOutputTypeDef],
+        "Scte35InputSettings": NotRequired[Scte35InputScheduleActionSettingsTypeDef],
+        "Scte35ReturnToNetworkSettings": NotRequired[
+            Scte35ReturnToNetworkScheduleActionSettingsTypeDef
+        ],
+        "Scte35SpliceInsertSettings": NotRequired[Scte35SpliceInsertScheduleActionSettingsTypeDef],
+        "Scte35TimeSignalSettings": NotRequired[
+            Scte35TimeSignalScheduleActionSettingsOutputTypeDef
+        ],
+        "StaticImageActivateSettings": NotRequired[
+            StaticImageActivateScheduleActionSettingsTypeDef
+        ],
+        "StaticImageDeactivateSettings": NotRequired[
+            StaticImageDeactivateScheduleActionSettingsTypeDef
+        ],
+        "StaticImageOutputActivateSettings": NotRequired[
+            StaticImageOutputActivateScheduleActionSettingsOutputTypeDef
+        ],
+        "StaticImageOutputDeactivateSettings": NotRequired[
+            StaticImageOutputDeactivateScheduleActionSettingsOutputTypeDef
         ],
     },
 )
 ScheduleActionSettingsTypeDef = TypedDict(
     "ScheduleActionSettingsTypeDef",
     {
         "HlsId3SegmentTaggingSettings": NotRequired[
@@ -4978,94 +5523,101 @@
             StaticImageOutputActivateScheduleActionSettingsTypeDef
         ],
         "StaticImageOutputDeactivateSettings": NotRequired[
             StaticImageOutputDeactivateScheduleActionSettingsTypeDef
         ],
     },
 )
-ChannelSummaryPaginatorTypeDef = TypedDict(
-    "ChannelSummaryPaginatorTypeDef",
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
         "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationPaginatorTypeDef]],
+        "Destinations": NotRequired[List[OutputDestinationOutputTypeDef]],
         "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
         "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentPaginatorTypeDef]],
+        "InputAttachments": NotRequired[List[InputAttachmentOutputTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
         "Maintenance": NotRequired[MaintenanceStatusTypeDef],
         "Name": NotRequired[str],
         "PipelinesRunningCount": NotRequired[int],
         "RoleArn": NotRequired[str],
         "State": NotRequired[ChannelStateType],
         "Tags": NotRequired[Dict[str, str]],
         "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+InputAttachmentUnionTypeDef = Union[InputAttachmentTypeDef, InputAttachmentExtraOutputTypeDef]
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
     {
-        "Arn": NotRequired[str],
-        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationTypeDef]],
-        "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
-        "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentTypeDef]],
-        "InputSpecification": NotRequired[InputSpecificationTypeDef],
-        "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceStatusTypeDef],
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
         "Name": NotRequired[str],
-        "PipelinesRunningCount": NotRequired[int],
-        "RoleArn": NotRequired[str],
-        "State": NotRequired[ChannelStateType],
-        "Tags": NotRequired[Dict[str, str]],
-        "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
         "Name": NotRequired[str],
     },
 )
-ScheduleActionPaginatorTypeDef = TypedDict(
-    "ScheduleActionPaginatorTypeDef",
+ScheduleActionExtraOutputTypeDef = TypedDict(
+    "ScheduleActionExtraOutputTypeDef",
+    {
+        "ActionName": str,
+        "ScheduleActionSettings": ScheduleActionSettingsExtraOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsExtraOutputTypeDef,
+    },
+)
+ScheduleActionOutputTypeDef = TypedDict(
+    "ScheduleActionOutputTypeDef",
     {
         "ActionName": str,
-        "ScheduleActionSettings": ScheduleActionSettingsPaginatorTypeDef,
-        "ScheduleActionStartSettings": ScheduleActionStartSettingsPaginatorTypeDef,
+        "ScheduleActionSettings": ScheduleActionSettingsOutputTypeDef,
+        "ScheduleActionStartSettings": ScheduleActionStartSettingsOutputTypeDef,
     },
 )
 ScheduleActionTypeDef = TypedDict(
     "ScheduleActionTypeDef",
     {
         "ActionName": str,
         "ScheduleActionSettings": ScheduleActionSettingsTypeDef,
         "ScheduleActionStartSettings": ScheduleActionStartSettingsTypeDef,
     },
 )
-ListChannelsResponsePaginatorTypeDef = TypedDict(
-    "ListChannelsResponsePaginatorTypeDef",
-    {
-        "Channels": List[ChannelSummaryPaginatorTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+EncoderSettingsOutputTypeDef = TypedDict(
+    "EncoderSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "VideoDescriptions": List[VideoDescriptionOutputTypeDef],
+        "AvailBlanking": NotRequired[AvailBlankingTypeDef],
+        "AvailConfiguration": NotRequired[AvailConfigurationTypeDef],
+        "BlackoutSlate": NotRequired[BlackoutSlateTypeDef],
+        "CaptionDescriptions": NotRequired[List[CaptionDescriptionOutputTypeDef]],
+        "FeatureActivations": NotRequired[FeatureActivationsTypeDef],
+        "GlobalConfiguration": NotRequired[GlobalConfigurationOutputTypeDef],
+        "MotionGraphicsConfiguration": NotRequired[MotionGraphicsConfigurationOutputTypeDef],
+        "NielsenConfiguration": NotRequired[NielsenConfigurationTypeDef],
+        "ThumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
+        "ColorCorrectionSettings": NotRequired[ColorCorrectionSettingsOutputTypeDef],
     },
 )
 EncoderSettingsTypeDef = TypedDict(
     "EncoderSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "OutputGroups": Sequence[OutputGroupTypeDef],
@@ -5079,101 +5631,74 @@
         "GlobalConfiguration": NotRequired[GlobalConfigurationTypeDef],
         "MotionGraphicsConfiguration": NotRequired[MotionGraphicsConfigurationTypeDef],
         "NielsenConfiguration": NotRequired[NielsenConfigurationTypeDef],
         "ThumbnailConfiguration": NotRequired[ThumbnailConfigurationTypeDef],
         "ColorCorrectionSettings": NotRequired[ColorCorrectionSettingsTypeDef],
     },
 )
-DescribeScheduleResponsePaginatorTypeDef = TypedDict(
-    "DescribeScheduleResponsePaginatorTypeDef",
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
     {
-        "NextToken": str,
-        "ScheduleActions": List[ScheduleActionPaginatorTypeDef],
+        "ScheduleActions": List[ScheduleActionExtraOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-BatchScheduleActionCreateRequestTypeDef = TypedDict(
-    "BatchScheduleActionCreateRequestTypeDef",
-    {
-        "ScheduleActions": Sequence[ScheduleActionTypeDef],
+        "NextToken": NotRequired[str],
     },
 )
 BatchScheduleActionCreateResultTypeDef = TypedDict(
     "BatchScheduleActionCreateResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
 BatchScheduleActionDeleteResultTypeDef = TypedDict(
     "BatchScheduleActionDeleteResultTypeDef",
     {
-        "ScheduleActions": List[ScheduleActionTypeDef],
+        "ScheduleActions": List[ScheduleActionOutputTypeDef],
     },
 )
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
+BatchScheduleActionCreateRequestTypeDef = TypedDict(
+    "BatchScheduleActionCreateRequestTypeDef",
     {
-        "NextToken": str,
-        "ScheduleActions": List[ScheduleActionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ScheduleActions": Sequence[ScheduleActionTypeDef],
     },
 )
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Arn": NotRequired[str],
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
         "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[List[OutputDestinationTypeDef]],
+        "Destinations": NotRequired[List[OutputDestinationOutputTypeDef]],
         "EgressEndpoints": NotRequired[List[ChannelEgressEndpointTypeDef]],
-        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
+        "EncoderSettings": NotRequired[EncoderSettingsOutputTypeDef],
         "Id": NotRequired[str],
-        "InputAttachments": NotRequired[List[InputAttachmentTypeDef]],
+        "InputAttachments": NotRequired[List[InputAttachmentOutputTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
         "Maintenance": NotRequired[MaintenanceStatusTypeDef],
         "Name": NotRequired[str],
         "PipelineDetails": NotRequired[List[PipelineDetailTypeDef]],
         "PipelinesRunningCount": NotRequired[int],
         "RoleArn": NotRequired[str],
         "State": NotRequired[ChannelStateType],
         "Tags": NotRequired[Dict[str, str]],
         "Vpc": NotRequired[VpcOutputSettingsDescriptionTypeDef],
     },
 )
-CreateChannelRequestRequestTypeDef = TypedDict(
-    "CreateChannelRequestRequestTypeDef",
-    {
-        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "ChannelClass": NotRequired[ChannelClassType],
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
-        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
-        "InputAttachments": NotRequired[Sequence[InputAttachmentTypeDef]],
-        "InputSpecification": NotRequired[InputSpecificationTypeDef],
-        "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceCreateSettingsTypeDef],
-        "Name": NotRequired[str],
-        "RequestId": NotRequired[str],
-        "Reserved": NotRequired[str],
-        "RoleArn": NotRequired[str],
-        "Tags": NotRequired[Mapping[str, str]],
-        "Vpc": NotRequired[VpcOutputSettingsTypeDef],
-    },
-)
 DeleteChannelResponseTypeDef = TypedDict(
     "DeleteChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5185,19 +5710,19 @@
 )
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5209,19 +5734,19 @@
 )
 RestartChannelPipelinesResponseTypeDef = TypedDict(
     "RestartChannelPipelinesResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "MaintenanceStatus": str,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
@@ -5234,19 +5759,19 @@
 )
 StartChannelResponseTypeDef = TypedDict(
     "StartChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
@@ -5258,63 +5783,83 @@
 )
 StopChannelResponseTypeDef = TypedDict(
     "StopChannelResponseTypeDef",
     {
         "Arn": str,
         "CdiInputSpecification": CdiInputSpecificationTypeDef,
         "ChannelClass": ChannelClassType,
-        "Destinations": List[OutputDestinationTypeDef],
+        "Destinations": List[OutputDestinationOutputTypeDef],
         "EgressEndpoints": List[ChannelEgressEndpointTypeDef],
-        "EncoderSettings": EncoderSettingsTypeDef,
+        "EncoderSettings": EncoderSettingsOutputTypeDef,
         "Id": str,
-        "InputAttachments": List[InputAttachmentTypeDef],
+        "InputAttachments": List[InputAttachmentOutputTypeDef],
         "InputSpecification": InputSpecificationTypeDef,
         "LogLevel": LogLevelType,
         "Maintenance": MaintenanceStatusTypeDef,
         "Name": str,
         "PipelineDetails": List[PipelineDetailTypeDef],
         "PipelinesRunningCount": int,
         "RoleArn": str,
         "State": ChannelStateType,
         "Tags": Dict[str, str],
         "Vpc": VpcOutputSettingsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChannelRequestRequestTypeDef = TypedDict(
-    "UpdateChannelRequestRequestTypeDef",
+CreateChannelRequestRequestTypeDef = TypedDict(
+    "CreateChannelRequestRequestTypeDef",
     {
-        "ChannelId": str,
         "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
-        "Destinations": NotRequired[Sequence[OutputDestinationTypeDef]],
+        "ChannelClass": NotRequired[ChannelClassType],
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
         "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
-        "InputAttachments": NotRequired[Sequence[InputAttachmentTypeDef]],
+        "InputAttachments": NotRequired[Sequence[InputAttachmentUnionTypeDef]],
         "InputSpecification": NotRequired[InputSpecificationTypeDef],
         "LogLevel": NotRequired[LogLevelType],
-        "Maintenance": NotRequired[MaintenanceUpdateSettingsTypeDef],
+        "Maintenance": NotRequired[MaintenanceCreateSettingsTypeDef],
         "Name": NotRequired[str],
+        "RequestId": NotRequired[str],
+        "Reserved": NotRequired[str],
         "RoleArn": NotRequired[str],
+        "Tags": NotRequired[Mapping[str, str]],
+        "Vpc": NotRequired[VpcOutputSettingsTypeDef],
     },
 )
-BatchUpdateScheduleRequestRequestTypeDef = TypedDict(
-    "BatchUpdateScheduleRequestRequestTypeDef",
+EncoderSettingsUnionTypeDef = Union[EncoderSettingsTypeDef, EncoderSettingsOutputTypeDef]
+UpdateChannelRequestRequestTypeDef = TypedDict(
+    "UpdateChannelRequestRequestTypeDef",
     {
         "ChannelId": str,
-        "Creates": NotRequired[BatchScheduleActionCreateRequestTypeDef],
-        "Deletes": NotRequired[BatchScheduleActionDeleteRequestTypeDef],
+        "CdiInputSpecification": NotRequired[CdiInputSpecificationTypeDef],
+        "Destinations": NotRequired[Sequence[OutputDestinationUnionTypeDef]],
+        "EncoderSettings": NotRequired[EncoderSettingsTypeDef],
+        "InputAttachments": NotRequired[Sequence[InputAttachmentUnionTypeDef]],
+        "InputSpecification": NotRequired[InputSpecificationTypeDef],
+        "LogLevel": NotRequired[LogLevelType],
+        "Maintenance": NotRequired[MaintenanceUpdateSettingsTypeDef],
+        "Name": NotRequired[str],
+        "RoleArn": NotRequired[str],
     },
 )
 BatchUpdateScheduleResponseTypeDef = TypedDict(
     "BatchUpdateScheduleResponseTypeDef",
     {
         "Creates": BatchScheduleActionCreateResultTypeDef,
         "Deletes": BatchScheduleActionDeleteResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchUpdateScheduleRequestRequestTypeDef = TypedDict(
+    "BatchUpdateScheduleRequestRequestTypeDef",
+    {
+        "ChannelId": str,
+        "Creates": NotRequired[BatchScheduleActionCreateRequestTypeDef],
+        "Deletes": NotRequired[BatchScheduleActionDeleteRequestTypeDef],
+    },
+)
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.py` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive/waiter.pyi` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.83
-Summary: Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.99
+Summary: Type annotations for boto3.MediaLive 1.34.99 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.99](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-medialive docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-medialive-1.34.83/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy_boto3_medialive-1.34.99/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.83/setup.py` & `mypy_boto3_medialive-1.34.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.34.83",
+    version="1.34.99",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MediaLive 1.34.83 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.MediaLive 1.34.99 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

