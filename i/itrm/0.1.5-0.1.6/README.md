# Comparing `tmp/itrm-0.1.5.tar.gz` & `tmp/itrm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.5.tar", last modified: Mon May  6 20:00:23 2024, max compression
+gzip compressed data, was "itrm-0.1.6.tar", last modified: Mon May  6 20:27:15 2024, max compression
```

## Comparing `itrm-0.1.5.tar` & `itrm-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.017254 itrm-0.1.5/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.5/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:00:23.017131 itrm-0.1.5/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.5/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.5/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:00:23.017485 itrm-0.1.5/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.015446 itrm-0.1.5/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.016145 itrm-0.1.5/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.5/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    49014 2024-05-06 19:59:29.000000 itrm-0.1.5/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.016933 itrm-0.1.5/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.318417 itrm-0.1.6/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.6/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:27:15.318290 itrm-0.1.6/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.6/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.6/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:27:15.318658 itrm-0.1.6/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.316415 itrm-0.1.6/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.317252 itrm-0.1.6/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.6/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      320 2024-05-06 20:25:41.000000 itrm-0.1.6/src/itrm/eg_iplot.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    49282 2024-05-06 20:23:16.000000 itrm-0.1.6/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:27:15.318071 itrm-0.1.6/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      264 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:27:15.000000 itrm-0.1.6/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.5/LICENSE.txt` & `itrm-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.5/PKG-INFO` & `itrm-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `itrm-0.1.5/README.md` & `itrm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `itrm-0.1.5/setup.cfg` & `itrm-0.1.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.5
+version = 0.1.6
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.5/src/itrm/itrm.py` & `itrm-0.1.6/src/itrm/itrm.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     rows = 20 # default row height
     ar = 2.1 # aspect ratio of characters
 
 
 class persistent: # persistent, run-time values
     t_last = None # last time value
     orig_term_attr = None # original terminal attributes
+    rows_last = None # last number of plot rows
 
 
 class limits: # x and y data limits
     def __init__(self, x_min=None, x_max=None, y_min=None, y_max=None):
         self.x_min = x_min
         self.x_max = x_max
         self.y_min = y_min
@@ -68,15 +69,15 @@
         self.subrows = subrows
         self.subcols = subcols
 
 # ------------------
 # Plotting functions
 # ------------------
 
-def plot(x, y=None, label=None, rows=1, cols=1, equal=0):
+def plot(x, y=None, label=None, rows=1, cols=1, equal=0, overlay=False):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
     plot. Otherwise, the default dimensions (config.cols, config.rows) will be
     used. Note that this function does not plot connecting lines, only the
     points specified by the (`x`, `y`) pairs.
 
@@ -108,14 +109,16 @@
     """
 
     # Check and (possibly) adjust the shapes of x and y.
     x, y = shape_xy(x, y)
 
     # Choose the canvas size.
     tws = screen_size(rows, cols)
+    if overlay:
+        print(f"\x1b[{persistent.rows_last + 2}A", end='', flush=True)
 
     # Get the data limits, adjusting for the terminal window size.
     lims, row_zero = limits_xy(x, y, tws, equal)
 
     # Map x and y to the expanded canvas, M, and the foreground color matrix, F.
     M, F = data_to_matrix(x, y, lims, tws)
 
@@ -126,15 +129,15 @@
     ranges = f"({ftostr(lims.x_min)}:{ftostr(lims.x_max)}, " \
             + f"{ftostr(lims.y_min)}:{ftostr(lims.y_max)})"
 
     # Draw the plot.
     draw_graph(C, ranges, label, F, row_zero)
 
 
-def iplot(x, y=None, label=None, rows=1, cols=1):
+def iplot(x, y=None, label=None, rows=1, cols=1, overlay=False):
     """
     Create an interactive, text-based plot of the path defined by (`x`, `y`)
     using characters. If the size of the terminal can be found, that will be
     used for sizing the plot. Otherwise, the default dimensions (config.cols,
     config.rows) will be used. Note that this function does not plot connecting
     lines, only the points specified by the (`x`, `y`) pairs. Once the function
     has been called, the terminal will be in interactive mode. The user can then
@@ -203,14 +206,16 @@
 
     # Check and (possibly) adjust the shapes of x and y.
     x, y = shape_xy(x, y)
     J, K = x.shape
 
     # Get the canvas size.
     tws = screen_size(rows, cols)
+    if overlay:
+        print(f"\x1b[{persistent.rows_last + 2}A", end='', flush=True)
 
     # Get the data limits, adjusting for the terminal window size.
     lims, _ = limits_xy(x, y, tws, 0) # ignore row_zero
 
     # --------------------
     # Draw a blank canvas.
     # --------------------
@@ -855,14 +860,15 @@
         subrows = 4
     else:
         subcols = 1
         subrows = 3
 
     # Load the dimensions into an object.
     tws = term_ws(rows, cols, subrows, subcols)
+    persistent.rows_last = rows
 
     return tws
 
 
 def shape_xy(x, y):
     # If only `x` is provided, copy to `y`
     # and make `x` an array of integers.
@@ -1198,18 +1204,18 @@
         Matrix of foreground 8-bit color values.
     row_zero : int, default -1
         Row index of y = 0.
     """
 
     # Define the box drawing characters.
     if config.uni:
-        b = ["\u250C", "\u2500", "\u2510",  # . - .
-                "\u2502", "\u2502",         # |   |
-                "\u251C", "\u2524",         # +   +
-                "\u2514", "\u2518"]         # '   '
+        b = ["\u250F", "\u2501", "\u2513",  # . - .
+                "\u2503", "\u2503",         # |   |
+                "\u2523", "\u252B",         # +   +
+                "\u2517", "\u251B"]         # '   '
         s = 0x2800 # braille space
     else:
         b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
         s = 0x20 # ASCII space
 
     # Replace zeros with spaces.
     C = np.where(C == 0, s, C)
@@ -1307,32 +1313,32 @@
     0.022614872267481156 1.00 # baseline
     0.007898384667653082 2.86 # skipping to deltas
     0.007420537999439004 3.05 # removing the recalculation of C
     """
 
     # Define the box drawing characters.
     if config.uni:
-        b = ["\u250C", "\u2500", "\u2510",  # . - .
-                "\u2502", "\u2502",         # |   |
-                "\u251C", "\u2524",         # +   +
-                "\u2514", "\u2518"]         # '   '
+        b = ["\u250F", "\u2501", "\u2513",  # . - .
+                "\u2503", "\u2503",         # |   |
+                "\u2523", "\u252B",         # +   +
+                "\u2517", "\u251B"]         # '   '
         s = 0x2800 # braille space
     else:
         b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
         s = 0x20 # ASCII space
 
     # Replace zeros with spaces.
     C = np.where(C == 0, s, C)
 
     # Move the cursor up to the top left corner of the border.
     rows, cols = C.shape
     print(f"\x1b[{rows + 2}A", end='', flush=True)
 
     # Draw the zoom bar.
-    print(b[0] + "\x1b[1m", end='', flush=True)
+    print(b[0], end='', flush=True)
     if (view.x_min > lims.x_min) or (view.x_max < lims.x_max):
         # Get the start and stop columns of the zoom bar.
         x_span = lims.x_max - lims.x_min
         bar_width = round(cols*(view.x_max - view.x_min)/x_span)
         bar_width = max(1, bar_width)
         if view.x_min == lims.x_min:
             col_a = 0
@@ -1345,19 +1351,19 @@
             col_center = round(cols*(x_view - lims.x_min)/x_span)
             col_a = max(0, round(col_center - bar_width/2))
             col_b = min(cols - 1, col_a + bar_width)
         # Draw the bar.
         print("\x1b[38;5;238m", end="", flush=True)
         for col in range(cols):
             if col == col_a:
-                print("\x1b[0;1m", end="", flush=True)
+                print("\x1b[0m", end="", flush=True)
             if col == col_b:
                 print("\x1b[38;5;238m", end="", flush=True)
             print(b[1], end='', flush=True)
-        print("\x1b[0;1m", end="", flush=True)
+        print("\x1b[0m", end="", flush=True)
     else:
         for col in range(cols):
             print(b[1], end='', flush=True)
     print(f"{b[2]}", flush=True)
 
     # For each row of the matrix, draw the contents.
     for row in range(rows):
```

### Comparing `itrm-0.1.5/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.6/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

