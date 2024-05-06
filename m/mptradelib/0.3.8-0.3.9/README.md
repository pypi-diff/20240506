# Comparing `tmp/mptradelib-0.3.8.tar.gz` & `tmp/mptradelib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.3.8.tar", max compression
+gzip compressed data, was "mptradelib-0.3.9.tar", max compression
```

## Comparing `mptradelib-0.3.8.tar` & `mptradelib-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.8/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.8/mptradelib/__init__.py
--rw-r--r--   0        0        0     4582 2024-05-04 11:45:49.548705 mptradelib-0.3.8/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.8/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.8/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.8/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.8/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.8/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2338 2024-05-04 09:41:29.250845 mptradelib-0.3.8/mptradelib/cli/new.py
--rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.8/mptradelib/feed.py
--rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.8/mptradelib/livetrade.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.8/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.8/mptradelib/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.3.8/mptradelib/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.8/mptradelib/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.8/mptradelib/test_renko.py
--rw-r--r--   0        0        0     2767 2024-05-04 12:41:24.598195 mptradelib-0.3.8/mptradelib/utils.py
--rw-r--r--   0        0        0      829 2024-05-04 12:42:41.512229 mptradelib-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.9/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4662 2024-05-05 15:13:06.736697 mptradelib-0.3.9/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.9/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5853 2024-05-05 15:12:34.719178 mptradelib-0.3.9/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.9/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.9/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.3.9/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2338 2024-05-04 09:41:29.250845 mptradelib-0.3.9/mptradelib/cli/new.py
+-rw-r--r--   0        0        0     4054 2024-05-03 03:52:00.848935 mptradelib-0.3.9/mptradelib/feed.py
+-rw-r--r--   0        0        0     1864 2024-05-03 09:17:03.492902 mptradelib-0.3.9/mptradelib/livetrade.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.9/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1097 2024-05-03 13:03:10.480806 mptradelib-0.3.9/mptradelib/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.3.9/mptradelib/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.3.9/mptradelib/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.9/mptradelib/test_renko.py
+-rw-r--r--   0        0        0     2767 2024-05-04 12:41:24.598195 mptradelib-0.3.9/mptradelib/utils.py
+-rw-r--r--   0        0        0      829 2024-05-05 17:14:03.977551 mptradelib-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 mptradelib-0.3.9/PKG-INFO
```

### Comparing `mptradelib-0.3.8/README.md` & `mptradelib-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/backtest.py` & `mptradelib-0.3.9/mptradelib/backtest.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 import numpy as np
 from dataclasses import dataclass, asdict
 from typing import Callable
 from tqdm import tqdm
 from hyperopt import fmin, tpe, hp, STATUS_OK
 from hyperopt.pyll import scope
+from retry import retry
 
 position = None
 orders = []
 
 @dataclass
 class Order:
     entry_time: dt.datetime
@@ -104,26 +105,28 @@
                 space[k] = scope.int(hp.quniform(k, v.start, v.stop, v.step))
             elif isinstance(v.step, float):
                 space[k] = hp.quniform(k, v.start, v.stop, v.step)
             else:
                 raise ValueError(f"step of {k} can not be {type(v.step)}")
         return space
 
+    @retry(tries=10)
     def _optimizer(self, **kwargs):
         space = self._define_space(kwargs)
         
         def objective(params):
             r = self.run(**params)
             return {'loss': -np.sum(r[0].profit), 'status': STATUS_OK}
         
         best = fmin(
             fn=objective,
             space=space,
             algo=tpe.suggest,
             max_evals=100,
+            show_progressbar=False
         )
         p = {k: int(v) for k, v in best.items()}
         r = self.run(**p)
         return best, np.sum(r[0].profit)
     
     def optimize(self, runs=5, **kwargs):
         results = []
```

### Comparing `mptradelib-0.3.8/mptradelib/broker/broker.py` & `mptradelib-0.3.9/mptradelib/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import datetime as dt
 
 try:
     import pandas as pd
 except ImportError:
     pass
 
-import os
+from retry import retry
 from .. import utils
 from .session import FyersSession, ShoonyaSession
 from ..shoonya import *
 from pydantic import BaseModel, Field
 
 
 class Historical:
     def __init__(self, session: FyersSession) -> None:
         self._session = session
         self._client = None
 
+    @retry(tries=5, delay=2)
     def historical(self, symbol, resolution, start, end):
         curr = start
         delta = dt.timedelta(days=100)
         final_data = []
         if self._client is None:
             self._client = self._session.init_client()
         
@@ -31,15 +32,18 @@
                 "date_format": "1",
                 "range_from": f'{curr:%Y-%m-%d}',
                 "range_to": f'{(curr + delta):%Y-%m-%d}',
                 "cont_flag": "1",
             }
             
             data = self._client.history(data=payload)
-            final_data += data["candles"]
+            try:
+                final_data += data["candles"]
+            except IndexError as e:
+                continue
             curr += delta + dt.timedelta(days=1)
         df = pd.DataFrame(final_data, columns=["datetime", "open", "high", "low", "close", "volume"])
         df.index = pd.to_datetime(df["datetime"], unit="s", utc=True)
         df.index = df.index.tz_convert("Asia/Kolkata")
         df.datetime = df.index
         df = df.sort_index()
         return df
```

### Comparing `mptradelib-0.3.8/mptradelib/broker/session.py` & `mptradelib-0.3.9/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/broker/ticker.py` & `mptradelib-0.3.9/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/cli/new.py` & `mptradelib-0.3.9/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/feed.py` & `mptradelib-0.3.9/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/livetrade.py` & `mptradelib-0.3.9/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/shoonya.py` & `mptradelib-0.3.9/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/templates/strategy/__init__.py.jinja` & `mptradelib-0.3.9/mptradelib/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.3.9/mptradelib/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/templates/strategy/livetrade.py.jinja` & `mptradelib-0.3.9/mptradelib/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/test_renko.py` & `mptradelib-0.3.9/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/mptradelib/utils.py` & `mptradelib-0.3.9/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.3.8/pyproject.toml` & `mptradelib-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.3.8/PKG-INFO` & `mptradelib-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

