# Comparing `tmp/decoutilities-0.2.0.tar.gz` & `tmp/decoutilities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.0.tar", last modified: Tue Apr 30 13:17:34 2024, max compression
+gzip compressed data, was "decoutilities-0.2.1.tar", last modified: Mon May  6 07:13:56 2024, max compression
```

## Comparing `decoutilities-0.2.0.tar` & `decoutilities-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:34.681937 decoutilities-0.2.0/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     9043 2024-04-30 13:17:34.651937 decoutilities-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8572 2024-04-30 13:10:29.000000 decoutilities-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:34.379302 decoutilities-0.2.0/decoutilities/
--rw-rw-rw-   0        0        0     4572 2024-04-30 13:10:46.000000 decoutilities-0.2.0/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:34.537937 decoutilities-0.2.0/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.0/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.0/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.0/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:34.595937 decoutilities-0.2.0/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.0/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.0/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-04-30 13:17:34.613937 decoutilities-0.2.0/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     9043 2024-04-30 13:17:33.000000 decoutilities-0.2.0/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-30 13:17:33.000000 decoutilities-0.2.0/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 13:17:33.000000 decoutilities-0.2.0/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-30 13:17:33.000000 decoutilities-0.2.0/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 13:17:34.682937 decoutilities-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-04-30 13:16:41.000000 decoutilities-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.443682 decoutilities-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     9043 2024-05-06 07:13:56.427681 decoutilities-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8572 2024-04-30 13:10:29.000000 decoutilities-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.137611 decoutilities-0.2.1/decoutilities/
+-rw-rw-rw-   0        0        0     4791 2024-05-06 07:06:49.000000 decoutilities-0.2.1/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.327106 decoutilities-0.2.1/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.1/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.1/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.1/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.398679 decoutilities-0.2.1/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.1/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.1/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:13:56.409681 decoutilities-0.2.1/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     9043 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-06 07:13:55.000000 decoutilities-0.2.1/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:13:56.443682 decoutilities-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-06 07:09:43.000000 decoutilities-0.2.1/setup.py
```

### Comparing `decoutilities-0.2.0/LICENSE` & `decoutilities-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.0/PKG-INFO` & `decoutilities-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.0/README.md` & `decoutilities-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.0/decoutilities/__init__.py` & `decoutilities-0.2.1/decoutilities/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,27 +100,35 @@
             time.sleep(seconds)
             return func(*args, **kwargs)
         return wrapper
     return decorator
 
 # @timeout(seconds)
 # Timeout a function after a number of seconds.
-def timeout(seconds):
-    import signal
+from threading import Thread
+import time
+
+class TimeoutException(Exception):
+    pass
 
+def timeout(seconds):
     def decorator(func):
         def wrapper(*args, **kwargs):
-            def handler(signum, frame):
-                raise Exception("Function timed out!")
-
-            signal.signal(signal.SIGALRM, handler)
-            signal.alarm(seconds)
-            result = func(*args, **kwargs)
-            signal.alarm(0)
-            return result
+            res = [TimeoutException('Function timed out!')]
+            def target():
+                try:
+                    res[0] = func(*args, **kwargs)
+                except Exception as e:
+                    res[0] = e
+            t = Thread(target=target)
+            t.start()
+            t.join(seconds)
+            if isinstance(res[0], BaseException):
+                raise res[0]
+            return res[0]
         return wrapper
     return decorator
 
 # @retry(attempts/-1, delay)
 # Retry a function a number of times with a delay between each attempt.
 def retry(attempts, delay):
     import time
```

### Comparing `decoutilities-0.2.0/decoutilities/config/config.py` & `decoutilities-0.2.1/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.0/decoutilities/config/configContainer.py` & `decoutilities-0.2.1/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.0/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.1/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.0/setup.py` & `decoutilities-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.0',
+version='0.2.1',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

