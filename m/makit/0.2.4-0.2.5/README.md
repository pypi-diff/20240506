# Comparing `tmp/makit-0.2.4.tar.gz` & `tmp/makit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makit-0.2.4.tar", last modified: Tue Apr 30 12:18:08 2024, max compression
+gzip compressed data, was "makit-0.2.5.tar", last modified: Mon May  6 07:51:30 2024, max compression
```

## Comparing `makit-0.2.4.tar` & `makit-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-30 12:18:08.500028 makit-0.2.4/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.4/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.4/MANIFEST.in
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-30 12:18:08.500028 makit-0.2.4/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.4/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-30 12:18:08.500028 makit-0.2.4/makeit/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.4/makeit/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.4/makeit/__main__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      573 2024-04-30 12:16:31.000000 makit-0.2.4/makeit/main.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3200 2024-04-30 12:15:49.000000 makit-0.2.4/makeit/make.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.4/makeit/py.typed
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3011 2024-04-29 11:55:50.000000 makit-0.2.4/makeit/tui.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-04-30 12:17:27.000000 makit-0.2.4/makeit/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-30 12:18:08.500028 makit-0.2.4/makit.egg-info/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/entry_points.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-04-30 12:18:08.000000 makit-0.2.4/makit.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-04-30 12:17:30.000000 makit-0.2.4/pyproject.toml
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-29 11:41:19.000000 makit-0.2.4/requirements.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-30 12:18:08.500028 makit-0.2.4/setup.cfg
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.4/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-05-06 07:51:30.616399 makit-0.2.5/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.5/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.5/MANIFEST.in
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-05-06 07:51:30.616399 makit-0.2.5/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.5/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-05-06 07:51:30.608399 makit-0.2.5/makeit/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.5/makeit/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.5/makeit/__main__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      573 2024-04-30 12:16:31.000000 makit-0.2.5/makeit/main.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3200 2024-04-30 12:15:49.000000 makit-0.2.5/makeit/make.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.5/makeit/py.typed
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3415 2024-05-06 07:49:36.000000 makit-0.2.5/makeit/tui.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-05-06 07:51:00.000000 makit-0.2.5/makeit/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-05-06 07:51:30.616399 makit-0.2.5/makit.egg-info/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/entry_points.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-05-06 07:51:30.000000 makit-0.2.5/makit.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-05-06 07:50:57.000000 makit-0.2.5/pyproject.toml
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-29 11:41:19.000000 makit-0.2.5/requirements.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-05-06 07:51:30.616399 makit-0.2.5/setup.cfg
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.5/setup.py
```

### Comparing `makit-0.2.4/LICENSE` & `makit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `makit-0.2.4/PKG-INFO` & `makit-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.4 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.5 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual>=0.58.0 # Makeit
 **makeit** is an interactive Makefile runner.
```

### Comparing `makit-0.2.4/makeit/main.py` & `makit-0.2.5/makeit/main.py`

 * *Files identical despite different names*

### Comparing `makit-0.2.4/makeit/make.py` & `makit-0.2.5/makeit/make.py`

 * *Files identical despite different names*

### Comparing `makit-0.2.4/makeit/tui.py` & `makit-0.2.5/makeit/tui.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,15 +67,24 @@
         if selected_index < 0 or selected_index >= len(self.steps):
             return None
         return self.steps[selected_index]
 
     def _get_listview(self) -> ListView:
         return self.query_one("#steps-list", ListView)
 
+    def _move_cursor_wrapping(self, delta: int):
+        index = self._get_listview().index
+        if index is not None:
+            self._get_listview().index = (index + delta + len(self.steps)) % len(self.steps)
+
     def on_key(self, event: events.Key) -> None:
         # self.post_logs.append(str(event))
         if event.key in {'q', 'escape'}:
             self.exit()
         elif event.key == 'home':
             self._get_listview().index = 0
         elif event.key == 'end':
             self._get_listview().index = len(self.steps) - 1
+        elif event.key == 'j':  # move down, wrapping around
+            self._move_cursor_wrapping(1)
+        elif event.key == 'k':  # move up
+            self._move_cursor_wrapping(-1)
```

### Comparing `makit-0.2.4/makit.egg-info/PKG-INFO` & `makit-0.2.5/makit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.4 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.5 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual>=0.58.0 # Makeit
 **makeit** is an interactive Makefile runner.
```

### Comparing `makit-0.2.4/pyproject.toml` & `makit-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "makit"
-version = "0.2.4"  # also in makeit/version.py
+version = "0.2.5"  # also in makeit/version.py
 description = "Interactive Makefile step picker"
 license = {text = "MIT"}
 authors = [
     { name = "igrek51", email = "igrek51.dev@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

