# Comparing `tmp/gyver-4.1.7.tar.gz` & `tmp/gyver-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-4.1.7.tar", max compression
+gzip compressed data, was "gyver-4.1.8.tar", max compression
```

## Comparing `gyver-4.1.7.tar` & `gyver-4.1.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.7/LICENSE
--rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.7/README.md
--rw-r--r--   0        0        0      158 2024-04-24 16:58:16.417729 gyver-4.1.7/gyver/__init__.py
--rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1066 2024-04-21 04:46:15.029128 gyver-4.1.7/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     8089 2024-04-23 11:43:36.217124 gyver-4.1.7/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/helpers.py
--rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/context.py
--rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/context/typedef.py
--rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/exc.py
--rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/model/__init__.py
--rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/model/v1.py
--rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/model/v2.py
--rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/py.typed
--rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/url/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-18 22:41:50.880985 gyver-4.1.7/gyver/url/core.py
--rw-r--r--   0        0        0      423 2024-04-18 20:01:32.234522 gyver-4.1.7/gyver/url/encode.py
--rw-r--r--   0        0        0     1631 2024-04-18 22:41:41.627434 gyver-4.1.7/gyver/url/fragment.py
--rw-r--r--   0        0        0     5027 2024-04-19 02:03:56.058338 gyver-4.1.7/gyver/url/netloc.py
--rw-r--r--   0        0        0     4830 2024-04-18 22:40:58.819756 gyver-4.1.7/gyver/url/path.py
--rw-r--r--   0        0        0     4022 2024-04-18 22:42:15.161559 gyver-4.1.7/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/url/utils.py
--rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/utils/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/utils/exc.py
--rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/utils/finder.py
--rw-r--r--   0        0        0     4762 2024-04-20 18:11:24.474173 gyver-4.1.7/gyver/utils/helpers.py
--rw-r--r--   0        0        0     1676 2024-04-20 18:13:47.304318 gyver-4.1.7/gyver/utils/json.py
--rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/utils/strings.py
--rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.7/gyver/utils/timezone.py
--rw-r--r--   0        0        0     1624 2024-04-24 16:58:16.431063 gyver-4.1.7/pyproject.toml
--rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 gyver-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-28 22:08:41.323819 gyver-4.1.8/LICENSE
+-rw-r--r--   0        0        0      610 2024-03-28 22:08:41.323819 gyver-4.1.8/README.md
+-rw-r--r--   0        0        0      158 2024-05-06 09:26:42.429092 gyver-4.1.8/gyver/__init__.py
+-rw-r--r--   0        0        0      795 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1315 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1066 2024-04-21 04:46:15.029128 gyver-4.1.8/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     8089 2024-04-23 11:43:36.217124 gyver-4.1.8/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1043 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     6716 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/helpers.py
+-rw-r--r--   0        0        0     2111 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     2014 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     2105 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0      419 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     3880 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2358 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     2734 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5447 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1984 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/context/typedef.py
+-rw-r--r--   0        0        0     2667 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/exc.py
+-rw-r--r--   0        0        0      225 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1748 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3248 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2865 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      111 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/model/__init__.py
+-rw-r--r--   0        0        0     1804 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/model/v1.py
+-rw-r--r--   0        0        0     1793 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/model/v2.py
+-rw-r--r--   0        0        0      101 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/py.typed
+-rw-r--r--   0        0        0      186 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/url/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-18 22:41:50.880985 gyver-4.1.8/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2024-04-18 20:01:32.234522 gyver-4.1.8/gyver/url/encode.py
+-rw-r--r--   0        0        0     1631 2024-04-18 22:41:41.627434 gyver-4.1.8/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5027 2024-04-19 02:03:56.058338 gyver-4.1.8/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4830 2024-04-18 22:40:58.819756 gyver-4.1.8/gyver/url/path.py
+-rw-r--r--   0        0        0     5837 2024-05-06 09:25:28.033860 gyver-4.1.8/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/url/utils.py
+-rw-r--r--   0        0        0      579 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/utils/__init__.py
+-rw-r--r--   0        0        0     1041 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/utils/exc.py
+-rw-r--r--   0        0        0    12855 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4762 2024-04-20 18:11:24.474173 gyver-4.1.8/gyver/utils/helpers.py
+-rw-r--r--   0        0        0     1676 2024-04-20 18:13:47.304318 gyver-4.1.8/gyver/utils/json.py
+-rw-r--r--   0        0        0     2749 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/utils/strings.py
+-rw-r--r--   0        0        0     1100 2024-03-28 22:08:41.327153 gyver-4.1.8/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     1624 2024-05-06 09:26:42.442426 gyver-4.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 gyver-4.1.8/PKG-INFO
```

### Comparing `gyver-4.1.7/LICENSE` & `gyver-4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/README.md` & `gyver-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/__init__.py` & `gyver-4.1.8/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/attrs.py` & `gyver-4.1.8/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/dataclass.py` & `gyver-4.1.8/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/factory.py` & `gyver-4.1.8/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/gattrs.py` & `gyver-4.1.8/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/helpers.py` & `gyver-4.1.8/gyver/config/adapter/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/interface.py` & `gyver-4.1.8/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/mark.py` & `gyver-4.1.8/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/config/adapter/pydantic.py` & `gyver-4.1.8/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/context/atomic_/bound.py` & `gyver-4.1.8/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/context/atomic_/core.py` & `gyver-4.1.8/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/context/atomic_/resolver.py` & `gyver-4.1.8/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/context/context.py` & `gyver-4.1.8/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/context/interfaces/adapter.py` & `gyver-4.1.8/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/exc.py` & `gyver-4.1.8/gyver/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/filetree/filetree.py` & `gyver-4.1.8/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/filetree/interface.py` & `gyver-4.1.8/gyver/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/filetree/typedef.py` & `gyver-4.1.8/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/filetree/virtual.py` & `gyver-4.1.8/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/model/v1.py` & `gyver-4.1.8/gyver/model/v1.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/model/v2.py` & `gyver-4.1.8/gyver/model/v2.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/pools/asyncio.py` & `gyver-4.1.8/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/pools/resource.py` & `gyver-4.1.8/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/pools/thread.py` & `gyver-4.1.8/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/url/core.py` & `gyver-4.1.8/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/url/fragment.py` & `gyver-4.1.8/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/url/netloc.py` & `gyver-4.1.8/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/url/path.py` & `gyver-4.1.8/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/url/query.py` & `gyver-4.1.8/gyver/url/query.py`

 * *Files 27% similar despite different names*

```diff
@@ -123,7 +123,50 @@
         self.params = defaultdict(list, sorted(self.params.items()))
         return self
 
     def copy(self) -> "Query":
         query = object.__new__(type(self))
         query.params = self.params.copy()
         return query
+
+    def first(self) -> dict[str, str]:
+        """Return a dictionary containing the first value for each query parameter.
+
+        Returns:
+            dict[str, str]: A dictionary where keys are query parameter names
+                and values are the first values associated with those parameters.
+        """
+        return {key: value[0] for key, value in self.params.items()}
+
+    def index_or_first(self, idx: int) -> dict[str, str]:
+        """Return a dictionary containing the value at index 'idx' for each query parameter,
+        or the first value if 'idx' exceeds the length of the parameter's value list.
+
+        Args:
+            idx (int): The index to retrieve for each query parameter.
+
+        Returns:
+            dict[str, str]: A dictionary where keys are query parameter names
+                and values are the values at index 'idx' or the first values
+                if 'idx' exceeds the length of the parameter's value list.
+        """
+        return {
+            key: value[0 if len(value) <= idx else idx]
+            for key, value in self.params.items()
+        }
+
+    def index_or_last(self, idx: int) -> dict[str, str]:
+        """Return a dictionary containing the value at index 'idx' for each query parameter,
+        or the last value if 'idx' exceeds the length of the parameter's value list.
+
+        Args:
+            idx (int): The index to retrieve for each query parameter.
+
+        Returns:
+            dict[str, str]: A dictionary where keys are query parameter names
+                and values are the values at index 'idx' or the last values
+                if 'idx' exceeds the length of the parameter's value list.
+        """
+        return {
+            key: value[-1 if len(value) <= idx else idx]
+            for key, value in self.params.items()
+        }
```

### Comparing `gyver-4.1.7/gyver/url/utils.py` & `gyver-4.1.8/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/__init__.py` & `gyver-4.1.8/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/exc.py` & `gyver-4.1.8/gyver/utils/exc.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/finder.py` & `gyver-4.1.8/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/helpers.py` & `gyver-4.1.8/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/json.py` & `gyver-4.1.8/gyver/utils/json.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/strings.py` & `gyver-4.1.8/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/gyver/utils/timezone.py` & `gyver-4.1.8/gyver/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `gyver-4.1.7/pyproject.toml` & `gyver-4.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "4.1.7"
+version = "4.1.8"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gyver-4.1.7/PKG-INFO` & `gyver-4.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 4.1.7
+Version: 4.1.8
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

