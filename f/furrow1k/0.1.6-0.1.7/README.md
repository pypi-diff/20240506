# Comparing `tmp/furrow1k-0.1.6.tar.gz` & `tmp/furrow1k-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furrow1k-0.1.6.tar", max compression
+gzip compressed data, was "furrow1k-0.1.7.tar", max compression
```

## Comparing `furrow1k-0.1.6.tar` & `furrow1k-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.6/LICENSE
--rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.6/README.md
--rw-r--r--   0        0        0      415 2024-05-06 02:30:14.709067 furrow1k-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.6/src/furrow1k/__init__.py
--rw-r--r--   0        0        0      536 2024-05-06 02:30:10.140308 furrow1k-0.1.6/src/furrow1k/furrow1k.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.7/LICENSE
+-rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.7/README.md
+-rw-r--r--   0        0        0      415 2024-05-06 02:33:17.279232 furrow1k-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.7/src/furrow1k/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-06 02:33:09.486303 furrow1k-0.1.7/src/furrow1k/furrow1k.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.7/PKG-INFO
```

### Comparing `furrow1k-0.1.6/LICENSE` & `furrow1k-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.6/README.md` & `furrow1k-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.6/src/furrow1k/furrow1k.py` & `furrow1k-0.1.7/src/furrow1k/furrow1k.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime as dt
 
 
 def main():
-    try:
+    while True:
         next_paycheck = input(
             """
             Is your paycheck this Friday or the next Friday? 
 
             1. This Friday
             2. Next Friday
             """
         )
         valid_options = [1, 2]
-        if next_paycheck not in valid_options:
-            raise ValueError
-    except:
-        print(f"Please enter a valid option: {valid_options=}")
+        if next_paycheck in valid_options:
+            break
+        else:
+            print(f"Please enter a valid option: {valid_options=}")
 
     readable = "This Friday" if next_paycheck == 1 else "Next Friday"
     print(f"Your next paycheck is {readable}.")
```

### Comparing `furrow1k-0.1.6/PKG-INFO` & `furrow1k-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furrow1k
-Version: 0.1.6
+Version: 0.1.7
 Summary: Help calculate percentage of salary to contribute to 401k
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.12.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

