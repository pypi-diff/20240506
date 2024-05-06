# Comparing `tmp/itrm-0.1.2.tar.gz` & `tmp/itrm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.2.tar", last modified: Mon May  6 19:25:39 2024, max compression
+gzip compressed data, was "itrm-0.1.3.tar", last modified: Mon May  6 19:38:06 2024, max compression
```

## Comparing `itrm-0.1.2.tar` & `itrm-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.106707 itrm-0.1.2/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.2/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:25:39.106592 itrm-0.1.2/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.2/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.2/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:25:39.106936 itrm-0.1.2/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.104223 itrm-0.1.2/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.105214 itrm-0.1.2/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.2/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    48555 2024-05-06 18:57:31.000000 itrm-0.1.2/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:25:39.106394 itrm-0.1.2/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:25:39.000000 itrm-0.1.2/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.491167 itrm-0.1.3/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.3/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:38:06.491044 itrm-0.1.3/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.3/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.3/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:38:06.491428 itrm-0.1.3/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.489276 itrm-0.1.3/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.490010 itrm-0.1.3/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.3/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    48595 2024-05-06 19:35:25.000000 itrm-0.1.3/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:38:06.490814 itrm-0.1.3/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:38:06.000000 itrm-0.1.3/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.2/LICENSE.txt` & `itrm-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.2/PKG-INFO` & `itrm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.2/README.md` & `itrm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.2/setup.cfg` & `itrm-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.2
+version = 0.1.3
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.2/src/itrm/itrm.py` & `itrm-0.1.3/src/itrm/itrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1223,29 +1223,29 @@
             r = b[6]
 
         # Get this row of data.
         F_row = 0 if F is None else F[row]
         C_row = C[row]
 
         # Draw this row.
-        print(l, end='', flush=True)
+        print(l + "\x1b[1m", end='', flush=True)
         f_last = 0
         for col in range(cols):
             # Get this column color.
             f = 0 if F is None else F_row[col]
 
             if f_last != f:
                 if f == 0:
-                    print("\x1b[0m", end='')
+                    print("\x1b[0;1m", end='')
                 else:
                     print(f"\x1b[38;5;{f}m", end='')
                 f_last = f
             print(chr(C_row[col]), end='', flush=True)
         if f_last != 0:
-            print("\x1b[0m", end='')
+            print("\x1b[0;1m", end='')
         print(r, flush=True)
 
     # Get the number of middle dashes.
     mid_dashes = cols - 2
     if left is not None:
         mid_dashes -= len(left) + 2
     if right is not None:
@@ -1315,15 +1315,15 @@
     C = np.where(C == 0, s, C)
 
     # Move the cursor up to the top left corner of the border.
     rows, cols = C.shape
     print(f"\x1b[{rows + 2}A", end='', flush=True)
 
     # Draw the zoom bar.
-    print(f"{b[0]}", end='', flush=True)
+    print(b[0] + "\x1b[1m", end='', flush=True)
     if (view.x_min > lims.x_min) or (view.x_max < lims.x_max):
         # Get the start and stop columns of the zoom bar.
         x_span = lims.x_max - lims.x_min
         bar_width = round(cols*(view.x_max - view.x_min)/x_span)
         bar_width = max(1, bar_width)
         if view.x_min == lims.x_min:
             col_a = 0
@@ -1336,32 +1336,32 @@
             col_center = round(cols*(x_view - lims.x_min)/x_span)
             col_a = max(0, round(col_center - bar_width/2))
             col_b = min(cols - 1, col_a + bar_width)
         # Draw the bar.
         print("\x1b[38;5;238m", end="", flush=True)
         for col in range(cols):
             if col == col_a:
-                print("\x1b[0m", end="", flush=True)
+                print("\x1b[0;1m", end="", flush=True)
             if col == col_b:
                 print("\x1b[38;5;238m", end="", flush=True)
             print(b[1], end='', flush=True)
-        print("\x1b[0m", end="", flush=True)
+        print("\x1b[0;1m", end="", flush=True)
     else:
         for col in range(cols):
             print(b[1], end='', flush=True)
     print(f"{b[2]}", flush=True)
 
     # For each row of the matrix, draw the contents.
     for row in range(rows):
         # Get this row of data.
         F_row = 0 if F is None else F[row]
         C_row = C[row]
 
         # Draw this row.
-        print("\x1b[1C", end='', flush=True) # Move forward past left border
+        print("\x1b[1C\x1b[1m", end='', flush=True) # Move forward past left border
         f_last = 0
         col_last = -1
         for col in range(cols):
             # Skip where there is no delta.
             if not D[row, col]:
                 continue
 
@@ -1377,26 +1377,26 @@
             else:
                 f = F_row[col]
                 if (col == ccol) and (f != 0): # Switch to bright colors.
                     f = BRIGHT_COLORS[NORMAL_COLORS.index(f)]
 
             # Display the cursor.
             if (col == ccol) and (C_row[col] == s):
-                print(cF + b[3] + '\x1b[0m', end='', flush=True)
+                print(cF + b[3] + '\x1b[0;1m', end='', flush=True)
                 f_last = 0
             else:
                 if f_last != f:
                     if f == 0:
-                        print("\x1b[0m", end='')
+                        print("\x1b[0;1m", end='')
                     else:
                         print(f"\x1b[38;5;{f}m", end='')
                     f_last = f
                 print(chr(C_row[col]), end='', flush=True)
         if f_last != 0:
-            print("\x1b[0m", end='', flush=True)
+            print("\x1b[0;1m", end='', flush=True)
         print('', flush=True)
 
     # Get the number of middle dashes.
     mid_dashes = cols - 2
     if left is not None:
         mid_dashes -= len(left) + 2
     if right is not None:
```

### Comparing `itrm-0.1.2/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.3/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

