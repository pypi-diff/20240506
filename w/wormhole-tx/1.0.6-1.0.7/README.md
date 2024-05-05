# Comparing `tmp/wormhole-tx-1.0.6.tar.gz` & `tmp/wormhole-tx-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormhole-tx-1.0.6.tar", last modified: Thu Apr 11 21:16:48 2024, max compression
+gzip compressed data, was "wormhole-tx-1.0.7.tar", last modified: Sun May  5 23:32:35 2024, max compression
```

## Comparing `wormhole-tx-1.0.6.tar` & `wormhole-tx-1.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.273988 wormhole-tx-1.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.227989 wormhole-tx-1.0.6/.github/
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.256987 wormhole-tx-1.0.6/.github/workflows/
--rw-rw-rw-   0        0        0      855 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      801 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_macos.yml
--rw-rw-rw-   0        0        0      803 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_ubuntu.yml
--rw-rw-rw-   0        0        0      800 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.github/workflows/push_win.yml
--rw-rw-rw-   0        0        0     1909 2024-02-08 21:58:57.000000 wormhole-tx-1.0.6/.gitignore
--rw-rw-rw-   0        0        0      186 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.pylintrc
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.259987 wormhole-tx-1.0.6/.vscode/
--rw-rw-rw-   0        0        0     1354 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/launch.json
--rw-rw-rw-   0        0        0      820 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/settings.json
--rw-rw-rw-   0        0        0     1109 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1064 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      104 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2206 2024-04-11 21:16:48.272987 wormhole-tx-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1766 2024-04-11 21:16:19.000000 wormhole-tx-1.0.6/README.md
--rw-rw-rw-   0        0        0      519 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/activate.sh
--rw-rw-rw-   0        0        0       11 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/clean
--rw-rw-rw-   0        0        0     1725 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/install
--rw-rw-rw-   0        0        0     6950 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/install.py
--rw-rw-rw-   0        0        0      447 2024-04-11 21:15:37.000000 wormhole-tx-1.0.6/lint
--rw-rw-rw-   0        0        0      897 2024-04-11 21:15:57.000000 wormhole-tx-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       60 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/requirements.testing.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 21:16:48.273988 wormhole-tx-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      428 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.229988 wormhole-tx-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.261987 wormhole-tx-1.0.6/src/tx/
--rw-rw-rw-   0        0        0        0 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/src/tx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.262987 wormhole-tx-1.0.6/src/tx/assets/
--rw-rw-rw-   0        0        0       54 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/src/tx/assets/example.txt
--rw-rw-rw-   0        0        0     4028 2024-04-11 21:15:15.000000 wormhole-tx-1.0.6/src/tx/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.270987 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/
--rw-rw-rw-   0        0        0     2206 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2024-04-11 21:16:48.000000 wormhole-tx-1.0.6/src/wormhole_tx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/test
-drwxrwxrwx   0        0        0        0 2024-04-11 21:16:48.271988 wormhole-tx-1.0.6/tests/
--rw-rw-rw-   0        0        0      364 2024-02-07 06:55:03.000000 wormhole-tx-1.0.6/tests/test_cli.py
--rw-rw-rw-   0        0        0      510 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/tox.ini
--rw-rw-rw-   0        0        0      291 2024-02-07 06:45:14.000000 wormhole-tx-1.0.6/upload_package.sh
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.973427 wormhole-tx-1.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.922428 wormhole-tx-1.0.7/.github/
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.952428 wormhole-tx-1.0.7/.github/workflows/
+-rw-rw-rw-   0        0        0      855 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      801 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.github/workflows/push_macos.yml
+-rw-rw-rw-   0        0        0      803 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.github/workflows/push_ubuntu.yml
+-rw-rw-rw-   0        0        0      800 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.github/workflows/push_win.yml
+-rw-rw-rw-   0        0        0     1909 2024-02-08 21:58:57.000000 wormhole-tx-1.0.7/.gitignore
+-rw-rw-rw-   0        0        0      186 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.pylintrc
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.956425 wormhole-tx-1.0.7/.vscode/
+-rw-rw-rw-   0        0        0     1354 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.vscode/launch.json
+-rw-rw-rw-   0        0        0      820 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1109 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1064 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      104 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2256 2024-05-05 23:32:35.972428 wormhole-tx-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1815 2024-05-05 23:32:15.000000 wormhole-tx-1.0.7/README.md
+-rw-rw-rw-   0        0        0      519 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/activate.sh
+-rw-rw-rw-   0        0        0       11 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/clean
+-rw-rw-rw-   0        0        0     1725 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/install
+-rw-rw-rw-   0        0        0     6950 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/install.py
+-rw-rw-rw-   0        0        0      447 2024-04-11 21:15:37.000000 wormhole-tx-1.0.7/lint
+-rw-rw-rw-   0        0        0      914 2024-05-05 23:32:04.000000 wormhole-tx-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       60 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/requirements.testing.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 23:32:35.973427 wormhole-tx-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      428 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.925426 wormhole-tx-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.958428 wormhole-tx-1.0.7/src/tx/
+-rw-rw-rw-   0        0        0        0 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/src/tx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.959426 wormhole-tx-1.0.7/src/tx/assets/
+-rw-rw-rw-   0        0        0       54 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/src/tx/assets/example.txt
+-rw-rw-rw-   0        0        0     4028 2024-04-11 21:15:15.000000 wormhole-tx-1.0.7/src/tx/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.970427 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/
+-rw-rw-rw-   0        0        0     2256 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2024-05-05 23:32:35.000000 wormhole-tx-1.0.7/src/wormhole_tx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/test
+drwxrwxrwx   0        0        0        0 2024-05-05 23:32:35.971426 wormhole-tx-1.0.7/tests/
+-rw-rw-rw-   0        0        0      364 2024-02-07 06:55:03.000000 wormhole-tx-1.0.7/tests/test_cli.py
+-rw-rw-rw-   0        0        0      510 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/tox.ini
+-rw-rw-rw-   0        0        0      291 2024-02-07 06:45:14.000000 wormhole-tx-1.0.7/upload_package.sh
```

### Comparing `wormhole-tx-1.0.6/.github/workflows/lint.yml` & `wormhole-tx-1.0.7/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.github/workflows/push_macos.yml` & `wormhole-tx-1.0.7/.github/workflows/push_macos.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.github/workflows/push_ubuntu.yml` & `wormhole-tx-1.0.7/.github/workflows/push_ubuntu.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.github/workflows/push_win.yml` & `wormhole-tx-1.0.7/.github/workflows/push_win.yml`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.gitignore` & `wormhole-tx-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.vscode/launch.json` & `wormhole-tx-1.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.vscode/settings.json` & `wormhole-tx-1.0.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/.vscode/tasks.json` & `wormhole-tx-1.0.7/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/LICENSE` & `wormhole-tx-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/PKG-INFO` & `wormhole-tx-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormhole-tx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Front end for wormhole, easier and more secure!
 Home-page: https://github.com/zackees/tx
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -55,11 +55,12 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
+  * 1.0.7: Adds missing dependency for colorama.
   * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.6/README.md` & `wormhole-tx-1.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -42,11 +42,12 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
+  * 1.0.7: Adds missing dependency for colorama.
   * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.6/activate.sh` & `wormhole-tx-1.0.7/activate.sh`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/install` & `wormhole-tx-1.0.7/install`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/install.py` & `wormhole-tx-1.0.7/install.py`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/pyproject.toml` & `wormhole-tx-1.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 description = "Front end for wormhole, easier and more secure!"
 requires-python = ">=3.7"
 keywords = ["template-python-cmd"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "magic-wormhole",
+    "colorama",
 ]
 # Change this with the version number bump.
-version = "1.0.6"
+version = "1.0.7"
 
 [tool.ruff]
 line-length = 200
 
 [tool.pylint."MESSAGES CONTROL"]
 good-names = [
     "c",
```

### Comparing `wormhole-tx-1.0.6/src/tx/cli.py` & `wormhole-tx-1.0.7/src/tx/cli.py`

 * *Files identical despite different names*

### Comparing `wormhole-tx-1.0.6/src/wormhole_tx.egg-info/PKG-INFO` & `wormhole-tx-1.0.7/src/wormhole_tx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wormhole-tx
-Version: 1.0.6
+Version: 1.0.7
 Summary: Front end for wormhole, easier and more secure!
 Home-page: https://github.com/zackees/tx
 Maintainer: Zachary Vorhies
 License: BSD 3-Clause License
 Keywords: template-python-cmd
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -55,11 +55,12 @@
 This environment requires you to use `git-bash`.
 
 # Linting
 
 Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
 
 # Versions
+  * 1.0.7: Adds missing dependency for colorama.
   * 1.0.6: Varius fixes and force UTF-8 on Windows to prevent crash during file send.
   * 1.0.3: Removes new typing system which doesn't work on python < 3.10
   * 1.0.2: Unknown arguments are passed onto `wormhole send`. Help now displays `wormhole --help`.
   * 1.0.1: Fixes missing `magic-wormhole` dependency.
```

### Comparing `wormhole-tx-1.0.6/src/wormhole_tx.egg-info/SOURCES.txt` & `wormhole-tx-1.0.7/src/wormhole_tx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

