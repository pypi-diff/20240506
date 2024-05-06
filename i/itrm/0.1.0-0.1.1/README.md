# Comparing `tmp/itrm-0.1.0.tar.gz` & `tmp/itrm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.1.0.tar", last modified: Mon May  6 19:12:00 2024, max compression
+gzip compressed data, was "itrm-0.1.1.tar", last modified: Mon May  6 19:17:56 2024, max compression
```

## Comparing `itrm-0.1.0.tar` & `itrm-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:12:00.515026 itrm-0.1.0/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.0/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8786 2024-05-06 19:12:00.514915 itrm-0.1.0/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8329 2024-05-06 19:10:54.000000 itrm-0.1.0/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.0/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:12:00.515255 itrm-0.1.0/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:12:00.513048 itrm-0.1.0/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:12:00.514708 itrm-0.1.0/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     8786 2024-05-06 19:12:00.000000 itrm-0.1.0/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      241 2024-05-06 19:12:00.000000 itrm-0.1.0/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:12:00.000000 itrm-0.1.0/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:12:00.000000 itrm-0.1.0/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-06 19:12:00.000000 itrm-0.1.0/src/itrm.egg-info/top_level.txt
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:12:00.514491 itrm-0.1.0/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.0/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    48555 2024-05-06 18:57:31.000000 itrm-0.1.0/src/trm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828937 itrm-0.1.1/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.1.1/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:17:56.828822 itrm-0.1.1/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8437 2024-05-06 19:17:36.000000 itrm-0.1.1/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.1.1/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-06 19:17:56.829162 itrm-0.1.1/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.827186 itrm-0.1.1/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828620 itrm-0.1.1/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     8894 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      241 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-06 19:17:56.000000 itrm-0.1.1/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-06 19:17:56.828403 itrm-0.1.1/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.1.1/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    48555 2024-05-06 18:57:31.000000 itrm-0.1.1/src/trm/itrm.py
```

### Comparing `itrm-0.1.0/LICENSE.txt` & `itrm-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.1.0/PKG-INFO` & `itrm-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,28 +103,22 @@
 resulting plot will be interactive with a cursor you can move to inspect the
 values. You can move the cursor left and right, at normal speed or fast speed.
 You can zoom in and out. And, you can cycle through which rows of the `x` and
 `y` data to focus on.
 
 The following table details the shortcut keys:
 
-| Keys           | Function                 |
-| :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |
-| `h`, `a`, `←`  | move cursor left         |
-| `l`, `d`, `→`  | move cursor right        |
-| `H`, `A`, `⇧←` | move cursor left fast    |
-| `L`, `D`, `⇧→` | move cursor right fast   |
-| `j`, `s`, `↓`  | zoom in                  |
-| `k`, `w`, `↑`  | zoom out                 |
-| `J`, `S`, `⇧↓` | zoom in fast             |
-| `K`, `W`, `⇧↑` | zoom out fast            |
-| `n`            | next data row            |
-| `p`            | previous data row        |
-| `c`            | center view on cursor    |
+| Keys           | Function                 |   | Keys           | Function                 |
+| :------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
+| `c`            | center view on cursor    |   | `p`            | previous data row        |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.0/README.md` & `itrm-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,28 +88,22 @@
 resulting plot will be interactive with a cursor you can move to inspect the
 values. You can move the cursor left and right, at normal speed or fast speed.
 You can zoom in and out. And, you can cycle through which rows of the `x` and
 `y` data to focus on.
 
 The following table details the shortcut keys:
 
-| Keys           | Function                 |
-| :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |
-| `h`, `a`, `←`  | move cursor left         |
-| `l`, `d`, `→`  | move cursor right        |
-| `H`, `A`, `⇧←` | move cursor left fast    |
-| `L`, `D`, `⇧→` | move cursor right fast   |
-| `j`, `s`, `↓`  | zoom in                  |
-| `k`, `w`, `↑`  | zoom out                 |
-| `J`, `S`, `⇧↓` | zoom in fast             |
-| `K`, `W`, `⇧↑` | zoom out fast            |
-| `n`            | next data row            |
-| `p`            | previous data row        |
-| `c`            | center view on cursor    |
+| Keys           | Function                 |   | Keys           | Function                 |
+| :------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
+| `c`            | center view on cursor    |   | `p`            | previous data row        |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.0/setup.cfg` & `itrm-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.1.0
+version = 0.1.1
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.1.0/src/itrm.egg-info/PKG-INFO` & `itrm-0.1.1/src/itrm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -103,28 +103,22 @@
 resulting plot will be interactive with a cursor you can move to inspect the
 values. You can move the cursor left and right, at normal speed or fast speed.
 You can zoom in and out. And, you can cycle through which rows of the `x` and
 `y` data to focus on.
 
 The following table details the shortcut keys:
 
-| Keys           | Function                 |
-| :------------: | ------------------------ |
-| `q`, `x`, `⌫`  | exit interactive plot    |
-| `h`, `a`, `←`  | move cursor left         |
-| `l`, `d`, `→`  | move cursor right        |
-| `H`, `A`, `⇧←` | move cursor left fast    |
-| `L`, `D`, `⇧→` | move cursor right fast   |
-| `j`, `s`, `↓`  | zoom in                  |
-| `k`, `w`, `↑`  | zoom out                 |
-| `J`, `S`, `⇧↓` | zoom in fast             |
-| `K`, `W`, `⇧↑` | zoom out fast            |
-| `n`            | next data row            |
-| `p`            | previous data row        |
-| `c`            | center view on cursor    |
+| Keys           | Function                 |   | Keys           | Function                 |
+| :------------: | ------------------------ | - | :------------: | ------------------------ |
+| `q`, `x`, `⌫`  | exit interactive plot    |   | `j`, `s`, `↓`  | zoom in                  |
+| `h`, `a`, `←`  | move cursor left         |   | `k`, `w`, `↑`  | zoom out                 |
+| `l`, `d`, `→`  | move cursor right        |   | `J`, `S`, `⇧↓` | zoom in fast             |
+| `H`, `A`, `⇧←` | move cursor left fast    |   | `K`, `W`, `⇧↑` | zoom out fast            |
+| `L`, `D`, `⇧→` | move cursor right fast   |   | `n`            | next data row            |
+| `c`            | center view on cursor    |   | `p`            | previous data row        |
 
 ## Bars
 
 ```python
 itrm.bars(x, labels=None, cols=1, fat=False)
 ```
```

### Comparing `itrm-0.1.0/src/trm/itrm.py` & `itrm-0.1.1/src/trm/itrm.py`

 * *Files identical despite different names*

