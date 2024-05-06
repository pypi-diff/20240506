# Comparing `tmp/types-regex-2024.4.28.20240430.tar.gz` & `tmp/types-regex-2024.4.28.20240506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2024.4.28.20240430.tar", last modified: Tue Apr 30 02:17:33 2024, max compression
+gzip compressed data, was "types-regex-2024.4.28.20240506.tar", last modified: Mon May  6 02:22:04 2024, max compression
```

## Comparing `types-regex-2024.4.28.20240430.tar` & `types-regex-2024.4.28.20240506.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:17:33.216557 types-regex-2024.4.28.20240430/
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-30 02:17:31.000000 types-regex-2024.4.28.20240430/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 02:17:31.000000 types-regex-2024.4.28.20240430/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-30 02:17:33.212557 types-regex-2024.4.28.20240430/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:17:33.212557 types-regex-2024.4.28.20240430/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 02:17:31.000000 types-regex-2024.4.28.20240430/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 02:17:20.000000 types-regex-2024.4.28.20240430/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 02:17:20.000000 types-regex-2024.4.28.20240430/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-30 02:17:20.000000 types-regex-2024.4.28.20240430/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 02:17:31.000000 types-regex-2024.4.28.20240430/regex-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-04-30 02:17:20.000000 types-regex-2024.4.28.20240430/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:17:33.216557 types-regex-2024.4.28.20240430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-30 02:17:31.000000 types-regex-2024.4.28.20240430/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:17:33.212557 types-regex-2024.4.28.20240430/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-30 02:17:33.000000 types-regex-2024.4.28.20240430/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 02:17:33.000000 types-regex-2024.4.28.20240430/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:17:33.000000 types-regex-2024.4.28.20240430/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 02:17:33.000000 types-regex-2024.4.28.20240430/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.844860 types-regex-2024.4.28.20240506/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-06 02:21:48.000000 types-regex-2024.4.28.20240506/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-06 02:22:02.000000 types-regex-2024.4.28.20240506/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 02:22:04.848860 types-regex-2024.4.28.20240506/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 02:22:04.000000 types-regex-2024.4.28.20240506/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2024.4.28.20240430/CHANGELOG.md` & `types-regex-2024.4.28.20240506/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 2024.4.28.20240506 (2024-05-06)
+
+regex: improve Pattern annotations (#11862)
+
+- Corrected types for `pos` and `endpos` arguments to `int | None = None`
+- Corrected type for `timeout` argument to `float | None = None`
+- Added default value `None` for `concurrent` and `timeout` parameters
+- Added default value `0` for `maxsplit` parameter
+- Added `partial` parameter where applicable
+- Removed invalid `flags` parameter from `sub` methods
+
 ## 2024.4.28.20240430 (2024-04-30)
 
 [stubsabot] Bump regex to 2024.4.28 (#11842)
 
 Release: https://pypi.org/pypi/regex/2024.4.28
 Homepage: https://github.com/mrabarnett/mrab-regex
 Repository: https://github.com/mrabarnett/mrab-regex
```

### Comparing `types-regex-2024.4.28.20240430/PKG-INFO` & `types-regex-2024.4.28.20240506/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.28.20240430
+Version: 2024.4.28.20240506
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.28`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9178f5a4142abe3721615329fefed415f71b9897` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

### Comparing `types-regex-2024.4.28.20240430/regex-stubs/_regex.pyi` & `types-regex-2024.4.28.20240506/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.28.20240430/regex-stubs/_regex_core.pyi` & `types-regex-2024.4.28.20240506/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.4.28.20240430/regex-stubs/regex.pyi` & `types-regex-2024.4.28.20240506/regex-stubs/regex.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -331,243 +331,245 @@
     def pattern(self) -> AnyStr: ...
     @property
     def named_lists(self) -> Mapping[str, frozenset[AnyStr]]: ...
     @overload
     def search(
         self: Pattern[str],
         string: str,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[str] | None: ...
     @overload
     def search(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[bytes] | None: ...
     @overload
     def match(
         self: Pattern[str],
         string: str,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[str] | None: ...
     @overload
     def match(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[bytes] | None: ...
     @overload
     def fullmatch(
         self: Pattern[str],
         string: str,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[str] | None: ...
     @overload
     def fullmatch(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        pos: int = ...,
-        endpos: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> Match[bytes] | None: ...
     @overload
     def split(
-        self: Pattern[str], string: str, maxsplit: int = ..., concurrent: bool | None = ..., timeout: float | None = ...
+        self: Pattern[str], string: str, maxsplit: int = 0, concurrent: bool | None = None, timeout: float | None = None
     ) -> list[str | Any]: ...
     @overload
     def split(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        maxsplit: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        maxsplit: int = 0,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> list[bytes | Any]: ...
     @overload
     def splititer(
-        self: Pattern[str], string: str, maxsplit: int = ..., concurrent: bool | None = ..., timeout: float | None = ...
+        self: Pattern[str], string: str, maxsplit: int = 0, concurrent: bool | None = None, timeout: float | None = None
     ) -> _regex.Splitter[str]: ...
     @overload
     def splititer(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        maxsplit: int = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        maxsplit: int = 0,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> _regex.Splitter[bytes]: ...
     @overload
     def findall(
         self: Pattern[str],
         string: str,
-        pos: int = ...,
-        endpos: int = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> list[Any]: ...
     @overload
     def findall(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        pos: int = ...,
-        endpos: int = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> list[Any]: ...
     @overload
     def finditer(
         self: Pattern[str],
         string: str,
-        pos: int = ...,
-        endpos: int = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> _regex.Scanner[str]: ...
     @overload
     def finditer(
         self: Pattern[bytes],
         string: ReadableBuffer,
-        pos: int = ...,
-        endpos: int = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> _regex.Scanner[bytes]: ...
     @overload
     def sub(
         self: Pattern[str],
         repl: str | Callable[[Match[str]], str],
         string: str,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> str: ...
     @overload
     def sub(
         self: Pattern[bytes],
         repl: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
         string: ReadableBuffer,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> bytes: ...
     @overload
     def subf(
         self: Pattern[str],
         format: str | Callable[[Match[str]], str],
         string: str,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> str: ...
     @overload
     def subf(
         self: Pattern[bytes],
         format: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
         string: ReadableBuffer,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> bytes: ...
     @overload
     def subn(
         self: Pattern[str],
         repl: str | Callable[[Match[str]], str],
         string: str,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> tuple[str, int]: ...
     @overload
     def subn(
         self: Pattern[bytes],
         repl: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
         string: ReadableBuffer,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> tuple[bytes, int]: ...
     @overload
     def subfn(
         self: Pattern[str],
         format: str | Callable[[Match[str]], str],
         string: str,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> tuple[str, int]: ...
     @overload
     def subfn(
         self: Pattern[bytes],
         format: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
         string: ReadableBuffer,
-        count: int = ...,
-        flags: int = ...,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        count: int = 0,
+        pos: int | None = None,
+        endpos: int | None = None,
+        concurrent: bool | None = None,
+        timeout: float | None = None,
     ) -> tuple[bytes, int]: ...
     @overload
     def scanner(
         self: Pattern[str],
         string: str,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> _regex.Scanner[str]: ...
     @overload
     def scanner(
         self: Pattern[bytes],
         string: bytes,
-        pos: int | None = ...,
-        endpos: int | None = ...,
-        overlapped: bool = ...,
-        concurrent: bool | None = ...,
-        timeout: float | None = ...,
+        pos: int | None = None,
+        endpos: int | None = None,
+        overlapped: bool = False,
+        concurrent: bool | None = None,
+        partial: bool = False,
+        timeout: float | None = None,
     ) -> _regex.Scanner[bytes]: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self) -> Self: ...
     if sys.version_info >= (3, 9):
         def __class_getitem__(cls, item: Any) -> GenericAlias: ...
 
 @final
```

### Comparing `types-regex-2024.4.28.20240430/setup.py` & `types-regex-2024.4.28.20240506/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.28`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9178f5a4142abe3721615329fefed415f71b9897` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.4.28.20240430",
+      version="2024.4.28.20240506",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2024.4.28.20240430/types_regex.egg-info/PKG-INFO` & `types-regex-2024.4.28.20240506/types_regex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.4.28.20240430
+Version: 2024.4.28.20240506
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.4.28`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9178f5a4142abe3721615329fefed415f71b9897` and was tested
-with mypy 1.10.0, pyright 1.1.360, and
+This package was generated from typeshed commit `8ff50fbea2f607380c23d9b120fccfb1926284e5` and was tested
+with mypy 1.10.0, pyright 1.1.361, and
 pytype 2024.4.11.
```

