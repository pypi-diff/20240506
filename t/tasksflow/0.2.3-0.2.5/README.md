# Comparing `tmp/tasksflow-0.2.3.tar.gz` & `tmp/tasksflow-0.2.5.tar.gz`

## Comparing `tasksflow-0.2.3.tar` & `tasksflow-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.3/.python-version
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.3/Dockerfile.ci
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 tasksflow-0.2.3/README_zh_CN.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tasksflow-0.2.3/requirements-dev.lock
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.3/requirements.lock
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tasksflow-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/dev.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/dev_zh_CN.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo1/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo1/main.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo1/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo2/README.md
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo2/main.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tasksflow-0.2.3/docs/demos/demo2/requirements.txt
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.3/scripts/entrypoint
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/__init__.py
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/cache.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/common.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/executer.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/pool.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 tasksflow-0.2.3/src/tasksflow/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tasksflow-0.2.3/tests/cache_test.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tasksflow-0.2.3/tests/cpu_intensive_test.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.3/tests/http_test.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 tasksflow-0.2.3/tests/normal_test.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tasksflow-0.2.3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.3/LICENSE
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tasksflow-0.2.3/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 tasksflow-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tasksflow-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.python-version
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.5/Dockerfile.ci
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 tasksflow-0.2.5/README_zh_CN.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 tasksflow-0.2.5/requirements-dev.lock
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.5/requirements.lock
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/dev.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/dev_zh_CN.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/README.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/main.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo1/requirements.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/README.md
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/main.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tasksflow-0.2.5/docs/demos/demo2/requirements.txt
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.5/scripts/entrypoint
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 tasksflow-0.2.5/scripts/release.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/__init__.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/cache.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/common.py
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/executer.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/pool.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 tasksflow-0.2.5/src/tasksflow/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/cache_test.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/cpu_intensive_test.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/http_test.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 tasksflow-0.2.5/tests/normal_test.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.2.5/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tasksflow-0.2.5/README.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 tasksflow-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tasksflow-0.2.5/PKG-INFO
```

### Comparing `tasksflow-0.2.3/README_zh_CN.md` & `tasksflow-0.2.5/README_zh_CN.md`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/requirements-dev.lock` & `tasksflow-0.2.5/requirements-dev.lock`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     # via aiohttp
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via uvicorn
+coverage==7.5.1
+    # via coverage
+    # via pytest-cov
 fastapi==0.110.2
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 h11==0.14.0
     # via uvicorn
 idna==3.7
@@ -46,15 +49,17 @@
     # via pytest
 pydantic==2.7.0
     # via fastapi
 pydantic-core==2.18.1
     # via pydantic
 pytest==8.1.1
     # via pytest-asyncio
+    # via pytest-cov
 pytest-asyncio==0.23.6
+pytest-cov==5.0.0
 requests==2.31.0
 ruff==0.4.1
 sniffio==1.3.1
     # via anyio
 starlette==0.37.2
     # via fastapi
 types-requests==2.31.0.20240406
```

### Comparing `tasksflow-0.2.3/.github/workflows/publish.yml` & `tasksflow-0.2.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/.github/workflows/test.yml` & `tasksflow-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/docs/dev_zh_CN.md` & `tasksflow-0.2.5/docs/dev_zh_CN.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,16 @@
 
 VSCode 安装 Docker 和 Remote Container 插件，点击 Docker Tab。等待 `tasksflow-dev` 容器状态由 `starting` 变为 `running` 后，选中 `tasksflow-dev` 容器，点击 `Attach Visual Studio Code / 附加 VSCode`，并打开容器内的 `/workspace` 文件夹。
 
 以下是常用命令
 
 ```sh
 rye test # 运行测试
+rye test -- --cov # 运行测试并打印测试覆盖率
 rye test -- -s # 运行测试并打印日志
+rye test -- -s ./tests/cache_test.py::test_cache_work # 运行单独测试并打印日志
 rye build # 构建 wheel 包
 mypy --python-executable .venv/bin/python . # 使用 mypy 进行检查
 /workspace/.venv/bin/ruff check # 使用 ruff 进行代码检查
 /workspace/.venv/bin/ruff format # 使用 ruff 进行代码格式化
+/workspace/.venv/bin/python /workspace/scripts/release.py
 ```
```

### Comparing `tasksflow-0.2.3/docs/demos/demo2/main.py` & `tasksflow-0.2.5/docs/demos/demo2/main.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/src/tasksflow/cache.py` & `tasksflow-0.2.5/src/tasksflow/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,53 +6,60 @@
 from .common import Code, Payload, PayloadBin
 from loguru import logger
 
 
 class CacheProvider(ABC):
     @abstractmethod
     def get(self, code: Code, params: Payload) -> Optional[Payload]:
-        '''
+        """
         get result for code and params from cache, return None if not found
 
         :param code: the code of the task
         :param params: the params of the task
-        '''
+        """
         raise NotImplementedError
 
     @abstractmethod
     def set(self, code: Code, params: Payload, result: Payload):
-        '''
+        """
         set result cache for code and params
 
         :param code: the code of the task
         :param params: the params of the task
         :param result: the result of the task
-        '''
+        """
         raise NotImplementedError
 
     @abstractmethod
     def clear(self, remain_records: int = 0):
-        '''
+        """
         clear cache, if remain_records is 0, clear all cache records
 
         :param remain_records: the number of records to remain
-        '''
+        """
         raise NotImplementedError
 
     def _check_valid(self) -> bool:
-        '''
+        """
         check if the cache provider is valid
-        '''
-        result = {"c": 3}
-        self.set("tasktest", {"a": 1, "b": 2}, result)
-        cache_result = self.get("tasktest", {"a": 1, "b": 2})
-        if cache_result is None:
-            return False
-        if cache_result != result:
-            return False
+        """
+
+        def _set_and_get(code: Code, params: Payload, result: Payload) -> bool:
+            self.set(code, params, result)
+            cache_result = self.get(code, params)
+            return cache_result == result
+
+        tests = [
+            ("tasktest", {"a": 1, "b": 2}, {"c": 3}),
+            ("tasktest2", {}, {"c": 3}),
+        ]
+        for code, params, result in tests:
+            if not _set_and_get(code, params, result):
+                return False
+
         self.clear()
         cache_result = self.get("tasktest", {"a": 1, "b": 2})
         return cache_result is None
 
 
 class MemoryCacheProvider(CacheProvider):
     def __init__(self: "MemoryCacheProvider"):
@@ -61,16 +68,19 @@
     def get(self, code: Code, params: Payload) -> Optional[Payload]:
         params_bin = pickle.dumps(params)
         return self.d.get((code, params_bin))
 
     def set(self, code: Code, params: Payload, result: Payload):
         params_bin = pickle.dumps(params)
         self.d[(code, params_bin)] = result
+        logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
+        logger.debug(f"cache: {self.d}")
 
     def clear(self, remain_records: int = 0):
+        logger.debug(f"clear cache, remain_records: {remain_records}")
         if remain_records < 0:
             raise ValueError("remain_records must be greater than or equal to 0")
         if remain_records == 0:
             self.d.clear()
         else:
             self.d = dict(list(self.d.items())[-remain_records:])
 
@@ -78,47 +88,49 @@
 class SqliteCacheProvider(CacheProvider):
     def __init__(self, db_path: Optional[Path] = None):
         if db_path is None:
             db_path = Path("cache.db")
         self.db_path = db_path
 
     def _create_db(self):
+        """
+        _create_db create the cache table if not exists
+        """
         if self.db_path.exists():
             return
 
         with sqlite3.connect(self.db_path) as conn:
             c = conn.cursor()
             # unique constraint (code, params)
             c.execute(
                 "CREATE TABLE cache (code TEXT, params TEXT, result TEXT, created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP, UNIQUE(code, params))"
             )
             conn.commit()
 
     def get(self, code: str, params: Payload) -> Optional[Payload]:
-        if not self.db_path.exists():
-            self._create_db()
+        self._create_db()
 
         params_bin = pickle.dumps(params)
 
         with sqlite3.connect(self.db_path) as conn:
             c = conn.cursor()
             c.execute(
                 "SELECT result FROM cache WHERE code = ? AND params = ?",
                 (code, params_bin),
             )
             record = c.fetchone()
+            logger.debug(f"record: {record}")
             if record is None:
                 return None
             result = pickle.loads(record[0])
             return result
 
     def set(self, code: str, params: Payload, result: Payload):
         logger.debug(f"set cache for code: {code}, params: {params}, result: {result}")
-        if not self.db_path.exists():
-            self._create_db()
+        self._create_db()
 
         params_bin = pickle.dumps(params)
         result_bin = pickle.dumps(result)
 
         with sqlite3.connect(self.db_path) as conn:
             c = conn.cursor()
             c.execute(
```

### Comparing `tasksflow-0.2.3/src/tasksflow/pool.py` & `tasksflow-0.2.5/src/tasksflow/pool.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from .common import Payload
 from .task import Task
 from loguru import logger
 from typing import Any, Optional, Callable
 from .cache import CacheProvider, SqliteCacheProvider
-from .executer import multiprocess_run
+from .executer import Executer, SerialExecuter, MultiprocessExecuter
 from copy import deepcopy
 
+
 class Pool:
     def __init__(
         self,
         tasks: list[Task],
         cache_provider: Optional[CacheProvider] = None,
-        executer: Callable[[list[Task]], Payload] = multiprocess_run,
+        executer: Optional[Executer] = None,
     ):
         """
         Pool of tasks
 
         :param tasks: list of tasks
         :param cache_provider: cache task execution result to avoid re-execution for the same input
         :param executer: function to execute tasks
@@ -23,23 +24,23 @@
 
         # use deepcopy to prevent tasks from being modified
         self.tasks = deepcopy(tasks)
 
         if cache_provider is None:
             cache_provider = SqliteCacheProvider()
             # cache_provider = MemoryCacheProvider()
-        if not cache_provider._check_valid():
-            raise ValueError(
-                "Cache provider is not valid, please ensure cache_provider._check_valid() returns True"
-            )
-        self.cache_provider = cache_provider
-
-        for task in self.tasks:
-            task.cache_provider = self.cache_provider
 
+        # if not cache_provider._check_valid():
+        #     raise ValueError(
+        #         "Cache provider is not valid, please ensure cache_provider._check_valid() returns True"
+        #     )
+
+        if executer is None:
+            # executer = SerialExecuter(cache_provider=cache_provider)
+            executer = MultiprocessExecuter(cache_provider=cache_provider)
         self.executer = executer
 
     def run(self):
         """
         Execute the tasks in the pool
         """
-        return self.executer(self.tasks)
+        return self.executer.run(self.tasks)
```

### Comparing `tasksflow-0.2.3/tests/cpu_intensive_test.py` & `tasksflow-0.2.5/tests/cpu_intensive_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,27 +49,27 @@
     if num_cores <= 1:
         logger.warning("The number of cpu cores is less than 2, skip the test")
         return
 
     tasks = [Task1(), Task2(), Task3(), Task4()]
     p = tasksflow.pool.Pool(
         tasks,
-        executer=tasksflow.executer.serial_run,
+        executer=tasksflow.executer.SerialExecuter(),
         cache_provider=tasksflow.cache.MemoryCacheProvider(),
     )
     start = time.time()
     result = p.run()
     serial_time = time.time() - start
 
     assert result == {"a": 1, "b": 2, "c": 3}
     assert serial_time > 5
 
     p = tasksflow.pool.Pool(
         tasks,
-        executer=tasksflow.executer.multiprocess_run,
+        executer=tasksflow.executer.MultiprocessExecuter(),
         cache_provider=tasksflow.cache.MemoryCacheProvider(),
     )
 
     start = time.time()
     result = p.run()
     multiprocess_time = time.time() - start
```

### Comparing `tasksflow-0.2.3/tests/http_test.py` & `tasksflow-0.2.5/tests/http_test.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/tests/normal_test.py` & `tasksflow-0.2.5/docs/demos/demo1/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import tasksflow.cache
-import tasksflow.executer
 import tasksflow.pool
 import tasksflow.task
-from loguru import logger
+import tasksflow.cache
 
-# logger.enable("tasksflow")
+from loguru import logger
 
+logger.enable("tasksflow")
 
 class Task1(tasksflow.task.Task):
     def run(self):
         return {"a": 1, "b": 2}
 
 
 class Task2(tasksflow.task.Task):
@@ -23,29 +22,22 @@
 
 
 class Task4(tasksflow.task.Task):
     def run(self, c: int):
         pass
 
 
-def test_serial_run():
-    tasks = [Task1(), Task2(), Task3(), Task4()]
-    p = tasksflow.pool.Pool(
-        tasks,
-        executer=tasksflow.executer.serial_run,
-        cache_provider=tasksflow.cache.MemoryCacheProvider(),
-    )
-    result = p.run()
 
-    assert result == {"a": 1, "b": 2, "c": 3}
+def main():
 
+    mem = tasksflow.cache.MemoryCacheProvider()
 
-def test_multiprocess_run():
     tasks = [Task1(), Task2(), Task3(), Task4()]
-    p = tasksflow.pool.Pool(
-        tasks,
-        executer=tasksflow.executer.multiprocess_run,
-        cache_provider=tasksflow.cache.MemoryCacheProvider(),
-    )
+    p = tasksflow.pool.Pool(tasks, cache_provider=mem)
     result = p.run()
+    print(f"result: {result}")
+    result = p.run()
+    print(f"result: {result}")
+
 
-    assert result == {"a": 1, "b": 2, "c": 3}
+if __name__ == "__main__":
+    main()
```

### Comparing `tasksflow-0.2.3/LICENSE` & `tasksflow-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/README.md` & `tasksflow-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.3/pyproject.toml` & `tasksflow-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tasksflow"
-version = "0.2.3"
+version = "0.2.5"
 description = "Handling Complex Workflows with Tasks"
 authors = [{ name = "117503445", email = "t117503445@gmail.com" }]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
@@ -18,14 +18,15 @@
     "aiohttp>=3.9.5",
     "pytest-asyncio>=0.23.6",
     "fastapi>=0.110.2",
     "requests>=2.31.0",
     "uvicorn>=0.29.0",
     "types-requests>=2.31.0.20240406",
     "ruff>=0.4.1",
+    "pytest-cov>=5.0.0",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/tasksflow"]
```

### Comparing `tasksflow-0.2.3/PKG-INFO` & `tasksflow-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tasksflow
-Version: 0.2.3
+Version: 0.2.5
 Summary: Handling Complex Workflows with Tasks
 Author-email: 117503445 <t117503445@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: loguru>=0.7.2
 Description-Content-Type: text/markdown
```

