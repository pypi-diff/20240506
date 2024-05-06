# Comparing `tmp/flowchart_explorer-0.1.0.tar.gz` & `tmp/flowchart_explorer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchart_explorer-0.1.0.tar", max compression
+gzip compressed data, was "flowchart_explorer-0.1.1.tar", max compression
```

## Comparing `flowchart_explorer-0.1.0.tar` & `flowchart_explorer-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0      100 2024-05-03 08:00:45.229782 flowchart_explorer-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1055 2024-05-03 08:00:45.229782 flowchart_explorer-0.1.0/LICENSE
--rw-r--r--   0        0        0      229 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/README.md
--rw-r--r--   0        0        0       22 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/flowchart_explorer/__init__.py
--rw-r--r--   0        0        0     5238 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/flowchart_explorer/explorer.py
--rw-r--r--   0        0        0        0 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/flowchart_explorer/graph/__init__.py
--rw-r--r--   0        0        0    10403 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/flowchart_explorer/graph/drawio.py
--rw-r--r--   0        0        0     1823 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/flowchart_explorer/methods.py
--rw-r--r--   0        0        0     2691 2024-05-03 08:00:45.233782 flowchart_explorer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 flowchart_explorer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1055 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/__init__.py
+-rw-r--r--   0        0        0     2274 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/chartpath.py
+-rw-r--r--   0        0        0     5238 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/explorer.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/flowchartdiagrams/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/flowchartdiagrams/nodes.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/graph/__init__.py
+-rw-r--r--   0        0        0    11225 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/graph/drawio.py
+-rw-r--r--   0        0        0     1823 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/methods.py
+-rw-r--r--   0        0        0     2680 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 flowchart_explorer-0.1.1/PKG-INFO
```

### Comparing `flowchart_explorer-0.1.0/LICENSE` & `flowchart_explorer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.0/flowchart_explorer/explorer.py` & `flowchart_explorer-0.1.1/flowchart_explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.0/flowchart_explorer/graph/drawio.py` & `flowchart_explorer-0.1.1/flowchart_explorer/graph/drawio.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,51 +47,74 @@
         loop_check: dict = {}
         for key in nodes.keys():
             graph_nodes, loops, loop_check = self._transform_node(key, nodes[key], graph_nodes, loops, loop_check)
         return graph_nodes, loops, loop_check
 
     def _transform_node(self, key: str, node: dict, graph_nodes: dict,
                         loops: dict, loop_check: dict) -> Tuple[dict, dict, dict]:
+
+        # get label
+        if 'value' in node['additional-details']:
+            label = node['additional-details']['value']
+        elif 'label' in node['additional-details']:
+            label = node['additional-details']['label']
+        else:
+            label = ""
+        # replace <br> to \n
+        label = label.replace("<br>", "\n")
+
+
         style = node['additional-details']['style']
         # in-loop
         if (style.startswith('shape=loopLimit;') and
                 "in-loop" in node['additional-details'].keys()):
 
             max_loop = self.MAX_LOOP
             if "max-loop" in node['additional-details']:
                 max_loop = node['additional-details']['max-loop']
 
             graph_nodes[key] = {'node-type': 'in-loop',
                                 'loop-id': node['additional-details']['in-loop'],
                                 'max-loop': max_loop,
+                                'label': label,
                                 'additional-details': node['additional-details']
                                 }
             loop_check = self._add_value_to_list(loop_check, node['additional-details']['in-loop'], 'in-loop')
             loops = self._add_value_to_dict(loops, node['additional-details']['in-loop'], 'in-loop', key)
 
         # out-loop
         elif (style.startswith('shape=loopLimit;') and
               "out-loop" in node['additional-details'].keys()):
             graph_nodes[key] = {'node-type': 'out-loop',
                                 'loop-id': node['additional-details']['out-loop'],
+                                'label': label,
                                 'additional-details': node['additional-details']
                                 }
             loop_check = self._add_value_to_list(loop_check, node['additional-details']['out-loop'], 'out-loop')
             loops = self._add_value_to_dict(loops, node['additional-details']['out-loop'], 'out-loop', key)
 
         # exit-loop
         elif (style.startswith('ellipse;') and
               "exit-loop" in node['additional-details'].keys()):
             graph_nodes[key] = {'node-type': 'exit-loop',
                                 'loop-id': node['additional-details']['exit-loop'],
+                                'label': label,
+                                'additional-details': node['additional-details']
+                                }
+
+        # decision
+        elif style.startswith('rhombus;'):
+            graph_nodes[key] = {'node-type': 'decision',
+                                'label': label,
                                 'additional-details': node['additional-details']
                                 }
         # normal(Cases other than the above)
         else:
             graph_nodes[key] = {'node-type': 'normal',
+                                'label': label,
                                 'additional-details': node['additional-details']
                                 }
 
         return graph_nodes, loops, loop_check
 
     @staticmethod
     def _get_start_node(nodes: dict, sources: set, targets: set) -> dict:
```

### Comparing `flowchart_explorer-0.1.0/flowchart_explorer/methods.py` & `flowchart_explorer-0.1.1/flowchart_explorer/methods.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.0/pyproject.toml` & `flowchart_explorer-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "flowchart_explorer"
-version = "0.1.0"
+version = "0.1.1"
 description = "FlowChart Explorer is a GitHub-integrated tool that analyzes all execution paths in a flowchart. It helps identify bottlenecks and redundancies in your codebase, providing a new level of clarity and control."
 authors = ["sabi2345"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sabi2345/flowchart-explorer"
-packages = [
-    { include = "flowchart_explorer" },
-    ]
+
 include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
+diagrams = "^0.23.4"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-mock = "^3.14.0"
 pytest-profiling = "^1.7.0"
 pytest-cov = "^5.0.0"
@@ -31,15 +30,15 @@
 [tool.poetry.group.ci]
 optional = true # デフォルトではインストールしない
 [tool.poetry.group.ci.dependencies]
 pytest-azurepipelines = "^1.0.4"
 
 [tool.pytest.ini_options]
 testpaths = ['tests']
-addopts = '--cov --cov-report=term --cov-report=xml --cov-report=html'
+#addopts = '--cov --cov-config=.coveragerc --cov-report=term --cov-report=xml --cov-report=html'
 log_cli = false  # ログを有効にしたい場合は true にします
 log_cli_level = 'DEBUG'
 log_cli_format = "message:%(message)s"
 #log_cli_format = "time:%(asctime)s.%(msecs)03d\tthread:%(threadName)s\tlogger:%(name)s\tlevel:%(levelname)s\tmessage:%(message)s"
 log_cli_date_format = '%Y-%m-%d %H:%M:%S'
 log_file = 'pytest.log'  # ログを出力するファイル名
 log_file_level = 'DEBUG'  # ファイルに出力するログのレベル
```

### Comparing `flowchart_explorer-0.1.0/PKG-INFO` & `flowchart_explorer-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: flowchart_explorer
-Version: 0.1.0
+Version: 0.1.1
 Summary: FlowChart Explorer is a GitHub-integrated tool that analyzes all execution paths in a flowchart. It helps identify bottlenecks and redundancies in your codebase, providing a new level of clarity and control.
 Home-page: https://github.com/sabi2345/flowchart-explorer
 License: MIT
 Author: sabi2345
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: diagrams (>=0.23.4,<0.24.0)
 Project-URL: Repository, https://github.com/sabi2345/flowchart-explorer
 Description-Content-Type: text/markdown
 
 # FlowChart Explorer
 FlowChart Explorer is a GitHub-integrated tool that analyzes all execution paths in a flowchart. It helps identify bottlenecks and redundancies in your codebase, providing a new level of clarity and control.
```

