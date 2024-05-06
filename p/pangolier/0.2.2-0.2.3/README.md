# Comparing `tmp/pangolier-0.2.2-py3-none-any.whl.zip` & `tmp/pangolier-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4989 bytes, number of entries: 11
+Zip file size: 4998 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 22-Aug-07 02:48 pangolier/__init__.py
 -rw-rw-r--  2.0 unx      377 b- defN 23-Jul-19 06:54 pangolier/common.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jul-19 06:54 pangolier/filters.py
+-rw-rw-r--  2.0 unx     1061 b- defN 24-May-06 10:30 pangolier/filters.py
 -rw-rw-r--  2.0 unx     3367 b- defN 23-Jul-19 06:54 pangolier/functions.py
 -rw-rw-r--  2.0 unx     4221 b- defN 23-Oct-09 03:40 pangolier/metrics.py
 -rw-rw-r--  2.0 unx     1453 b- defN 23-Jul-19 06:54 pangolier/prefixes.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-19 06:54 pangolier/py.typed
--rw-rw-r--  2.0 unx      696 b- defN 24-Mar-24 09:49 pangolier-0.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Mar-24 09:49 pangolier-0.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 24-Mar-24 09:49 pangolier-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      837 b- defN 24-Mar-24 09:49 pangolier-0.2.2.dist-info/RECORD
-11 files, 11984 bytes uncompressed, 3577 bytes compressed:  70.2%
+-rw-rw-r--  2.0 unx      696 b- defN 24-May-06 10:30 pangolier-0.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-06 10:30 pangolier-0.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 24-May-06 10:30 pangolier-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      838 b- defN 24-May-06 10:30 pangolier-0.2.3.dist-info/RECORD
+11 files, 12115 bytes uncompressed, 3586 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pangolier/prefixes.py
 Comment: 
 
 Filename: pangolier/py.typed
 Comment: 
 
-Filename: pangolier-0.2.2.dist-info/METADATA
+Filename: pangolier-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: pangolier-0.2.2.dist-info/WHEEL
+Filename: pangolier-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: pangolier-0.2.2.dist-info/top_level.txt
+Filename: pangolier-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pangolier-0.2.2.dist-info/RECORD
+Filename: pangolier-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pangolier/filters.py

```diff
@@ -22,14 +22,19 @@
 
 
 class RegexpFilter(FilterBase):
     def to_str(self, pretty: bool = False) -> str:
         return '=~"%s"' % self.expression
 
 
+class NotRegexpFilter(FilterBase):
+    def to_str(self, pretty: bool = False) -> str:
+        return '!~"%s"' % self.expression
+
+
 FilterValueType = Union[str, FilterBase]
 FilterTuple = tuple[str, FilterBase]
 
 
 def _make_filter(value: FilterValueType) -> FilterBase:
     if isinstance(value, str):
         return EqualFilter(value)
```

## Comparing `pangolier-0.2.2.dist-info/METADATA` & `pangolier-0.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangolier
-Version: 0.2.2
+Version: 0.2.3
 Summary: build PromQL by Python code
 Home-page: https://pangolier.readthedocs.io
 Project-URL: Documentation, https://pangolier.readthedocs.io
 Project-URL: Source, https://github.com/lexdene/pangolier
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

## Comparing `pangolier-0.2.2.dist-info/RECORD` & `pangolier-0.2.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pangolier/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pangolier/common.py,sha256=enIr17z5ft5Yc1RB0t-gSuspvFaPxv2efJF2ZxS8sLc,377
-pangolier/filters.py,sha256=tTKNnyQERNe7EvzLqVjlqqlI0F2O5fiCxkKzVcMeUrQ,931
+pangolier/filters.py,sha256=MCL1p4P8oloIPQHnwEzv7_0YZNe3U5A10gc0g_6Gz6E,1061
 pangolier/functions.py,sha256=OqE9ZoZ0FmDPtl85_b14Na_QXhCnxGwqNXfgflynUrY,3367
 pangolier/metrics.py,sha256=oIVav13E59ROzQhIXqXpWtmUkSARvqzsJxdDFn4wZdQ,4221
 pangolier/prefixes.py,sha256=H5gT5EPUEpnU9ObfpxILnANxhMHj2PgHfQZXEA02_54,1453
 pangolier/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pangolier-0.2.2.dist-info/METADATA,sha256=ytYXAAotY3_X3i5DF5FUuPmJgEsMhZm8ZQ2MabcCBbM,696
-pangolier-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pangolier-0.2.2.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
-pangolier-0.2.2.dist-info/RECORD,,
+pangolier-0.2.3.dist-info/METADATA,sha256=ksEjAij5bPvdjCFAvihsiXu2u5UcPdwt_G1ZPaZOz3M,696
+pangolier-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pangolier-0.2.3.dist-info/top_level.txt,sha256=oVjXI9K4K47ZzdvnhAwezlDWfgBGevyp1bX99_TSZlk,10
+pangolier-0.2.3.dist-info/RECORD,,
```

