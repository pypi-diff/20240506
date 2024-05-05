# Comparing `tmp/pop_cli-6.0.1.tar.gz` & `tmp/pop_cli-7.0.0.tar.gz`

## Comparing `pop_cli-6.0.1.tar` & `pop_cli-7.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-6.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pop_cli-6.0.1/setup.py
--rwxr-xr-x   0        0        0      906 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/hub/__main__.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/config.yaml
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/cli.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/completer.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/config.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/console.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/init.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-6.0.1/src/pop_cli/plugin/state.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-6.0.1/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-6.0.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-6.0.1/README.rst
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pop_cli-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pop_cli-7.0.0/setup.py
+-rwxr-xr-x   0        0        0     1000 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/hub/__main__.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/config.yaml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/cli.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/completer.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/config.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/console.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/init.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/legacy.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-7.0.0/src/pop_cli/plugin/state.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-7.0.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-7.0.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-7.0.0/README.rst
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 pop_cli-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-7.0.0/PKG-INFO
```

### Comparing `pop_cli-6.0.1/.pre-commit-config.yaml` & `pop_cli-7.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/src/hub/__main__.py` & `pop_cli-7.0.0/src/hub/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,26 +15,30 @@
         loop.close()
 
 
 async def amain(loop):
     async with cpop.hub.Hub(cli="cli") as hub:
         await hub.log.debug("Initialized the hub")
 
+        if "legacy" in hub.cli:
+            await hub.cli.legacy.patch(loop=loop)
+
         # Start the hub cli
-        task = asyncio.create_task(hub._holder())
+        hold = asyncio.create_task(hub._holder())
 
         try:
             await hub.cli.init.run()
         except KeyboardInterrupt:
             await hub.log.error("Caught keyboard interrupt.  Cancelling...")
         except SystemExit:
             ...
         finally:
             await hub.log.debug("Cleaning up")
             await hub._tasks.put(cpop.hub.SHUTDOWN_SIGNAL)
-            if task:
-                await task
+            await asyncio.sleep(0)
+
+            await hold
             await loop.shutdown_asyncgens()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pop_cli-6.0.1/src/pop_cli/config.yaml` & `pop_cli-7.0.0/src/pop_cli/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
   - aioconsole.server
   - aiopath
   - asyncio
   - ast
   - builtins
   - functools
   - pdb
+  - pop.hub
   - pickle
   - pprint
   - prompt_toolkit
   - readline
   - rlcompleter
   - sys
   - typing
```

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/cli.py` & `pop_cli-7.0.0/src/pop_cli/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/completer.py` & `pop_cli-7.0.0/src/pop_cli/plugin/completer.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
             self._cursor_position = document._cursor_position
             self._selection = document._selection
             self._cache = document._cache
 
         def __hash__(self):
             return hash(
                 (self._text, self._cursor_position, self._selection, self._cache)
-
             )
 
     class HubCompleter(hub.lib.prompt_toolkit.completion.Completer):
         def get_completions(self, document, complete_event):
             return _get_completions(HashableDocument(document))
 
     completer = HubCompleter()
```

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/config.py` & `pop_cli-7.0.0/src/pop_cli/plugin/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     new_config = hub.lib.collections.defaultdict(dict)
     for namespace, data in opts.items():
         try:
             for k, v in data.items():
                 if namespace == "pop" and k in ("subparser", "global_clis"):
                     continue
-                    
+
                 new_config[namespace][k] = {"default": v}
         except AttributeError:
             continue
 
     # There is a user defined-cli, let it parse the remaining args it's own way
     hub._opt = await hub.pop.config.load(
         # Pass all remaining args onto the new parser
```

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/console.py` & `pop_cli-7.0.0/src/pop_cli/plugin/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/init.py` & `pop_cli-7.0.0/src/pop_cli/plugin/init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/ref.py` & `pop_cli-7.0.0/src/pop_cli/plugin/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/src/pop_cli/plugin/state.py` & `pop_cli-7.0.0/src/pop_cli/plugin/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/conftest.py` & `pop_cli-7.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_cli.py` & `pop_cli-7.0.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_config.py` & `pop_cli-7.0.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_console.py` & `pop_cli-7.0.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_init.py` & `pop_cli-7.0.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_ref.py` & `pop_cli-7.0.0/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/tests/integration/test_state.py` & `pop_cli-7.0.0/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/.gitignore` & `pop_cli-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/README.rst` & `pop_cli-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-6.0.1/pyproject.toml` & `pop_cli-7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "setuptools"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "6.0.1"
+version = "7.0.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
     "aiopath",
-    "cPop>=35.0.6",
+    "cPop>=36.0.1",
     "aioconsole",
     "prompt-toolkit",
 ]
 
 
 [project.optional-dependencies]
 test = [
```

### Comparing `pop_cli-6.0.1/PKG-INFO` & `pop_cli-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 6.0.1
+Version: 7.0.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
 Requires-Dist: aiopath
-Requires-Dist: cpop>=35.0.6
+Requires-Dist: cpop>=36.0.1
 Requires-Dist: prompt-toolkit
 Provides-Extra: test
 Requires-Dist: cpop[test]; extra == 'test'
 Requires-Dist: pexpect; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
```

