# Comparing `tmp/py-memoize-2.0.0.tar.gz` & `tmp/py-memoize-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-memoize-2.0.0.tar", last modified: Sat May  4 16:34:55 2024, max compression
+gzip compressed data, was "py-memoize-2.1.0.tar", last modified: Mon May  6 11:52:32 2024, max compression
```

## Comparing `py-memoize-2.0.0.tar` & `py-memoize-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:34:55.765524 py-memoize-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 16:34:44.000000 py-memoize-2.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 16:34:44.000000 py-memoize-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-04 16:34:55.765524 py-memoize-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-05-04 16:34:44.000000 py-memoize-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:34:55.765524 py-memoize-2.0.0/memoize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/coerced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/entrybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/invalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/memoize_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-04 16:34:44.000000 py-memoize-2.0.0/memoize/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:34:55.765524 py-memoize-2.0.0/py_memoize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-04 16:34:55.000000 py-memoize-2.0.0/py_memoize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 16:34:55.000000 py-memoize-2.0.0/py_memoize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:34:55.000000 py-memoize-2.0.0/py_memoize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 16:34:55.000000 py-memoize-2.0.0/py_memoize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 16:34:55.000000 py-memoize-2.0.0/py_memoize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:34:55.765524 py-memoize-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 16:34:44.000000 py-memoize-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:52:32.492176 py-memoize-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-06 11:52:24.000000 py-memoize-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-06 11:52:24.000000 py-memoize-2.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-06 11:52:24.000000 py-memoize-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19315 2024-05-06 11:52:32.492176 py-memoize-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-05-06 11:52:24.000000 py-memoize-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:52:32.492176 py-memoize-2.1.0/memoize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/entrybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/memoize_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-06 11:52:24.000000 py-memoize-2.1.0/memoize/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:52:32.492176 py-memoize-2.1.0/py_memoize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19315 2024-05-06 11:52:32.000000 py-memoize-2.1.0/py_memoize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 11:52:32.000000 py-memoize-2.1.0/py_memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:52:32.000000 py-memoize-2.1.0/py_memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 11:52:32.000000 py-memoize-2.1.0/py_memoize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 11:52:32.000000 py-memoize-2.1.0/py_memoize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:52:32.492176 py-memoize-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 11:52:24.000000 py-memoize-2.1.0/setup.py
```

### Comparing `py-memoize-2.0.0/LICENCE` & `py-memoize-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/PKG-INFO` & `py-memoize-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 2.0.0
+Version: 2.1.0
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -215,14 +215,18 @@
 * storage for cached entries/items (see `memoize.storage.CacheStorage`);
   in-memory storage is already provided;
   for convenience of implementing new storage adapters some SerDe (`memoize.serde.SerDe`) are provided;
 * eviction strategy (see `memoize.eviction.EvictionStrategy`);
   least-recently-updated strategy is already provided;
 * entry builder (see `memoize.entrybuilder.CacheEntryBuilder`)
   which has control over ``update_after``  & ``expires_after`` described in `Tunable eviction & async refreshing`_
+* value post-processing (see `memoize.postprocessing.Postprocessing`);
+  noop is the default one;
+  deep-copy post-processing is also provided (be wary of deep-copy cost & limitations,
+  but deep-copying allows callers to safely modify values retrieved from an in-memory cache).
 
 All of these elements are open for extension (you can implement and plug-in your own).
 Please contribute!
 
 Example how to customize default config (everything gets overridden):
 
 ..
@@ -232,38 +236,41 @@
 
     from datetime import timedelta
 
     from memoize.configuration import MutableCacheConfiguration, DefaultInMemoryCacheConfiguration
     from memoize.entrybuilder import ProvidedLifeSpanCacheEntryBuilder
     from memoize.eviction import LeastRecentlyUpdatedEvictionStrategy
     from memoize.key import EncodedMethodNameAndArgsKeyExtractor
+    from memoize.postprocessing import DeepcopyPostprocessing
     from memoize.storage import LocalInMemoryCacheStorage
     from memoize.wrapper import memoize
 
-
-    @memoize(configuration=MutableCacheConfiguration
-             .initialized_with(DefaultInMemoryCacheConfiguration())
-             .set_method_timeout(value=timedelta(minutes=2))
-             .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
-                                                                  expire_after=timedelta(minutes=5)))
-             .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
-             .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
-             .set_storage(LocalInMemoryCacheStorage())
-             )
+    @memoize(
+        configuration=MutableCacheConfiguration
+        .initialized_with(DefaultInMemoryCacheConfiguration())
+        .set_method_timeout(value=timedelta(minutes=2))
+        .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
+                                                             expire_after=timedelta(minutes=5)))
+        .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
+        .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
+        .set_storage(LocalInMemoryCacheStorage())
+        .set_postprocessing(DeepcopyPostprocessing())
+    )
     async def cached():
         return 'dummy'
 
 
 Still, you can use default configuration which:
 
 * sets timeout for underlying method to 2 minutes;
 * uses in-memory storage;
 * uses method instance & arguments to infer cache key;
 * stores up to 4096 elements in cache and evicts entries according to least recently updated policy;
-* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes.
+* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes;
+* does not post-process cached values.
 
 If that satisfies you, just use default config:
 
 ..
     _example_source: examples/configuration/default_configuration.py
 
 .. code-block:: python
```

### Comparing `py-memoize-2.0.0/README.rst` & `py-memoize-2.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -188,14 +188,18 @@
 * storage for cached entries/items (see :class:`memoize.storage.CacheStorage`);
   in-memory storage is already provided;
   for convenience of implementing new storage adapters some SerDe (:class:`memoize.serde.SerDe`) are provided;
 * eviction strategy (see :class:`memoize.eviction.EvictionStrategy`);
   least-recently-updated strategy is already provided;
 * entry builder (see :class:`memoize.entrybuilder.CacheEntryBuilder`)
   which has control over ``update_after``  & ``expires_after`` described in `Tunable eviction & async refreshing`_
+* value post-processing (see :class:`memoize.postprocessing.Postprocessing`);
+  noop is the default one;
+  deep-copy post-processing is also provided (be wary of deep-copy cost & limitations,
+  but deep-copying allows callers to safely modify values retrieved from an in-memory cache).
 
 All of these elements are open for extension (you can implement and plug-in your own).
 Please contribute!
 
 Example how to customize default config (everything gets overridden):
 
 ..
@@ -205,38 +209,41 @@
 
     from datetime import timedelta
 
     from memoize.configuration import MutableCacheConfiguration, DefaultInMemoryCacheConfiguration
     from memoize.entrybuilder import ProvidedLifeSpanCacheEntryBuilder
     from memoize.eviction import LeastRecentlyUpdatedEvictionStrategy
     from memoize.key import EncodedMethodNameAndArgsKeyExtractor
+    from memoize.postprocessing import DeepcopyPostprocessing
     from memoize.storage import LocalInMemoryCacheStorage
     from memoize.wrapper import memoize
 
-
-    @memoize(configuration=MutableCacheConfiguration
-             .initialized_with(DefaultInMemoryCacheConfiguration())
-             .set_method_timeout(value=timedelta(minutes=2))
-             .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
-                                                                  expire_after=timedelta(minutes=5)))
-             .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
-             .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
-             .set_storage(LocalInMemoryCacheStorage())
-             )
+    @memoize(
+        configuration=MutableCacheConfiguration
+        .initialized_with(DefaultInMemoryCacheConfiguration())
+        .set_method_timeout(value=timedelta(minutes=2))
+        .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
+                                                             expire_after=timedelta(minutes=5)))
+        .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
+        .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
+        .set_storage(LocalInMemoryCacheStorage())
+        .set_postprocessing(DeepcopyPostprocessing())
+    )
     async def cached():
         return 'dummy'
 
 
 Still, you can use default configuration which:
 
 * sets timeout for underlying method to 2 minutes;
 * uses in-memory storage;
 * uses method instance & arguments to infer cache key;
 * stores up to 4096 elements in cache and evicts entries according to least recently updated policy;
-* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes.
+* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes;
+* does not post-process cached values.
 
 If that satisfies you, just use default config:
 
 ..
     _example_source: examples/configuration/default_configuration.py
 
 .. code-block:: python
```

### Comparing `py-memoize-2.0.0/memoize/coerced.py` & `py-memoize-2.1.0/memoize/coerced.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/configuration.py` & `py-memoize-2.1.0/memoize/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from abc import ABCMeta, abstractmethod
 from datetime import timedelta
 
 from memoize.entrybuilder import CacheEntryBuilder, ProvidedLifeSpanCacheEntryBuilder
 from memoize.eviction import EvictionStrategy, LeastRecentlyUpdatedEvictionStrategy
 from memoize.key import KeyExtractor, EncodedMethodReferenceAndArgsKeyExtractor
+from memoize.postprocessing import Postprocessing, NoPostprocessing
 from memoize.storage import CacheStorage
 from memoize.storage import LocalInMemoryCacheStorage
 
 
 class NotConfiguredCacheCalledException(Exception):
     pass
 
@@ -47,48 +48,59 @@
         raise NotImplementedError()
 
     @abstractmethod
     def eviction_strategy(self) -> EvictionStrategy:
         """ Determines which EvictionStrategy is to be used by cache. """
         raise NotImplementedError()
 
+    @abstractmethod
+    def postprocessing(self) -> Postprocessing:
+        """ Determines which/if Postprocessing is to be used by cache. """
+        raise NotImplementedError()
+
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
-        return "{name}[configured={configured}, method_timeout={method_timeout}, entry_builder={entry_builder}," \
-               " key_extractor={key_extractor}, storage={storage}, eviction_strategy={eviction_strategy}]" \
-            .format(name=self.__class__, configured=self.configured(), method_timeout=self.method_timeout(),
-                    entry_builder=self.entry_builder(), key_extractor=self.key_extractor(), storage=self.storage(),
-                    eviction_strategy=self.eviction_strategy())
+        return (f"{self.__class__}["
+                f"configured={self.configured()}, "
+                f"method_timeout={self.method_timeout()}, "
+                f"entry_builder={self.entry_builder()}, "
+                f"key_extractor={self.key_extractor()}, "
+                f"storage={self.storage()}, "
+                f"eviction_strategy={self.eviction_strategy()}, "
+                f"postprocessing={self.postprocessing()}"
+                f"]")
 
 
 class MutableCacheConfiguration(CacheConfiguration):
     """ Mutable configuration which can be change at runtime.
     May be also used to customize existing configuration (for example a default one, which is immutable)."""
 
     def __init__(self, configured: bool, storage: CacheStorage, key_extractor: KeyExtractor,
-                 eviction_strategy: EvictionStrategy, entry_builder: CacheEntryBuilder,
+                 eviction_strategy: EvictionStrategy, entry_builder: CacheEntryBuilder, postprocessing: Postprocessing,
                  method_timeout: timedelta) -> None:
         self.__storage = storage
         self.__configured = configured
         self.__key_extractor = key_extractor
         self.__entry_builder = entry_builder
         self.__method_timeout = method_timeout
         self.__eviction_strategy = eviction_strategy
+        self.__postprocessing = postprocessing
 
     @staticmethod
     def initialized_with(configuration: CacheConfiguration) -> 'MutableCacheConfiguration':
         return MutableCacheConfiguration(
             storage=configuration.storage(),
             configured=configuration.configured(),
             key_extractor=configuration.key_extractor(),
             entry_builder=configuration.entry_builder(),
             method_timeout=configuration.method_timeout(),
             eviction_strategy=configuration.eviction_strategy(),
+            postprocessing=configuration.postprocessing(),
         )
 
     def method_timeout(self) -> timedelta:
         return self.__method_timeout
 
     def key_extractor(self) -> KeyExtractor:
         return self.__key_extractor
@@ -101,14 +113,17 @@
 
     def entry_builder(self) -> CacheEntryBuilder:
         return self.__entry_builder
 
     def eviction_strategy(self) -> EvictionStrategy:
         return self.__eviction_strategy
 
+    def postprocessing(self) -> Postprocessing:
+        return self.__postprocessing
+
     def set_method_timeout(self, value: timedelta) -> 'MutableCacheConfiguration':
         self.__method_timeout = value
         return self
 
     def set_key_extractor(self, value: KeyExtractor) -> 'MutableCacheConfiguration':
         self.__key_extractor = value
         return self
@@ -125,27 +140,32 @@
         self.__entry_builder = value
         return self
 
     def set_eviction_strategy(self, value: EvictionStrategy) -> 'MutableCacheConfiguration':
         self.__eviction_strategy = value
         return self
 
+    def set_postprocessing(self, value: Postprocessing) -> 'MutableCacheConfiguration':
+        self.__postprocessing = value
+        return self
+
 
 class DefaultInMemoryCacheConfiguration(CacheConfiguration):
     """ Default parameters that describe in-memory cache. Be ware that parameters used do not suit every case. """
 
     def __init__(self, capacity: int = 4096, method_timeout: timedelta = timedelta(minutes=2),
                  update_after: timedelta = timedelta(minutes=10),
                  expire_after: timedelta = timedelta(minutes=30)) -> None:
         self.__configured = True
         self.__method_timeout = method_timeout
         self.__storage = LocalInMemoryCacheStorage()
         self.__key_extractor = EncodedMethodReferenceAndArgsKeyExtractor()
         self.__eviction_strategy = LeastRecentlyUpdatedEvictionStrategy(capacity=capacity)
         self.__entry_builder = ProvidedLifeSpanCacheEntryBuilder(update_after=update_after, expire_after=expire_after)
+        self.__postprocessing = NoPostprocessing()
 
     def configured(self) -> bool:
         return self.__configured
 
     def method_timeout(self) -> timedelta:
         return self.__method_timeout
 
@@ -156,7 +176,10 @@
         return self.__entry_builder
 
     def eviction_strategy(self) -> LeastRecentlyUpdatedEvictionStrategy:
         return self.__eviction_strategy
 
     def key_extractor(self) -> EncodedMethodReferenceAndArgsKeyExtractor:
         return self.__key_extractor
+
+    def postprocessing(self) -> Postprocessing:
+        return self.__postprocessing
```

### Comparing `py-memoize-2.0.0/memoize/entry.py` & `py-memoize-2.1.0/memoize/entry.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/entrybuilder.py` & `py-memoize-2.1.0/memoize/entrybuilder.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/eviction.py` & `py-memoize-2.1.0/memoize/eviction.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/invalidation.py` & `py-memoize-2.1.0/memoize/invalidation.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/key.py` & `py-memoize-2.1.0/memoize/key.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/serde.py` & `py-memoize-2.1.0/memoize/serde.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/statuses.py` & `py-memoize-2.1.0/memoize/statuses.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/storage.py` & `py-memoize-2.1.0/memoize/storage.py`

 * *Files identical despite different names*

### Comparing `py-memoize-2.0.0/memoize/wrapper.py` & `py-memoize-2.1.0/memoize/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,10 +141,10 @@
         elif current_entry.update_after <= now:
             logger.debug('Entry update point expired - entry update (async - current entry returned) for key %s', key)
             _call_soon(refresh, current_entry, key, value_future_provider, configuration_snapshot)
             result = current_entry
         else:
             result = current_entry
 
-        return result.value
+        return configuration_snapshot.postprocessing().apply(result.value)
 
     return wrapper
```

### Comparing `py-memoize-2.0.0/py_memoize.egg-info/PKG-INFO` & `py-memoize-2.1.0/py_memoize.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 2.0.0
+Version: 2.1.0
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -215,14 +215,18 @@
 * storage for cached entries/items (see `memoize.storage.CacheStorage`);
   in-memory storage is already provided;
   for convenience of implementing new storage adapters some SerDe (`memoize.serde.SerDe`) are provided;
 * eviction strategy (see `memoize.eviction.EvictionStrategy`);
   least-recently-updated strategy is already provided;
 * entry builder (see `memoize.entrybuilder.CacheEntryBuilder`)
   which has control over ``update_after``  & ``expires_after`` described in `Tunable eviction & async refreshing`_
+* value post-processing (see `memoize.postprocessing.Postprocessing`);
+  noop is the default one;
+  deep-copy post-processing is also provided (be wary of deep-copy cost & limitations,
+  but deep-copying allows callers to safely modify values retrieved from an in-memory cache).
 
 All of these elements are open for extension (you can implement and plug-in your own).
 Please contribute!
 
 Example how to customize default config (everything gets overridden):
 
 ..
@@ -232,38 +236,41 @@
 
     from datetime import timedelta
 
     from memoize.configuration import MutableCacheConfiguration, DefaultInMemoryCacheConfiguration
     from memoize.entrybuilder import ProvidedLifeSpanCacheEntryBuilder
     from memoize.eviction import LeastRecentlyUpdatedEvictionStrategy
     from memoize.key import EncodedMethodNameAndArgsKeyExtractor
+    from memoize.postprocessing import DeepcopyPostprocessing
     from memoize.storage import LocalInMemoryCacheStorage
     from memoize.wrapper import memoize
 
-
-    @memoize(configuration=MutableCacheConfiguration
-             .initialized_with(DefaultInMemoryCacheConfiguration())
-             .set_method_timeout(value=timedelta(minutes=2))
-             .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
-                                                                  expire_after=timedelta(minutes=5)))
-             .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
-             .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
-             .set_storage(LocalInMemoryCacheStorage())
-             )
+    @memoize(
+        configuration=MutableCacheConfiguration
+        .initialized_with(DefaultInMemoryCacheConfiguration())
+        .set_method_timeout(value=timedelta(minutes=2))
+        .set_entry_builder(ProvidedLifeSpanCacheEntryBuilder(update_after=timedelta(minutes=2),
+                                                             expire_after=timedelta(minutes=5)))
+        .set_eviction_strategy(LeastRecentlyUpdatedEvictionStrategy(capacity=2048))
+        .set_key_extractor(EncodedMethodNameAndArgsKeyExtractor(skip_first_arg_as_self=False))
+        .set_storage(LocalInMemoryCacheStorage())
+        .set_postprocessing(DeepcopyPostprocessing())
+    )
     async def cached():
         return 'dummy'
 
 
 Still, you can use default configuration which:
 
 * sets timeout for underlying method to 2 minutes;
 * uses in-memory storage;
 * uses method instance & arguments to infer cache key;
 * stores up to 4096 elements in cache and evicts entries according to least recently updated policy;
-* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes.
+* refreshes elements after 10 minutes & ignores unrefreshed elements after 30 minutes;
+* does not post-process cached values.
 
 If that satisfies you, just use default config:
 
 ..
     _example_source: examples/configuration/default_configuration.py
 
 .. code-block:: python
```

### Comparing `py-memoize-2.0.0/setup.py` & `py-memoize-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # but don't work at PyPi - therefore are removed
     description = description.replace(":class:", "")
     return description
 
 
 setup(
     name='py-memoize',
-    version='2.0.0',
+    version='2.1.0',
     author='Michal Zmuda',
     author_email='zmu.michal@gmail.com',
     url='https://github.com/DreamLab/memoize',
     maintainer='DreamLab',
     packages=['memoize'],
     test_suite='tests',
     license='Apache License 2.0',
```

