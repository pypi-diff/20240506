# Comparing `tmp/infrable-0.1.1.tar.gz` & `tmp/infrable-0.1.2.tar.gz`

## Comparing `infrable-0.1.1.tar` & `infrable-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.1/.envrc
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/errors.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/files.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/host.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/infra.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/init.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/meta.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/paths.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/readfile.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/service.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/switch.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/template.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/files.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/main.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/remote.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/cli/switch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/__init__.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/linux.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.1/infrable/distro/ubuntu.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.1/LICENSE
--rw-r--r--   0        0        0    17862 2020-02-02 00:00:00.000000 infrable-0.1.1/README.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    31688 2020-02-02 00:00:00.000000 infrable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 infrable-0.1.2/.envrc
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/errors.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/files.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/host.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/infra.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/init.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/meta.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/paths.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/readfile.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/service.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/switch.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/template.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/files.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/main.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/remote.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/cli/switch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/__init__.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/linux.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 infrable-0.1.2/infrable/distro/ubuntu.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 infrable-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 infrable-0.1.2/LICENSE
+-rw-r--r--   0        0        0    17862 2020-02-02 00:00:00.000000 infrable-0.1.2/README.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 infrable-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    31688 2020-02-02 00:00:00.000000 infrable-0.1.2/PKG-INFO
```

### Comparing `infrable-0.1.1/infrable/errors.py` & `infrable-0.1.2/infrable/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class SwitchCaseError(Error, ValueError):
     def __init__(self, path, options, cases):
         _options = ", ".join(options)
         _cases = ", ".join(cases.keys())
 
         super().__init__(
-            f"{path}: all options are not covered by cases."
+            f"{path}: cases are incompatible with the options."
             f" Options are: {_options}, Cases are: {_cases}"
         )
 
 
 class SwitchError(Error, ValueError):
     def __init__(self, path, val, cases):
         _cases = ", ".join(cases.keys())
```

### Comparing `infrable-0.1.1/infrable/files.py` & `infrable-0.1.2/infrable/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/host.py` & `infrable-0.1.2/infrable/host.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/infra.py` & `infrable-0.1.2/infrable/infra.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/init.py` & `infrable-0.1.2/infrable/init.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/readfile.py` & `infrable-0.1.2/infrable/readfile.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/service.py` & `infrable-0.1.2/infrable/service.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/switch.py` & `infrable-0.1.2/infrable/switch.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,28 @@
     meta: Meta = field(default_factory=Meta)
 
     def __post_init__(self):
         self.path = paths.switches / "-".join(sorted(self.options))
         if not self.path.exists():
             self.set(self.init)
 
-    def __call__(self, **cases: Any) -> Any:
+    def __call__(self, **cases: Any) -> Any | None:
+        """Get the current value of the switch. returns None if not defined."""
+
+        if not cases:
+            cases = {opt: opt for opt in self.options}
+        elif len(set(cases.keys()) - self.options) > 0:
+            raise errors.SwitchCaseError(self.path, options=self.options, cases=cases)
+
+        val = self.path.read_text().strip()
+        return cases.get(val)
+
+    def strict(self, **cases: Any) -> Any:
+        """Strictly require all cases to be defined."""
+
         if not cases:
             cases = {opt: opt for opt in self.options}
         elif set(cases.keys()) != self.options:
             raise errors.SwitchCaseError(self.path, options=self.options, cases=cases)
 
         val = self.path.read_text().strip()
         if val in cases:
```

### Comparing `infrable-0.1.1/infrable/template.py` & `infrable-0.1.2/infrable/template.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/util.py` & `infrable-0.1.2/infrable/util.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/cli/files.py` & `infrable-0.1.2/infrable/cli/files.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/cli/main.py` & `infrable-0.1.2/infrable/cli/main.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/cli/remote.py` & `infrable-0.1.2/infrable/cli/remote.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/distro/linux.py` & `infrable-0.1.2/infrable/distro/linux.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/infrable/distro/ubuntu.py` & `infrable-0.1.2/infrable/distro/ubuntu.py`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/.gitignore` & `infrable-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/LICENSE` & `infrable-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/README.md` & `infrable-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/pyproject.toml` & `infrable-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infrable-0.1.1/PKG-INFO` & `infrable-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: infrable
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hanny's legendary infrastructure as code solution.
 Project-URL: Homepage, https://github.com/stckme/infrable
 Author-email: Arijit Basu <sayanarijit@gmail.com>
 Maintainer-email: Arijit Basu <sayanarijit@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

