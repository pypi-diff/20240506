# Comparing `tmp/external_resources_io-0.1.8.tar.gz` & `tmp/external_resources_io-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "external_resources_io-0.1.8.tar", max compression
+gzip compressed data, was "external_resources_io-0.1.9.tar", max compression
```

## Comparing `external_resources_io-0.1.8.tar` & `external_resources_io-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,4 @@
--rw-r--r--   0        0        0        0 2024-01-10 18:48:54.354880 external_resources_io-0.1.8/README.md
--rw-r--r--   0        0        0       37 2024-01-10 19:11:47.128001 external_resources_io-0.1.8/external_resources_io/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-10 19:11:47.128213 external_resources_io-0.1.8/external_resources_io/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-10 19:11:47.127723 external_resources_io-0.1.8/external_resources_io/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2024-01-10 19:11:47.128460 external_resources_io-0.1.8/external_resources_io/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-10 19:11:47.128791 external_resources_io-0.1.8/external_resources_io/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     2577 2024-01-17 16:01:27.015454 external_resources_io-0.1.8/external_resources_io/input.py
--rw-r--r--   0        0        0      403 2024-01-17 16:01:32.491623 external_resources_io-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 external_resources_io-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      127 2024-01-23 10:37:00.187282 external_resources_io-0.1.9/README.md
+-rw-r--r--   0        0        0     2672 2024-03-14 10:58:17.873257 external_resources_io-0.1.9/external_resources_io/input.py
+-rw-r--r--   0        0        0      403 2024-03-14 10:58:42.900555 external_resources_io-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 external_resources_io-0.1.9/PKG-INFO
```

### Comparing `external_resources_io-0.1.8/external_resources_io/input.py` & `external_resources_io-0.1.9/external_resources_io/input.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 import base64
 import json
 from typing import TypeVar, Type, Any
 from collections.abc import Mapping
 import os
 
+# EXAMPLE INPUT
 # {
 #   "data": {
 #     "identifier": "test-external-resources-iam-role",
 #     "assume_role": {
 #       "aws": null,
 #       "service": [
 #         "ec2.amazonaws.com"
@@ -39,35 +40,39 @@
 
 class TerraformProvisionOptions(BaseModel):
     tf_state_bucket: str
     tf_state_region: str
     tf_state_dynamodb_table: str
     tf_state_key: str
 
-class AppInterfaceProvision(BaseModel):
+class Provision(BaseModel):
     provision_provider: str  # aws
     provisioner: str  # ter-int-dev
     provider: str  # aws-iam-role
     identifier: str
-
     target_cluster: str
     target_namespace: str
     target_secret_name: Optional[str]
-    module_provision_data: TerraformProvisionOptions
 
-T = TypeVar('T', bound=BaseModel)
-def parse_model(model_class: Type[T], data: Mapping[str,Any]) -> T:
-    input = model_class.model_validate(data)
-    return input
+class Output(Provision):
+    data: dict[str, Any]
+
+class AppInterfaceProvision(Provision):
+    module_provision_data: TerraformProvisionOptions
 
 def read_input_data(b64data: str) -> dict[str, Any]:
     str_input = base64.b64decode(b64data.encode("utf-8")).decode("utf-8")
     data = json.loads(str_input)
     return data
 
+T = TypeVar('T', bound=BaseModel)
+def parse_model(model_class: Type[T], data: Mapping[str,Any]) -> T:
+    input = model_class.model_validate(data)
+    return input
+
 def parse_base64_model(model_class: Type[T], b64data: str) -> T:
     data = read_input_data(b64data)
     return parse_model(model_class=model_class, data=data)
 
 def parse_app_interface_provision(b64data: str) -> AppInterfaceProvision:
     data = read_input_data(b64data)
     provision: AppInterfaceProvision = parse_model(AppInterfaceProvision, data["provision"])
```

