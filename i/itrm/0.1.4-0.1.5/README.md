# Comparing `tmp/itrm-0.1.4.tar.gz` & `tmp/itrm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.4.tar", last modified: Mon May  6 19:49:18 2024, max compression
+gzip compressed data, was "itrm-0.1.5.tar", last modified: Mon May  6 20:00:23 2024, max compression
```

## Comparing `itrm-0.1.4.tar` & `itrm-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.049425 itrm-0.1.4/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.4/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:49:18.049304 itrm-0.1.4/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.4/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.4/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:49:18.049650 itrm-0.1.4/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.047679 itrm-0.1.4/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.048373 itrm-0.1.4/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.4/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    48599 2024-05-06 19:47:46.000000 itrm-0.1.4/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:49:18.049121 itrm-0.1.4/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 19:49:18.000000 itrm-0.1.4/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.017254 itrm-0.1.5/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.5/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:00:23.017131 itrm-0.1.5/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8531 2024-05-06 19:59:43.000000 itrm-0.1.5/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.5/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 20:00:23.017485 itrm-0.1.5/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.015446 itrm-0.1.5/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.016145 itrm-0.1.5/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.5/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    49014 2024-05-06 19:59:29.000000 itrm-0.1.5/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 20:00:23.016933 itrm-0.1.5/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8988 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-06 20:00:23.000000 itrm-0.1.5/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.1.4/LICENSE.txt` & `itrm-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.4/PKG-INFO` & `itrm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -110,15 +110,16 @@
 | Keys           | Function                 |   | Keys           | Function                 |
 | :------------: | ------------------------ | - | :------------: | ------------------------ |
 | `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
 | `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
 | `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
 | `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
 | `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `c`            | center view on cursor    |   | `p`            | previous data row        |
+| `g`            | move cursor to start     |   | `p`            | previous data row        |
+| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.4/README.md` & `itrm-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 | Keys           | Function                 |   | Keys           | Function                 |
 | :------------: | ------------------------ | - | :------------: | ------------------------ |
 | `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
 | `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
 | `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
 | `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
 | `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `c`            | center view on cursor    |   | `p`            | previous data row        |
+| `g`            | move cursor to start     |   | `p`            | previous data row        |
+| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.4/setup.cfg` & `itrm-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.4
+version = 0.1.5
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.4/src/itrm/itrm.py` & `itrm-0.1.5/src/itrm/itrm.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,25 +155,28 @@
         less than 1.
     cols : int, default 1
         Desired number of columns if greater than 1 or fraction of window
         columns if less than 1.
 
     Shortcuts
     ---------
-    h : move cursor left
-    l : move cursor right
-    H : move cursor left fast
-    L : move cursor right fast
-    j : zoom in
-    k : zoom out
-    J : zoom in fast
-    K : zoom out fast
-    n : next data row
-    p : previous data row
-    c : center view on cursor
+    q, x, ⌫  : exit interactive plot
+    h, a, ←  : move cursor left
+    l, d, →  : move cursor right
+    H, A, ⇧← : move cursor left fast
+    L, D, ⇧→ : move cursor right fast
+    g        : move cursor to start
+    G        : move cursor to end
+    j, s, ↓  : zoom in
+    k, w, ↑  : zoom out
+    J, S, ⇧↓ : zoom in fast
+    K, W, ⇧↑ : zoom out fast
+    n        : next data row
+    p        : previous data row
+    c, z     : center view on cursor
 
     Notes
     -----
     Non-finite values will be ignored.
     """
 
     # Check if this is a tty.
@@ -340,19 +343,25 @@
             zoom_sf = 0.25
         elif char == 'n':
             cstate = cstate + 1 if cstate < J - 1 else -1
             recursor = True
         elif char == 'p':
             cstate = cstate - 1 if cstate > -1 else J - 1
             recursor = True
-        elif char == 'c':
+        elif (char == 'c') or (char == 'z'):
             view = center_view(xc, view)
             view = limit_view(view, lims)
             recursor = True
             remap = True
+        elif char == 'g':
+            jump_sf = (lims.x_min - xc)/dx
+            recursor = True
+        elif char == 'G':
+            jump_sf = (lims.x_max - xc)/dx
+            recursor = True
         else:
             continue
 
         # Process the zoom scaling factor.
         if zoom_sf != 1.0:
             if (zoom_sf > 1) and (view.x_min == lims.x_min) \
                     and (view.x_max == lims.x_max): # skip if zoomed out
@@ -1353,15 +1362,15 @@
     # For each row of the matrix, draw the contents.
     for row in range(rows):
         # Get this row of data.
         F_row = 0 if F is None else F[row]
         C_row = C[row]
 
         # Draw this row.
-        print("\x1b[1C\x1b[1m", end='', flush=True) # Move forward past left border
+        print("\x1b[1C\x1b[1m", end='', flush=True) # Move past left border
         f_last = 0
         col_last = -1
         for col in range(cols):
             # Skip where there is no delta.
             if not D[row, col]:
                 continue
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `itrm-0.1.4/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.5/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -110,15 +110,16 @@
 | Keys           | Function                 |   | Keys           | Function                 |
 | :------------: | ------------------------ | - | :------------: | ------------------------ |
 | `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
 | `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
 | `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
 | `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
 | `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
-| `c`            | center view on cursor    |   | `p`            | previous data row        |
+| `g`            | move cursor to start     |   | `p`            | previous data row        |
+| `G`            | move cursor to end       |   | `c`, `z`       | center view on cursor    |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

