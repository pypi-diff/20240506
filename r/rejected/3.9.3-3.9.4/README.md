# Comparing `tmp/rejected-3.9.3.tar.gz` & `tmp/rejected-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rejected-3.9.3.tar", last modified: Thu Oct  8 19:38:29 2015, max compression
+gzip compressed data, was "dist/rejected-3.9.4.tar", last modified: Thu Oct 15 01:00:05 2015, max compression
```

## Comparing `rejected-3.9.3.tar` & `rejected-3.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-08 19:38:29.000000 rejected-3.9.3/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected/
--rw-rw-r--   0 travis    (1000) travis    (1000)      708 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    39449 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/consumer.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4020 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/controller.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2764 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/data.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      962 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/example.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1039 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/log.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    22689 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/mcp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1661 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/mixins.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    29909 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/process.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3323 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/state.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1815 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/stats.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2628 2015-10-08 19:37:49.000000 rejected-3.9.3/rejected/statsd.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     8706 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)      488 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       55 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       49 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        9 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-10-08 19:38:29.000000 rejected-3.9.3/rejected.egg-info/zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)     1501 2015-10-08 19:37:49.000000 rejected-3.9.3/LICENSE
--rw-rw-r--   0 travis    (1000) travis    (1000)       35 2015-10-08 19:37:49.000000 rejected-3.9.3/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     6399 2015-10-08 19:37:49.000000 rejected-3.9.3/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1634 2015-10-08 19:37:49.000000 rejected-3.9.3/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8706 2015-10-08 19:38:29.000000 rejected-3.9.3/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)       59 2015-10-08 19:38:29.000000 rejected-3.9.3/setup.cfg
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-15 01:00:05.000000 rejected-3.9.4/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      708 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    39607 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/consumer.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4020 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/controller.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2764 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/data.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      962 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/example.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1039 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/log.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    22689 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/mcp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1661 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/mixins.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    30079 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/process.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3323 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/state.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1815 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/stats.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2628 2015-10-15 00:59:25.000000 rejected-3.9.4/rejected/statsd.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8706 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)      488 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       55 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       49 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/requires.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        9 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2015-10-15 01:00:05.000000 rejected-3.9.4/rejected.egg-info/zip-safe
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1501 2015-10-15 00:59:25.000000 rejected-3.9.4/LICENSE
+-rw-rw-r--   0 travis    (1000) travis    (1000)       35 2015-10-15 00:59:25.000000 rejected-3.9.4/MANIFEST.in
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6399 2015-10-15 00:59:25.000000 rejected-3.9.4/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1634 2015-10-15 00:59:25.000000 rejected-3.9.4/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8706 2015-10-15 01:00:05.000000 rejected-3.9.4/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)       59 2015-10-15 01:00:05.000000 rejected-3.9.4/setup.cfg
```

### Comparing `rejected-3.9.3/rejected/__init__.py` & `rejected-3.9.4/rejected/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Rejected is a Python RabbitMQ Consumer Framework and Controller Daemon
 
 """
 __author__ = 'Gavin M. Roy <gavinmroy@gmail.com>'
 __since__ = "2009-09-10"
-__version__ = "3.9.3"
+__version__ = "3.9.4"
 
 import logging
 try:
     # not available in python 2.6
     from logging import NullHandler
 except ImportError:
```

### Comparing `rejected-3.9.3/rejected/consumer.py` & `rejected-3.9.4/rejected/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,17 @@
         self._settings = settings
         self._statsd = None
         self._yield_condition = locks.Condition()
 
         # Create a logger that attaches correlation ID to the record
         self.logger = log.CorrelationAdapter(LOGGER, self)
 
+        # Set a Sentry context for the consumer
+        self.set_sentry_context('consumer', self.name)
+
         # Run any child object specified initialization
         self.initialize()
 
     def initialize(self):
         """Extend this method for any initialization tasks that occur only when
         the `Consumer` class is created."""
         pass
@@ -481,26 +484,26 @@
         """
         if not self._message:
             return None
         return self._message.properties.user_id
 
     @property
     def sentry_client(self):
-        """
-        Access the raven ``Client`` instance or ``None``
-
-        :rtype: :class:`raven.base.Client`
+        """Access the Sentry raven ``Client`` instance or ``None``
 
         Use this object to add tags or additional context to Sentry
         error reports (see :meth:`raven.base.Client.tags_context`) or
         to report messages (via :meth:`raven.base.Client.captureMessage`)
         directly to Sentry.
 
+        :rtype: :class:`raven.base.Client`
+
         """
-        return self._process.sentry_client
+        if hasattr(self._process, 'sentry_client'):
+            return self._process.sentry_client
 
     def _clear(self):
         """Resets all assigned data for the current message."""
         self._finished = False
         self._message = None
         self._message_body = None
```

### Comparing `rejected-3.9.3/rejected/controller.py` & `rejected-3.9.4/rejected/controller.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/data.py` & `rejected-3.9.4/rejected/data.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/example.py` & `rejected-3.9.4/rejected/example.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/log.py` & `rejected-3.9.4/rejected/log.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/mcp.py` & `rejected-3.9.4/rejected/mcp.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/mixins.py` & `rejected-3.9.4/rejected/mixins.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/process.py` & `rejected-3.9.4/rejected/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,21 @@
     :return: tuple(Class, str)
 
     """
 
     parts = value.split('.')
     import_name = '.'.join(parts[0:-1])
     import_handle = importlib.import_module(import_name)
+    version = None
     if hasattr(import_handle, '__version__'):
         version = import_handle.__version__
-    else:
-        version = None
+    elif len(parts) > 2:
+        package_handle = importlib.import_module(parts[0])
+        if hasattr(package_handle, '__version__'):
+            version = package_handle.__version__
 
     # Return the class handle
     return getattr(import_handle, parts[-1]), version
 
 
 class Process(multiprocessing.Process, state.State):
     """Core process class that manages the consumer object and communicates
```

### Comparing `rejected-3.9.3/rejected/state.py` & `rejected-3.9.4/rejected/state.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/stats.py` & `rejected-3.9.4/rejected/stats.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected/statsd.py` & `rejected-3.9.4/rejected/statsd.py`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/rejected.egg-info/PKG-INFO` & `rejected-3.9.4/rejected.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rejected
-Version: 3.9.3
+Version: 3.9.4
 Summary: Rejected is a Python RabbitMQ Consumer Framework and Controller Daemon
 Home-page: https://github.com/gmr/rejected
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD
 Description: Rejected
         ========
```

### Comparing `rejected-3.9.3/LICENSE` & `rejected-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/README.rst` & `rejected-3.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `rejected-3.9.3/setup.py` & `rejected-3.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                   'msgpack': ['msgpack-python']}
 
 if sys.version_info < (2, 7, 0):
     install_requires.append('backport_collections')
     install_requires.append('importlib')
 
 setup(name='rejected',
-      version='3.9.3',
+      version='3.9.4',
       description='Rejected is a Python RabbitMQ Consumer Framework and '
                   'Controller Daemon',
       long_description=open('README.rst').read(),
       classifiers=classifiers,
       keywords='amqp rabbitmq',
       author='Gavin M. Roy',
       author_email='gavinmroy@gmail.com',
```

### Comparing `rejected-3.9.3/PKG-INFO` & `rejected-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rejected
-Version: 3.9.3
+Version: 3.9.4
 Summary: Rejected is a Python RabbitMQ Consumer Framework and Controller Daemon
 Home-page: https://github.com/gmr/rejected
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD
 Description: Rejected
         ========
```

