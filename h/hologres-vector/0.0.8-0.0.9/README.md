# Comparing `tmp/hologres_vector-0.0.8.tar.gz` & `tmp/hologres_vector-0.0.9.tar.gz`

## Comparing `hologres_vector-0.0.8.tar` & `hologres_vector-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/Develop.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/env.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/src/hologres_vector/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/src/hologres_vector/__init__.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/src/hologres_vector/hologres_vector.py
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/src/hologres_vector/hologres_wrapper.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/tests/test_hologres_vector.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/README.md
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 hologres_vector-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/Develop.md
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/src/hologres_vector/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/src/hologres_vector/__init__.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/src/hologres_vector/hologres_vector.py
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/src/hologres_vector/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     8207 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/tests/test_hologres_vector.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/README.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 hologres_vector-0.0.9/PKG-INFO
```

### Comparing `hologres_vector-0.0.8/src/hologres_vector/hologres_vector.py` & `hologres_vector-0.0.9/src/hologres_vector/hologres_vector.py`

 * *Files identical despite different names*

### Comparing `hologres_vector-0.0.8/src/hologres_vector/hologres_wrapper.py` & `hologres_vector-0.0.9/src/hologres_vector/hologres_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 
 class HologresWrapper:
     DISTANCE_METHOD_TO_FUNC_NAME: ClassVar[dict[str, str]] = {
         "SquaredEuclidean": "pm_approx_squared_euclidean_distance",
         "Euclidean": "pm_approx_euclidean_distance",
         "InnerProduct": "pm_approx_inner_product_distance",
     }
+    DISTANCE_METHOD_TO_SORT_ORDER: ClassVar[dict[str, str]] = {
+        "SquaredEuclidean": "asc",
+        "Euclidean": "asc",
+        "InnerProduct": "desc",
+    }
 
     def __init__(
         self,
         connection_string: str,
         ndims: int,
         table_name: str,
         distance_method: str,
@@ -172,15 +177,16 @@
             for col_name in select_columns:
                 col_names += f", {col_name}"
 
         sql = (
             f"select id, metadata::text, "
             f"{self.DISTANCE_METHOD_TO_FUNC_NAME[self.distance_method]}("
             f"vector, array{json.dumps(vector)}::float4[]) as distance {col_names} "
-            f"from {self.table_name} {filter_clause} order by distance asc limit %s;"
+            f"from {self.table_name} {filter_clause} "
+            f"order by distance {self.DISTANCE_METHOD_TO_SORT_ORDER[self.distance_method]} limit %s;"
         )
         self.cursor.execute(sql, (*params, k))
         self.conn.commit()
         return self.cursor.fetchall()
 
     def query_by_filters(
         self,
```

### Comparing `hologres_vector-0.0.8/tests/test_hologres_vector.py` & `hologres_vector-0.0.9/tests/test_hologres_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,30 @@
         f"select count(1) from hologres.hg_table_properties "
         f"where table_name = '{table_name}' and property_key = 'table_id'"
     )
     assert res[0][0] == 1
     holo.run_sql(f"drop table {table_name}", False)
 
 
-def insert_example_data(holo: HologresVector, use_metadata: bool = False, use_id: bool = False):
+def normalize(v):
+    # 计算向量的欧几里得范数(L2范数)
+    norm = sum(x**2 for x in v) ** 0.5
+    # 避免除以0
+    if norm == 0:
+        return v
+    # 归一化向量
+    return [x / norm for x in v]
+
+
+def insert_example_data(
+    holo: HologresVector, use_metadata: bool = False, use_id: bool = False, do_normalize: bool = False
+):
     vectors = [[0, 1, 2, 3, 4], [5, 6, 7, 8, 9], [10, 11, 12, 13, 14]]
+    if do_normalize:
+        vectors = [normalize(v) for v in vectors]
     schema_datas = [
         {"t": "text 0", "date": "2023-08-02 13:00:00", "i": 0},
         {"t": "text 1", "date": "2023-08-02 14:00:00", "i": 1},
         {"t": "text 2", "date": "2023-08-02 15:00:00", "i": 2},
     ]
     metadatas = None
     if use_metadata:
@@ -260,16 +274,16 @@
         5,
         table_name=table_name,
         table_schema={"t": "text", "date": "timestamptz", "i": "int"},
         distance_method=distance_method,
         pre_delete_table=True,
         logger=logger,
     )
-    insert_example_data(holo)
+    insert_example_data(holo, do_normalize=True)
 
-    res = holo.search([2, 2, 2, 2, 2], k=2, select_columns=["t", "date", "i"])
+    res = holo.search(normalize([0, 1, 2, 3, 4]), k=2, select_columns=["t", "date", "i"])
     assert len(res) == 2
     for i in range(2):
         assert res[i]["i"] == i
         assert res[i]["t"] == f"text {i}"
 
     holo.run_sql(f"drop table {table_name}", False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hologres_vector-0.0.8/LICENSE.txt` & `hologres_vector-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hologres_vector-0.0.8/README.md` & `hologres_vector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hologres_vector-0.0.8/pyproject.toml` & `hologres_vector-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hologres_vector-0.0.8/PKG-INFO` & `hologres_vector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hologres-vector
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/unknown/hologres-vector#readme
 Project-URL: Issues, https://github.com/unknown/hologres-vector/issues
 Project-URL: Source, https://github.com/unknown/hologres-vector
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

