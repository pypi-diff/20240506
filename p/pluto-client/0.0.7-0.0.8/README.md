# Comparing `tmp/pluto_client-0.0.7.tar.gz` & `tmp/pluto_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluto_client-0.0.7.tar", max compression
+gzip compressed data, was "pluto_client-0.0.8.tar", max compression
```

## Comparing `pluto_client-0.0.7.tar` & `pluto_client-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.7/LICENSE
--rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.7/README.md
--rw-r--r--   0        0        0      593 2024-04-23 09:34:27.660381 pluto_client-0.0.7/pluto_client/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-23 09:17:42.415282 pluto_client-0.0.7/pluto_client/bucket.py
--rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/__init__.py
--rw-r--r--   0        0        0      269 2024-04-23 09:09:43.024707 pluto_client-0.0.7/pluto_client/clients/aws/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-23 13:39:35.016299 pluto_client-0.0.7/pluto_client/clients/aws/bucket_s3.py
--rw-r--r--   0        0        0     2788 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/function_lambda.py
--rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/kvstore_dynamodb.py
--rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/aws/queue_sns.py
--rw-r--r--   0        0        0     1058 2024-04-22 13:09:52.133703 pluto_client-0.0.7/pluto_client/clients/aws/sagemaker.py
--rw-r--r--   0        0        0      376 2024-04-23 13:16:59.263894 pluto_client-0.0.7/pluto_client/clients/aws/test.py
--rw-r--r--   0        0        0      575 2024-04-23 09:49:31.514283 pluto_client-0.0.7/pluto_client/clients/aws/utils.py
--rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/errors.py
--rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/shared/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/clients/shared/router.py
--rw-r--r--   0        0        0     1882 2024-04-23 08:14:10.375522 pluto_client-0.0.7/pluto_client/function.py
--rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/kvstore.py
--rw-r--r--   0        0        0     1889 2024-04-23 09:23:49.411273 pluto_client-0.0.7/pluto_client/queue.py
--rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/router.py
--rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.7/pluto_client/sagemaker.py
--rw-r--r--   0        0        0     1276 2024-04-23 09:38:53.027207 pluto_client-0.0.7/pluto_client/schedule.py
--rw-r--r--   0        0        0      796 2024-04-23 13:53:53.724431 pluto_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.8/LICENSE
+-rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.8/README.md
+-rw-r--r--   0        0        0      593 2024-04-28 03:53:08.789970 pluto_client-0.0.8/pluto_client/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-28 03:53:08.790970 pluto_client-0.0.8/pluto_client/bucket.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-28 03:53:08.790970 pluto_client-0.0.8/pluto_client/clients/aws/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-28 03:53:08.791970 pluto_client-0.0.8/pluto_client/clients/aws/bucket_s3.py
+-rw-r--r--   0        0        0     2830 2024-05-06 09:18:56.382401 pluto_client-0.0.8/pluto_client/clients/aws/function_lambda.py
+-rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/aws/kvstore_dynamodb.py
+-rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/aws/queue_sns.py
+-rw-r--r--   0        0        0     1058 2024-04-28 03:53:08.792971 pluto_client-0.0.8/pluto_client/clients/aws/sagemaker.py
+-rw-r--r--   0        0        0      575 2024-04-28 03:53:08.793970 pluto_client-0.0.8/pluto_client/clients/aws/utils.py
+-rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/errors.py
+-rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/shared/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/shared/router.py
+-rw-r--r--   0        0        0     1972 2024-05-06 09:18:21.896053 pluto_client-0.0.8/pluto_client/function.py
+-rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/kvstore.py
+-rw-r--r--   0        0        0     1889 2024-05-06 07:22:25.100312 pluto_client-0.0.8/pluto_client/queue.py
+-rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/router.py
+-rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/sagemaker.py
+-rw-r--r--   0        0        0     1276 2024-04-28 03:53:08.793970 pluto_client-0.0.8/pluto_client/schedule.py
+-rw-r--r--   0        0        0      796 2024-05-06 09:55:57.058392 pluto_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.8/PKG-INFO
```

### Comparing `pluto_client-0.0.7/LICENSE` & `pluto_client-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/__init__.py` & `pluto_client-0.0.8/pluto_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/bucket.py` & `pluto_client-0.0.8/pluto_client/bucket.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/bucket_s3.py` & `pluto_client-0.0.8/pluto_client/clients/aws/bucket_s3.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/function_lambda.py` & `pluto_client-0.0.8/pluto_client/clients/aws/function_lambda.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,21 @@
     "RequestResponse": 200,
     "Event": 202,
     "DryRun": 204,
 }
 
 
 class LambdaFunction(IFunctionClient[FnHandler]):
-    def __init__(self, func: FnHandler, opts: Optional[FunctionOptions] = None):
-        name = (opts.name if opts else None) or DEFAULT_FUNCTION_NAME
+    def __init__(
+        self,
+        func: FnHandler,
+        name: Optional[str] = None,
+        opts: Optional[FunctionOptions] = None,
+    ):
+        name = name or DEFAULT_FUNCTION_NAME
         self.__id = gen_resource_id(Function.fqn, name)
         self.__lambda_name = gen_aws_resource_name(self.__id)
 
     def url(self) -> str:
         return get_env_val_for_property(self.__id, "url")
 
     def invoke(self, *args, **kwargs) -> Any:
```

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/kvstore_dynamodb.py` & `pluto_client-0.0.8/pluto_client/clients/aws/kvstore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/queue_sns.py` & `pluto_client-0.0.8/pluto_client/clients/aws/queue_sns.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/sagemaker.py` & `pluto_client-0.0.8/pluto_client/clients/aws/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/clients/aws/utils.py` & `pluto_client-0.0.8/pluto_client/clients/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/function.py` & `pluto_client-0.0.8/pluto_client/function.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 class DirectCallResponse:
     code: int
     body: Any
 
 
 @dataclass
 class FunctionOptions:
-    name: str | None = None
     memory: int | None = 128  # The memory size in MB, default is 128.
     envs: Dict[str, Any] | None = None
 
 
 class IFunctionClientApi(Generic[FnHandler], IResourceClientApi):
     def invoke(self, *args, **kwargs) -> Any:
         raise NotImplementedError
@@ -49,23 +48,30 @@
 class IFunctionInfra(IFunctionInfraApi, IFunctionCapturedProps):
     pass
 
 
 class Function(IResource, IFunctionClient[FnHandler], IFunctionInfra):
     fqn = "@plutolang/pluto.Function"
 
-    def __init__(self, func: FnHandler, opts: Optional[FunctionOptions] = None):
+    def __init__(
+        self,
+        func: FnHandler,
+        name: Optional[str] = None,
+        opts: Optional[FunctionOptions] = None,
+    ):
         raise NotImplementedError(
             "Cannot instantiate this class, instead of its subclass depending on the target runtime."
         )
 
     @staticmethod
     def build_client(
-        func: FnHandler, opts: Optional[FunctionOptions] = None
+        func: FnHandler,
+        name: Optional[str] = None,
+        opts: Optional[FunctionOptions] = None,
     ) -> IFunctionClient[FnHandler]:
         platform_type = utils.current_platform_type()
         if platform_type == PlatformType.AWS:
             from .clients import aws
 
-            return aws.LambdaFunction(func, opts)
+            return aws.LambdaFunction(func, name, opts)
         else:
             raise ValueError(f"not support this runtime '{platform_type}'")
```

### Comparing `pluto_client-0.0.7/pluto_client/kvstore.py` & `pluto_client-0.0.8/pluto_client/kvstore.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/queue.py` & `pluto_client-0.0.8/pluto_client/queue.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/router.py` & `pluto_client-0.0.8/pluto_client/router.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/sagemaker.py` & `pluto_client-0.0.8/pluto_client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pluto_client/schedule.py` & `pluto_client-0.0.8/pluto_client/schedule.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.7/pyproject.toml` & `pluto_client-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pluto-client"
-version = "0.0.7"
+version = "0.0.8"
 description = "The Client Library for Pluto Programming Language."
 authors = ["Jade Zheng <zheng.shoujian@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     'Development Status :: 1 - Planning',
     'Environment :: Console',
```

### Comparing `pluto_client-0.0.7/PKG-INFO` & `pluto_client-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluto-client
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Client Library for Pluto Programming Language.
 License: Apache-2.0
 Author: Jade Zheng
 Author-email: zheng.shoujian@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

