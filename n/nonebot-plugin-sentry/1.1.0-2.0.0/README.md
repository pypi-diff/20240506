# Comparing `tmp/nonebot_plugin_sentry-1.1.0.tar.gz` & `tmp/nonebot_plugin_sentry-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sentry-1.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sentry-2.0.0.tar", max compression
```

## Comparing `nonebot_plugin_sentry-1.1.0.tar` & `nonebot_plugin_sentry-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/LICENSE
--rw-r--r--   0        0        0     1456 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/README.md
--rw-r--r--   0        0        0      846 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/__init__.py
--rw-r--r--   0        0        0      760 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/compat.py
--rw-r--r--   0        0        0     1418 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/config.py
--rw-r--r--   0        0        0     1459 2024-02-14 03:21:31.645187 nonebot_plugin_sentry-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1456 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/README.md
+-rw-r--r--   0        0        0      846 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/__init__.py
+-rw-r--r--   0        0        0      760 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/compat.py
+-rw-r--r--   0        0        0     1492 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/config.py
+-rw-r--r--   0        0        0     2124 2024-05-06 09:36:05.327533 nonebot_plugin_sentry-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2375 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-2.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_sentry-1.1.0/LICENSE` & `nonebot_plugin_sentry-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-1.1.0/README.md` & `nonebot_plugin_sentry-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/__init__.py` & `nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/compat.py` & `nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-1.1.0/nonebot_plugin_sentry/config.py` & `nonebot_plugin_sentry-2.0.0/nonebot_plugin_sentry/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from nonebot import get_driver
 from pydantic import Field, BaseModel
 from sentry_sdk.integrations import Integration
 from nonebot.compat import PYDANTIC_V2, ConfigDict
 from sentry_sdk.integrations.loguru import LoguruIntegration
 
-from .compat import field_validator, model_validator
+from .compat import model_validator
 
 driver = get_driver()
 
 
 class Config(BaseModel):
     sentry_dsn: Optional[str] = None
     sentry_environment: str = driver.env
-    sentry_integrations: List[Integration] = Field(
+    sentry_integrations: list[Integration] = Field(
         default_factory=lambda: [LoguruIntegration()]
     )
 
     # [FIXED] https://github.com/getsentry/sentry-python/issues/653
     # sentry_default_integrations: bool = False
 
     if PYDANTIC_V2:
-        model_config: ConfigDict = ConfigDict(
-            extra="allow", arbitrary_types_allowed=True
-        )
+        model_config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
     else:
 
         class Config:
             extra = "allow"
             arbitrary_types_allowed = True
 
     @model_validator(mode="before")
     @classmethod
-    def filter_sentry_configs(cls, values: Dict[str, Any]):
+    def filter_sentry_configs(cls, values: dict[str, Any]):
         return {
             key: value for key, value in values.items() if key.startswith("sentry_")
         }
 
-    @field_validator("sentry_integrations", mode="after")
-    def validate_integrations(cls, v: List[Integration]):
-        ids = {i.identifier for i in v}
-        if LoguruIntegration.identifier not in ids:
-            v.append(LoguruIntegration())
-        return v
+    # [FIXED] https://github.com/getsentry/sentry-python/pull/2671
+    # LoguruIntegration is auto enabled by sentry_sdk now
+    # @field_validator("sentry_integrations", mode="after")
+    # def validate_integrations(cls, v: list[Integration]):
+    #     ids = {i.identifier for i in v}
+    #     if LoguruIntegration.identifier not in ids:
+    #         v.append(LoguruIntegration())
+    #     return v
```

