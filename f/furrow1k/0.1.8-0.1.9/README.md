# Comparing `tmp/furrow1k-0.1.8.tar.gz` & `tmp/furrow1k-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furrow1k-0.1.8.tar", max compression
+gzip compressed data, was "furrow1k-0.1.9.tar", max compression
```

## Comparing `furrow1k-0.1.8.tar` & `furrow1k-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.8/LICENSE
--rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.8/README.md
--rw-r--r--   0        0        0      415 2024-05-06 02:36:55.448498 furrow1k-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.8/src/furrow1k/__init__.py
--rw-r--r--   0        0        0      754 2024-05-06 02:36:48.289620 furrow1k-0.1.8/src/furrow1k/furrow1k.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.9/LICENSE
+-rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.9/README.md
+-rw-r--r--   0        0        0      415 2024-05-06 02:38:20.671228 furrow1k-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.9/src/furrow1k/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-06 02:38:12.938312 furrow1k-0.1.9/src/furrow1k/furrow1k.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.9/PKG-INFO
```

### Comparing `furrow1k-0.1.8/LICENSE` & `furrow1k-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.8/README.md` & `furrow1k-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.8/src/furrow1k/furrow1k.py` & `furrow1k-0.1.9/src/furrow1k/furrow1k.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 
 
 
 def main():
     while True:
         valid_options = [1, 2]
         try:
-            next_paycheck = input(
-                dedent(
-                    """
-                    Is your paycheck this Friday or the next Friday? 
-
-                        1. This Friday
-                        2. Next Friday
-                    """
+            next_paycheck = int(
+                input(
+                    dedent(
+                        """\
+                        Is your paycheck this Friday or the next Friday? 
+
+                            1. This Friday
+                            2. Next Friday
+                        """
+                    )
                 )
             )
         except ValueError:
-            print("Please input a valid integer.")
+            print(f"Please enter a valid option: {valid_options=}")
 
         if next_paycheck in valid_options:
             break
         else:
             print(f"Please enter a valid option: {valid_options=}")
 
     readable = "This Friday" if next_paycheck == 1 else "Next Friday"
```

### Comparing `furrow1k-0.1.8/PKG-INFO` & `furrow1k-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furrow1k
-Version: 0.1.8
+Version: 0.1.9
 Summary: Help calculate percentage of salary to contribute to 401k
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.12.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

