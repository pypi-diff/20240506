# Comparing `tmp/queue_app_provider-0.1.tar.gz` & `tmp/queue_app_provider-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_app_provider-0.1.tar", last modified: Thu Apr  4 19:42:35 2024, max compression
+gzip compressed data, was "queue_app_provider-0.2.tar", last modified: Mon May  6 17:58:10 2024, max compression
```

## Comparing `queue_app_provider-0.1.tar` & `queue_app_provider-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-04-04 19:42:35.266704 queue_app_provider-0.1/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      822 2024-04-04 19:42:35.266882 queue_app_provider-0.1/PKG-INFO
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1978 2023-06-05 14:48:05.799242 queue_app_provider-0.1/README
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-04-04 19:42:35.264724 queue_app_provider-0.1/queue_app_provider/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2937 2023-06-02 09:51:06.498136 queue_app_provider-0.1/queue_app_provider/AppProvider.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1769 2023-06-02 09:26:36.183251 queue_app_provider-0.1/queue_app_provider/HandlerOutput.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1320 2023-06-05 14:48:05.799429 queue_app_provider-0.1/queue_app_provider/InputEntry.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2032 2023-06-02 09:35:07.701698 queue_app_provider-0.1/queue_app_provider/QueueThread.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      189 2024-04-04 19:16:40.600584 queue_app_provider-0.1/queue_app_provider/__init__.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)       39 2024-04-04 19:22:08.004721 queue_app_provider-0.1/setup.cfg
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1686 2024-04-04 19:42:16.897474 queue_app_provider-0.1/setup.py
-drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-04-04 19:42:35.266626 queue_app_provider-0.1/test/
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2485 2023-06-06 11:38:00.287220 queue_app_provider-0.1/test/test_AppProviderTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1468 2023-06-05 14:48:05.799708 queue_app_provider-0.1/test/test_HandlerOutputTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1346 2023-06-05 14:48:05.799807 queue_app_provider-0.1/test/test_InputEntryTest.py
--rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1386 2023-06-05 14:48:05.799872 queue_app_provider-0.1/test/test_QueueThreadTest.py
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.812460 queue_app_provider-0.2/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      822 2024-05-06 17:58:10.812597 queue_app_provider-0.2/PKG-INFO
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1978 2023-06-05 14:48:05.799242 queue_app_provider-0.2/README
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.810747 queue_app_provider-0.2/queue_app_provider/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2937 2023-06-02 09:51:06.498136 queue_app_provider-0.2/queue_app_provider/AppProvider.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1967 2024-05-06 17:39:44.760644 queue_app_provider-0.2/queue_app_provider/HandlerOutput.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1440 2024-05-06 17:48:37.443999 queue_app_provider-0.2/queue_app_provider/InputEntry.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2087 2024-05-06 17:31:07.272714 queue_app_provider-0.2/queue_app_provider/QueueThread.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)      189 2024-04-04 19:16:40.600584 queue_app_provider-0.2/queue_app_provider/__init__.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)       39 2024-04-04 19:22:08.004721 queue_app_provider-0.2/setup.cfg
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1686 2024-05-06 17:52:29.378428 queue_app_provider-0.2/setup.py
+drwxr-xr-x   0 davidrodriguezalfayate   (501) staff       (20)        0 2024-05-06 17:58:10.812394 queue_app_provider-0.2/test/
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     2485 2023-06-06 11:38:00.287220 queue_app_provider-0.2/test/test_AppProviderTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1468 2023-06-05 14:48:05.799708 queue_app_provider-0.2/test/test_HandlerOutputTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1346 2023-06-05 14:48:05.799807 queue_app_provider-0.2/test/test_InputEntryTest.py
+-rw-r--r--   0 davidrodriguezalfayate   (501) staff       (20)     1386 2023-06-05 14:48:05.799872 queue_app_provider-0.2/test/test_QueueThreadTest.py
```

### Comparing `queue_app_provider-0.1/PKG-INFO` & `queue_app_provider-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: queue_app_provider
-Version: 0.1
+Version: 0.2
 Summary: Simple backend processor that receives binary data and stores it in a queue that its processed in a background thread.
 Home-page: https://github.com/drodriguezalfayate/flask-binary-queue/
 Author: David Rodriguez Alfayate
 Author-email: david.rodriguez.alfayate@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: QUEUE BACKGROUND PROCESSOR
```

### Comparing `queue_app_provider-0.1/README` & `queue_app_provider-0.2/README`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.1/queue_app_provider/AppProvider.py` & `queue_app_provider-0.2/queue_app_provider/AppProvider.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.1/queue_app_provider/HandlerOutput.py` & `queue_app_provider-0.2/queue_app_provider/HandlerOutput.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 
 import requests
 
+logger = logging.getLogger('HandlerOutput')
+
 
 # This class is a holder for all information regarding the processing
 # of a handler, a handler is the function accountable of working on
 # a image or binary data to create proper output.
 #
 # It's just a wrapper of a `success` a `text` or a `file` if the
 # output of processor is a file.
@@ -18,27 +20,29 @@
 # Version: 1.0
 class HandlerOutput:
     def __init__(self, success: bool, text: str, file=""):
         self.success = success
         self.file = file
         self.text = text
 
-    # As stated above the notify method receives the callback url, and according this
+    # As stated above the notify method receives the callback url, and according to its
     # object internal state it sends the proper response to the origin.
     def notify(self, callback: str):
         try:
             # On fail
             if not self.success:
+                logger.debug('Sending fail message %s to % endpoint', self.text, callback)
                 requests.post(callback, json={"success": False, "error": self.text})
                 return
             # On success, but a file
             if self.file:
+                logger.debug('Sending success file to % endpoint', callback)
                 requests.post(callback, json={"success": True}, files={'file': open(self.file, 'rb')})
                 return
             # Normal text
             requests.post(callback, json={"success": True, "data": self.text})
-        except requests.exceptions.RequestException:
+        except requests.exceptions.RequestException as e:
             # In a more complex scenario we should, perhaps, enqueue this callback response, expecting
             # than in the near future the remote server could be up again. For this simple example,
             # we are just ignoring the request, logging the error event
-            logging.exception('There was an error sending callback')
+            logger.exception(e, exc_info=True)
             return
```

### Comparing `queue_app_provider-0.1/queue_app_provider/InputEntry.py` & `queue_app_provider-0.2/queue_app_provider/InputEntry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import os
 import tempfile
 from typing import Callable
 
 from werkzeug.datastructures import FileStorage
 
-
 # Very simple class, an InputEntry is just a holder for queue entries in our
 # processing system.
 #
 # Since we are working with files, this InputEntry receives a `FileStorage`
 # object from the flask request, and dumps original file object to
 # a local file. When queue process this entry, handler is called and
 # after that the local file is purged from system
 #
 # Created by: David Rodríguez Alfayate
 # Version: 1.0
 from queue_app_provider.HandlerOutput import HandlerOutput
+import logging
+
+logger = logging.getLogger('InputEntry')
 
 
 class InputEntry:
     def __init__(self, file_storage: FileStorage, callback):
         self.callback = callback
         self.fh, self.file = tempfile.mkstemp()
+        logger.debug('Storing temporary file in %s', self.file)
         file_storage.save(self.file)
 
     # Temporary file removal
     def clear(self):
         os.close(self.fh)
         os.remove(self.file)
```

### Comparing `queue_app_provider-0.1/queue_app_provider/QueueThread.py` & `queue_app_provider-0.2/queue_app_provider/QueueThread.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 # Queue is stopped using provided event_handler
 #
 # Created by: David Rodríguez Alfayate
 # Version: 1.0
 from typing import Callable
 
 from queue_app_provider.HandlerOutput import HandlerOutput
+import logging
+
+logger = logging.getLogger('QueueThread')
 
 
 class QueueThread(threading.Thread):
     def __init__(self, handler: Callable[[str], HandlerOutput], shared_queue: queue.Queue,
                  event_handler: threading.Event, timeout=30):
         threading.Thread.__init__(self)
         self.handler = handler
         self.queue = shared_queue
         self.event_handler = event_handler
         self.timeout = timeout
 
     def run(self):
-        logging.debug("Starting main queue processor")
+        logger.debug("Starting main queue processor")
         while True:
             # Very simple logic, we are just reading the queue in a non-blocking way,
             # therefore if queue is not empty we recover last entry and process it
             # in any other case we wait (sleep) for a 'timeout' number of seconds.
             #
             # Since we need to stop thread, we are also listening on event_handler,
             # if it's set, processing is stopped and this thread "dies" gracefully
@@ -37,16 +40,16 @@
                 if self.event_handler.is_set():
                     global_break = True
                     break
                 entry = self.queue.get_nowait()
                 entry.handle(self.handler)
 
             if global_break:
-                logging.debug("Breaking thread due to user interrupt")
+                logger.debug("Breaking thread due to user interrupt")
                 break
 
             # As stated above we wait til handler is set or timeout is exceded,
             # if timeout is exceded we continue with normal workflow, that is
             # run forever ;)
             if self.event_handler.wait(timeout=self.timeout):
-                logging.debug("Breaking thread due to user interrupt")
+                logger.debug("Breaking thread due to user interrupt")
                 break
```

### Comparing `queue_app_provider-0.1/setup.py` & `queue_app_provider-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='queue_app_provider',  # How you named your package folder (MyLib)
     packages=['queue_app_provider'],  # Chose the same as "name"
-    version='0.1',  # Start with a small number and increase it with every change you make
+    version='0.2',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Simple backend processor that receives binary data and stores it in a queue that it''s processed in '
                 'a background thread.',  # Give a short description about your library
     author='David Rodriguez Alfayate',  # Type in your name
     author_email='david.rodriguez.alfayate@gmail.com',  # Type in your E-Mail
     url='https://github.com/drodriguezalfayate/flask-binary-queue/',  # Provide either the link to your github or to your website
     keywords=['QUEUE BACKGROUND PROCESSOR'],  # Keywords that define your package best
```

### Comparing `queue_app_provider-0.1/test/test_AppProviderTest.py` & `queue_app_provider-0.2/test/test_AppProviderTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.1/test/test_HandlerOutputTest.py` & `queue_app_provider-0.2/test/test_HandlerOutputTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.1/test/test_InputEntryTest.py` & `queue_app_provider-0.2/test/test_InputEntryTest.py`

 * *Files identical despite different names*

### Comparing `queue_app_provider-0.1/test/test_QueueThreadTest.py` & `queue_app_provider-0.2/test/test_QueueThreadTest.py`

 * *Files identical despite different names*

