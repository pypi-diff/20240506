# Comparing `tmp/dbt_loom-0.5.1.tar.gz` & `tmp/dbt_loom-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_loom-0.5.1.tar", max compression
+gzip compressed data, was "dbt_loom-0.5.2.tar", max compression
```

## Comparing `dbt_loom-0.5.1.tar` & `dbt_loom-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1211 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/LICENSE
--rw-r--r--   0        0        0     6654 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/README.md
--rw-r--r--   0        0        0     5553 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/__init__.py
--rw-r--r--   0        0        0     2088 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/clients/az_blob.py
--rw-r--r--   0        0        0     2675 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/clients/dbt_cloud.py
--rw-r--r--   0        0        0     1603 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/clients/gcs.py
--rw-r--r--   0        0        0     1641 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/clients/s3.py
--rw-r--r--   0        0        0     1161 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/config.py
--rw-r--r--   0        0        0     4578 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/dbt_loom/manifests.py
--rw-r--r--   0        0        0     1059 2024-04-22 17:10:20.919595 dbt_loom-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 dbt_loom-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/LICENSE
+-rw-r--r--   0        0        0     6654 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/README.md
+-rw-r--r--   0        0        0     5823 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/__init__.py
+-rw-r--r--   0        0        0     2088 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/az_blob.py
+-rw-r--r--   0        0        0     2675 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/dbt_cloud.py
+-rw-r--r--   0        0        0     1603 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/gcs.py
+-rw-r--r--   0        0        0     1641 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/clients/s3.py
+-rw-r--r--   0        0        0     1161 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/config.py
+-rw-r--r--   0        0        0     4550 2024-05-06 19:53:58.008566 dbt_loom-0.5.2/dbt_loom/manifests.py
+-rw-r--r--   0        0        0     1059 2024-05-06 19:53:58.012566 dbt_loom-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 dbt_loom-0.5.2/PKG-INFO
```

### Comparing `dbt_loom-0.5.1/LICENSE` & `dbt_loom-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/README.md` & `dbt_loom-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/__init__.py` & `dbt_loom-0.5.2/dbt_loom/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 import yaml
 from dbt.contracts.graph.node_args import ModelNodeArgs
 from dbt.events.functions import fire_event
 from dbt.events.types import Note
 from dbt.plugins.manager import dbt_hook, dbtPlugin
 from dbt.plugins.manifest import PluginNodes
 from dbt.config.project import VarProvider
-
+from dbt.node_types import NodeType
 
 from dbt_loom.config import dbtLoomConfig
 from dbt_loom.manifests import ManifestLoader, ManifestNode
 
 
 def identify_node_subgraph(manifest) -> Dict[str, ManifestNode]:
     """
     Identify all nodes that should be selected from the manifest, and return ManifestNodes.
     """
 
     output = {}
 
     # We're going to temporarily allow all nodes here.
     for unique_id in manifest["nodes"].keys():
-        if unique_id.split(".")[0] in ("tests", "macros"):
+        if unique_id.split(".")[0] in (NodeType.Test.value, NodeType.Macro.value):
             continue
 
         node = manifest.get("nodes", {}).get(unique_id)
 
         if not node:
             continue
 
         if node.get("access") is None:
             node["access"] = node.get("config", {}).get("access", "protected")
 
+        # Versions may be floats or strings. Standardize on strings for compatibility.
+        for key in ("version", "latest_version"):
+            if node.get(key):
+                node[key] = str(node[key])
+
         output[unique_id] = ManifestNode(**(node))
 
     return output
 
 
 def convert_model_nodes_to_model_node_args(
     selected_nodes: Dict[str, ManifestNode],
```

### Comparing `dbt_loom-0.5.1/dbt_loom/clients/az_blob.py` & `dbt_loom-0.5.2/dbt_loom/clients/az_blob.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/clients/dbt_cloud.py` & `dbt_loom-0.5.2/dbt_loom/clients/dbt_cloud.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/clients/gcs.py` & `dbt_loom-0.5.2/dbt_loom/clients/gcs.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/clients/s3.py` & `dbt_loom-0.5.2/dbt_loom/clients/s3.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/config.py` & `dbt_loom-0.5.2/dbt_loom/config.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.1/dbt_loom/manifests.py` & `dbt_loom-0.5.2/dbt_loom/manifests.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     """A basic ManifestNode that can be referenced across projects."""
 
     name: str
     package_name: str
     schema_name: str = Field(alias="schema")
     database: Optional[str] = None
     relation_name: Optional[str] = None
-    version: Optional[Union[str, float]] = None
-    latest_version: Optional[Union[str, float]] = None
+    version: Optional[str] = None
+    latest_version: Optional[str] = None
     deprecation_date: Optional[datetime.datetime] = None
     access: Optional[str] = "protected"
     generated_at: datetime.datetime = Field(default_factory=datetime.datetime.utcnow)
     depends_on: Optional[DependsOn] = None
     depends_on_nodes: List[str] = Field(default_factory=list)
     enabled: bool = True
```

### Comparing `dbt_loom-0.5.1/pyproject.toml` & `dbt_loom-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dbt-loom"
-version = "0.5.1"
+version = "0.5.2"
 description = "A dbt-core plugin to import public nodes in multi-project deployments."
 authors = ["Nicholas Yager <yager@nicholasyager.com>"]
 readme = "README.md"
 packages = [{ include = "dbt_loom" }]
 
 [tool.commitizen]
-version = "0.5.1"
+version = "0.5.2"
 version_files = ["pyproject.toml:^version"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 dbt-core = ">=1.6.0,<1.8.0"
 requests = "^2.31.0"
 google-cloud-storage = "^2.13.0"
```

### Comparing `dbt_loom-0.5.1/PKG-INFO` & `dbt_loom-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-loom
-Version: 0.5.1
+Version: 0.5.2
 Summary: A dbt-core plugin to import public nodes in multi-project deployments.
 Author: Nicholas Yager
 Author-email: yager@nicholasyager.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

