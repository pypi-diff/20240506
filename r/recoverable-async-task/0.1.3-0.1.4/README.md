# Comparing `tmp/recoverable_async_task-0.1.3.tar.gz` & `tmp/recoverable_async_task-0.1.4.tar.gz`

## Comparing `recoverable_async_task-0.1.3.tar` & `recoverable_async_task-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/recoverable_async_task.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/.gitignore
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/README.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11243 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/recoverable_async_task.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/README.md
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.4/PKG-INFO
```

### Comparing `recoverable_async_task-0.1.3/recoverable_async_task.py` & `recoverable_async_task-0.1.4/recoverable_async_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from loguru import logger
 from tqdm import tqdm
 
 JSON_ITEM = TypeVar("JSON_ITEM", bound=Union[str, int, float, bool, None])
 
 JSON = Union[JSON_ITEM, dict[str, "JSON"], list["JSON"]]
 
-
 T = TypeVar("T", bound=JSON)
 
 
 class TaskException(Exception):
     def __init__(
         self,
         error_num: int,
@@ -145,27 +144,42 @@
 
 
 class CheckpointData(TypedDict):
     id: int | str
     data: JSON
 
 
+def json_default_serializer(o: JSON_ITEM):
+    logger.warning(
+        f"Object {str(o)} of type {o.__class__.__name__} is not JSON serializable"
+    )
+    return str(o)
+
+
 class Checkpoint:
     @staticmethod
     def load(checkpoint_path: str | Path) -> Iterator[CheckpointData]:
         logger.debug(f"load checkpoint from {checkpoint_path}")
         with Path(checkpoint_path).open() as f:
-            for line in f:
-                yield json.loads(line)
+            for ln, line in enumerate(f):
+                line = line.strip()
+                try:
+                    yield json.loads(line)
+                except json.JSONDecodeError as e:
+                    logger.warning(
+                        f'Failed to load checkpoint:\n  File "{checkpoint_path}", line {ln+1}\n    {line=}\n{e}'
+                    )
 
     @staticmethod
     def save_datas(save_path: str | Path, datas: JSON):
         logger.debug(f"save checkpoint to {save_path}")
         with (saved := Path(save_path)).open("w") as f:
-            json.dump(datas, f, ensure_ascii=False, indent=4)
+            json.dump(
+                datas, f, ensure_ascii=False, indent=4, default=json_default_serializer
+            )
 
         return saved
 
     def __init__(self, checkpoint_path_name: str) -> None:
         self.name = checkpoint_path_name
         self.checkpoint_path = Path(checkpoint_path_name).with_name(
             Path(checkpoint_path_name).stem + "-checkpoint.jsonl"
@@ -179,15 +193,20 @@
 
         self.saved = None
 
     def add(self, data: JSON, id: int | str):
         assert id not in self.datas, f"id {id} already exists"
         self.datas[id] = data
         with self.checkpoint_path.open("a") as f:
-            json.dump(CheckpointData(id=id, data=data), f, ensure_ascii=False)
+            json.dump(
+                CheckpointData(id=id, data=data),
+                f,
+                ensure_ascii=False,
+                default=json_default_serializer,
+            )
             f.write("\n")
 
     def save(self, save_path: str | Path | None = None):
         self.saved = Checkpoint.save_datas(
             save_path
             or Path(self.name).with_name(
                 Path(self.name).name + f"-results-{len(self.datas)}.json"
```

### Comparing `recoverable_async_task-0.1.3/README.md` & `recoverable_async_task-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.3/pyproject.toml` & `recoverable_async_task-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.3/PKG-INFO` & `recoverable_async_task-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: recoverable-async-task
-Version: 0.1.3
+Version: 0.1.4
 Summary: `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
 Project-URL: Homepage, https://github.com/Haskely/recoverable-async-task
 Project-URL: Bug Reports, https://github.com/Haskely/recoverable-async-task/issues
 Project-URL: Source, https://github.com/Haskely/recoverable-async-task
 Author-email: Haskely <Haskely@live.com>
 Requires-Python: >=3.8
 Requires-Dist: loguru>=0.7.2
```

