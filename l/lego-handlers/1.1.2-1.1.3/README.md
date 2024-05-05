# Comparing `tmp/lego_handlers-1.1.2.tar.gz` & `tmp/lego_handlers-1.1.3.tar.gz`

## Comparing `lego_handlers-1.1.2.tar` & `lego_handlers-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/scripts/new-release.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/scripts/new-release.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.3/PKG-INFO
```

### Comparing `lego_handlers-1.1.2/requirements-dev.lock` & `lego_handlers-1.1.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.2/.github/workflows/CD.yml` & `lego_handlers-1.1.3/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.2/.github/workflows/CI.yml` & `lego_handlers-1.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.2/scripts/new-release.py` & `lego_handlers-1.1.3/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.2/src/lego_handlers/__init__.py` & `lego_handlers-1.1.3/src/lego_handlers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 
 async def process_result(
     result: Result[tuple[R, list[DomainEvent]], E],
     handler: Callable[[Result[R, E]], T],
     *,
     publish_events: bool,
 ) -> T:
-    if isinstance(result, Ok):
-        response_data, events = result.unwrap()
-        if publish_events:
-            await _publish_events(events=events)
-        return handler(Ok(response_data))
-    if isinstance(result, Err):
-        return handler(result)
-    assert_never(result)
+    match result:
+        case Ok(data_and_events):
+            response_data, events = data_and_events
+            if publish_events:
+                await _publish_events(events=events)
+            return handler(Ok(response_data))
+        case Err(error):
+            return handler(Err(error))
+        case _:
+            assert_never(result)
 
 
 async def _publish_events(events: list[DomainEvent]) -> None:
     """Publish events."""
     await asyncio.gather(
         *(event.publish() for event in events), return_exceptions=False
     )
```

### Comparing `lego_handlers-1.1.2/tests/test_something.py` & `lego_handlers-1.1.3/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.2/pyproject.toml` & `lego_handlers-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "1.1.2"
+version = "1.1.3"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

