# Comparing `tmp/modgeosys_graph_algorithms-0.4.1.tar.gz` & `tmp/modgeosys_graph_algorithms-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.4.1.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.4.2.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.4.1.tar` & `modgeosys_graph_algorithms-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4214 2024-04-29 04:40:54.037521 modgeosys_graph_algorithms-0.4.1/README.md
--rw-r--r--   0        0        0      489 2024-05-02 19:43:56.661844 modgeosys_graph_algorithms-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.4.1/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3219 2024-04-29 04:36:13.020391 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      625 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      408 2024-04-29 04:36:13.064391 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/edge_weight.py
--rw-r--r--   0        0        0     1760 2024-05-02 19:43:56.665844 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     7744 2024-04-29 04:44:15.842283 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     4727 2024-04-29 04:44:15.878284 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     8338 2024-04-29 04:44:15.866284 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3775 2024-04-29 04:36:13.028391 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4214 2024-04-29 04:40:54.037521 modgeosys_graph_algorithms-0.4.2/README.md
+-rw-r--r--   0        0        0      489 2024-05-06 18:16:05.601395 modgeosys_graph_algorithms-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.4.2/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3219 2024-04-29 04:36:13.020391 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      625 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      408 2024-04-29 04:36:13.064391 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/edge_weight.py
+-rw-r--r--   0        0        0     2390 2024-05-06 17:51:12.677941 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7939 2024-05-06 17:45:41.825191 modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     6232 2024-05-06 18:12:28.840870 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8338 2024-04-29 04:44:15.866284 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    24746 2024-05-06 18:13:39.525041 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3775 2024-04-29 04:36:13.028391 modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.4.2/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.4.1/README.md` & `modgeosys_graph_algorithms-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.4.2/src/modgeosys/graph/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 
 type NodeSequence = Sequence[Node]
 type EdgeSequence = Sequence[Edge]
 type EdgeDefinition = tuple[tuple, int | float | None, dict]
 type EdgeDefinitionSequence = Sequence[EdgeDefinition]
 type AdjacencyMap = Mapping[Node, Sequence[Edge]]
 type DistanceCallable = Callable[[Node, Node], int | float]
-type ValidEdgeCallable = Callable[[Edge], bool]
+type ValidEdgeCallable = Callable[Graph, Edge, {int}, {Edge}, {int}, {Edge}]
 type EdgeWeightCallable = Callable[Graph, Edge]
 
 
 COMPUTED_WEIGHT = None
 
 
 @dataclass
 class Node:
     """A node in a graph."""
     coordinates: Vector[np.float64]
     properties: dict = field(default_factory=dict)
+    terminal: bool = field(default=True, compare=False)
 
     def __post_init__(self):
         self.coordinates = np.array(self.coordinates, dtype=np.float64)
         if not isinstance(self.properties, dict):
             self.properties = dict(self.properties)
 
     def __hash__(self):
@@ -42,37 +43,32 @@
     def __eq__(self, other):
         return np.all(self.coordinates == other.coordinates)
 
     def __lt__(self, other: 'Node') -> bool:
         return not np.all(self.coordinates < other.coordinates)
 
     def __add__(self, other):
-        if isinstance(other, Node):
-            other = other.coordinates
-        return Node(self.coordinates + other)
+        other_coordinates = other.coordinates if isinstance(other, Node) else other
+        return Node(self.coordinates + other_coordinates)
 
     def __sub__(self, other):
-        if isinstance(other, Node):
-            other = other.coordinates
-        return Node(self.coordinates - other)
+        other_coordinates = other.coordinates if isinstance(other, Node) else other
+        return Node(self.coordinates - other_coordinates)
 
     def __mul__(self, other):
-        if isinstance(other, Node):
-            other = other.coordinates
-        return Node(self.coordinates * other)
+        other_coordinates = other.coordinates if isinstance(other, Node) else other
+        return Node(self.coordinates * other_coordinates)
 
     def __truediv__(self, other):
-        if isinstance(other, Node):
-            other = other.coordinates
-        return Node(self.coordinates / other)
+        other_coordinates = other.coordinates if isinstance(other, Node) else other
+        return Node(self.coordinates / other_coordinates)
 
     def __floordiv__(self, other):
-        if isinstance(other, Node):
-            other = other.coordinates
-        return Node(self.coordinates // other)
+        other_coordinates = other.coordinates if isinstance(other, Node) else other
+        return Node(self.coordinates // other_coordinates)
 
     def __array__(self):
         return self.coordinates
```

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 @pytest.fixture
 def valid_nodes():
     return [Node(properties={}, coordinates=(0.0, 0.0)), Node(properties={}, coordinates=(0.0, 2.0)), Node(properties={}, coordinates=(1.0, 0.0)), Node(properties={}, coordinates=(2.0, 1.0)), Node(properties={}, coordinates=(2.0, 3.0))]
 
 
 @pytest.fixture
+def valid_nodes_with_steiner_nodes():
+    return [Node(properties={}, coordinates=(0.0, 0.0), terminal=True), Node(properties={}, coordinates=(0.0, 2.0), terminal=True), Node(properties={}, coordinates=(1.0, 0.0), terminal=True), Node(properties={}, coordinates=(1.0, 1.0), terminal=False), Node(properties={}, coordinates=(2.0, 1.0), terminal=True), Node(properties={}, coordinates=(2.0, 3.0), terminal=True), Node(properties={}, coordinates=(8.0, 8.0), terminal=False)]
+
+
+@pytest.fixture
 def valid_edges1():
     return (Edge(properties={}, weight=2, node_indices=frozenset((0, 1))),
             Edge(properties={}, weight=1, node_indices=frozenset((0, 2))),
             Edge(properties={}, weight=1, node_indices=frozenset((2, 3))),
             Edge(properties={}, weight=3, node_indices=frozenset((1, 4))),
             Edge(properties={}, weight=1, node_indices=frozenset((3, 4))))
 
@@ -53,14 +58,27 @@
             Edge(properties={'cost_per_unit': 1}, weight=1.0, node_indices=frozenset((0, 2))),
             Edge(properties={'cost_per_unit': 1}, weight=2.0, node_indices=frozenset((2, 3))),
             Edge(properties={'cost_per_unit': 3}, weight=9.0, node_indices=frozenset((1, 4))),
             Edge(properties={'cost_per_unit': 1}, weight=2.0, node_indices=frozenset((3, 4))))
 
 
 @pytest.fixture
+def valid_edges4():
+    return (Edge(properties={}, weight=2, node_indices=frozenset((0, 1))),
+            Edge(properties={}, weight=1, node_indices=frozenset((0, 2))),
+            Edge(properties={}, weight=1, node_indices=frozenset((0, 3))),
+            Edge(properties={}, weight=1, node_indices=frozenset((1, 3))),
+            Edge(properties={}, weight=1, node_indices=frozenset((2, 3))),
+            Edge(properties={}, weight=1, node_indices=frozenset((4, 3))),
+            Edge(properties={}, weight=1, node_indices=frozenset((5, 3))),
+            Edge(properties={}, weight=1, node_indices=frozenset((2, 4))),
+            Edge(properties={}, weight=3, node_indices=frozenset((1, 5))),
+            Edge(properties={}, weight=1, node_indices=frozenset((4, 5))))
+
+@pytest.fixture
 def valid_graph1(valid_nodes, valid_edges1):
     return Graph(properties={}, nodes=valid_nodes, edges=valid_edges1, distance_function=manhattan_distance)
 
 
 @pytest.fixture
 def valid_graph2(valid_nodes, valid_edges2):
     return Graph(properties={}, nodes=valid_nodes, edges=valid_edges2, distance_function=manhattan_distance)
@@ -68,14 +86,19 @@
 
 @pytest.fixture
 def valid_graph3(valid_nodes, valid_edges3):
     return Graph(properties={}, nodes=valid_nodes, edges=valid_edges3, distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 
 @pytest.fixture
+def valid_graph4_with_steiner_node(valid_nodes_with_steiner_nodes, valid_edges4):
+    return Graph(properties={}, nodes=valid_nodes_with_steiner_nodes, edges=valid_edges4, distance_function=manhattan_distance)
+
+
+@pytest.fixture
 def valid_graph_from_edge_definitions():
     return Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
                                                          (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
                                                          (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
```

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_prim.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,26 @@
     assert result == {Edge(weight=2.0, node_indices=frozenset({0, 1})),
                       Edge(weight=1.0, node_indices=frozenset({0, 2})),
                       Edge(weight=1.0, node_indices=frozenset({2, 3})),
                       Edge(weight=1.0, node_indices=frozenset({3, 4}))}
     assert sum(edge.weight for edge in result) == 5.0
 
 
+def test_prim_finds_steiner_minimal_tree(valid_graph4_with_steiner_node):
+    result = prim(graph=valid_graph4_with_steiner_node, start_node_index=0)
+
+    assert len(result) == 5
+    assert result == {Edge(weight=1.0, node_indices=frozenset({3, 4}), properties={}),
+                      Edge(weight=1.0, node_indices=frozenset({2, 3}), properties={}),
+                      Edge(weight=1.0, node_indices=frozenset({0, 3}), properties={}),
+                      Edge(weight=1.0, node_indices=frozenset({4, 5}), properties={}),
+                      Edge(weight=1.0, node_indices=frozenset({1, 3}), properties={})}
+    assert sum(edge.weight for edge in result) == 5.0
+
+
 def test_prim_finds_minimum_spanning_tree_from_edge_definitions(valid_graph_from_edge_definitions):
     result = prim(graph=valid_graph_from_edge_definitions, start_node_index=0)
 
     assert len(result) == 4
     assert result == {Edge(weight=1.0, node_indices=frozenset({0, 2}), properties={'cost_per_unit': 1}),
                       Edge(weight=2.0, node_indices=frozenset({3, 4}), properties={'cost_per_unit': 1}),
                       Edge(weight=2.0, node_indices=frozenset({2, 3}), properties={'cost_per_unit': 1}),
```

### Comparing `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.4.2/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.1/PKG-INFO` & `modgeosys_graph_algorithms-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
```

