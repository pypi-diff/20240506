# Comparing `tmp/pyhectiqlab-2.1.9.tar.gz` & `tmp/pyhectiqlab-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hectiq-lab/hectiq-lab/python-client/dist/.tmp-cfgkv0q1/pyhectiqlab-2.1.9.tar", last modified: Tue Nov 28 19:21:57 2023, max compression
+gzip compressed data, was "pyhectiqlab-3.0.0.tar", last modified: Mon May  6 17:31:16 2024, max compression
```

## Comparing `pyhectiqlab-2.1.9.tar` & `pyhectiqlab-3.0.0.tar`

### file list

```diff
@@ -1,68 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab/
--rwxr-xr-x   0 runner    (1001) docker     (127)      145 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab/callbacks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       32 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/callbacks/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)      115 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/config_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/events_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/mlmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/notebooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15923 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/pulse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30216 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      736 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyhectiqlab/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 19:21:34.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/artifacts/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/artifacts/test_img2.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/create_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/dataset/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/dataset/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/dataset/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/mlmodel/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/mlmodel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/mlmodel/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/mlmodel/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/mlmodel/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 19:21:57.000000 pyhectiqlab-2.1.9/tests/step_artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)   158372 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step1.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   165197 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step2.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   726799 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step3.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   172506 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step4.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   165748 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step8.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)   153112 2023-11-28 19:21:21.000000 pyhectiqlab-2.1.9/tests/step_artifacts/step9.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24825 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 17:31:16.000000 pyhectiqlab-3.0.0/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:31:16.149129 pyhectiqlab-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-06 17:30:59.000000 pyhectiqlab-3.0.0/tests/test_run.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyhectiqlab-2.1.9/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.0/pyhectiqlab/metrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,168 @@
 from collections import defaultdict
-from pyhectiqlab.timer import RepeatedTimer
+from typing import Callable, List, Literal, Optional
+from functools import partial
 
+import threading
 import numpy as np
 import time
 import datetime as dt
-
 import logging
-logger = logging.getLogger('pyhectiqlab')
 
-class MetricsManager():
+logger = logging.getLogger("pyhectiqlab")
+
 
-    def __init__(self, max_cache_timeout=10,  # Maximum number of seconds in the cache
-                    max_cache_length=100, # Number of elements in the cache to trigger a cache dump
-                    min_cache_flush_delay=5, # Minimum number of seconds between two dumps
-                    aggregate_metrics="none", # Wheter to push all data in cache or aggregate
-                    push_method=None):
+class RepeatedTimer(threading.Thread):
+    """
+    RepeatedTimer class is used to run a method at a given interval.
+
+    Args:
+        method (callable): Method to run.
+        delay (int): Delay between two executions.
+    """
+
+    def __init__(self, method: Callable[[], None], delay: int):
+        super().__init__()
+        self.daemon = True
+        self._stopper = threading.Event()
+        self.delay = delay
+        self.method = method
+
+    def run(self):
+        while not self._stopper.wait(self.delay):
+            self.method()
+
+    def stopped(self):
+        return self._stopper.is_set()
+
+    def stop(self):
+        self._stopper.set()
+
+
+class MetricsManager:
+    """
+    MetricsManager class is used to manage the metrics cache and push data to the server.
+
+    Args:
+        push_method (callable, optional): Function to push data to the server
+        max_cache_timeout (int): Maximum number of seconds in the cache
+        max_cache_length (int): Number of elements in the cache to trigger a cache dump
+        min_cache_flush_delay (int): Minimum number of seconds between two dumps
+        aggregate_metrics (str): Wheter to push all data in cache or aggregate
+    """
+
+    __max_cache_quantity_per_second = 200
+
+    def __init__(
+        self,
+        push_method: Callable[[str, List[float]], None],
+        run: Optional[str] = None,
+        max_cache_timeout: int = 10,
+        max_cache_length: int = 100,
+        min_cache_flush_delay: int = 5,
+        aggregate_metrics: str = "none",
+    ):
         self.cache = defaultdict(list)
         self.cache_last_push = {}
-        self.__max_cache_quantity_per_second = 200
         self._warning_is_shown = False
         self.max_cache_length = max_cache_length
-        self.min_cache_flush_delay  = min_cache_flush_delay
-        self.push_method = push_method
+        self.min_cache_flush_delay = min_cache_flush_delay
+
+        self.push_method = partial(push_method, run=run)
         self.set_aggr(aggregate_metrics)
 
         self.timer = RepeatedTimer(self.flush_cache, max_cache_timeout)
         self.timer.start()
         return
 
-    def update_cache_settings(self, max_cache_timeout, max_cache_length, min_cache_flush_delay):
+    def update_cache_settings(
+        self,
+        max_cache_timeout: Optional[int] = None,
+        max_cache_length: Optional[int] = None,
+        min_cache_flush_delay: Optional[int] = None,
+    ):
+        """
+        Update cache settings.
+        """
+
         if max_cache_timeout is not None:
             self.max_cache_timeout = max_cache_timeout
             self.timer.stop()
             self.timer = RepeatedTimer(self.flush_cache, max_cache_timeout)
             self.timer.start()
         if max_cache_length is not None:
             self.max_cache_length = max_cache_length
         if min_cache_flush_delay is not None:
             self.min_cache_flush_delay = min_cache_flush_delay
-            
-    def set_aggr(self, new_value):
-        vals = ['none', 'sum', 'max', 'mean']
+
+    def set_aggr(self, new_value: Literal["none", "sum", "max", "mean"]):
+        vals = ["none", "sum", "max", "mean"]
         assert new_value in vals, f"Aggr must be in {vals}"
         self.aggregate_metrics = new_value
 
-    def add(self, key, value, step):
+    def add(self, key: str, step: int, value: float) -> None:
+        """
+        Add a new metric to the cache.
+        """
         if value is None:
             return
         self.cache[key].append((float(step), float(value), dt.datetime.now(tz=dt.timezone.utc).timestamp()))
-        if len(self.cache[key])>self.max_cache_length:
+        if len(self.cache[key]) > self.max_cache_length:
             if key in self.cache_last_push:
                 last_push_time = self.cache_last_push[key]
                 elapsed = time.time() - last_push_time
-                if elapsed<self.min_cache_flush_delay:
-                    return      
+                if elapsed < self.min_cache_flush_delay:
+                    return
             self.push_data(key)
 
-    def subsample(self, data):
-        normalized_max = int(self.__max_cache_quantity_per_second*self.min_cache_flush_delay)
-        if len(data)<=normalized_max:
+    def subsample(self, data: List[float]) -> List[float]:
+        normalized_max = int(self.__max_cache_quantity_per_second * self.min_cache_flush_delay)
+        if len(data) <= normalized_max:
             return data
-        else:
-            if self._warning_is_shown==False:
-                logger.warning(f"Your metrics rate ({len(data)//self.min_cache_flush_delay} metrics/second) is exceeding the maximum rate ({self.__max_cache_quantity_per_second}/second). Your metrics have been subsampled automatically.")
-                logger.warning("Consider reducing the number of metrics you push or setting an aggregation method with `run.set_metrics_aggr('mean')`.")
-                logger.warning("See the documentation for details https://docs.hectiq.ai/objects/metrics/.")
-                self._warning_is_shown = True
-            indexes = np.linspace(0, len(data)-1, normalized_max).astype(int)
-            return np.array(data)[indexes].tolist()
+        if self._warning_is_shown == False:
+            logger.warning(
+                f"Your metrics rate ({len(data)//self.min_cache_flush_delay} metrics/second) is exceeding the "
+                "maximum rate ({MetricsManager.__max_cache_quantity_per_second}/second). Your metrics have been "
+                "subsampled automatically."
+            )
+            logger.warning(
+                "Consider reducing the number of metrics you push or setting an aggregation method with "
+                "`run.set_metrics_aggr('mean')`."
+            )
+            logger.warning("See the documentation for details https://docs.hectiq.ai/objects/metrics/.")
+            self._warning_is_shown = True
+        indexes = np.linspace(0, len(data) - 1, normalized_max).astype(int)
+        return np.array(data)[indexes].tolist()
 
-    def push_data(self, key):
+    def push_data(self, key: str) -> None:
         self.cache_last_push[key] = time.time()
+        if self.push_method is None:
+            self.cache[key] = []
+            if self._warning_is_shown == False:
+                logger.warning(
+                    "No push method has been set. Please set a push method with `run.set_metrics_push_method`."
+                )
+            return
 
-        if self.aggregate_metrics=="none":
+        if self.aggregate_metrics == "none":
             data = self.subsample(self.cache[key])
             self.push_method(key, data)
-        elif self.aggregate_metrics=="mean":
+        elif self.aggregate_metrics == "mean":
             k = [_[0] for _ in self.cache[key]]
             s = [_[1] for _ in self.cache[key]]
             t = [_[2] for _ in self.cache[key]]
             if len(k) > 0:
                 self.push_method(key, [(float(np.max(k)), float(np.mean(s)), float(np.mean(s)))])
-        elif self.aggregate_metrics=="max":
+        elif self.aggregate_metrics == "max":
             k = [_[0] for _ in self.cache[key]]
             s = [_[1] for _ in self.cache[key]]
             t = [_[2] for _ in self.cache[key]]
             if len(k) > 0:
                 self.push_method(key, [(float(np.max(k)), float(np.max(s)), float(np.mean(s)))])
-        elif self.aggregate_metrics=="sum":
+        elif self.aggregate_metrics == "sum":
             k = [_[0] for _ in self.cache[key]]
             s = [_[1] for _ in self.cache[key]]
             t = [_[2] for _ in self.cache[key]]
             if len(k) > 0:
                 self.push_method(key, [(float(np.max(k)), float(np.sum(s)), float(np.mean(t)))])
         self.cache[key] = []
```

