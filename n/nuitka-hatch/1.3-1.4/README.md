# Comparing `tmp/nuitka_hatch-1.3.tar.gz` & `tmp/nuitka_hatch-1.4.tar.gz`

## Comparing `nuitka_hatch-1.3.tar` & `nuitka_hatch-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/src/nuitka_hatch/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/src/nuitka_hatch/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/src/nuitka_hatch/hooks.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/src/nuitka_hatch/plugin.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/tests/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/tests/test_build.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/tests/utils.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/README.md
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/pyproject.toml
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 nuitka_hatch-1.3/PKG-INFO
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/src/nuitka_hatch/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/src/nuitka_hatch/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/src/nuitka_hatch/hooks.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/src/nuitka_hatch/plugin.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/tests/test_build.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/tests/utils.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/README.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/pyproject.toml
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 nuitka_hatch-1.4/PKG-INFO
```

### Comparing `nuitka_hatch-1.3/src/nuitka_hatch/plugin.py` & `nuitka_hatch-1.4/src/nuitka_hatch/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,16 @@
             "--remove-output",
         ]
         args = args or default_args
         process = subprocess.run(
             ["nuitka3", *args],
         )
         msg = process.stdout or process.stderr
-        if process.returncode and not msg:
-            raise Exception("Failed to build wheel")
+        if process.returncode and msg:
+            raise Exception(f"Failed to build wheel: {msg}")
 
         build_data["infer_tag"] = True
         build_data["pure_python"] = False
         build_data["artifacts"].extend(self.artifact_patterns)
         build_data["force_include"] = self.get_inclusion_map()
 
     def finalize(self, version: str, build_data: dict[str, Any], artifact_path: str) -> None:
```

### Comparing `nuitka_hatch-1.3/tests/conftest.py` & `nuitka_hatch-1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.3/LICENSE.txt` & `nuitka_hatch-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.3/pyproject.toml` & `nuitka_hatch-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nuitka_hatch-1.3/PKG-INFO` & `nuitka_hatch-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nuitka-hatch
-Version: 1.3
+Version: 1.4
 Summary: hatch nuitka plugin
 Project-URL: Documentation, https://github.com/HSPK/hatch-nuitka#readme
 Project-URL: Issues, https://github.com/HSPK/hatch-nuitka/issues
 Project-URL: Source, https://github.com/HSPK/hatch-nuitka
 Author-email: HSPK <whxway@whu.edu.cn>
 License-Expression: MIT
 License-File: LICENSE.txt
```

