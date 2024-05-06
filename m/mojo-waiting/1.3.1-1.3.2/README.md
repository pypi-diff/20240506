# Comparing `tmp/mojo_waiting-1.3.1.tar.gz` & `tmp/mojo_waiting-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_waiting-1.3.1.tar", max compression
+gzip compressed data, was "mojo_waiting-1.3.2.tar", max compression
```

## Comparing `mojo_waiting-1.3.1.tar` & `mojo_waiting-1.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:56:08.212782 mojo_waiting-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     4751 2024-01-26 02:56:08.212951 mojo_waiting-1.3.1/README.rst
--rw-r--r--   0        0        0      816 2024-04-24 03:52:13.742837 mojo_waiting-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      585 2024-01-26 02:56:08.214529 mojo_waiting-1.3.1/source/packages/mojo/waiting/__init__.py
--rw-r--r--   0        0        0      779 2024-01-26 02:56:08.214679 mojo_waiting-1.3.1/source/packages/mojo/waiting/constants.py
--rw-r--r--   0        0        0     3080 2024-01-26 02:56:08.214770 mojo_waiting-1.3.1/source/packages/mojo/waiting/waitfunction.py
--rw-r--r--   0        0        0     9208 2024-01-26 02:56:08.214876 mojo_waiting-1.3.1/source/packages/mojo/waiting/waitmodel.py
--rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 mojo_waiting-1.3.1/setup.py
--rw-r--r--   0        0        0     5555 1970-01-01 00:00:00.000000 mojo_waiting-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:56:08.212782 mojo_waiting-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     4751 2024-01-26 02:56:08.212951 mojo_waiting-1.3.2/README.rst
+-rw-r--r--   0        0        0      816 2024-05-06 00:01:01.429602 mojo_waiting-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-01-26 02:56:08.214529 mojo_waiting-1.3.2/source/packages/mojo/waiting/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-02 03:02:19.102016 mojo_waiting-1.3.2/source/packages/mojo/waiting/constants.py
+-rw-r--r--   0        0        0     2904 2024-05-02 03:02:19.102217 mojo_waiting-1.3.2/source/packages/mojo/waiting/waitfunction.py
+-rw-r--r--   0        0        0     8941 2024-05-02 03:02:19.102419 mojo_waiting-1.3.2/source/packages/mojo/waiting/waitmodel.py
+-rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 mojo_waiting-1.3.2/setup.py
+-rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 mojo_waiting-1.3.2/PKG-INFO
```

### Comparing `mojo_waiting-1.3.1/LICENSE.txt` & `mojo_waiting-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.3.1/README.rst` & `mojo_waiting-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.3.1/pyproject.toml` & `mojo_waiting-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-waiting"
 description = "Automation Mojo Waiting Module"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -17,15 +17,15 @@
 ]
 packages = [{ include="mojo", from = "source/packages" }]
 
 homepage = "http://automationmojo.com"
 repository = "https://github.com/automationmojo/mojo-waiting"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `mojo_waiting-1.3.1/source/packages/mojo/waiting/__init__.py` & `mojo_waiting-1.3.2/source/packages/mojo/waiting/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_waiting-1.3.1/source/packages/mojo/waiting/constants.py` & `mojo_waiting-1.3.2/source/packages/mojo/waiting/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 
 """
 .. module:: constants
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Module which contains the TimeoutContext object and very generic constants.
+    :synopsis: Module which contains the Timeout related constants.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
 
 
 DEFAULT_WAIT_DELAY = 0
 DEFAULT_WAIT_INTERVAL = 5
 DEFAULT_WAIT_TIMEOUT = 60
 
 MSG_TEMPL_TIME_COMPONENTS = "    timeout={} start_time={}, end_time={} now_time={} time_diff={}"
```

### Comparing `mojo_waiting-1.3.1/source/packages/mojo/waiting/waitfunction.py` & `mojo_waiting-1.3.2/source/packages/mojo/waiting/waitfunction.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Any, Dict, Optional
 
 import time
 
 
 from mojo.waiting.constants import (
```

### Comparing `mojo_waiting-1.3.1/source/packages/mojo/waiting/waitmodel.py` & `mojo_waiting-1.3.2/source/packages/mojo/waiting/waitmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 """
 .. module:: waitmodel
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Module which contains the object used in conjunction with waiting.
+    :synopsis: Module which contains objects used in conjunction with waiting.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
 
-from typing import Any, Dict, List, Optional, Protocol, Type
+
+from typing import List, Optional, Protocol, Type
 
 from types import TracebackType
 
 import os
 import threading
 import time
 
 from datetime import datetime, timedelta
 
 from mojo.waiting.constants import (
-    DEFAULT_WAIT_DELAY,
-    DEFAULT_WAIT_INTERVAL,
-    DEFAULT_WAIT_TIMEOUT,
     TimeoutState,
     MSG_TEMPL_TIME_COMPONENTS,
 )
 
 
 class TimeoutContext:
     """
```

### Comparing `mojo_waiting-1.3.1/setup.py` & `mojo_waiting-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['mojo', 'mojo.waiting']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-waiting',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'Automation Mojo Waiting Module',
     'long_description': '\n=============================================\nAutomation Mojo Waiting Module - mojo-waiting\n=============================================\n\nThis package provides support for enhanced context based waiting.  This module will greatly enhance the\ninformation presented when a wait timeout occurs.  Wait contexts are particularly useful for distributed\nautomation.  Distributed automation scenarios required lots of wait loops in order wait for the effects\nof an effect to distributed throughout the distributed system.\n\nThe waiting code patterns used are designed to present the best results in test stacktraces presented\nwhen a wait fails.  This makes the `mojo.waiting` module perfect for use with\ntest frameworks such as `pytest` and `testplus` that show code context in the error\nreport stack traces.\n\nAnother important aspect of the `mojo.waiting` module is that it uses `datetime`\ntimestamps and `timespan` for lengths of time so timeouts in error reporting are easier\nto interpret.\n\n.. code::\n\n    Traceback (most recent call last):\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 97, in test_basic_wait_for_it_timeout\n        future.result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 451, in result\n        return self.__get_result()\n    File "/usr/lib/python3.10/concurrent/futures/_base.py", line 403, in __get_result\n        raise self._exception\n    File "/usr/lib/python3.10/concurrent/futures/thread.py", line 58, in run\n        result = self.fn(*self.args, **self.kwargs)\n    File "/home/myron/repos/mojo.waiting/source/tests/test_wait_for_it.py", line 88, in wait_task\n        ctxwait.wait_for_it(wait_helper, interval=.5, timeout=2)\n    File "/home/myron/repos/mojo.waiting/source/packages/ctxwait/waiting.py", line 103, in wait_for_it\n        raise toerr\n    TimeoutError: Timeout waiting for \'wait_helper\':\n        timeout=2 start_time=2023-03-13 14:57:29.860302, end_time=2023-03-13 14:57:31.860302 now_time=2023-03-13 14:57:31.863681 time_diff=0:00:02.003379\n\n\nThe following is an example of how the `mojo.waiting` module is used.\n\n.. code:: python\n\n    from ctxwait import WaitContext, wait_for_it\n\n    def some_wait_helper(wctx: WaitContext):\n        finished = False\n\n        // TODO: Check if something is finished, the code and variables used\n        //       here will show up in any tracebacks from pytest or testplus\n        //       because the timeout is being raised in the appropriate scope.\n\n        if not finished and wctx.final_attempt:\n            whatfor = "Test timeout"\n            toerr = wctx.create_timeout(whatfor)\n            raise toerr\n\n        return finished\n\n    wait_for_it(some_wait_helper)\n\n\nThe `wait_for_it` method has many different parameters that can be used to override the\nbehavior of the wait loop.\n\n.. code:: python\n\n    def wait_for_it(looper: WaitCallback, *largs, what_for: Optional[str]=None, delay: float=DEFAULT_WAIT_DELAY,\n                interval: float=DEFAULT_WAIT_INTERVAL, timeout: float=DEFAULT_WAIT_TIMEOUT,\n                lkwargs: Dict[Any, Any]={}, wctx: Optional[WaitContext]=None):\n        """\n            Provides for convenient mechanism to wait for criteria to be met before proceeding.\n\n            :param looper: A callback method that is repeatedly called while it returns `False` up-to\n                        the end of a timeout period, and that will return `True` if a waited on\n                        condition is met prior to a timeout condition being met.\n            :param largs: Arguements to pass to the looper callback function.\n            :param what_for: A breif description of what is being waited for.\n            :param delay: An initial time delay to consume before beginning the waiting process.\n            :param interval: A period of time to delay between rechecks of the wait conditon\n            :param timeout: The maximum period of time in seconds that should be waited before timing out.\n            :param lkwargs: Additional keyword arguments to pass to the looper function\n\n            :raises TimeoutError: A timeout error with details around the wait condition.\n\n            ..note: The \'delay\', \'interval\' and \'timeout\' parameters will be ignored if the \'wctx\' parameter\n                    is passed as the wctx (WaitContext) parameter includes these values with it.\n        """\n        ...\n\nThe `wait_for_it` function must be passed a method that follows the `WaitCallback` protocol.  The function\ncan have variable arguments and keyword arguements but the first parameter to the `WaitCallback` method\nmust be a `WaitContext` object.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`_\n- `Coding Standards <userguide/10-00-coding-standards.rst>`_\n\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_waiting-1.3.1/PKG-INFO` & `mojo_waiting-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mojo-waiting
-Version: 1.3.1
+Version: 1.3.2
 Summary: Automation Mojo Waiting Module
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Project-URL: Repository, https://github.com/automationmojo/mojo-waiting
 Description-Content-Type: text/x-rst
```

