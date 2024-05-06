# Comparing `tmp/state-machine-2-0.2.2.tar.gz` & `tmp/state-machine-2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state-machine-2-0.2.2.tar", last modified: Tue Mar 26 15:31:15 2024, max compression
+gzip compressed data, was "state-machine-2-0.2.4.tar", last modified: Mon May  6 14:39:59 2024, max compression
```

## Comparing `state-machine-2-0.2.2.tar` & `state-machine-2-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-03-26 15:31:15.769056 state-machine-2-0.2.2/
--rw-r--r--   0 wangx     (1000) wangx     (1000)    35149 2021-01-17 09:43:10.000000 state-machine-2-0.2.2/LICENSE
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1560 2024-03-26 15:31:15.769056 state-machine-2-0.2.2/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1217 2021-01-20 14:22:40.000000 state-machine-2-0.2.2/README.md
--rw-r--r--   0 wangx     (1000) wangx     (1000)       38 2024-03-26 15:31:15.769056 state-machine-2-0.2.2/setup.cfg
--rw-r--r--   0 wangx     (1000) wangx     (1000)      770 2024-03-26 15:30:52.000000 state-machine-2-0.2.2/setup.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-03-26 15:31:15.769056 state-machine-2-0.2.2/state_machine/
--rw-r--r--   0 wangx     (1000) wangx     (1000)      235 2021-01-17 09:43:10.000000 state-machine-2-0.2.2/state_machine/__init__.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1807 2023-11-08 11:51:31.000000 state-machine-2-0.2.2/state_machine/backends.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)      265 2021-01-17 09:43:10.000000 state-machine-2-0.2.2/state_machine/base.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1734 2021-01-20 13:16:23.000000 state-machine-2-0.2.2/state_machine/core.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)      605 2024-01-24 14:45:47.000000 state-machine-2-0.2.2/state_machine/exceptions.py
--rw-r--r--   0 wangx     (1000) wangx     (1000)        0 2024-03-26 15:27:23.000000 state-machine-2-0.2.2/state_machine/py.typed
--rw-r--r--   0 wangx     (1000) wangx     (1000)      878 2024-01-24 14:45:47.000000 state-machine-2-0.2.2/state_machine/utils.py
-drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-03-26 15:31:15.769056 state-machine-2-0.2.2/state_machine_2.egg-info/
--rw-r--r--   0 wangx     (1000) wangx     (1000)     1560 2024-03-26 15:31:15.000000 state-machine-2-0.2.2/state_machine_2.egg-info/PKG-INFO
--rw-r--r--   0 wangx     (1000) wangx     (1000)      390 2024-03-26 15:31:15.000000 state-machine-2-0.2.2/state_machine_2.egg-info/SOURCES.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2024-03-26 15:31:15.000000 state-machine-2-0.2.2/state_machine_2.egg-info/dependency_links.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)        6 2024-03-26 15:31:15.000000 state-machine-2-0.2.2/state_machine_2.egg-info/requires.txt
--rw-r--r--   0 wangx     (1000) wangx     (1000)       14 2024-03-26 15:31:15.000000 state-machine-2-0.2.2/state_machine_2.egg-info/top_level.txt
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-05-06 14:39:59.371546 state-machine-2-0.2.4/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)    35149 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/LICENSE
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1669 2024-05-06 14:39:59.371546 state-machine-2-0.2.4/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1289 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/README.md
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       38 2024-05-06 14:39:59.371546 state-machine-2-0.2.4/setup.cfg
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      770 2024-05-06 14:39:05.000000 state-machine-2-0.2.4/setup.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-05-06 14:39:59.371546 state-machine-2-0.2.4/state_machine/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      235 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/__init__.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1827 2024-05-06 14:38:48.000000 state-machine-2-0.2.4/state_machine/backends.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      265 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/base.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1871 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/core.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      605 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/exceptions.py
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        0 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/py.typed
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      927 2024-05-06 14:38:08.000000 state-machine-2-0.2.4/state_machine/utils.py
+drwxr-xr-x   0 wangx     (1000) wangx     (1000)        0 2024-05-06 14:39:59.371546 state-machine-2-0.2.4/state_machine_2.egg-info/
+-rw-r--r--   0 wangx     (1000) wangx     (1000)     1669 2024-05-06 14:39:59.000000 state-machine-2-0.2.4/state_machine_2.egg-info/PKG-INFO
+-rw-r--r--   0 wangx     (1000) wangx     (1000)      390 2024-05-06 14:39:59.000000 state-machine-2-0.2.4/state_machine_2.egg-info/SOURCES.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        1 2024-05-06 14:39:59.000000 state-machine-2-0.2.4/state_machine_2.egg-info/dependency_links.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)        6 2024-05-06 14:39:59.000000 state-machine-2-0.2.4/state_machine_2.egg-info/requires.txt
+-rw-r--r--   0 wangx     (1000) wangx     (1000)       14 2024-05-06 14:39:59.000000 state-machine-2-0.2.4/state_machine_2.egg-info/top_level.txt
```

### Comparing `state-machine-2-0.2.2/LICENSE` & `state-machine-2-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `state-machine-2-0.2.2/PKG-INFO` & `state-machine-2-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: state-machine-2
-Version: 0.2.2
+Version: 0.2.4
 Summary: a state machine that support multi process
 Home-page: https://github.com/ramwin/state-machine
 Author: Xiang Wang
 Author-email: ramwin@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # state-machine
+[documentation](https://state-machine.readthedocs.io/en/latest/)  
 a state machine that can change difference backends (current only redis backend, lately the filelockbackend)  
 and keep state synchronously in different state even different host.
 
 # Install
 ```
 sudo pip3 install state-machine-2
 ```
 
-# Usage
+# Quick Start
 1. Create a State Backend
 ```
 from state_machine import StateMachine, RedisBackend
 from redis import Redis
 # you will need to install redis
 # see more information here: https://redis.io/download#installation
 redis_backend = RedisBackend(con=Redis(decode_responses=True))
@@ -50,11 +53,13 @@
 >>> job1_1.state = "STARTED"
 Error: StateChangedException() # raise Exception because the state has changed by job1_0
 ```
 
 # test and contribute
 ```
 git clone git@github.com:ramwin/state-machine.git
+cd state-machine
 pip3 install -e ./
-cd tests
-python3 __init__.py
+sh test.sh
 ```
+
+
```

### Comparing `state-machine-2-0.2.2/README.md` & `state-machine-2-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # state-machine
+[documentation](https://state-machine.readthedocs.io/en/latest/)  
 a state machine that can change difference backends (current only redis backend, lately the filelockbackend)  
 and keep state synchronously in different state even different host.
 
 # Install
 ```
 sudo pip3 install state-machine-2
 ```
 
-# Usage
+# Quick Start
 1. Create a State Backend
 ```
 from state_machine import StateMachine, RedisBackend
 from redis import Redis
 # you will need to install redis
 # see more information here: https://redis.io/download#installation
 redis_backend = RedisBackend(con=Redis(decode_responses=True))
@@ -38,11 +39,11 @@
 >>> job1_1.state = "STARTED"
 Error: StateChangedException() # raise Exception because the state has changed by job1_0
 ```
 
 # test and contribute
 ```
 git clone git@github.com:ramwin/state-machine.git
+cd state-machine
 pip3 install -e ./
-cd tests
-python3 __init__.py
+sh test.sh
 ```
```

### Comparing `state-machine-2-0.2.2/setup.py` & `state-machine-2-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "state-machine-2",
-    version = "0.2.2",
+    version = "0.2.4",
     author="Xiang Wang",
     author_email="ramwin@qq.com",
     description="a state machine that support multi process",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ramwin/state-machine",
     packages=["state_machine"],
```

### Comparing `state-machine-2-0.2.2/state_machine/backends.py` & `state-machine-2-0.2.4/state_machine/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,22 @@
             self.expired(your_state=default, remote_state=latest_state)
         return latest_state
 
     def get_remote_state(self, backend_key):
         state_key = f"state_machine:state:{backend_key}"
         return self.con.get(state_key)
 
-    def change_state(self, backend_key, from_state, to_state):
+    def change_state(self, backend_key, from_state, to_state) -> bool:
         """
         return True if success
         raise Exception if fail
         """
         lock_key = f"state_machine:lock:{backend_key}"
         state_key = f"state_machine:state:{backend_key}"
-        lock = self.con.lock(lock_key)
+        lock = self.con.lock(lock_key, timeout=10)
         if not lock.acquire(blocking=False):
             return self.block()
         remote_state = self.get_state(backend_key, from_state)
         if remote_state != from_state:
             return self.expired(your_state=from_state, remote_state=remote_state)
         self.con.set(state_key, to_state)
         lock.release()
```

### Comparing `state-machine-2-0.2.2/state_machine/core.py` & `state-machine-2-0.2.4/state_machine/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # Xiang Wang @ 2021-01-16 10:30:34
 
 
 import logging
 
 from . import exceptions
-from .backends import RedisBackend
+from .backends import BaseBackend, RedisBackend
 from .base import Event
 
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 
 
@@ -28,15 +28,18 @@
         #                 raise exceptions.StateUnexcepedException
         #             log.info(Event)
         #         setattr(new_class, "save_" + key, event_function)
         return new_class
 
 
 class StateMachine(metaclass=StateMachineMetaClass):
-    backend = None
+    """
+    A StateMachine can safely change the state of an object without worrying changed by other process
+    """
+    backend: BaseBackend
     _state = None
     state_key = "state"
 
     def __init__(self, *args, **kwargs):
         if self.backend is None:
             raise Exception("please add backend=RedisBackend() in your StateMachine")
         state_value = kwargs.pop(self.state_key)
```

### Comparing `state-machine-2-0.2.2/state_machine/exceptions.py` & `state-machine-2-0.2.4/state_machine/exceptions.py`

 * *Files identical despite different names*

### Comparing `state-machine-2-0.2.2/state_machine/utils.py` & `state-machine-2-0.2.4/state_machine/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     has_error = False
     for item in items:
         origin_state[item.backend_key] = item.state
         try:
             item.state = target_state
         except StateMachineBaseException:
             has_error = True
+            # del origin_state[item.backend_key]
             break
     if has_error:
         for item in items:
             if item.backend_key in origin_state:
                 item.state = origin_state.pop(item.backend_key)
         return False
     return True
```

### Comparing `state-machine-2-0.2.2/state_machine_2.egg-info/PKG-INFO` & `state-machine-2-0.2.4/state_machine_2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: state-machine-2
-Version: 0.2.2
+Version: 0.2.4
 Summary: a state machine that support multi process
 Home-page: https://github.com/ramwin/state-machine
 Author: Xiang Wang
 Author-email: ramwin@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # state-machine
+[documentation](https://state-machine.readthedocs.io/en/latest/)  
 a state machine that can change difference backends (current only redis backend, lately the filelockbackend)  
 and keep state synchronously in different state even different host.
 
 # Install
 ```
 sudo pip3 install state-machine-2
 ```
 
-# Usage
+# Quick Start
 1. Create a State Backend
 ```
 from state_machine import StateMachine, RedisBackend
 from redis import Redis
 # you will need to install redis
 # see more information here: https://redis.io/download#installation
 redis_backend = RedisBackend(con=Redis(decode_responses=True))
@@ -50,11 +53,13 @@
 >>> job1_1.state = "STARTED"
 Error: StateChangedException() # raise Exception because the state has changed by job1_0
 ```
 
 # test and contribute
 ```
 git clone git@github.com:ramwin/state-machine.git
+cd state-machine
 pip3 install -e ./
-cd tests
-python3 __init__.py
+sh test.sh
 ```
+
+
```

