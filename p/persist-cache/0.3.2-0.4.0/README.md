# Comparing `tmp/persist_cache-0.3.2.tar.gz` & `tmp/persist_cache-0.4.0.tar.gz`

## Comparing `persist_cache-0.3.2.tar` & `persist_cache-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 persist_cache-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 persist_cache-0.3.2/.github/workflows/bench.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 persist_cache-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/caching.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/helpers.py
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/persist_cache.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/pickle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/py.typed
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 persist_cache-0.3.2/src/persist_cache/serialization.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/bench.py
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/test_persist_cache.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/.gitignore
--rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af___init___py.html
--rw-r--r--   0        0        0    28319 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_caching_py.html
--rw-r--r--   0        0        0    24941 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_helpers_py.html
--rw-r--r--   0        0        0    43073 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_persist_cache_py.html
--rw-r--r--   0        0        0    46292 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_serialization_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/status.json
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 persist_cache-0.3.2/tests/htmlcov/style.css
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 persist_cache-0.3.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 persist_cache-0.3.2/LICENCE
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 persist_cache-0.3.2/README.md
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 persist_cache-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 persist_cache-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 persist_cache-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 persist_cache-0.4.0/.github/workflows/bench.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 persist_cache-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 persist_cache-0.4.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/caching.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/helpers.py
+-rw-r--r--   0        0        0    12523 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/persist_cache.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/pickle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/py.typed
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 persist_cache-0.4.0/src/persist_cache/serialization.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/bench.py
+-rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/test_persist_cache.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/.gitignore
+-rw-r--r--   0        0        0    22489 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af___init___py.html
+-rw-r--r--   0        0        0    31134 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_caching_py.html
+-rw-r--r--   0        0        0    24959 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_helpers_py.html
+-rw-r--r--   0        0        0    71001 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_persist_cache_py.html
+-rw-r--r--   0        0        0     8604 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_pickle_py.html
+-rw-r--r--   0        0        0    46522 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_serialization_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/status.json
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 persist_cache-0.4.0/tests/htmlcov/style.css
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 persist_cache-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 persist_cache-0.4.0/LICENCE
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 persist_cache-0.4.0/README.md
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 persist_cache-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 persist_cache-0.4.0/PKG-INFO
```

### Comparing `persist_cache-0.3.2/CHANGELOG.md` & `persist_cache-0.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ## Changelog 🔄
 All notable changes to `persist-cache` will be documented here. This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] - 2024-05-06
+## Added
+- Added support for the caching of both synchronous and asynchronous generator functions.
+- Added `delete()`, `clear()` and `flush()` helper functions for deleting, clearing and flushing caches.
+
 ## [0.3.2] - 2024-03-21
 ### Changed
 - Began hashing the names of caches with `XXH3` to ensure caches may be assigned any arbitrary name, regardless of whether it is compatible with the local file system.
 
 ## [0.3.1] - 2024-03-20
 ### Fixed
 - Fixed a bug causing `cache()` to raise a `TypeError` when attempting to cache a function call that contains an argument that is a list containing a dictionary ([#4](https://github.com/umarbutler/persist-cache/issues/4)) ([ec07874](https://github.com/umarbutler/persist-cache/commit/ec07874)).
@@ -34,12 +39,14 @@
 - Fixed `cache()`'s inability to identify certain wrapped asynchronous functions and methods as being asynchronous ([#1](https://github.com/umarbutler/persist-cache/issues/1)) ([fe7aa6c](https://github.com/umarbutler/persist-cache/commit/fe7aa6ccd2f7fbeebaa53e4c1cc0230f6ef35cb4)).
 - Fixed `cache()`'s inability to cache function calls returning `bytes`, `bytearray` and `memoryview` objects ([#2](https://github.com/umarbutler/persist-cache/issues/2)) ([f763ce7](https://github.com/umarbutler/persist-cache/commit/f763ce7040c8048112dc93b59991bbcf943cc33a)).
 
 ## [0.1.0] - 2024-03-12
 ### Added
 - Added the `cache()` decorator, which locally and persistently caches functions.
 
+[0.4.0]: https://github.com/umarbutler/persist-cache/compare/v0.3.2...v0.4.0
+[0.3.2]: https://github.com/umarbutler/persist-cache/compare/v0.3.1...v0.3.2
 [0.3.1]: https://github.com/umarbutler/persist-cache/compare/v0.3.0...v0.3.1
 [0.3.0]: https://github.com/umarbutler/persist-cache/compare/v0.2.0...v0.3.0
 [0.2.0]: https://github.com/umarbutler/persist-cache/compare/v0.1.1...v0.2.0
 [0.1.1]: https://github.com/umarbutler/persist-cache/compare/v0.1.0...v0.1.1
 [0.1.0]: https://github.com/umarbutler/persist-cache/releases/tag/v0.1.0
```

### Comparing `persist_cache-0.3.2/.github/workflows/bench.yml` & `persist_cache-0.4.0/.github/workflows/bench.yml`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/.github/workflows/ci.yml` & `persist_cache-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/src/persist_cache/caching.py` & `persist_cache-0.4.0/src/persist_cache/caching.py`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/src/persist_cache/helpers.py` & `persist_cache-0.4.0/src/persist_cache/helpers.py`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/src/persist_cache/persist_cache.py` & `persist_cache-0.4.0/src/persist_cache/persist_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -85,16 +85,79 @@
             # Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.
             if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE:
                 value = await func(*args, **kwargs)
                 caching.set(key, value, dir)
             
             return value
         
-        # Identify the appropriate wrapper for the function by checking whether it is asynchronous or not.
-        wrapper = async_wrapper if is_async(func) else sync_wrapper
+        # Initialise a wrapper for generator functions.
+        def generator_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any:
+            nonlocal dir, expiry, is_method
+
+            # Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.
+            arguments = inflate_arguments(signature, args_parameter, args_i, args[is_method:], kwargs)
+            
+            # Hash the arguments to produce the cache key.
+            key = caching.hash(arguments)
+            
+            # Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.
+            if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE:
+                value = []
+                
+                for item in func(*args, **kwargs):
+                    value.append(item)
+                    
+                    yield item
+
+                caching.set(key, value, dir)
+                
+                return
+
+            for item in value:
+                yield item
+        
+        # Initialise a wrapper for asynchronous generator functions.
+        async def async_generator_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any:
+            nonlocal dir, expiry, is_method
+
+            # Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.
+            arguments = inflate_arguments(signature, args_parameter, args_i, args[is_method:], kwargs)
+            
+            # Hash the arguments to produce the cache key.
+            key = caching.hash(arguments)
+            
+            # Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.
+            if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE:
+                value = []
+                
+                async for item in func(*args, **kwargs):
+                    value.append(item)
+                    
+                    yield item
+
+                caching.set(key, value, dir)
+                
+                return
+
+            for item in value:
+                yield item
+
+        # Identify the appropriate wrapper for the function.
+        if is_async(func):
+            if inspect.isasyncgenfunction(func):
+                wrapper = async_generator_wrapper
+            
+            else:
+                wrapper = async_wrapper
+        
+        elif inspect.isgeneratorfunction(func):
+            wrapper = generator_wrapper
+        
+        else:
+            wrapper = sync_wrapper
         
         # Attach convenience functions to the wrapper for modifying the cache.
         def delete_cache() -> None:
             """Delete the cache."""
             nonlocal dir
             
             caching.delete(dir)
@@ -107,16 +170,20 @@
         
         def flush_cache() -> None:
             """Flush expired keys from the cache."""
             nonlocal dir, expiry, is_method
             
             caching.flush(dir, expiry)
         
-        def set_expiry(value: int) -> None:
-            """Set the expiry of the cache."""
+        def set_expiry(value: Union[int, float, timedelta, None]) -> None:
+            """Set the expiry of the cache.
+            
+            Arguments:
+                expiry (`int | float | timedelta`): How long, in seconds or as a `timedelta`, function calls should persist in the cache."""
+
             nonlocal expiry
             
             expiry = value
         
         wrapper.delete_cache = delete_cache
         wrapper.clear_cache = clear_cache
         wrapper.cache_clear = wrapper.clear_cache # Add an alias for cache_clear which is used by lru_cache.
@@ -134,8 +201,36 @@
     # If the first argument is a function and all of the other arguments are `None`, indicating that this decorator factory was invoked without passing any arguments, return the result of passing that function to the decorator while also emptying the first argument to avoid it being used by the decorator.
     if callable(name) and dir is expiry is None:
         func = name
         name = None
         
         return decorator(func)
     
-    return decorator
+    return decorator
+
+def delete(function_or_name: Union[str, Callable]) -> None:
+    """Delete the cache of the given function or name.
+    
+    Arguments:
+        function_or_name (`str | Callable`): The function or name of the cache to be deleted."""
+    
+    name = function_or_name if isinstance(function_or_name, str) else function_or_name.__qualname__
+    caching.delete(f'.persist_cache/{caching.shorthash(name)}')
+
+def clear(function_or_name: Union[str, Callable]) -> None:
+    """Clear the cache of the given function or name.
+    
+    Arguments:
+        function_or_name (`str | Callable`): The function or name of the cache to be cleared."""
+    
+    name = function_or_name if isinstance(function_or_name, str) else function_or_name.__qualname__
+    caching.clear(f'.persist_cache/{caching.shorthash(name)}')
+
+def flush(function_or_name: Union[str, Callable], expiry: Union[int, float, timedelta]) -> None:
+    """Flush expired keys from the cache of the given function or name.
+    
+    Arguments:
+        function_or_name (`str | Callable`): The function or name of the cache to be flushed.
+        expiry (`int | float | timedelta`): How long, in seconds or as a `timedelta`, function calls should persist in the cache."""
+    
+    name = function_or_name if isinstance(function_or_name, str) else function_or_name.__qualname__
+    caching.flush(f'.persist_cache/{caching.shorthash(name)}', expiry)
```

### Comparing `persist_cache-0.3.2/src/persist_cache/serialization.py` & `persist_cache-0.4.0/src/persist_cache/serialization.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import pickle
 from typing import Any, Union
 
 import msgspec
-import pickle
 
 Msgpackables = Union[str, int, list, dict, bool, float, None]
 """Types that are directly msgpackable."""
 
 # Initialise msgpack encoders and decoders once to speed up subsequent serialization and deserialization.
 msgpack_encoder = msgspec.msgpack.Encoder()
 msgpack_decoder = msgspec.msgpack.Decoder(type=Msgpackables)
```

### Comparing `persist_cache-0.3.2/tests/bench.py` & `persist_cache-0.4.0/tests/bench.py`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/tests/test_persist_cache.py` & `persist_cache-0.4.0/tests/test_persist_cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test persist-cache."""
 import os
 import random
 import shutil
 import time
-from typing import Callable, Union
+from typing import AsyncGenerator, Callable, Generator, Union
 
 import persist_cache
 
 
 def _time_consuming_function(
     *args,
     str_: str = None,
@@ -46,14 +46,26 @@
     class_: type = None,
     recursive: dict[str, Union[list[tuple[bytes, bool]], float]] = None,
 ) -> tuple[str, int, list[int], dict[str, int], tuple[int, str], set[int], frozenset[int], bytes, bytearray, bool, float, None, type, dict[str, Union[list[tuple[bytes, bool]], float]], float]:
     """A time-consuming function."""
     
     return str_, int_, list_, dict_, tuple_, set_, frozenset_, bytes_, bytearray_, bool_, float_, none_, class_, recursive, random.random()
 
+def _time_consuming_generator_function(x: int) -> Generator[int, None, None]:
+    """A time-consuming generator function."""
+    
+    for i in range(x):
+        yield i
+
+async def _async_time_consuming_generator_function(x: int) -> AsyncGenerator[int, None]:
+    """A time-consuming generator function."""
+    
+    for i in range(x):
+        yield i
+
 class _TimeConsumingClass:
     def _time_consuming_function(
         self,
         *args,
         str_: str = None,
         int_: int = None,
         list_: list[int] = None,
@@ -140,21 +152,32 @@
     keyword_data_sample = {field: value for i, (field, value) in enumerate(data.items()) if i >= 5}
     assert cached_function(*positional_data_sample, **keyword_data_sample) == cached_function(*positional_data_sample, **keyword_data_sample)
     
     # Test clearing the cache.
     cached_result = cached_function(**data)
     cached_function.clear_cache()
     assert cached_function(**data) != cached_result
+    
+    if dir is None:
+        cached_result = cached_function(**data)
+        persist_cache.clear(cached_function)
+        assert cached_function(**data) != cached_result
 
     # Test flushing the cache.
     if expiry:
         cached_result = cached_function(**data)
-        time.sleep(expiry+1)
+        time.sleep(expiry + 1)
         cached_function.flush_cache()
         assert cached_function(**data) != cached_result
+        
+        if dir is None:
+            cached_result = cached_function(**data)
+            time.sleep(expiry + 1)
+            persist_cache.flush(cached_function, expiry)
+            assert cached_function(**data) != cached_result
 
     # Test setting the time-to-live of the cache.
     cached_function.set_expiry(2)
     cached_result = cached_function(**data)
     time.sleep(3)
     assert cached_function(**data) != cached_result
     
@@ -208,33 +231,72 @@
     keyword_data_sample = {field: value for i, (field, value) in enumerate(data.items()) if i >= 5}
     assert await cached_function(*positional_data_sample, **keyword_data_sample) == await cached_function(*positional_data_sample, **keyword_data_sample)
     
     # Test clearing the cache.
     cached_result = await cached_function(**data)
     cached_function.clear_cache()
     assert await cached_function(**data) != cached_result
+    
+    if dir is None:
+        cached_result = await cached_function(**data)
+        persist_cache.clear(cached_function)
+        assert await cached_function(**data) != cached_result
 
     # Test flushing the cache.
     if expiry:
         cached_result = await cached_function(**data)
-        time.sleep(expiry+1)
+        time.sleep(expiry + 1)
         cached_function.flush_cache()
         assert await cached_function(**data) != cached_result
+        
+        if dir is None:
+            cached_result = await cached_function(**data)
+            time.sleep(expiry + 1)
+            persist_cache.flush(cached_function, expiry)
+            assert await cached_function(**data) != cached_result
 
     # Test setting the time-to-live of the cache.
     cached_function.set_expiry(2)
     cached_result = await cached_function(**data)
     time.sleep(3)
     assert await cached_function(**data) != cached_result
     
     # Test deleting the cache if the cache's directory is known.
     if dir:
         cached_function.delete_cache()
         assert not os.path.exists(dir)
 
+def _test_cached_generator_function(cached_generator_function: Callable, dir: str = None, expiry: int = None) -> None:
+    """Test a cached generator function."""
+    
+    # Initialise test data.
+    data = 10
+    
+    # Test the caching of the time-consuming generator function's responses to the test data.
+    assert list(cached_generator_function(data)) == list(cached_generator_function(data))
+ 
+async def _async_test_cached_generator_function(cached_generator_function: Callable, dir: str = None, expiry: int = None) -> None:
+    """Test an async cached generator function."""
+    
+    # Initialise test data.
+    data = 10
+    
+    # Test the caching of the time-consuming generator function's responses to the test data.
+    y1 = []
+    
+    async for element in cached_generator_function(data):
+        y1 += [element]
+    
+    y2 = []
+    
+    async for element in cached_generator_function(data):
+        y2 += [element]
+    
+    assert y1 == y2
+
 async def _test_sync_and_async_time_consuming_function(_time_consuming_function: Callable, _async_time_consuming_function: Callable) -> None:
     """Test a time-consuming function and its async equivalent."""
     
     # Cache and test the time-consuming function without arguments.
     cached_function = persist_cache.cache(_time_consuming_function)
     print('Testing the caching of the time-consuming function without arguments.')
     _test_cached_function(cached_function)
@@ -285,14 +347,24 @@
     _test_cached_function(cached_function, dir='.persist_cache/custom_function')
     
     # Cache and test the async time-consuming function with a custom name.
     cached_function = persist_cache.cache(name='.custom_function')(_async_time_consuming_function)
     print('Testing the caching of the async time-consuming function with a custom directory.')
     await _async_test_cached_function(cached_function, dir='.persist_cache/custom_function')
     
+    # Cache and test the time-consuming generator function.
+    cached_generator_function = persist_cache.cache()(_time_consuming_generator_function)
+    print('Testing the caching of the time-consuming generator function.')
+    _test_cached_generator_function(cached_generator_function)
+    
+    # Cache and test the async time-consuming generator function.
+    cached_generator_function = persist_cache.cache()(_async_time_consuming_generator_function)
+    print('Testing the caching of the async time-consuming generator function.')
+    await _async_test_cached_generator_function(cached_generator_function)
+    
     # Remove cache directories.
     for dir in {'.persist_cache', '.custom_cache'}:
         shutil.rmtree(dir, ignore_errors=True)
 
 async def test_persist_cache() -> None:
     """Test `persist_cache.persist_cache()`."""
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/coverage_html.js` & `persist_cache-0.4.0/tests/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af___init___py.html` & `persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_caching_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 20:59 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -78,23 +78,23 @@
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""An easy-to-use Python library for lightning-fast persistent function caching."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">persist_cache</span> <span class="key">import</span> <span class="nam">cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">persist_cache</span> <span class="key">import</span> <span class="nam">cache</span><span class="op">,</span> <span class="nam">clear</span><span class="op">,</span> <span class="nam">delete</span><span class="op">,</span> <span class="nam">flush</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_caching_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 20:59 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  11 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 20:59 +1100
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
 _1"""An easy-to-use Python library for lightning-fast persistent function
 caching.""" 
 _2 
-_3from .persist_cache import cache 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 20:59 +1100
+_3from .persist_cache import cache, clear, delete, flush 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_caching_py.html` & `persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_caching_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\caching.py: 100%</title>
+    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\caching.py: 81%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\caching.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">81%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">39 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">39<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <span class="text">43 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">35<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">8<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -82,15 +82,15 @@
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">shutil</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">datetime</span> <span class="key">import</span> <span class="nam">datetime</span><span class="op">,</span> <span class="nam">timedelta</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">filelock</span> <span class="key">import</span> <span class="nam">FileLock</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">xxhash</span> <span class="key">import</span> <span class="nam">xxh3_64_hexdigest</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">xxhash</span> <span class="key">import</span> <span class="nam">xxh3_64_hexdigest</span><span class="op">,</span> <span class="nam">xxh3_128_hexdigest</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">serialization</span> <span class="key">import</span> <span class="nam">deserialize</span><span class="op">,</span> <span class="nam">serialize</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">NOT_IN_CACHE</span> <span class="op">=</span> <span class="nam">object</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">"""A sentinel object that flags that a key is not in the cache."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">def</span> <span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">value</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -119,66 +119,79 @@
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="com"># Get the time at which the key was last set.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="nam">timestamp</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">getmtime</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="com"># If the entry is expired, remove it from the cache and return `NOT_IN_CACHE`.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">expiry</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">)</span> <span class="key">and</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">fromtimestamp</span><span class="op">(</span><span class="nam">timestamp</span><span class="op">)</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">or</span> <span class="nam">timestamp</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">timestamp</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="com"># Remove the entry.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">                <span class="key">return</span> <span class="nam">NOT_IN_CACHE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">                <span class="key">return</span> <span class="nam">NOT_IN_CACHE</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="com"># Read, deserialize and return the value.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">with</span> <span class="nam">open</span><span class="op">(</span><span class="nam">path</span><span class="op">,</span> <span class="str">'rb'</span><span class="op">)</span> <span class="key">as</span> <span class="nam">file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">                <span class="key">return</span> <span class="nam">deserialize</span><span class="op">(</span><span class="nam">file</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="key">def</span> <span class="nam">hash</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="str">"""Hash the given data."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="key">return</span> <span class="nam">xxh3_64_hexdigest</span><span class="op">(</span><span class="nam">serialize</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="key">def</span> <span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="str">"""Delete the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="com"># Remove the cache directory and all its contents.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="nam">shutil</span><span class="op">.</span><span class="nam">rmtree</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="key">def</span> <span class="nam">clear</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="str">"""Clear the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="com"># Delete the cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="com"># Recreate the cache directory.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">os</span><span class="op">.</span><span class="nam">makedirs</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t"><span class="key">def</span> <span class="nam">flush</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="str">"""Flush expired keys from the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="com"># Iterate over keys in the cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">for</span> <span class="nam">file</span> <span class="key">in</span> <span class="nam">os</span><span class="op">.</span><span class="nam">listdir</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">path</span> <span class="op">=</span> <span class="str">f'{dir}/{file}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="com"># Serialise the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">serialize</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="com"># Hash the data and affix its length, preceded by a hyphen (to reduce the likelihood of collisions).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">return</span> <span class="str">f'{xxh3_128_hexdigest(data)}{len(data)}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="key">def</span> <span class="nam">shorthash</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="str">"""Hash the given data."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="com"># Serialise the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">serialize</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="com"># Hash the data and affix its length, preceded by a hyphen (to reduce the likelihood of collisions).</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">return</span> <span class="str">f'{xxh3_64_hexdigest(data)}{len(data)}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="key">def</span> <span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="str">"""Delete the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="com"># Remove the cache directory and all its contents.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="nam">shutil</span><span class="op">.</span><span class="nam">rmtree</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">ignore_errors</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="key">def</span> <span class="nam">clear</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="str">"""Clear the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="com"># Lock the entry before reading it.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">with</span> <span class="nam">FileLock</span><span class="op">(</span><span class="str">f'{path}.lock'</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="com"># Get the time at which the key was last set.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="nam">timestamp</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">getmtime</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="com"># If the entry is expired, remove it from the cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">expiry</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">)</span> <span class="key">and</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">fromtimestamp</span><span class="op">(</span><span class="nam">timestamp</span><span class="op">)</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="key">or</span> <span class="op">(</span><span class="nam">timestamp</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">timestamp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">                <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="com"># Delete the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="com"># Recreate the cache directory.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">os</span><span class="op">.</span><span class="nam">makedirs</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="key">def</span> <span class="nam">flush</span><span class="op">(</span><span class="nam">dir</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="str">"""Flush expired keys from the provided cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="com"># Iterate over keys in the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="key">for</span> <span class="nam">file</span> <span class="key">in</span> <span class="nam">os</span><span class="op">.</span><span class="nam">listdir</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">path</span> <span class="op">=</span> <span class="str">f'{dir}/{file}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="com"># Lock the entry before reading it.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">with</span> <span class="nam">FileLock</span><span class="op">(</span><span class="str">f'{path}.lock'</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="com"># Get the time at which the key was last set.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">            <span class="nam">timestamp</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">getmtime</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">            <span class="com"># If the entry is expired, remove it from the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">expiry</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">)</span> <span class="key">and</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">fromtimestamp</span><span class="op">(</span><span class="nam">timestamp</span><span class="op">)</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">            <span class="key">or</span> <span class="op">(</span><span class="nam">timestamp</span> <span class="op">+</span> <span class="nam">expiry</span> <span class="op">&lt;</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">timestamp</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">                <span class="nam">os</span><span class="op">.</span><span class="nam">remove</span><span class="op">(</span><span class="nam">path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
 ************ CCoovveerraaggee ffoorr CC::\\PPyytthhoonn331111\\LLiibb\\ssiittee--ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\ccaacchhiinngg..ppyy::
-110000%% ************
+8811%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3399 ssttaatteemmeennttss ?  3399 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
+********** 4433 ssttaatteemmeennttss ?  3355 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
 _1import os 
 _2import shutil 
 _3from datetime import datetime, timedelta 
 _4from typing import Any, Union 
 _5 
 _6from filelock import FileLock 
-_7from xxhash import xxh3_64_hexdigest 
+_7from xxhash import xxh3_64_hexdigest, xxh3_128_hexdigest 
 _8 
 _9from .serialization import deserialize, serialize 
 _1_0 
 _1_1NOT_IN_CACHE = object() 
 _1_2"""A sentinel object that flags that a key is not in the cache.""" 
 _1_3 
 _1_4def set(key: str, value: Any, dir: str) -> None: 
@@ -66,43 +66,58 @@
 _4_8 # Read, deserialize and return the value. 
 _4_9 with open(path, 'rb') as file: 
 _5_0 return deserialize(file.read()) 
 _5_1 
 _5_2def hash(data: Any) -> str: 
 _5_3 """Hash the given data.""" 
 _5_4 
-_5_5 return xxh3_64_hexdigest(serialize(data)) 
-_5_6 
-_5_7def delete(dir: str) -> None: 
-_5_8 """Delete the provided cache.""" 
-_5_9 
-_6_0 # Remove the cache directory and all its contents. 
-_6_1 shutil.rmtree(dir, ignore_errors=True) 
-_6_2 
-_6_3def clear(dir: str) -> None: 
-_6_4 """Clear the provided cache.""" 
-_6_5 
-_6_6 # Delete the cache. 
-_6_7 delete(dir) 
-_6_8 
-_6_9 # Recreate the cache directory. 
-_7_0 os.makedirs(dir, exist_ok=True) 
-_7_1 
-_7_2def flush(dir: str, expiry: Union[int, float, timedelta, None]) -> None: 
-_7_3 """Flush expired keys from the provided cache.""" 
-_7_4 
-_7_5 # Iterate over keys in the cache. 
-_7_6 for file in os.listdir(dir): 
-_7_7 path = f'{dir}/{file}' 
+_5_5 # Serialise the data. 
+_5_6 data = serialize(data) 
+_5_7 
+_5_8 # Hash the data and affix its length, preceded by a hyphen (to reduce the
+likelihood of collisions). 
+_5_9 return f'{xxh3_128_hexdigest(data)}{len(data)}' 
+_6_0 
+_6_1def shorthash(data: Any) -> str: 
+_6_2 """Hash the given data.""" 
+_6_3 
+_6_4 # Serialise the data. 
+_6_5 data = serialize(data) 
+_6_6 
+_6_7 # Hash the data and affix its length, preceded by a hyphen (to reduce the
+likelihood of collisions). 
+_6_8 return f'{xxh3_64_hexdigest(data)}{len(data)}' 
+_6_9 
+_7_0def delete(dir: str) -> None: 
+_7_1 """Delete the provided cache.""" 
+_7_2 
+_7_3 # Remove the cache directory and all its contents. 
+_7_4 shutil.rmtree(dir, ignore_errors=True) 
+_7_5 
+_7_6def clear(dir: str) -> None: 
+_7_7 """Clear the provided cache.""" 
 _7_8 
-_7_9 # Lock the entry before reading it. 
-_8_0 with FileLock(f'{path}.lock'): 
-_8_1 # Get the time at which the key was last set. 
-_8_2 timestamp = os.path.getmtime(path) 
-_8_3 
-_8_4 # If the entry is expired, remove it from the cache. 
-_8_5 if (isinstance(expiry, timedelta) and datetime.fromtimestamp(timestamp) +
+_7_9 # Delete the cache. 
+_8_0 delete(dir) 
+_8_1 
+_8_2 # Recreate the cache directory. 
+_8_3 os.makedirs(dir, exist_ok=True) 
+_8_4 
+_8_5def flush(dir: str, expiry: Union[int, float, timedelta, None]) -> None: 
+_8_6 """Flush expired keys from the provided cache.""" 
+_8_7 
+_8_8 # Iterate over keys in the cache. 
+_8_9 for file in os.listdir(dir): 
+_9_0 path = f'{dir}/{file}' 
+_9_1 
+_9_2 # Lock the entry before reading it. 
+_9_3 with FileLock(f'{path}.lock'): 
+_9_4 # Get the time at which the key was last set. 
+_9_5 timestamp = os.path.getmtime(path) 
+_9_6 
+_9_7 # If the entry is expired, remove it from the cache. 
+_9_8 if (isinstance(expiry, timedelta) and datetime.fromtimestamp(timestamp) +
 expiry < datetime.now()) \ 
-_8_6 or (timestamp + expiry < datetime.now().timestamp()): 
-_8_7 os.remove(path) 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
+_9_9 or (timestamp + expiry < datetime.now().timestamp()): 
+_1_0_0 os.remove(path) 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_helpers_py.html` & `persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_helpers_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\helpers.py: 86%</title>
+    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\helpers.py: 81%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\helpers.py</b>:
-            <span class="pc_cov">86%</span>
+            <span class="pc_cov">81%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">36 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">31<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">29<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">7<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_caching_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_persist_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -111,15 +111,15 @@
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="str">"""Map arguments to their keywords or the keyword of the args parameter where necessary using the given mapping of a function's arguments to their default values and the name and index of the function's args parameter if such a parameter exists."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="com"># Copy the signature to avoid modifying the original.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">signature</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="com"># Map positional arguments to their keywords by zipping the function's arguments with the provided positional arguments truncated to the index of the args parameter if such a parameter exists.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">for</span> <span class="nam">argument</span><span class="op">,</span> <span class="nam">positional_argument</span> <span class="key">in</span> <span class="nam">zip</span><span class="op">(</span><span class="nam">arguments</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="op">:</span><span class="nam">args_i</span><span class="op">]</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">arguments</span><span class="op">[</span><span class="nam">argument</span><span class="op">]</span> <span class="op">=</span> <span class="nam">positional_argument</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">arguments</span><span class="op">[</span><span class="nam">argument</span><span class="op">]</span> <span class="op">=</span> <span class="nam">positional_argument</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="com"># If the args parameter exists, map the remaining positional arguments to the args parameter.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">if</span> <span class="nam">args_parameter</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">arguments</span><span class="op">[</span><span class="nam">args_parameter</span><span class="op">]</span> <span class="op">=</span> <span class="nam">args</span><span class="op">[</span><span class="nam">args_i</span><span class="op">:</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="com"># Merge positional and keyword arguments with the function's arguments.</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">arguments</span> <span class="op">|=</span> <span class="nam">kwargs</span>&nbsp;</span><span class="r"></span></p>
@@ -127,15 +127,15 @@
     <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">return</span> <span class="nam">arguments</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="key">def</span> <span class="nam">is_async</span><span class="op">(</span><span class="nam">func</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="str">"""Determine whether a callable is asynchronous."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="com"># If `inspect.iscoroutinefunction` identifies the callable as asynchronous, then return `True`. If it doesn't, then try to search for a line that begins (ignoring preceeding whitespace) with `async def` followed by the callable's name and a `(` character inside its source code, returning `True` if such a line is found and there is no such line beginning with `def` (indicating that asynchronous and synchronous functions with the same name were defined in the same block as the callable).</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">if</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">iscoroutinefunction</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">source</span> <span class="op">=</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">getsource</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="key">except</span> <span class="op">(</span><span class="nam">OSError</span><span class="op">,</span> <span class="nam">TypeError</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -153,13 +153,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_caching_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_persist_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 ************ CCoovveerraaggee ffoorr CC::\\PPyytthhoonn331111\\LLiibb\\ssiittee--ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\hheellppeerrss..ppyy::
-8866%% ************
+8811%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3366 ssttaatteemmeennttss ?  3311 rruunn 55 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
+********** 3366 ssttaatteemmeennttss ?  2299 rruunn 77 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
 _1import inspect 
 _2import re 
 _3from typing import Any, Callable, Union 
 _4 
 _5 
 _6def signaturize(func: Callable) -> tuple[dict[str, Any], Union[str, None],
 Union[int, None], Union[str, None]]: 
@@ -95,9 +95,9 @@
 _6_3 has_sync_def = re.search(r'^\s*def\s+' + re.escape(func.__name__) + r'\s*\
 (', source, re.MULTILINE) 
 _6_4 
 _6_5 if not has_sync_def: 
 _6_6 return True 
 _6_7 
 _6_8 return False 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_persist_cache_py.html` & `persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_serialization_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\persist_cache.py: 100%</title>
+    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\serialization.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\persist_cache.py</b>:
+            <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\serialization.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,187 +50,197 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">55 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">55<span class="text"> run</span></button>
+            <span class="text">75 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">75<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_pickle_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_serialization_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">asyncio</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">inspect</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">datetime</span> <span class="key">import</span> <span class="nam">timedelta</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">wraps</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">caching</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">caching</span> <span class="key">import</span> <span class="nam">NOT_IN_CACHE</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">inflate_arguments</span><span class="op">,</span> <span class="nam">is_async</span><span class="op">,</span> <span class="nam">signaturize</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">pickle</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">msgspec</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="nam">Msgpackables</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">list</span><span class="op">,</span> <span class="nam">dict</span><span class="op">,</span> <span class="nam">bool</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="str">"""Types that are directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># Initialise msgpack encoders and decoders once to speed up subsequent serialization and deserialization.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">msgpack_encoder</span> <span class="op">=</span> <span class="nam">msgspec</span><span class="op">.</span><span class="nam">msgpack</span><span class="op">.</span><span class="nam">Encoder</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">msgpack_decoder</span> <span class="op">=</span> <span class="nam">msgspec</span><span class="op">.</span><span class="nam">msgpack</span><span class="op">.</span><span class="nam">Decoder</span><span class="op">(</span><span class="nam">type</span><span class="op">=</span><span class="nam">Msgpackables</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">def</span> <span class="nam">cache</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="nam">name</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">dir</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">expiry</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">Callable</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="str">"""Persistently and locally cache the returns of a function.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    The function to be cached must accept and return dillable objects only (with the exception of methods' `self` argument, which is always ignored). Additionally, for consistent caching across subsequent sessions, arguments and returns should also be hashable.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        name (`str | Callable`, optional): The name of the cache (or, if `cache()` is being called as an argument-less decorator (ie, as `@cache` instead of `@cache(...)`), the function to be cached). Defaults to the hash of the qualified name of the function. If `dir` is set, this argument will be ignored.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        dir (`str`, optional): The directory in which the cache should be stored. Defaults to a subdirectory bearing the name of the cache in a parent folder called '.persist_cache' in the current working directory.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">        expiry (`int | float | timedelta`, optional): How long, in seconds or as a `timedelta`, function calls should persist in the cache. Defaults to `None`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">        `Callable`: If `cache()` is called with arguments, a decorator that wraps the function to be cached, otherwise, the wrapped function itself. Once wrapped, the function will have the following methods attached to it:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">            - `set_expiry(value: int | float | timedelta) -> None`: Set the expiry of the cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">            - `flush_cache() -> None`: Flush out any expired cached returns.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">            - `clear_cache() -> None`: Clear out all cached returns.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">            - `delete_cache() -> None`: Delete the cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">def</span> <span class="nam">decorator</span><span class="op">(</span><span class="nam">func</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Callable</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">nonlocal</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="com"># If the cache directory has not been set, and the name of the cache has, set it to a subdirectory by that name in a directory called '.persist_cache' in the current working directory, or, if the name of the cache has not been set, set the name of that subdirectory to the hash of the qualified name of the function.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">if</span> <span class="nam">dir</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">if</span> <span class="nam">name</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">                <span class="nam">dir</span> <span class="op">=</span> <span class="str">f'.persist_cache/{name}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">dir</span> <span class="op">=</span> <span class="str">f'.persist_cache/{caching.hash(func.__qualname__)}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="com"># Create the cache directory and any other necessary directories if it does not exist.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">os</span><span class="op">.</span><span class="nam">makedirs</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="com"># Flag whether the function is a method to enable the exclusion of the first argument (which will be the instance of the function's class) from being hashed to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">is_method</span> <span class="op">=</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">ismethod</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="com"># Preserve a map of the function's arguments to their default values and the name and index of the args parameter if such a parameter exists to enable the remapping of positional arguments to their keywords, which thereby allows for the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span> <span class="op">=</span> <span class="nam">signaturize</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="com"># Initialise a wrapper for synchronous functions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="key">def</span> <span class="nam">sync_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">SIGNATURE_SEPARATOR</span> <span class="op">=</span> <span class="str">'\x1c\x1e'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">"""A separator used to distinguish between a signature indicating how data has been serialized and the data itself."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">TUPLE_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#127799;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a tuple."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="nam">SET_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129530;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a set."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">FROZENSET_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129482;&#129530;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a frozenset."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="nam">LISTED_SIGNATURES</span> <span class="op">=</span> <span class="op">{</span><span class="nam">TUPLE_SIGNATURE</span><span class="op">,</span> <span class="nam">SET_SIGNATURE</span><span class="op">,</span> <span class="nam">FROZENSET_SIGNATURE</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">"""The signatures of data types that are serialized as lists."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="nam">PICKLE_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129362;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a pickled object."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="nam">BYTES_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#128287;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a bytes object."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="nam">BYTEARRAY_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#128290;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a bytearray."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="com"># Preserve the lengths of the signatures to avoid having to constantly recompute them.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="nam">PICKLE_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="nam">BYTES_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">BYTES_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="nam">BYTEARRAY_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="nam">STR_SIGNATURES</span> <span class="op">=</span> <span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">,</span> <span class="nam">BYTES_SIGNATURE</span><span class="op">,</span> <span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">"""The signatures of data types that are serialized as strings."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="nam">ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES</span> <span class="op">=</span> <span class="op">(</span><span class="nam">bool</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span><span class="op">,</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">"""Types that are absolutely directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""Determine whether the provided data is directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="com"># Data will be directly msgpackable if:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="com"># - It is a string and it does not start with any of the signatures of data types that are serialized as strings;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="com"># - It is an integer and is between -2**63 and 2**64-1, inclusive;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="com"># - It is a list and all of its elements are directly msgpackable and it is either empty or its first element is not a signature of a data type that is serialized as a list;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="com"># - It is a dictionary and all of its keys and values are directly msgpackable; or</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="com"># - It is of a type specified by `ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="key">if</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">any</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">str_signature</span><span class="op">)</span> <span class="key">for</span> <span class="nam">str_signature</span> <span class="key">in</span> <span class="nam">STR_SIGNATURES</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">or</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">and</span> <span class="op">-</span><span class="num">2</span><span class="op">**</span><span class="num">63</span> <span class="op">&lt;=</span> <span class="nam">data</span> <span class="op">&lt;=</span> <span class="num">2</span><span class="op">**</span><span class="num">64</span><span class="op">-</span><span class="num">1</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">or</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span> <span class="key">and</span> <span class="nam">all</span><span class="op">(</span><span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span> <span class="key">or</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">or</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">LISTED_SIGNATURES</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="key">or</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span> <span class="key">and</span> <span class="nam">all</span><span class="op">(</span><span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">k</span><span class="op">)</span> <span class="key">and</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">data</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="key">or</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="key">def</span> <span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Msgpackables</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="str">"""Make the given data capable of being directly serialized to msgpack."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="com"># If the data is directly msgpackable, return it as is.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="com"># Initialise a wrapper for asynchronous functions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">async</span> <span class="key">def</span> <span class="nam">async_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="com"># If the data is a tuple, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a tuple.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">tuple</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">TUPLE_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="com"># Identify the appropriate wrapper for the function by checking whether it is asynchronous or not.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">async_wrapper</span> <span class="key">if</span> <span class="nam">is_async</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span> <span class="key">else</span> <span class="nam">sync_wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="com"># If the data is a set, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a set.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">set</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">SET_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="com"># If the data is a bytes object, return it as a string with a signature indicating that it is a bytes object.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">bytes</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">return</span> <span class="str">f'{BYTES_SIGNATURE}{data.decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="com"># If the data is a frozenset, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a frozenset.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">frozenset</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">FROZENSET_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="com"># If the data is a bytearray, return it as a string with a signature indicating that it is a bytearray.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">bytearray</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">return</span> <span class="str">f'{BYTEARRAY_SIGNATURE}{data.decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="com"># Attach convenience functions to the wrapper for modifying the cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="key">def</span> <span class="nam">delete_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">            <span class="str">"""Delete the cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="key">def</span> <span class="nam">clear_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="str">"""Clear the cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">        <span class="key">def</span> <span class="nam">flush_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">            <span class="str">"""Flush expired keys from the cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="com"># If the data is incapable of other being forced into a directly msgpackable form, pickle it and return it as a string with a signature indicating that it is a pickled object.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">return</span> <span class="str">f'{PICKLE_SIGNATURE}{pickle.dumps(data).decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="key">def</span> <span class="nam">serialize</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="str">"""Serialize the provided data as msgpack."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="com"># Force the data into a directly msgpackable form.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="com"># Encode the data as msgpack.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">msgpack_encoder</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="key">def</span> <span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Msgpackables</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="str">"""Transform the provided msgpackable data back into Python objects."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">def</span> <span class="nam">set_expiry</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="str">"""Set the expiry of the cache."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">expiry</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="nam">expiry</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="com"># If the data is a string, check if it has a signature indicating that it is a pickled object, bytes object or bytearray and then decode it to the corresponding object, otherwise return it as is.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">if</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="key">return</span> <span class="nam">pickle</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="nam">PICKLE_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">elif</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">BYTES_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="key">return</span> <span class="nam">data</span><span class="op">[</span><span class="nam">BYTES_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">delete_cache</span> <span class="op">=</span> <span class="nam">delete_cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">clear_cache</span> <span class="op">=</span> <span class="nam">clear_cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">cache_clear</span> <span class="op">=</span> <span class="nam">wrapper</span><span class="op">.</span><span class="nam">clear_cache</span> <span class="com"># Add an alias for cache_clear which is used by lru_cache.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">flush_cache</span> <span class="op">=</span> <span class="nam">flush_cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">set_expiry</span> <span class="op">=</span> <span class="nam">set_expiry</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="com"># Preserve the original function.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">__wrapped__</span> <span class="op">=</span> <span class="nam">func</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="com"># Preserve the function's original signature.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">wraps</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">(</span><span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="key">return</span> <span class="nam">wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">elif</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="key">return</span> <span class="nam">bytearray</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="nam">BYTEARRAY_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="com"># If the data is a list, check if it has a signature indicating that it is a tuple, set or frozenset and then decode it to the corresponding object, otherwise return it as is.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="key">if</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">TUPLE_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">elif</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">SET_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="key">return</span> <span class="nam">set</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="com"># If the first argument is a function and all of the other arguments are `None`, indicating that this decorator factory was invoked without passing any arguments, return the result of passing that function to the decorator while also emptying the first argument to avoid it being used by the decorator.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="key">if</span> <span class="nam">callable</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span> <span class="key">and</span> <span class="nam">dir</span> <span class="key">is</span> <span class="nam">expiry</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">func</span> <span class="op">=</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">name</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="key">elif</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">FROZENSET_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                <span class="key">return</span> <span class="nam">frozenset</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">return</span> <span class="nam">decorator</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">    <span class="key">return</span> <span class="nam">decorator</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="com"># If the data is neither a string nor a list, return it as is.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="key">def</span> <span class="nam">deserialize</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="str">"""Deserialize the provided msgpack-encoded data."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="com"># Decode the data.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">msgpack_decoder</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">    <span class="com"># Transform the data back into Python objects.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_pickle_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_serialization_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:04 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,197 +1,187 @@
 ************ CCoovveerraaggee ffoorr CC::\\PPyytthhoonn331111\\LLiibb\\ssiittee--
-ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\ppeerrssiisstt__ccaacchhee..ppyy:: 110000%% ************
+ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\sseerriiaalliizzaattiioonn..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 5555 ssttaatteemmeennttss ?  5555 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
-_1import asyncio 
-_2import inspect 
-_3import os 
-_4from datetime import timedelta 
-_5from functools import wraps 
-_6from typing import Any, Callable, Union 
-_7 
-_8from . import caching 
-_9from .caching import NOT_IN_CACHE 
-_1_0from .helpers import inflate_arguments, is_async, signaturize 
-_1_1 
+********** 7755 ssttaatteemmeennttss ?  7755 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
+_1import pickle 
+_2from typing import Any, Union 
+_3 
+_4import msgspec 
+_5 
+_6Msgpackables = Union[str, int, list, dict, bool, float, None] 
+_7"""Types that are directly msgpackable.""" 
+_8 
+_9# Initialise msgpack encoders and decoders once to speed up subsequent
+serialization and deserialization. 
+_1_0msgpack_encoder = msgspec.msgpack.Encoder() 
+_1_1msgpack_decoder = msgspec.msgpack.Decoder(type=Msgpackables) 
 _1_2 
-_1_3def cache( 
-_1_4 name: Union[str, Callable, None] = None, 
-_1_5 dir: Union[str, None] = None, 
-_1_6 expiry: Union[int, float, timedelta, None] = None, 
-_1_7 ) -> Callable: 
-_1_8 """Persistently and locally cache the returns of a function. 
-_1_9  
-_2_0 The function to be cached must accept and return dillable objects only (with
-the exception of methods' `self` argument, which is always ignored).
-Additionally, for consistent caching across subsequent sessions, arguments and
-returns should also be hashable. 
-_2_1  
-_2_2 Arguments: 
-_2_3 name (`str | Callable`, optional): The name of the cache (or, if `cache()`
-is being called as an argument-less decorator (ie, as `@cache` instead of
-`@cache(...)`), the function to be cached). Defaults to the hash of the
-qualified name of the function. If `dir` is set, this argument will be
-ignored. 
-_2_4  
-_2_5 dir (`str`, optional): The directory in which the cache should be stored.
-Defaults to a subdirectory bearing the name of the cache in a parent folder
-called '.persist_cache' in the current working directory. 
-_2_6  
-_2_7 expiry (`int | float | timedelta`, optional): How long, in seconds or as a
-`timedelta`, function calls should persist in the cache. Defaults to `None`. 
-_2_8  
-_2_9 Returns: 
-_3_0 `Callable`: If `cache()` is called with arguments, a decorator that wraps
-the function to be cached, otherwise, the wrapped function itself. Once
-wrapped, the function will have the following methods attached to it: 
-_3_1 - `set_expiry(value: int | float | timedelta) -> None`: Set the expiry of
-the cache. 
-_3_2 - `flush_cache() -> None`: Flush out any expired cached returns. 
-_3_3 - `clear_cache() -> None`: Clear out all cached returns. 
-_3_4 - `delete_cache() -> None`: Delete the cache.""" 
-_3_5 
-_3_6 def decorator(func: Callable) -> Callable: 
-_3_7 nonlocal name, dir, expiry 
-_3_8 
-_3_9 # If the cache directory has not been set, and the name of the cache has,
-set it to a subdirectory by that name in a directory called '.persist_cache' in
-the current working directory, or, if the name of the cache has not been set,
-set the name of that subdirectory to the hash of the qualified name of the
-function. 
-_4_0 if dir is None: 
-_4_1 if name is not None: 
-_4_2 dir = f'.persist_cache/{name}' 
-_4_3 else: 
-_4_4 dir = f'.persist_cache/{caching.hash(func.__qualname__)}' 
-_4_5 
-_4_6 # Create the cache directory and any other necessary directories if it does
-not exist. 
-_4_7 if not os.path.exists(dir): 
-_4_8 os.makedirs(dir, exist_ok=True) 
-_4_9 
-_5_0 # Flag whether the function is a method to enable the exclusion of the first
-argument (which will be the instance of the function's class) from being hashed
-to produce the cache key. 
-_5_1 is_method = inspect.ismethod(func) 
-_5_2 
-_5_3 # Preserve a map of the function's arguments to their default values and the
-name and index of the args parameter if such a parameter exists to enable the
-remapping of positional arguments to their keywords, which thereby allows for
-the consistent caching of function calls where positional arguments are used on
-some occasions and keyword arguments are used on others. 
-_5_4 signature, args_parameter, args_i = signaturize(func) 
-_5_5 
-_5_6 # Initialise a wrapper for synchronous functions. 
-_5_7 def sync_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any: 
-_5_8 nonlocal dir, expiry, is_method 
-_5_9 
-_6_0 # Map arguments to their keywords or the keyword of the args parameter where
-necessary, filtering out the first argument if the function is a method, to
-enable the consistent caching of function calls where positional arguments are
-used on some occasions and keyword arguments are used on others. 
-_6_1 arguments = inflate_arguments(signature, args_parameter, args_i, args
-[is_method:], kwargs) 
-_6_2 
-_6_3 # Hash the arguments to produce the cache key. 
-_6_4 key = caching.hash(arguments) 
+_1_3SIGNATURE_SEPARATOR = '\x1c\x1e' 
+_1_4"""A separator used to distinguish between a signature indicating how data
+has been serialized and the data itself.""" 
+_1_5 
+_1_6TUPLE_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
+_1_7"""A signature indicating that serialized data is a tuple.""" 
+_1_8 
+_1_9SET_SIGNATURE = f'狀{SIGNATURE_SEPARATOR}' 
+_2_0"""A signature indicating that serialized data is a set.""" 
+_2_1 
+_2_2FROZENSET_SIGNATURE = f'流狀{SIGNATURE_SEPARATOR}' 
+_2_3"""A signature indicating that serialized data is a frozenset.""" 
+_2_4 
+_2_5LISTED_SIGNATURES = {TUPLE_SIGNATURE, SET_SIGNATURE, FROZENSET_SIGNATURE} 
+_2_6"""The signatures of data types that are serialized as lists.""" 
+_2_7 
+_2_8PICKLE_SIGNATURE = f'勒{SIGNATURE_SEPARATOR}' 
+_2_9"""A signature indicating that serialized data is a pickled object.""" 
+_3_0 
+_3_1BYTES_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
+_3_2"""A signature indicating that serialized data is a bytes object.""" 
+_3_3 
+_3_4BYTEARRAY_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
+_3_5"""A signature indicating that serialized data is a bytearray.""" 
+_3_6 
+_3_7# Preserve the lengths of the signatures to avoid having to constantly
+recompute them. 
+_3_8PICKLE_SIGNATURE_LEN = len(PICKLE_SIGNATURE) 
+_3_9BYTES_SIGNATURE_LEN = len(BYTES_SIGNATURE) 
+_4_0BYTEARRAY_SIGNATURE_LEN = len(BYTEARRAY_SIGNATURE) 
+_4_1 
+_4_2STR_SIGNATURES = (PICKLE_SIGNATURE, BYTES_SIGNATURE, BYTEARRAY_SIGNATURE) 
+_4_3"""The signatures of data types that are serialized as strings.""" 
+_4_4 
+_4_5ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES = (bool, float, type(None),) 
+_4_6"""Types that are absolutely directly msgpackable.""" 
+_4_7 
+_4_8def directly_msgpackable(data: Any) -> bool: 
+_4_9 """Determine whether the provided data is directly msgpackable.""" 
+_5_0 
+_5_1 # Data will be directly msgpackable if: 
+_5_2 # - It is a string and it does not start with any of the signatures of data
+types that are serialized as strings; 
+_5_3 # - It is an integer and is between -2**63 and 2**64-1, inclusive; 
+_5_4 # - It is a list and all of its elements are directly msgpackable and it is
+either empty or its first element is not a signature of a data type that is
+serialized as a list; 
+_5_5 # - It is a dictionary and all of its keys and values are directly
+msgpackable; or 
+_5_6 # - It is of a type specified by `ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES`. 
+_5_7 if (isinstance(data, str) and not any(data.startswith(str_signature) for
+str_signature in STR_SIGNATURES)) \ 
+_5_8 or isinstance(data, int) and -2**63 <= data <= 2**64-1 \ 
+_5_9 or (isinstance(data, list) and all(directly_msgpackable(d) for d in data)
+and (len(data) == 0 or not isinstance(data[0], str) or data[0] not in
+LISTED_SIGNATURES)) \ 
+_6_0 or (isinstance(data, dict) and all(directly_msgpackable(k) and
+directly_msgpackable(v) for k, v in data.items())) \ 
+_6_1 or isinstance(data, ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES): 
+_6_2 return True 
+_6_3 
+_6_4 return False 
 _6_5 
-_6_6 # Get the value of the key from the cache if it is not expired, otherwise,
-call the function and set the value of the key in the cache to the result of
-that call. 
-_6_7 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
-_6_8 value = func(*args, **kwargs) 
-_6_9 caching.set(key, value, dir) 
-_7_0 
-_7_1 return value 
+_6_6def make_directly_msgpackable(data: Any) -> Msgpackables: 
+_6_7 """Make the given data capable of being directly serialized to msgpack.""" 
+_6_8 
+_6_9 # If the data is directly msgpackable, return it as is. 
+_7_0 if directly_msgpackable(data): 
+_7_1 return data 
 _7_2 
-_7_3 # Initialise a wrapper for asynchronous functions. 
-_7_4 async def async_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any:
- 
-_7_5 nonlocal dir, expiry, is_method 
+_7_3 # If the data is a tuple, make all of its elements directly msgpackable and
+return it as a list with a signature indicating that it is a tuple. 
+_7_4 elif isinstance(data, tuple): 
+_7_5 return [TUPLE_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
 _7_6 
-_7_7 # Map arguments to their keywords or the keyword of the args parameter where
-necessary, filtering out the first argument if the function is a method, to
-enable the consistent caching of function calls where positional arguments are
-used on some occasions and keyword arguments are used on others. 
-_7_8 arguments = inflate_arguments(signature, args_parameter, args_i, args
-[is_method:], kwargs) 
-_7_9 
-_8_0 # Hash the arguments to produce the cache key. 
-_8_1 key = caching.hash(arguments) 
-_8_2 
-_8_3 # Get the value of the key from the cache if it is not expired, otherwise,
-call the function and set the value of the key in the cache to the result of
-that call. 
-_8_4 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
-_8_5 value = await func(*args, **kwargs) 
-_8_6 caching.set(key, value, dir) 
-_8_7 
-_8_8 return value 
-_8_9 
-_9_0 # Identify the appropriate wrapper for the function by checking whether it
-is asynchronous or not. 
-_9_1 wrapper = async_wrapper if is_async(func) else sync_wrapper 
+_7_7 # If the data is a set, make all of its elements directly msgpackable and
+return it as a list with a signature indicating that it is a set. 
+_7_8 elif isinstance(data, set): 
+_7_9 return [SET_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
+_8_0 
+_8_1 # If the data is a bytes object, return it as a string with a signature
+indicating that it is a bytes object. 
+_8_2 elif isinstance(data, bytes): 
+_8_3 return f'{BYTES_SIGNATURE}{data.decode("latin1")}' 
+_8_4 
+_8_5 # If the data is a frozenset, make all of its elements directly msgpackable
+and return it as a list with a signature indicating that it is a frozenset. 
+_8_6 elif isinstance(data, frozenset): 
+_8_7 return [FROZENSET_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
+_8_8 
+_8_9 # If the data is a bytearray, return it as a string with a signature
+indicating that it is a bytearray. 
+_9_0 elif isinstance(data, bytearray): 
+_9_1 return f'{BYTEARRAY_SIGNATURE}{data.decode("latin1")}' 
 _9_2 
-_9_3 # Attach convenience functions to the wrapper for modifying the cache. 
-_9_4 def delete_cache() -> None: 
-_9_5 """Delete the cache.""" 
-_9_6 nonlocal dir 
-_9_7 
-_9_8 caching.delete(dir) 
-_9_9 
-_1_0_0 def clear_cache() -> None: 
-_1_0_1 """Clear the cache.""" 
-_1_0_2 nonlocal dir 
-_1_0_3 
-_1_0_4 caching.clear(dir) 
-_1_0_5 
-_1_0_6 def flush_cache() -> None: 
-_1_0_7 """Flush expired keys from the cache.""" 
-_1_0_8 nonlocal dir, expiry, is_method 
+_9_3 # If the data is incapable of other being forced into a directly msgpackable
+form, pickle it and return it as a string with a signature indicating that it
+is a pickled object. 
+_9_4 return f'{PICKLE_SIGNATURE}{pickle.dumps(data).decode("latin1")}' 
+_9_5 
+_9_6def serialize(data: Any) -> str: 
+_9_7 """Serialize the provided data as msgpack.""" 
+_9_8 
+_9_9 # Force the data into a directly msgpackable form. 
+_1_0_0 data = make_directly_msgpackable(data) 
+_1_0_1 
+_1_0_2 # Encode the data as msgpack. 
+_1_0_3 data = msgpack_encoder.encode(data) 
+_1_0_4 
+_1_0_5 return data 
+_1_0_6 
+_1_0_7def make_pythonic(data: Msgpackables) -> Any: 
+_1_0_8 """Transform the provided msgpackable data back into Python objects.""" 
 _1_0_9 
-_1_1_0 caching.flush(dir, expiry) 
-_1_1_1 
-_1_1_2 def set_expiry(value: int) -> None: 
-_1_1_3 """Set the expiry of the cache.""" 
-_1_1_4 nonlocal expiry 
-_1_1_5 
-_1_1_6 expiry = value 
+_1_1_0 # If the data is a string, check if it has a signature indicating that it
+is a pickled object, bytes object or bytearray and then decode it to the
+corresponding object, otherwise return it as is. 
+_1_1_1 if isinstance(data, str): 
+_1_1_2 if data.startswith(PICKLE_SIGNATURE): 
+_1_1_3 return pickle.loads(data[PICKLE_SIGNATURE_LEN:].encode("latin1")) 
+_1_1_4 
+_1_1_5 elif data.startswith(BYTES_SIGNATURE): 
+_1_1_6 return data[BYTES_SIGNATURE_LEN:].encode("latin1") 
 _1_1_7 
-_1_1_8 wrapper.delete_cache = delete_cache 
-_1_1_9 wrapper.clear_cache = clear_cache 
-_1_2_0 wrapper.cache_clear = wrapper.clear_cache # Add an alias for cache_clear
-which is used by lru_cache. 
-_1_2_1 wrapper.flush_cache = flush_cache 
-_1_2_2 wrapper.set_expiry = set_expiry 
-_1_2_3 
-_1_2_4 # Preserve the original function. 
-_1_2_5 wrapper.__wrapped__ = func 
-_1_2_6 
-_1_2_7 # Preserve the function's original signature. 
-_1_2_8 wrapper = wraps(func)(wrapper) 
-_1_2_9 
-_1_3_0 return wrapper 
+_1_1_8 elif data.startswith(BYTEARRAY_SIGNATURE): 
+_1_1_9 return bytearray(data[BYTEARRAY_SIGNATURE_LEN:].encode("latin1")) 
+_1_2_0 
+_1_2_1 return data 
+_1_2_2 
+_1_2_3 # If the data is a list, check if it has a signature indicating that it is
+a tuple, set or frozenset and then decode it to the corresponding object,
+otherwise return it as is. 
+_1_2_4 elif isinstance(data, list): 
+_1_2_5 if len(data) != 0: 
+_1_2_6 if data[0] == TUPLE_SIGNATURE: 
+_1_2_7 return tuple(make_pythonic(d) for d in data[1:]) 
+_1_2_8 
+_1_2_9 elif data[0] == SET_SIGNATURE: 
+_1_3_0 return set(make_pythonic(d) for d in data[1:]) 
 _1_3_1 
-_1_3_2 # If the first argument is a function and all of the other arguments are
-`None`, indicating that this decorator factory was invoked without passing any
-arguments, return the result of passing that function to the decorator while
-also emptying the first argument to avoid it being used by the decorator. 
-_1_3_3 if callable(name) and dir is expiry is None: 
-_1_3_4 func = name 
-_1_3_5 name = None 
+_1_3_2 elif data[0] == FROZENSET_SIGNATURE: 
+_1_3_3 return frozenset(make_pythonic(d) for d in data[1:]) 
+_1_3_4 
+_1_3_5 return data 
 _1_3_6 
-_1_3_7 return decorator(func) 
-_1_3_8 
-_1_3_9 return decorator 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 21:04 +1100
+_1_3_7 # If the data is neither a string nor a list, return it as is. 
+_1_3_8 return data 
+_1_3_9 
+_1_4_0def deserialize(data: str) -> Any: 
+_1_4_1 """Deserialize the provided msgpack-encoded data.""" 
+_1_4_2 
+_1_4_3 # Decode the data. 
+_1_4_4 data = msgpack_decoder.decode(data) 
+_1_4_5 
+_1_4_6 # Transform the data back into Python objects. 
+_1_4_7 data = make_pythonic(data) 
+_1_4_8 
+_1_4_9 return data 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/d_5cadf2fa0b1853af_serialization_py.html` & `persist_cache-0.4.0/tests/htmlcov/d_5cadf2fa0b1853af_persist_cache_py.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\serialization.py: 100%</title>
+    <title>Coverage for C:\Python311\Lib\site-packages\persist_cache\persist_cache.py: 57%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\serialization.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="text">Coverage for </span><b>C:\Python311\Lib\site-packages\persist_cache\persist_cache.py</b>:
+            <span class="pc_cov">57%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,197 +50,284 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">75 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">75<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <span class="text">94 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">54<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">40<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_persist_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_pickle_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 20:59 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">dill</span> <span class="key">as</span> <span class="nam">pickle</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">msgspec</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="nam">Msgpackables</span> <span class="op">=</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">list</span><span class="op">,</span> <span class="nam">dict</span><span class="op">,</span> <span class="nam">bool</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="str">"""Types that are directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># Initialise msgpack encoders and decoders once to speed up subsequent serialization and deserialization.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">msgpack_encoder</span> <span class="op">=</span> <span class="nam">msgspec</span><span class="op">.</span><span class="nam">msgpack</span><span class="op">.</span><span class="nam">Encoder</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="nam">msgpack_decoder</span> <span class="op">=</span> <span class="nam">msgspec</span><span class="op">.</span><span class="nam">msgpack</span><span class="op">.</span><span class="nam">Decoder</span><span class="op">(</span><span class="nam">type</span><span class="op">=</span><span class="nam">Msgpackables</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">SIGNATURE_SEPARATOR</span> <span class="op">=</span> <span class="str">'\x1c\x1e'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="str">"""A separator used to distinguish between a signature indicating how data has been serialized and the data itself."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">TUPLE_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#127799;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a tuple."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="nam">SET_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129530;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a set."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="nam">FROZENSET_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129482;&#129530;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a frozenset."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="nam">LISTED_SIGNATURES</span> <span class="op">=</span> <span class="op">{</span><span class="nam">TUPLE_SIGNATURE</span><span class="op">,</span> <span class="nam">SET_SIGNATURE</span><span class="op">,</span> <span class="nam">FROZENSET_SIGNATURE</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">"""The signatures of data types that are serialized as lists."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="nam">PICKLE_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#129362;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a pickled object."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="nam">BYTES_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#128287;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a bytes object."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="nam">BYTEARRAY_SIGNATURE</span> <span class="op">=</span> <span class="str">f'&#128290;{SIGNATURE_SEPARATOR}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">"""A signature indicating that serialized data is a bytearray."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="com"># Preserve the lengths of the signatures to avoid having to constantly recompute them.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="nam">PICKLE_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="nam">BYTES_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">BYTES_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="nam">BYTEARRAY_SIGNATURE_LEN</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">inspect</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">datetime</span> <span class="key">import</span> <span class="nam">timedelta</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">functools</span> <span class="key">import</span> <span class="nam">wraps</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Union</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span> <span class="key">import</span> <span class="nam">caching</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">caching</span> <span class="key">import</span> <span class="nam">NOT_IN_CACHE</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">inflate_arguments</span><span class="op">,</span> <span class="nam">is_async</span><span class="op">,</span> <span class="nam">signaturize</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">def</span> <span class="nam">cache</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="nam">name</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="nam">dir</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">expiry</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">Callable</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="str">"""Persistently and locally cache the returns of a function.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="str">    The function to be cached must accept and return dillable objects only (with the exception of methods' `self` argument, which is always ignored). Additionally, for consistent caching across subsequent sessions, arguments and returns should also be hashable.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t"><span class="str">        name (`str | Callable`, optional): The name of the cache (or, if `cache()` is being called as an argument-less decorator (ie, as `@cache` instead of `@cache(...)`), the function to be cached). Defaults to the qualified name of the function. If `dir` is set, this argument will be ignored.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="str">        dir (`str`, optional): The directory in which the cache should be stored. Defaults to a subdirectory named after the hash of the cache's name in a parent folder named '.persist_cache' in the current working directory.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">        </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">        expiry (`int | float | timedelta`, optional): How long, in seconds or as a `timedelta`, function calls should persist in the cache. Defaults to `None`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">    Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">        `Callable`: If `cache()` is called with arguments, a decorator that wraps the function to be cached, otherwise, the wrapped function itself. Once wrapped, the function will have the following methods attached to it:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">            - `set_expiry(value: int | float | timedelta) -> None`: Set the expiry of the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">            - `flush_cache() -> None`: Flush out any expired cached returns.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">            - `clear_cache() -> None`: Clear out all cached returns.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">            - `delete_cache() -> None`: Delete the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">def</span> <span class="nam">decorator</span><span class="op">(</span><span class="nam">func</span><span class="op">:</span> <span class="nam">Callable</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Callable</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">nonlocal</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="com"># If the cache directory has not been set, and the name of the cache has, set it to a subdirectory by the name of the hash of that name in a directory named '.persist_cache' in the current working directory, or, if the name of the cache has not been set, set the name of that subdirectory to the hash of the qualified name of the function.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">if</span> <span class="nam">dir</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="nam">name</span> <span class="op">=</span> <span class="nam">name</span> <span class="key">if</span> <span class="nam">name</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span> <span class="key">else</span> <span class="nam">func</span><span class="op">.</span><span class="nam">__qualname__</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="nam">STR_SIGNATURES</span> <span class="op">=</span> <span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">,</span> <span class="nam">BYTES_SIGNATURE</span><span class="op">,</span> <span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">"""The signatures of data types that are serialized as strings."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="nam">ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES</span> <span class="op">=</span> <span class="op">(</span><span class="nam">bool</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span><span class="op">,</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">"""Types that are absolutely directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="nam">dir</span> <span class="op">=</span> <span class="str">f'.persist_cache/{caching.shorthash(name)}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="com"># Create the cache directory and any other necessary directories if it does not exist.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="nam">os</span><span class="op">.</span><span class="nam">makedirs</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">exist_ok</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="key">def</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="str">"""Determine whether the provided data is directly msgpackable."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="com"># Data will be directly msgpackable if:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="com"># - It is a string and it does not start with any of the signatures of data types that are serialized as strings;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="com"># - It is an integer and is between -2**63 and 2**64-1, inclusive;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="com"># - It is a list and all of its elements are directly msgpackable and it is either empty or its first element is not a signature of a data type that is serialized as a list;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="com"># - It is a dictionary and all of its keys and values are directly msgpackable; or</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="com"># - It is of a type specified by `ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="key">if</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">any</span><span class="op">(</span><span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">str_signature</span><span class="op">)</span> <span class="key">for</span> <span class="nam">str_signature</span> <span class="key">in</span> <span class="nam">STR_SIGNATURES</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">or</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">int</span><span class="op">)</span> <span class="key">and</span> <span class="op">-</span><span class="num">2</span><span class="op">**</span><span class="num">63</span> <span class="op">&lt;=</span> <span class="nam">data</span> <span class="op">&lt;=</span> <span class="num">2</span><span class="op">**</span><span class="num">64</span><span class="op">-</span><span class="num">1</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">or</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span> <span class="key">and</span> <span class="nam">all</span><span class="op">(</span><span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">)</span> <span class="key">and</span> <span class="op">(</span><span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span> <span class="key">or</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">LISTED_SIGNATURES</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="key">or</span> <span class="op">(</span><span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span> <span class="key">and</span> <span class="nam">all</span><span class="op">(</span><span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">k</span><span class="op">)</span> <span class="key">and</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">v</span><span class="op">)</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">data</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span> <span class="xx">\</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="key">or</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="key">def</span> <span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Msgpackables</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="str">"""Make the given data capable of being directly serialized to msgpack."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="com"># If the data is directly msgpackable, return it as is.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="nam">directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="com"># If an expiry has been set, flush out any expired cached returns.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">if</span> <span class="nam">expiry</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="com"># Flag whether the function is a method to enable the exclusion of the first argument (which will be the instance of the function's class) from being hashed to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">is_method</span> <span class="op">=</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">ismethod</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="com"># Preserve a map of the function's arguments to their default values and the name and index of the args parameter if such a parameter exists to enable the remapping of positional arguments to their keywords, which thereby allows for the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span> <span class="op">=</span> <span class="nam">signaturize</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="com"># Initialise a wrapper for synchronous functions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">def</span> <span class="nam">sync_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="com"># If the data is a tuple, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a tuple.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">tuple</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">TUPLE_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="com"># If the data is a set, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a set.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">set</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">SET_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="com"># If the data is a bytes object, return it as a string with a signature indicating that it is a bytes object.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">bytes</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">return</span> <span class="str">f'{BYTES_SIGNATURE}{data.decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="com"># Initialise a wrapper for asynchronous functions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">async</span> <span class="key">def</span> <span class="nam">async_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="com"># If the data is a frozenset, make all of its elements directly msgpackable and return it as a list with a signature indicating that it is a frozenset.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">frozenset</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">            <span class="key">return</span> <span class="op">[</span><span class="nam">FROZENSET_SIGNATURE</span><span class="op">,</span> <span class="op">*</span><span class="op">[</span><span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="com"># If the data is a bytearray, return it as a string with a signature indicating that it is a bytearray.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">bytearray</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">return</span> <span class="str">f'{BYTEARRAY_SIGNATURE}{data.decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="com"># If the data is incapable of other being forced into a directly msgpackable form, pickle it and return it as a string with a signature indicating that it is a pickled object.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">return</span> <span class="str">f'{PICKLE_SIGNATURE}{pickle.dumps(data).decode("latin1")}'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">            <span class="key">return</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="com"># Initialise a wrapper for generator functions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="key">def</span> <span class="nam">generator_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="key">def</span> <span class="nam">serialize</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="str">"""Serialize the provided data as msgpack."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="com"># Force the data into a directly msgpackable form.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">make_directly_msgpackable</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="com"># Encode the data as msgpack.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">msgpack_encoder</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="key">def</span> <span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">Msgpackables</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="str">"""Transform the provided msgpackable data back into Python objects."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">    <span class="com"># If the data is a string, check if it has a signature indicating that it is a pickled object, bytes object or bytearray and then decode it to the corresponding object, otherwise return it as is.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="key">if</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">PICKLE_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="key">return</span> <span class="nam">pickle</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="nam">PICKLE_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                    <span class="nam">value</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">item</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                    <span class="key">yield</span> <span class="nam">item</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="key">elif</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">BYTES_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="key">return</span> <span class="nam">data</span><span class="op">[</span><span class="nam">BYTES_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">value</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="key">yield</span> <span class="nam">item</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="key">elif</span> <span class="nam">data</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="nam">BYTEARRAY_SIGNATURE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">            <span class="key">return</span> <span class="nam">bytearray</span><span class="op">(</span><span class="nam">data</span><span class="op">[</span><span class="nam">BYTEARRAY_SIGNATURE_LEN</span><span class="op">:</span><span class="op">]</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"latin1"</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="com"># If the data is a list, check if it has a signature indicating that it is a tuple, set or frozenset and then decode it to the corresponding object, otherwise return it as is.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span> <span class="op">!=</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="key">if</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">TUPLE_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                <span class="key">return</span> <span class="nam">tuple</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">elif</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">SET_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="key">return</span> <span class="nam">set</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="com"># Initialise a wrapper for asynchronous generator functions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">async</span> <span class="key">def</span> <span class="nam">async_generator_wrapper</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">:</span> <span class="nam">tuple</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">            <span class="com"># Map arguments to their keywords or the keyword of the args parameter where necessary, filtering out the first argument if the function is a method, to enable the consistent caching of function calls where positional arguments are used on some occasions and keyword arguments are used on others.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="nam">arguments</span> <span class="op">=</span> <span class="nam">inflate_arguments</span><span class="op">(</span><span class="nam">signature</span><span class="op">,</span> <span class="nam">args_parameter</span><span class="op">,</span> <span class="nam">args_i</span><span class="op">,</span> <span class="nam">args</span><span class="op">[</span><span class="nam">is_method</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">            <span class="com"># Hash the arguments to produce the cache key.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">arguments</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">            <span class="com"># Get the value of the key from the cache if it is not expired, otherwise, call the function and set the value of the key in the cache to the result of that call.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="key">if</span> <span class="op">(</span><span class="nam">value</span> <span class="op">:=</span> <span class="nam">caching</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span><span class="op">)</span> <span class="key">is</span> <span class="nam">NOT_IN_CACHE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="nam">value</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">            <span class="key">elif</span> <span class="nam">data</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">==</span> <span class="nam">FROZENSET_SIGNATURE</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                <span class="key">return</span> <span class="nam">frozenset</span><span class="op">(</span><span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">d</span><span class="op">)</span> <span class="key">for</span> <span class="nam">d</span> <span class="key">in</span> <span class="nam">data</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="key">async</span> <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">func</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                    <span class="nam">value</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">item</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                    <span class="key">yield</span> <span class="nam">item</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="com"># If the data is neither a string nor a list, return it as is.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="key">def</span> <span class="nam">deserialize</span><span class="op">(</span><span class="nam">data</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="str">"""Deserialize the provided msgpack-encoded data."""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">    <span class="com"># Decode the data.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">msgpack_decoder</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">    <span class="com"># Transform the data back into Python objects.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">make_pythonic</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="nam">caching</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">value</span><span class="op">,</span> <span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">value</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                <span class="key">yield</span> <span class="nam">item</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="com"># Identify the appropriate wrapper for the function.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">if</span> <span class="nam">is_async</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">if</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">isasyncgenfunction</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">async_generator_wrapper</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">    <span class="key">return</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">async_wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="key">elif</span> <span class="nam">inspect</span><span class="op">.</span><span class="nam">isgeneratorfunction</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">            <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">generator_wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">            <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">sync_wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="com"># Attach convenience functions to the wrapper for modifying the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="key">def</span> <span class="nam">delete_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="str">"""Delete the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="key">def</span> <span class="nam">clear_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">            <span class="str">"""Clear the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="nam">dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="key">def</span> <span class="nam">flush_cache</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">            <span class="str">"""Flush expired keys from the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">,</span> <span class="nam">is_method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">            <span class="nam">caching</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="nam">dir</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">def</span> <span class="nam">set_expiry</span><span class="op">(</span><span class="nam">value</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="str">"""Set the expiry of the cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t"><span class="str">            </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t"><span class="str">            Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t"><span class="str">                expiry (`int | float | timedelta`): How long, in seconds or as a `timedelta`, function calls should persist in the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="key">nonlocal</span> <span class="nam">expiry</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">            <span class="nam">expiry</span> <span class="op">=</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">delete_cache</span> <span class="op">=</span> <span class="nam">delete_cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">clear_cache</span> <span class="op">=</span> <span class="nam">clear_cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">cache_clear</span> <span class="op">=</span> <span class="nam">wrapper</span><span class="op">.</span><span class="nam">clear_cache</span> <span class="com"># Add an alias for cache_clear which is used by lru_cache.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">flush_cache</span> <span class="op">=</span> <span class="nam">flush_cache</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">set_expiry</span> <span class="op">=</span> <span class="nam">set_expiry</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="com"># Preserve the original function.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="nam">wrapper</span><span class="op">.</span><span class="nam">__wrapped__</span> <span class="op">=</span> <span class="nam">func</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">        <span class="com"># Preserve the function's original signature.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="nam">wrapper</span> <span class="op">=</span> <span class="nam">wraps</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span><span class="op">(</span><span class="nam">wrapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">return</span> <span class="nam">wrapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="com"># If the first argument is a function and all of the other arguments are `None`, indicating that this decorator factory was invoked without passing any arguments, return the result of passing that function to the decorator while also emptying the first argument to avoid it being used by the decorator.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">if</span> <span class="nam">callable</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span> <span class="key">and</span> <span class="nam">dir</span> <span class="key">is</span> <span class="nam">expiry</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="nam">func</span> <span class="op">=</span> <span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="nam">name</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="key">return</span> <span class="nam">decorator</span><span class="op">(</span><span class="nam">func</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">    <span class="key">return</span> <span class="nam">decorator</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="key">def</span> <span class="nam">delete</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">    <span class="str">"""Delete the cache of the given function or name.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t"><span class="str">        function_or_name (`str | Callable`): The function or name of the cache to be deleted."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="nam">function_or_name</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">function_or_name</span><span class="op">.</span><span class="nam">__qualname__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">    <span class="nam">caching</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="str">f'.persist_cache/{caching.shorthash(name)}'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="key">def</span> <span class="nam">clear</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="str">"""Clear the cache of the given function or name.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">        function_or_name (`str | Callable`): The function or name of the cache to be cleared."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="nam">function_or_name</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">function_or_name</span><span class="op">.</span><span class="nam">__qualname__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">    <span class="nam">caching</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="str">f'.persist_cache/{caching.shorthash(name)}'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="key">def</span> <span class="nam">flush</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">]</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">:</span> <span class="nam">Union</span><span class="op">[</span><span class="nam">int</span><span class="op">,</span> <span class="nam">float</span><span class="op">,</span> <span class="nam">timedelta</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">    <span class="str">"""Flush expired keys from the cache of the given function or name.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">    </span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">    Arguments:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">        function_or_name (`str | Callable`): The function or name of the cache to be flushed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">        expiry (`int | float | timedelta`): How long, in seconds or as a `timedelta`, function calls should persist in the cache."""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="nam">function_or_name</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">function_or_name</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span> <span class="key">else</span> <span class="nam">function_or_name</span><span class="op">.</span><span class="nam">__qualname__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="nam">caching</span><span class="op">.</span><span class="nam">flush</span><span class="op">(</span><span class="str">f'.persist_cache/{caching.shorthash(name)}'</span><span class="op">,</span> <span class="nam">expiry</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_persist_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_helpers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af_pickle_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 20:59 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,186 +1,314 @@
 ************ CCoovveerraaggee ffoorr CC::\\PPyytthhoonn331111\\LLiibb\\ssiittee--
-ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\sseerriiaalliizzaattiioonn..ppyy:: 110000%% ************
+ppaacckkaaggeess\\ppeerrssiisstt__ccaacchhee\\ppeerrssiisstt__ccaacchhee..ppyy:: 5577%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 7755 ssttaatteemmeennttss ?  7755 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 20:59 +1100
-_1from typing import Any, Union 
-_2 
-_3import dill as pickle 
-_4import msgspec 
-_5 
-_6Msgpackables = Union[str, int, list, dict, bool, float, None] 
-_7"""Types that are directly msgpackable.""" 
-_8 
-_9# Initialise msgpack encoders and decoders once to speed up subsequent
-serialization and deserialization. 
-_1_0msgpack_encoder = msgspec.msgpack.Encoder() 
-_1_1msgpack_decoder = msgspec.msgpack.Decoder(type=Msgpackables) 
-_1_2 
-_1_3SIGNATURE_SEPARATOR = '\x1c\x1e' 
-_1_4"""A separator used to distinguish between a signature indicating how data
-has been serialized and the data itself.""" 
-_1_5 
-_1_6TUPLE_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
-_1_7"""A signature indicating that serialized data is a tuple.""" 
-_1_8 
-_1_9SET_SIGNATURE = f'狀{SIGNATURE_SEPARATOR}' 
-_2_0"""A signature indicating that serialized data is a set.""" 
-_2_1 
-_2_2FROZENSET_SIGNATURE = f'流狀{SIGNATURE_SEPARATOR}' 
-_2_3"""A signature indicating that serialized data is a frozenset.""" 
-_2_4 
-_2_5LISTED_SIGNATURES = {TUPLE_SIGNATURE, SET_SIGNATURE, FROZENSET_SIGNATURE} 
-_2_6"""The signatures of data types that are serialized as lists.""" 
-_2_7 
-_2_8PICKLE_SIGNATURE = f'勒{SIGNATURE_SEPARATOR}' 
-_2_9"""A signature indicating that serialized data is a pickled object.""" 
-_3_0 
-_3_1BYTES_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
-_3_2"""A signature indicating that serialized data is a bytes object.""" 
-_3_3 
-_3_4BYTEARRAY_SIGNATURE = f'{SIGNATURE_SEPARATOR}' 
-_3_5"""A signature indicating that serialized data is a bytearray.""" 
-_3_6 
-_3_7# Preserve the lengths of the signatures to avoid having to constantly
-recompute them. 
-_3_8PICKLE_SIGNATURE_LEN = len(PICKLE_SIGNATURE) 
-_3_9BYTES_SIGNATURE_LEN = len(BYTES_SIGNATURE) 
-_4_0BYTEARRAY_SIGNATURE_LEN = len(BYTEARRAY_SIGNATURE) 
+********** 9944 ssttaatteemmeennttss ?  5544 rruunn 4400 mmiissssiinngg 00 eexxcclluuddeedd **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
+_1import inspect 
+_2import os 
+_3from datetime import timedelta 
+_4from functools import wraps 
+_5from typing import Any, Callable, Union 
+_6 
+_7from . import caching 
+_8from .caching import NOT_IN_CACHE 
+_9from .helpers import inflate_arguments, is_async, signaturize 
+_1_0 
+_1_1 
+_1_2def cache( 
+_1_3 name: Union[str, Callable, None] = None, 
+_1_4 dir: Union[str, None] = None, 
+_1_5 expiry: Union[int, float, timedelta, None] = None, 
+_1_6 ) -> Callable: 
+_1_7 """Persistently and locally cache the returns of a function. 
+_1_8  
+_1_9 The function to be cached must accept and return dillable objects only (with
+the exception of methods' `self` argument, which is always ignored).
+Additionally, for consistent caching across subsequent sessions, arguments and
+returns should also be hashable. 
+_2_0  
+_2_1 Arguments: 
+_2_2 name (`str | Callable`, optional): The name of the cache (or, if `cache()`
+is being called as an argument-less decorator (ie, as `@cache` instead of
+`@cache(...)`), the function to be cached). Defaults to the qualified name of
+the function. If `dir` is set, this argument will be ignored. 
+_2_3  
+_2_4 dir (`str`, optional): The directory in which the cache should be stored.
+Defaults to a subdirectory named after the hash of the cache's name in a parent
+folder named '.persist_cache' in the current working directory. 
+_2_5  
+_2_6 expiry (`int | float | timedelta`, optional): How long, in seconds or as a
+`timedelta`, function calls should persist in the cache. Defaults to `None`. 
+_2_7  
+_2_8 Returns: 
+_2_9 `Callable`: If `cache()` is called with arguments, a decorator that wraps
+the function to be cached, otherwise, the wrapped function itself. Once
+wrapped, the function will have the following methods attached to it: 
+_3_0 - `set_expiry(value: int | float | timedelta) -> None`: Set the expiry of
+the cache. 
+_3_1 - `flush_cache() -> None`: Flush out any expired cached returns. 
+_3_2 - `clear_cache() -> None`: Clear out all cached returns. 
+_3_3 - `delete_cache() -> None`: Delete the cache.""" 
+_3_4 
+_3_5 def decorator(func: Callable) -> Callable: 
+_3_6 nonlocal name, dir, expiry 
+_3_7 
+_3_8 # If the cache directory has not been set, and the name of the cache has,
+set it to a subdirectory by the name of the hash of that name in a directory
+named '.persist_cache' in the current working directory, or, if the name of the
+cache has not been set, set the name of that subdirectory to the hash of the
+qualified name of the function. 
+_3_9 if dir is None: 
+_4_0 name = name if name is not None else func.__qualname__ 
 _4_1 
-_4_2STR_SIGNATURES = (PICKLE_SIGNATURE, BYTES_SIGNATURE, BYTEARRAY_SIGNATURE) 
-_4_3"""The signatures of data types that are serialized as strings.""" 
-_4_4 
-_4_5ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES = (bool, float, type(None),) 
-_4_6"""Types that are absolutely directly msgpackable.""" 
+_4_2 dir = f'.persist_cache/{caching.shorthash(name)}' 
+_4_3 
+_4_4 # Create the cache directory and any other necessary directories if it does
+not exist. 
+_4_5 if not os.path.exists(dir): 
+_4_6 os.makedirs(dir, exist_ok=True) 
 _4_7 
-_4_8def directly_msgpackable(data: Any) -> bool: 
-_4_9 """Determine whether the provided data is directly msgpackable.""" 
-_5_0 
-_5_1 # Data will be directly msgpackable if: 
-_5_2 # - It is a string and it does not start with any of the signatures of data
-types that are serialized as strings; 
-_5_3 # - It is an integer and is between -2**63 and 2**64-1, inclusive; 
-_5_4 # - It is a list and all of its elements are directly msgpackable and it is
-either empty or its first element is not a signature of a data type that is
-serialized as a list; 
-_5_5 # - It is a dictionary and all of its keys and values are directly
-msgpackable; or 
-_5_6 # - It is of a type specified by `ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES`. 
-_5_7 if (isinstance(data, str) and not any(data.startswith(str_signature) for
-str_signature in STR_SIGNATURES)) \ 
-_5_8 or isinstance(data, int) and -2**63 <= data <= 2**64-1 \ 
-_5_9 or (isinstance(data, list) and all(directly_msgpackable(d) for d in data)
-and (len(data) == 0 or data[0] not in LISTED_SIGNATURES)) \ 
-_6_0 or (isinstance(data, dict) and all(directly_msgpackable(k) and
-directly_msgpackable(v) for k, v in data.items())) \ 
-_6_1 or isinstance(data, ABSOLUTELY_DIRECTLY_MSGPACKABLE_TYPES): 
-_6_2 return True 
-_6_3 
-_6_4 return False 
-_6_5 
-_6_6def make_directly_msgpackable(data: Any) -> Msgpackables: 
-_6_7 """Make the given data capable of being directly serialized to msgpack.""" 
-_6_8 
-_6_9 # If the data is directly msgpackable, return it as is. 
-_7_0 if directly_msgpackable(data): 
-_7_1 return data 
+_4_8 # If an expiry has been set, flush out any expired cached returns. 
+_4_9 if expiry is not None: 
+_5_0 caching.flush(dir, expiry) 
+_5_1 
+_5_2 # Flag whether the function is a method to enable the exclusion of the first
+argument (which will be the instance of the function's class) from being hashed
+to produce the cache key. 
+_5_3 is_method = inspect.ismethod(func) 
+_5_4 
+_5_5 # Preserve a map of the function's arguments to their default values and the
+name and index of the args parameter if such a parameter exists to enable the
+remapping of positional arguments to their keywords, which thereby allows for
+the consistent caching of function calls where positional arguments are used on
+some occasions and keyword arguments are used on others. 
+_5_6 signature, args_parameter, args_i = signaturize(func) 
+_5_7 
+_5_8 # Initialise a wrapper for synchronous functions. 
+_5_9 def sync_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any: 
+_6_0 nonlocal dir, expiry, is_method 
+_6_1 
+_6_2 # Map arguments to their keywords or the keyword of the args parameter where
+necessary, filtering out the first argument if the function is a method, to
+enable the consistent caching of function calls where positional arguments are
+used on some occasions and keyword arguments are used on others. 
+_6_3 arguments = inflate_arguments(signature, args_parameter, args_i, args
+[is_method:], kwargs) 
+_6_4 
+_6_5 # Hash the arguments to produce the cache key. 
+_6_6 key = caching.hash(arguments) 
+_6_7 
+_6_8 # Get the value of the key from the cache if it is not expired, otherwise,
+call the function and set the value of the key in the cache to the result of
+that call. 
+_6_9 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
+_7_0 value = func(*args, **kwargs) 
+_7_1 caching.set(key, value, dir) 
 _7_2 
-_7_3 # If the data is a tuple, make all of its elements directly msgpackable and
-return it as a list with a signature indicating that it is a tuple. 
-_7_4 elif isinstance(data, tuple): 
-_7_5 return [TUPLE_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
-_7_6 
-_7_7 # If the data is a set, make all of its elements directly msgpackable and
-return it as a list with a signature indicating that it is a set. 
-_7_8 elif isinstance(data, set): 
-_7_9 return [SET_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
-_8_0 
-_8_1 # If the data is a bytes object, return it as a string with a signature
-indicating that it is a bytes object. 
-_8_2 elif isinstance(data, bytes): 
-_8_3 return f'{BYTES_SIGNATURE}{data.decode("latin1")}' 
+_7_3 return value 
+_7_4 
+_7_5 # Initialise a wrapper for asynchronous functions. 
+_7_6 async def async_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any:
+ 
+_7_7 nonlocal dir, expiry, is_method 
+_7_8 
+_7_9 # Map arguments to their keywords or the keyword of the args parameter where
+necessary, filtering out the first argument if the function is a method, to
+enable the consistent caching of function calls where positional arguments are
+used on some occasions and keyword arguments are used on others. 
+_8_0 arguments = inflate_arguments(signature, args_parameter, args_i, args
+[is_method:], kwargs) 
+_8_1 
+_8_2 # Hash the arguments to produce the cache key. 
+_8_3 key = caching.hash(arguments) 
 _8_4 
-_8_5 # If the data is a frozenset, make all of its elements directly msgpackable
-and return it as a list with a signature indicating that it is a frozenset. 
-_8_6 elif isinstance(data, frozenset): 
-_8_7 return [FROZENSET_SIGNATURE, *[make_directly_msgpackable(d) for d in data]] 
-_8_8 
-_8_9 # If the data is a bytearray, return it as a string with a signature
-indicating that it is a bytearray. 
-_9_0 elif isinstance(data, bytearray): 
-_9_1 return f'{BYTEARRAY_SIGNATURE}{data.decode("latin1")}' 
-_9_2 
-_9_3 # If the data is incapable of other being forced into a directly msgpackable
-form, pickle it and return it as a string with a signature indicating that it
-is a pickled object. 
-_9_4 return f'{PICKLE_SIGNATURE}{pickle.dumps(data).decode("latin1")}' 
+_8_5 # Get the value of the key from the cache if it is not expired, otherwise,
+call the function and set the value of the key in the cache to the result of
+that call. 
+_8_6 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
+_8_7 value = await func(*args, **kwargs) 
+_8_8 caching.set(key, value, dir) 
+_8_9 
+_9_0 return value 
+_9_1 
+_9_2 # Initialise a wrapper for generator functions. 
+_9_3 def generator_wrapper(*args: tuple[Any], **kwargs: dict[str, Any]) -> Any: 
+_9_4 nonlocal dir, expiry, is_method 
 _9_5 
-_9_6def serialize(data: Any) -> str: 
-_9_7 """Serialize the provided data as msgpack.""" 
+_9_6 # Map arguments to their keywords or the keyword of the args parameter where
+necessary, filtering out the first argument if the function is a method, to
+enable the consistent caching of function calls where positional arguments are
+used on some occasions and keyword arguments are used on others. 
+_9_7 arguments = inflate_arguments(signature, args_parameter, args_i, args
+[is_method:], kwargs) 
 _9_8 
-_9_9 # Force the data into a directly msgpackable form. 
-_1_0_0 data = make_directly_msgpackable(data) 
+_9_9 # Hash the arguments to produce the cache key. 
+_1_0_0 key = caching.hash(arguments) 
 _1_0_1 
-_1_0_2 # Encode the data as msgpack. 
-_1_0_3 data = msgpack_encoder.encode(data) 
-_1_0_4 
-_1_0_5 return data 
-_1_0_6 
-_1_0_7def make_pythonic(data: Msgpackables) -> Any: 
-_1_0_8 """Transform the provided msgpackable data back into Python objects.""" 
-_1_0_9 
-_1_1_0 # If the data is a string, check if it has a signature indicating that it
-is a pickled object, bytes object or bytearray and then decode it to the
-corresponding object, otherwise return it as is. 
-_1_1_1 if isinstance(data, str): 
-_1_1_2 if data.startswith(PICKLE_SIGNATURE): 
-_1_1_3 return pickle.loads(data[PICKLE_SIGNATURE_LEN:].encode("latin1")) 
+_1_0_2 # Get the value of the key from the cache if it is not expired, otherwise,
+call the function and set the value of the key in the cache to the result of
+that call. 
+_1_0_3 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
+_1_0_4 value = [] 
+_1_0_5 
+_1_0_6 for item in func(*args, **kwargs): 
+_1_0_7 value.append(item) 
+_1_0_8 
+_1_0_9 yield item 
+_1_1_0 
+_1_1_1 caching.set(key, value, dir) 
+_1_1_2 
+_1_1_3 return 
 _1_1_4 
-_1_1_5 elif data.startswith(BYTES_SIGNATURE): 
-_1_1_6 return data[BYTES_SIGNATURE_LEN:].encode("latin1") 
+_1_1_5 for item in value: 
+_1_1_6 yield item 
 _1_1_7 
-_1_1_8 elif data.startswith(BYTEARRAY_SIGNATURE): 
-_1_1_9 return bytearray(data[BYTEARRAY_SIGNATURE_LEN:].encode("latin1")) 
-_1_2_0 
-_1_2_1 return data 
-_1_2_2 
-_1_2_3 # If the data is a list, check if it has a signature indicating that it is
-a tuple, set or frozenset and then decode it to the corresponding object,
-otherwise return it as is. 
-_1_2_4 elif isinstance(data, list): 
-_1_2_5 if len(data) != 0: 
-_1_2_6 if data[0] == TUPLE_SIGNATURE: 
-_1_2_7 return tuple(make_pythonic(d) for d in data[1:]) 
-_1_2_8 
-_1_2_9 elif data[0] == SET_SIGNATURE: 
-_1_3_0 return set(make_pythonic(d) for d in data[1:]) 
+_1_1_8 # Initialise a wrapper for asynchronous generator functions. 
+_1_1_9 async def async_generator_wrapper(*args: tuple[Any], **kwargs: dict[str,
+Any]) -> Any: 
+_1_2_0 nonlocal dir, expiry, is_method 
+_1_2_1 
+_1_2_2 # Map arguments to their keywords or the keyword of the args parameter
+where necessary, filtering out the first argument if the function is a method,
+to enable the consistent caching of function calls where positional arguments
+are used on some occasions and keyword arguments are used on others. 
+_1_2_3 arguments = inflate_arguments(signature, args_parameter, args_i, args
+[is_method:], kwargs) 
+_1_2_4 
+_1_2_5 # Hash the arguments to produce the cache key. 
+_1_2_6 key = caching.hash(arguments) 
+_1_2_7 
+_1_2_8 # Get the value of the key from the cache if it is not expired, otherwise,
+call the function and set the value of the key in the cache to the result of
+that call. 
+_1_2_9 if (value := caching.get(key, dir, expiry)) is NOT_IN_CACHE: 
+_1_3_0 value = [] 
 _1_3_1 
-_1_3_2 elif data[0] == FROZENSET_SIGNATURE: 
-_1_3_3 return frozenset(make_pythonic(d) for d in data[1:]) 
+_1_3_2 async for item in func(*args, **kwargs): 
+_1_3_3 value.append(item) 
 _1_3_4 
-_1_3_5 return data 
+_1_3_5 yield item 
 _1_3_6 
-_1_3_7 # If the data is neither a string nor a list, return it as is. 
-_1_3_8 return data 
-_1_3_9 
-_1_4_0def deserialize(data: str) -> Any: 
-_1_4_1 """Deserialize the provided msgpack-encoded data.""" 
-_1_4_2 
-_1_4_3 # Decode the data. 
-_1_4_4 data = msgpack_decoder.decode(data) 
-_1_4_5 
-_1_4_6 # Transform the data back into Python objects. 
-_1_4_7 data = make_pythonic(data) 
+_1_3_7 caching.set(key, value, dir) 
+_1_3_8 
+_1_3_9 return 
+_1_4_0 
+_1_4_1 for item in value: 
+_1_4_2 yield item 
+_1_4_3 
+_1_4_4 # Identify the appropriate wrapper for the function. 
+_1_4_5 if is_async(func): 
+_1_4_6 if inspect.isasyncgenfunction(func): 
+_1_4_7 wrapper = async_generator_wrapper 
 _1_4_8 
-_1_4_9 return data 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-
-14 20:59 +1100
+_1_4_9 else: 
+_1_5_0 wrapper = async_wrapper 
+_1_5_1 
+_1_5_2 elif inspect.isgeneratorfunction(func): 
+_1_5_3 wrapper = generator_wrapper 
+_1_5_4 
+_1_5_5 else: 
+_1_5_6 wrapper = sync_wrapper 
+_1_5_7 
+_1_5_8 # Attach convenience functions to the wrapper for modifying the cache. 
+_1_5_9 def delete_cache() -> None: 
+_1_6_0 """Delete the cache.""" 
+_1_6_1 nonlocal dir 
+_1_6_2 
+_1_6_3 caching.delete(dir) 
+_1_6_4 
+_1_6_5 def clear_cache() -> None: 
+_1_6_6 """Clear the cache.""" 
+_1_6_7 nonlocal dir 
+_1_6_8 
+_1_6_9 caching.clear(dir) 
+_1_7_0 
+_1_7_1 def flush_cache() -> None: 
+_1_7_2 """Flush expired keys from the cache.""" 
+_1_7_3 nonlocal dir, expiry, is_method 
+_1_7_4 
+_1_7_5 caching.flush(dir, expiry) 
+_1_7_6 
+_1_7_7 def set_expiry(value: Union[int, float, timedelta, None]) -> None: 
+_1_7_8 """Set the expiry of the cache. 
+_1_7_9  
+_1_8_0 Arguments: 
+_1_8_1 expiry (`int | float | timedelta`): How long, in seconds or as a
+`timedelta`, function calls should persist in the cache.""" 
+_1_8_2 
+_1_8_3 nonlocal expiry 
+_1_8_4 
+_1_8_5 expiry = value 
+_1_8_6 
+_1_8_7 wrapper.delete_cache = delete_cache 
+_1_8_8 wrapper.clear_cache = clear_cache 
+_1_8_9 wrapper.cache_clear = wrapper.clear_cache # Add an alias for cache_clear
+which is used by lru_cache. 
+_1_9_0 wrapper.flush_cache = flush_cache 
+_1_9_1 wrapper.set_expiry = set_expiry 
+_1_9_2 
+_1_9_3 # Preserve the original function. 
+_1_9_4 wrapper.__wrapped__ = func 
+_1_9_5 
+_1_9_6 # Preserve the function's original signature. 
+_1_9_7 wrapper = wraps(func)(wrapper) 
+_1_9_8 
+_1_9_9 return wrapper 
+_2_0_0 
+_2_0_1 # If the first argument is a function and all of the other arguments are
+`None`, indicating that this decorator factory was invoked without passing any
+arguments, return the result of passing that function to the decorator while
+also emptying the first argument to avoid it being used by the decorator. 
+_2_0_2 if callable(name) and dir is expiry is None: 
+_2_0_3 func = name 
+_2_0_4 name = None 
+_2_0_5 
+_2_0_6 return decorator(func) 
+_2_0_7 
+_2_0_8 return decorator 
+_2_0_9 
+_2_1_0def delete(function_or_name: Union[str, Callable]) -> None: 
+_2_1_1 """Delete the cache of the given function or name. 
+_2_1_2  
+_2_1_3 Arguments: 
+_2_1_4 function_or_name (`str | Callable`): The function or name of the cache to
+be deleted.""" 
+_2_1_5 
+_2_1_6 name = function_or_name if isinstance(function_or_name, str) else
+function_or_name.__qualname__ 
+_2_1_7 caching.delete(f'.persist_cache/{caching.shorthash(name)}') 
+_2_1_8 
+_2_1_9def clear(function_or_name: Union[str, Callable]) -> None: 
+_2_2_0 """Clear the cache of the given function or name. 
+_2_2_1  
+_2_2_2 Arguments: 
+_2_2_3 function_or_name (`str | Callable`): The function or name of the cache to
+be cleared.""" 
+_2_2_4 
+_2_2_5 name = function_or_name if isinstance(function_or_name, str) else
+function_or_name.__qualname__ 
+_2_2_6 caching.clear(f'.persist_cache/{caching.shorthash(name)}') 
+_2_2_7 
+_2_2_8def flush(function_or_name: Union[str, Callable], expiry: Union[int, float,
+timedelta]) -> None: 
+_2_2_9 """Flush expired keys from the cache of the given function or name. 
+_2_3_0  
+_2_3_1 Arguments: 
+_2_3_2 function_or_name (`str | Callable`): The function or name of the cache to
+be flushed. 
+_2_3_3 expiry (`int | float | timedelta`): How long, in seconds or as a
+`timedelta`, function calls should persist in the cache.""" 
+_2_3_4 
+_2_3_5 name = function_or_name if isinstance(function_or_name, str) else
+function_or_name.__qualname__ 
+_2_3_6 caching.flush(f'.persist_cache/{caching.shorthash(name)}', expiry) 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-
+06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/favicon_32.png` & `persist_cache-0.4.0/tests/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/tests/htmlcov/index.html` & `persist_cache-0.4.0/tests/htmlcov/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">98%</span>
+            <span class="pc_cov">75%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:06 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -66,60 +66,67 @@
                 <td>1</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="1 1">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_5cadf2fa0b1853af_caching_py.html">C:\Python311\Lib\site-packages\persist_cache\caching.py</a></td>
-                <td>39</td>
+                <td>43</td>
+                <td>8</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="39 39">100%</td>
+                <td class="right" data-ratio="35 43">81%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_5cadf2fa0b1853af_helpers_py.html">C:\Python311\Lib\site-packages\persist_cache\helpers.py</a></td>
                 <td>36</td>
-                <td>5</td>
+                <td>7</td>
                 <td>0</td>
-                <td class="right" data-ratio="31 36">86%</td>
+                <td class="right" data-ratio="29 36">81%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_5cadf2fa0b1853af_persist_cache_py.html">C:\Python311\Lib\site-packages\persist_cache\persist_cache.py</a></td>
-                <td>55</td>
+                <td>94</td>
+                <td>40</td>
                 <td>0</td>
+                <td class="right" data-ratio="54 94">57%</td>
+            </tr>
+            <tr class="file">
+                <td class="name left"><a href="d_5cadf2fa0b1853af_pickle_py.html">C:\Python311\Lib\site-packages\persist_cache\pickle.py</a></td>
+                <td>9</td>
+                <td>9</td>
                 <td>0</td>
-                <td class="right" data-ratio="55 55">100%</td>
+                <td class="right" data-ratio="0 9">0%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_5cadf2fa0b1853af_serialization_py.html">C:\Python311\Lib\site-packages\persist_cache\serialization.py</a></td>
                 <td>75</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="75 75">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>206</td>
-                <td>5</td>
+                <td>258</td>
+                <td>64</td>
                 <td>0</td>
-                <td class="right" data-ratio="201 206">98%</td>
+                <td class="right" data-ratio="194 258">75%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2024-03-14 21:06 +1100
+            created at 2024-05-06 20:49 +1000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_5cadf2fa0b1853af_serialization_py.html"/>
         <a id="nextFileLink" class="nav" href="d_5cadf2fa0b1853af___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9988%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 7755%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-14 21:06 +1100
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-06 20:49 +1000
 MMoodduullee                                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  1          0       0        100%
 _p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_____i_n_i_t_____._p_y
-_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  39         0       0        100%
+_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  43         8       0        81%
 _p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_c_a_c_h_i_n_g_._p_y
-_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  36         5       0        86%
+_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  36         7       0        81%
 _p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_h_e_l_p_e_r_s_._p_y
-_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  55         0       0        100%
+_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  94         40      0        57%
 _p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_p_e_r_s_i_s_t___c_a_c_h_e_._p_y
+_C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  9          9       0        0%
+_p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_p_i_c_k_l_e_._p_y
 _C_:_\_P_y_t_h_o_n_3_1_1_\_L_i_b_\_s_i_t_e_-                  75         0       0        100%
 _p_a_c_k_a_g_e_s_\_p_e_r_s_i_s_t___c_a_c_h_e_\_s_e_r_i_a_l_i_z_a_t_i_o_n_._p_y
-Total                                   206        5       0        98%
+Total                                   258        64      0        75%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-03-14 21:06 +1100
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2024-05-06 20:49 +1000
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/keybd_closed.png` & `persist_cache-0.4.0/tests/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/tests/htmlcov/keybd_open.png` & `persist_cache-0.4.0/tests/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/tests/htmlcov/status.json` & `persist_cache-0.4.0/tests/htmlcov/status.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9657021604938272%*

 * *Differences: {"'files'": "{'d_5cadf2fa0b1853af___init___py': {'hash': '7837b614b3568f8ad6b49ef1be2102c3'}, "*

 * *            "'d_5cadf2fa0b1853af_caching_py': {'hash': 'ca762ffba4a0dab4dca201171d405afd', "*

 * *            "'index': {'nums': {insert: [(2, 43), (4, 8)], delete: [3, 2]}}}, "*

 * *            "'d_5cadf2fa0b1853af_helpers_py': {'hash': 'b14979acb4ee81ad98d8e7b70b9983bd', "*

 * *            "'index': {'nums': {insert: [(4, 7)], delete: [4]}}}, "*

 * *            "'d_5cadf2fa0b1853af_persist_cache_py': {'hash': '3559fa8aefa249f51e05 […]*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_5cadf2fa0b1853af___init___py": {
-            "hash": "d15316c8c6dd8f7e77f03079a319c404",
+            "hash": "7837b614b3568f8ad6b49ef1be2102c3",
             "index": {
                 "html_filename": "d_5cadf2fa0b1853af___init___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -14,66 +14,83 @@
                     0,
                     0
                 ],
                 "relative_filename": "C:\\Python311\\Lib\\site-packages\\persist_cache\\__init__.py"
             }
         },
         "d_5cadf2fa0b1853af_caching_py": {
-            "hash": "e5c50bcaa366c3fc980ad7a9c2a03b24",
+            "hash": "ca762ffba4a0dab4dca201171d405afd",
             "index": {
                 "html_filename": "d_5cadf2fa0b1853af_caching_py.html",
                 "nums": [
                     0,
                     1,
-                    39,
-                    0,
+                    43,
                     0,
+                    8,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "C:\\Python311\\Lib\\site-packages\\persist_cache\\caching.py"
             }
         },
         "d_5cadf2fa0b1853af_helpers_py": {
-            "hash": "aa6982852b10557cb56831c375b60d91",
+            "hash": "b14979acb4ee81ad98d8e7b70b9983bd",
             "index": {
                 "html_filename": "d_5cadf2fa0b1853af_helpers_py.html",
                 "nums": [
                     0,
                     1,
                     36,
                     0,
-                    5,
+                    7,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "C:\\Python311\\Lib\\site-packages\\persist_cache\\helpers.py"
             }
         },
         "d_5cadf2fa0b1853af_persist_cache_py": {
-            "hash": "2a97ca5bc92c712146005b91a3da2354",
+            "hash": "3559fa8aefa249f51e0500b76dc91039",
             "index": {
                 "html_filename": "d_5cadf2fa0b1853af_persist_cache_py.html",
                 "nums": [
                     0,
                     1,
-                    55,
-                    0,
+                    94,
                     0,
+                    40,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "C:\\Python311\\Lib\\site-packages\\persist_cache\\persist_cache.py"
             }
         },
+        "d_5cadf2fa0b1853af_pickle_py": {
+            "hash": "8c3c16aff4cfbc06225cdafb64d2f87b",
+            "index": {
+                "html_filename": "d_5cadf2fa0b1853af_pickle_py.html",
+                "nums": [
+                    0,
+                    1,
+                    9,
+                    0,
+                    9,
+                    0,
+                    0,
+                    0
+                ],
+                "relative_filename": "C:\\Python311\\Lib\\site-packages\\persist_cache\\pickle.py"
+            }
+        },
         "d_5cadf2fa0b1853af_serialization_py": {
-            "hash": "72c281e0a027271d5955d10b127aed56",
+            "hash": "b6440cd226ee8aea33833c1e23ec0cd1",
             "index": {
                 "html_filename": "d_5cadf2fa0b1853af_serialization_py.html",
                 "nums": [
                     0,
                     1,
                     75,
                     0,
```

### Comparing `persist_cache-0.3.2/tests/htmlcov/style.css` & `persist_cache-0.4.0/tests/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/LICENCE` & `persist_cache-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `persist_cache-0.3.2/README.md` & `persist_cache-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 `persist-cache` is an *easy-to-use* Python library for lightning-fast persistent function caching. It is capable of caching both synchronous and asynchronous functions as well as methods, and is also process-safe and thread-safe.
 
 ## Features 🎯
 - **⚡ Lightning-fast**: a function call can be cached in as little as 145 microseconds and be returned back in as few as 95 microseconds.
 - **💽 Persistent**: cached returns persist across sessions and are stored locally.
 - **⌛ Stale-free**: cached returns may be given a shelf life, after which they will be automatically flushed out.
 - **🦺 Process- and thread-safe**: interprocess file locks prevent processes and threads from writing over each other.
-- **⏱️ Async-compatible**: asynchronous functions can be cached with the same decorator as synchronous ones.
+- **⏱️ Async-compatible**: asynchronous functions can be cached with the same decorator as synchronous ones, generators included.
 - **👨‍🏫 Class-compatible**: methods can be cached with the same decorator as functions (although the `self` argument is always ignored).
 
 ## Installation 🧑‍🔧
 `persist-cache` may be installed with `pip`:
 ```bash
 pip install persist-cache
 ```
@@ -45,18 +45,25 @@
 
 @cache(name='my_shared_cache', expiry=60 * 60 * 24 * 30)
 def my_other_function(): ...
 ```
 
 Once created, cached functions may be managed as follows:
 ```python
-my_function.set_expiry(60 * 60) # Change cached returns to expire after an hour.
-my_function.flush_cache() # Flush out any expired cached returns.
-my_function.clear_cache() # Clear out all cached returns.
-my_function.delete_cache() # Delete the cache.
+# Change cached returns to expire after an hour.
+my_function.set_expiry(60 * 60)
+
+# Flush out any expired cached returns.
+my_function.flush_cache() or persist_cache.flush(my_function, 60 * 60) or persist_cache.flush('my_shared_cache', 60 * 60)
+
+# Clear out all cached returns.
+my_function.clear_cache() or persist_cache.clear(my_function) or persist_cache.clear('my_shared_cache')
+
+# Delete the cache.
+my_function.delete_cache() or persist_cache.delete(my_function) or persist_cache.delete('my_shared_cache')
 ```
 
 ## API 🧩
 ### `cache()`
 ```python
 def cache(
     name: str | Callable | None = None,
@@ -79,9 +86,39 @@
 
 After being wrapped, the cached function will have the following methods attached to it:
 - `set_expiry(value: int | float | timedelta) -> None`: Sets the expiry of the cache.
 - `flush_cache() -> None`: Flushes out any expired cached returns.
 - `clear_cache() -> None`: Clears out all cached returns.
 - `delete_cache() -> None`: Deletes the cache.
 
+### `flush()`
+```python
+def flush(
+    function_or_name: str | Callable,
+    expiry: int | float | timedelta,
+) -> None
+```
+
+`flush()` flushes out any expired cached returns from a cache.
+
+`function_or_name` represents the function or the name of the cache to be flushed.
+
+### `clear()`
+```python
+def clear(function_or_name: str | Callable) -> None
+```
+
+`clear()` clears out all cached returns from a cache.
+
+`function_or_name` represents the function or the name of the cache to be cleared.
+
+### `delete()`
+```python
+def delete(function_or_name: str | Callable) -> None
+```
+
+`delete()` deletes a cache.
+
+`function_or_name` represents the function or the name of the cache to be deleted.
+
 ## Licence 📜
 This library is licensed under the [MIT Licence](https://github.com/umarbutler/persist-cache/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -7,47 +7,60 @@
 safe. ## Features ð¯ - **â¡ Lightning-fast**: a function call can be cached
 in as little as 145 microseconds and be returned back in as few as 95
 microseconds. - **ð½ Persistent**: cached returns persist across sessions and
 are stored locally. - **â Stale-free**: cached returns may be given a shelf
 life, after which they will be automatically flushed out. - **ð¦º Process- and
 thread-safe**: interprocess file locks prevent processes and threads from
 writing over each other. - **â±ï¸ Async-compatible**: asynchronous functions
-can be cached with the same decorator as synchronous ones. - **ð¨âð«
-Class-compatible**: methods can be cached with the same decorator as functions
-(although the `self` argument is always ignored). ## Installation ð§âð§
-`persist-cache` may be installed with `pip`: ```bash pip install persist-cache
-``` ## Usage ð©âð» The code snippet below demonstrates how both
-synchronous and asynchronous functions as well as methods may be cached with
-`persist-cache`: ```python from persist_cache import cache @cache def
-my_function(): ... @cache async def my_function(): ... class MyClass: @cache
-def my_method(self): ... @cache async def my_method(self): ... ``` It is also
-possible to name caches and specify their shelf life: ```python from datetime
-import timedelta @cache(name='my_shared_cache', expiry=timedelta(months=1)) def
-my_function(): ... @cache(name='my_shared_cache', expiry=60 * 60 * 24 * 30) def
-my_other_function(): ... ``` Once created, cached functions may be managed as
-follows: ```python my_function.set_expiry(60 * 60) # Change cached returns to
-expire after an hour. my_function.flush_cache() # Flush out any expired cached
-returns. my_function.clear_cache() # Clear out all cached returns.
-my_function.delete_cache() # Delete the cache. ``` ## API ð§© ### `cache()`
-```python def cache( name: str | Callable | None = None, dir: str | None =
-None, expiry: int | float | timedelta | None = None, ) -> None ``` `cache()`
-persistently and locally cache the returns of a function. The function to be
-cached must accept and return [dillable](https://dill.readthedocs.io/en/latest/
-) objects only (with the exception of methods' `self` argument, which is always
-ignored). Additionally, for consistent caching across subsequent sessions,
-arguments and returns should also be hashable. `name` represents the name of
-the cache (or, if `cache()` is being called as an argument-less decorator (ie,
-as `@cache` instead of `@cache(...)`), the function to be cached). It defaults
-to the qualified name of the function. If `dir` is set, `name` will be ignored.
-`dir` represents the directory in which the cache should be stored. It defaults
-to a subdirectory named after the hash of the cache's name in a parent folder
-named '.persist_cache' in the current working directory. `expiry` represents
-how long, in seconds or as a `timedelta`, function calls should persist in the
+can be cached with the same decorator as synchronous ones, generators included.
+- **ð¨âð« Class-compatible**: methods can be cached with the same
+decorator as functions (although the `self` argument is always ignored). ##
+Installation ð§âð§ `persist-cache` may be installed with `pip`: ```bash
+pip install persist-cache ``` ## Usage ð©âð» The code snippet below
+demonstrates how both synchronous and asynchronous functions as well as methods
+may be cached with `persist-cache`: ```python from persist_cache import cache
+@cache def my_function(): ... @cache async def my_function(): ... class
+MyClass: @cache def my_method(self): ... @cache async def my_method(self): ...
+``` It is also possible to name caches and specify their shelf life: ```python
+from datetime import timedelta @cache(name='my_shared_cache', expiry=timedelta
+(months=1)) def my_function(): ... @cache(name='my_shared_cache', expiry=60 *
+60 * 24 * 30) def my_other_function(): ... ``` Once created, cached functions
+may be managed as follows: ```python # Change cached returns to expire after an
+hour. my_function.set_expiry(60 * 60) # Flush out any expired cached returns.
+my_function.flush_cache() or persist_cache.flush(my_function, 60 * 60) or
+persist_cache.flush('my_shared_cache', 60 * 60) # Clear out all cached returns.
+my_function.clear_cache() or persist_cache.clear(my_function) or
+persist_cache.clear('my_shared_cache') # Delete the cache.
+my_function.delete_cache() or persist_cache.delete(my_function) or
+persist_cache.delete('my_shared_cache') ``` ## API ð§© ### `cache()` ```python
+def cache( name: str | Callable | None = None, dir: str | None = None, expiry:
+int | float | timedelta | None = None, ) -> None ``` `cache()` persistently and
+locally cache the returns of a function. The function to be cached must accept
+and return [dillable](https://dill.readthedocs.io/en/latest/) objects only
+(with the exception of methods' `self` argument, which is always ignored).
+Additionally, for consistent caching across subsequent sessions, arguments and
+returns should also be hashable. `name` represents the name of the cache (or,
+if `cache()` is being called as an argument-less decorator (ie, as `@cache`
+instead of `@cache(...)`), the function to be cached). It defaults to the
+qualified name of the function. If `dir` is set, `name` will be ignored. `dir`
+represents the directory in which the cache should be stored. It defaults to a
+subdirectory named after the hash of the cache's name in a parent folder named
+'.persist_cache' in the current working directory. `expiry` represents how
+long, in seconds or as a `timedelta`, function calls should persist in the
 cache. It defaults to `None`. If `cache()` is called with arguments, a
 decorator that wraps the function to be cached will be returned, otherwise, the
 wrapped function itself will be returned. After being wrapped, the cached
 function will have the following methods attached to it: - `set_expiry(value:
 int | float | timedelta) -> None`: Sets the expiry of the cache. - `flush_cache
 () -> None`: Flushes out any expired cached returns. - `clear_cache() -> None`:
 Clears out all cached returns. - `delete_cache() -> None`: Deletes the cache.
-## Licence ð This library is licensed under the [MIT Licence](https://
-github.com/umarbutler/persist-cache/blob/main/LICENCE).
+### `flush()` ```python def flush( function_or_name: str | Callable, expiry:
+int | float | timedelta, ) -> None ``` `flush()` flushes out any expired cached
+returns from a cache. `function_or_name` represents the function or the name of
+the cache to be flushed. ### `clear()` ```python def clear(function_or_name:
+str | Callable) -> None ``` `clear()` clears out all cached returns from a
+cache. `function_or_name` represents the function or the name of the cache to
+be cleared. ### `delete()` ```python def delete(function_or_name: str |
+Callable) -> None ``` `delete()` deletes a cache. `function_or_name` represents
+the function or the name of the cache to be deleted. ## Licence ð This
+library is licensed under the [MIT Licence](https://github.com/umarbutler/
+persist-cache/blob/main/LICENCE).
```

### Comparing `persist_cache-0.3.2/pyproject.toml` & `persist_cache-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "persist-cache"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   {name="Umar Butler", email="umar@umar.au"},
 ]
 description = "An easy-to-use Python library for lightning-fast persistent function caching."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
```

