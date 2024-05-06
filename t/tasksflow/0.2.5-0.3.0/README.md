# Comparing `tmp/tasksflow-0.2.5.tar.gz` & `tmp/tasksflow-0.3.0.tar.gz`

## Comparing `tasksflow-0.2.5.tar` & `tasksflow-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.python-version
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.5/Dockerfile.ci
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 tasksflow-0.2.5/README_zh_CN.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 tasksflow-0.2.5/requirements-dev.lock
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.5/requirements.lock
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/dev.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/dev_zh_CN.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/README.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/main.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/README.md
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/main.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/requirements.txt
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.5/scripts/entrypoint
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 tasksflow-0.2.5/scripts/release.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/__init__.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/cache.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/common.py
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/executer.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/pool.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/cache_test.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/cpu_intensive_test.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/http_test.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/normal_test.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.5/LICENSE
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tasksflow-0.2.5/README.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tasksflow-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tasksflow-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.3.0/.python-version
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.3.0/Dockerfile.ci
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 tasksflow-0.3.0/README_zh_CN.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 tasksflow-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.3.0/requirements.lock
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tasksflow-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/dev.md
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/dev_zh_CN.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo1/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo1/main.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo1/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo2/README.md
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo2/main.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tasksflow-0.3.0/docs/demos/demo2/requirements.txt
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.3.0/scripts/entrypoint
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 tasksflow-0.3.0/scripts/release.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/__init__.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/cache.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/common.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/executer.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/pool.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 tasksflow-0.3.0/src/tasksflow/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 tasksflow-0.3.0/tests/cache_test.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 tasksflow-0.3.0/tests/cpu_intensive_test.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 tasksflow-0.3.0/tests/http_test.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 tasksflow-0.3.0/tests/normal_test.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.3.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tasksflow-0.3.0/README.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tasksflow-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tasksflow-0.3.0/PKG-INFO
```

### Comparing `tasksflow-0.2.5/README_zh_CN.md` & `tasksflow-0.3.0/README_zh_CN.md`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/requirements-dev.lock` & `tasksflow-0.3.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/.github/workflows/publish.yml` & `tasksflow-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/.github/workflows/test.yml` & `tasksflow-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/docs/dev_zh_CN.md` & `tasksflow-0.3.0/docs/dev_zh_CN.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
 ```sh
 rye test # 运行测试
 rye test -- --cov # 运行测试并打印测试覆盖率
 rye test -- -s # 运行测试并打印日志
 rye test -- -s ./tests/cache_test.py::test_cache_work # 运行单独测试并打印日志
 rye build # 构建 wheel 包
-mypy --python-executable .venv/bin/python . # 使用 mypy 进行检查
-/workspace/.venv/bin/ruff check # 使用 ruff 进行代码检查
+mypy --python-executable .venv/bin/python --exclude docs . # 使用 mypy 进行检查
+/workspace/.venv/bin/ruff check --fix # 使用 ruff 进行代码检查并自动修复
 /workspace/.venv/bin/ruff format # 使用 ruff 进行代码格式化
-/workspace/.venv/bin/python /workspace/scripts/release.py
+/workspace/.venv/bin/python /workspace/scripts/release.py # 发布新版本
 ```
```

### Comparing `tasksflow-0.2.5/docs/demos/demo1/main.py` & `tasksflow-0.3.0/docs/demos/demo1/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import tasksflow.task
 import tasksflow.cache
 
 from loguru import logger
 
 logger.enable("tasksflow")
 
+
 class Task1(tasksflow.task.Task):
     def run(self):
         return {"a": 1, "b": 2}
 
 
 class Task2(tasksflow.task.Task):
     def run(self, a: int, b: int):
@@ -22,22 +23,16 @@
 
 
 class Task4(tasksflow.task.Task):
     def run(self, c: int):
         pass
 
 
-
 def main():
-
-    mem = tasksflow.cache.MemoryCacheProvider()
-
     tasks = [Task1(), Task2(), Task3(), Task4()]
-    p = tasksflow.pool.Pool(tasks, cache_provider=mem)
-    result = p.run()
-    print(f"result: {result}")
+    p = tasksflow.pool.Pool(tasks)
     result = p.run()
     print(f"result: {result}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tasksflow-0.2.5/docs/demos/demo2/main.py` & `tasksflow-0.3.0/docs/demos/demo2/main.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/scripts/release.py` & `tasksflow-0.3.0/scripts/release.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/src/tasksflow/cache.py` & `tasksflow-0.3.0/src/tasksflow/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sqlite3
 import pickle
 from abc import ABC, abstractmethod
 from typing import Optional
 from pathlib import Path
 from .common import Code, Payload, PayloadBin
-from loguru import logger
 
 
 class CacheProvider(ABC):
     @abstractmethod
     def get(self, code: Code, params: Payload) -> Optional[Payload]:
         """
         get result for code and params from cache, return None if not found
@@ -68,19 +67,19 @@
     def get(self, code: Code, params: Payload) -> Optional[Payload]:
         params_bin = pickle.dumps(params)
         return self.d.get((code, params_bin))
 
     def set(self, code: Code, params: Payload, result: Payload):
         params_bin = pickle.dumps(params)
         self.d[(code, params_bin)] = result
-        logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
-        logger.debug(f"cache: {self.d}")
+        # logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
+        # logger.debug(f"cache: {self.d}")
 
     def clear(self, remain_records: int = 0):
-        logger.debug(f"clear cache, remain_records: {remain_records}")
+        # logger.debug(f"clear cache, remain_records: {remain_records}")
         if remain_records < 0:
             raise ValueError("remain_records must be greater than or equal to 0")
         if remain_records == 0:
             self.d.clear()
         else:
             self.d = dict(list(self.d.items())[-remain_records:])
 
@@ -114,22 +113,22 @@
         with sqlite3.connect(self.db_path) as conn:
             c = conn.cursor()
             c.execute(
                 "SELECT result FROM cache WHERE code = ? AND params = ?",
                 (code, params_bin),
             )
             record = c.fetchone()
-            logger.debug(f"record: {record}")
+            # logger.debug(f"record: {record}")
             if record is None:
                 return None
             result = pickle.loads(record[0])
             return result
 
     def set(self, code: str, params: Payload, result: Payload):
-        logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
+        # logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
         self._create_db()
 
         params_bin = pickle.dumps(params)
         result_bin = pickle.dumps(result)
 
         with sqlite3.connect(self.db_path) as conn:
             c = conn.cursor()
```

### Comparing `tasksflow-0.2.5/src/tasksflow/executer.py` & `tasksflow-0.3.0/src/tasksflow/executer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .common import Payload
 
 from .task import Task
 from .cache import CacheProvider
 from loguru import logger
 import concurrent.futures
 from enum import Enum
-from typing import Any, Optional, Callable
+from typing import Optional
 import multiprocessing
 from abc import ABC, abstractmethod
 import inspect
 
 
 def _get_task_params_names(task: Task) -> list[str]:
     # https://stackoverflow.com/a/40363565
@@ -131,23 +131,23 @@
 
         ctx = multiprocessing.get_context(
             "spawn"
         )  # https://docs.python.org/3/whatsnew/3.12.html#:~:text=101588%20%E4%B8%AD%E8%B4%A1%E7%8C%AE%E3%80%82%EF%BC%89-,multiprocessing,-%3A%20In%20Python%203.14
         with concurrent.futures.ProcessPoolExecutor(mp_context=ctx) as executor:
             futures: list[concurrent.futures.Future] = []  # list of executing tasks
 
-            def _submit_prepared_tasks(pre_task: Optional[RunableTask] = None):
+            def _submit_prepared_tasks() -> None:
                 """
                 submit tasks that are prepared in rtasks
 
                 :param pre_task: the task that triggers the submission
                 """
-                cache_prepared_tasks: list[RunableTask] = (
-                    []
-                )  # tasks that are prepared by cache, can be finished without waiting
+                cache_prepared_tasks: list[
+                    RunableTask
+                ] = []  # tasks that are prepared by cache
                 for rtask in rtasks:
                     if rtask.status == TaskStatus.NOT_STARTED and rtask.is_prepared():
                         task_params = {}
                         for param in _get_task_params_names(rtask.task):
                             task_params[param] = d_payload[param]
 
                         rtask.task_params = task_params
@@ -156,47 +156,52 @@
                             rtask.task, task_params
                         )
 
                         if result is not None:
                             d_payload.update(result)
                             rtask.status = TaskStatus.DONE
                             cache_prepared_tasks.append(rtask)
+
+                            logger.debug(
+                                f"cache hit task: {rtask.task.__class__.__name__}"
+                            )
                         else:
                             rtask.status = TaskStatus.RUNNING
                             future = executor.submit(rtask.task._execute, **task_params)
                             futures.append(future)
                             rtask.future = future
 
-                        if pre_task is not None:
-                            logger.debug(f"submit task {rtask} by {pre_task.task}")
-                        else:
-                            logger.debug(f"submit task {rtask}")
+                            logger.debug(
+                                f"submit task: {rtask.task.__class__.__name__}"
+                            )
 
-                for rtask in cache_prepared_tasks:
-                    _submit_prepared_tasks(rtask)
+                if cache_prepared_tasks:
+                    _submit_prepared_tasks()
 
             # get the task that is done
             def wait_until_any(futures: list[concurrent.futures.Future]):
                 for f in concurrent.futures.as_completed(futures):
                     return f
                 raise ValueError("No task is done")
 
             _submit_prepared_tasks()
             while futures:
                 future = wait_until_any(futures)
                 futures.remove(future)
 
                 result = future.result()
-                rtask = next(rtask for rtask in rtasks if rtask.future == future) # find rtask by future
+                rtask = next(
+                    rtask for rtask in rtasks if rtask.future == future
+                )  # find rtask by future
                 if rtask.task_params is None:
                     raise ValueError(f"rtask {rtask} task_params should not be None")
                 self._set_task_result_to_cache(rtask.task, rtask.task_params, result)
                 rtask.status = TaskStatus.DONE
                 d_payload.update(result)
 
-                _submit_prepared_tasks(rtask)
+                _submit_prepared_tasks()
 
             for rtask in rtasks:
                 if rtask.status != TaskStatus.DONE:
                     raise ValueError(f"rtask {rtask} is not done")
 
         return d_payload
```

### Comparing `tasksflow-0.2.5/src/tasksflow/pool.py` & `tasksflow-0.3.0/src/tasksflow/pool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from .common import Payload
 from .task import Task
-from loguru import logger
-from typing import Any, Optional, Callable
+from typing import Optional
 from .cache import CacheProvider, SqliteCacheProvider
-from .executer import Executer, SerialExecuter, MultiprocessExecuter
+from .executer import Executer, MultiprocessExecuter
 from copy import deepcopy
 
 
 class Pool:
     def __init__(
         self,
         tasks: list[Task],
```

### Comparing `tasksflow-0.2.5/src/tasksflow/task.py` & `tasksflow-0.3.0/src/tasksflow/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import inspect
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Callable
-from copy import deepcopy
-from .cache import CacheProvider, SqliteCacheProvider
+from typing import Optional
+from .cache import CacheProvider
 from .common import Payload
-from loguru import logger
 
 
 def _is_payload_valid(payload: Payload) -> bool:
     if payload is None:
         return False
     if not isinstance(payload, dict):
         return False
```

### Comparing `tasksflow-0.2.5/tests/cache_test.py` & `tasksflow-0.3.0/tests/cache_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tasksflow.task
 import tasksflow.pool
 from loguru import logger
 
 logger.enable("tasksflow")
 
 
-def test_provider_valid():
+def test_provider_valid() -> None:
     sqlite_cache_provider = tasksflow.cache.SqliteCacheProvider(Path("test.db"))
 
     cache_providers: list[tasksflow.cache.CacheProvider] = [
         sqlite_cache_provider,
         tasksflow.cache.MemoryCacheProvider(),
     ]
```

### Comparing `tasksflow-0.2.5/tests/cpu_intensive_test.py` & `tasksflow-0.3.0/tests/cpu_intensive_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,8 +70,8 @@
     )
 
     start = time.time()
     result = p.run()
     multiprocess_time = time.time() - start
 
     assert result == {"a": 1, "b": 2, "c": 3}
-    assert multiprocess_time < 4 # 0.5 + 0.5 + 2 = 3
+    assert multiprocess_time < 4  # 0.5 + 0.5 + 2 = 3
```

### Comparing `tasksflow-0.2.5/tests/http_test.py` & `tasksflow-0.3.0/tests/http_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import tasksflow.task
 import tasksflow.cache
 import asyncio
 import pytest
 import json
 import requests
 from aiohttp import web
-from loguru import logger
 
 routes = web.RouteTableDef()
 
 db_items = {
     1: {"description": "This is an item"},
     2: {"description": "This is another item"},
 }
```

### Comparing `tasksflow-0.2.5/tests/normal_test.py` & `tasksflow-0.3.0/tests/normal_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,24 @@
         tasks,
         executer=tasksflow.executer.MultiprocessExecuter(),
         cache_provider=tasksflow.cache.MemoryCacheProvider(),
     )
     try:
         p.run()
         raise Exception("Should raise an exception when Task5 not executed")
-    except Exception as e:
+    except Exception:
         pass
 
+
 def test_multiprocess_run_with_cache():
     memory_cache_provider = tasksflow.cache.MemoryCacheProvider()
     tasks = [Task1(), Task2(), Task3(), Task4(), Task6()]
     p = tasksflow.pool.Pool(
         tasks,
         executer=tasksflow.executer.MultiprocessExecuter(),
         cache_provider=memory_cache_provider,
     )
     result = p.run()
     assert result == {"a": 1, "b": 2, "c": 3, "d": 4, "e": 5, "f": 12}
 
     result = p.run()
-    assert result == {"a": 1, "b": 2, "c": 3, "d": 4, "e": 5, "f": 12}
+    assert result == {"a": 1, "b": 2, "c": 3, "d": 4, "e": 5, "f": 12}
```

### Comparing `tasksflow-0.2.5/LICENSE` & `tasksflow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/README.md` & `tasksflow-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.5/pyproject.toml` & `tasksflow-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tasksflow"
-version = "0.2.5"
+version = "0.3.0"
 description = "Handling Complex Workflows with Tasks"
 authors = [{ name = "117503445", email = "t117503445@gmail.com" }]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
```

### Comparing `tasksflow-0.2.5/PKG-INFO` & `tasksflow-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tasksflow
-Version: 0.2.5
+Version: 0.3.0
 Summary: Handling Complex Workflows with Tasks
 Author-email: 117503445 <t117503445@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: loguru>=0.7.2
 Description-Content-Type: text/markdown
```

