# Comparing `tmp/nuitka_hatch-1.1.tar.gz` & `tmp/nuitka_hatch-1.2.tar.gz`

## Comparing `nuitka_hatch-1.1.tar` & `nuitka_hatch-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/src/nuitka_hatch/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/src/nuitka_hatch/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/src/nuitka_hatch/hooks.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/src/nuitka_hatch/plugin.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/tests/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/tests/test_build.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/tests/utils.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/README.md
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/pyproject.toml
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 nuitka_hatch-1.1/PKG-INFO
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/src/nuitka_hatch/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/src/nuitka_hatch/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/src/nuitka_hatch/hooks.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/src/nuitka_hatch/plugin.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/tests/test_build.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/tests/utils.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/README.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/pyproject.toml
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 nuitka_hatch-1.2/PKG-INFO
```

### Comparing `nuitka_hatch-1.1/src/nuitka_hatch/plugin.py` & `nuitka_hatch-1.2/src/nuitka_hatch/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         ]
         args = args or default_args
         process = subprocess.run(
             ["nuitka3", *args],
         )
         if process.returncode:
             msg = process.stdout
+            if not msg:
+                msg = process.stderr
+            if not msg:
+                msg = f"Nuitka failed with return code {process.returncode}"
             if isinstance(msg, bytes):
                 msg = msg.decode("utf-8")
             raise Exception(msg)
 
         build_data["infer_tag"] = True
         build_data["pure_python"] = False
         build_data["artifacts"].extend(self.artifact_patterns)
```

### Comparing `nuitka_hatch-1.1/tests/conftest.py` & `nuitka_hatch-1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.1/LICENSE.txt` & `nuitka_hatch-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.1/pyproject.toml` & `nuitka_hatch-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.1/PKG-INFO` & `nuitka_hatch-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nuitka-hatch
-Version: 1.1
+Version: 1.2
 Summary: hatch nuitka plugin
 Project-URL: Documentation, https://github.com/HSPK/hatch-nuitka#readme
 Project-URL: Issues, https://github.com/HSPK/hatch-nuitka/issues
 Project-URL: Source, https://github.com/HSPK/hatch-nuitka
 Author-email: HSPK <whxway@whu.edu.cn>
 License-Expression: MIT
 License-File: LICENSE.txt
```

