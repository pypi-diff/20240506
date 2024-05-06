# Comparing `tmp/sc-supertree-2024.2.29.post1.tar.gz` & `tmp/sc-supertree-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-supertree-2024.2.29.post1.tar", last modified: Thu Feb 29 00:49:54 2024, max compression
+gzip compressed data, was "sc-supertree-2024.5.6.tar", last modified: Mon May  6 06:07:37 2024, max compression
```

## Comparing `sc-supertree-2024.2.29.post1.tar` & `sc-supertree-2024.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      693 2024-02-16 00:58:41.635401 sc-supertree-2024.2.29.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1502 2024-02-20 06:24:43.597948 sc-supertree-2024.2.29.post1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2753 2024-02-16 00:43:49.954237 sc-supertree-2024.2.29.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     2053 2024-02-26 00:02:31.152694 sc-supertree-2024.2.29.post1/.github/workflows/linters.yml
--rw-r--r--   0        0        0      762 2024-02-20 06:25:19.151635 sc-supertree-2024.2.29.post1/.github/workflows/type_check.yml
--rw-r--r--   0        0        0     3096 2024-02-13 05:59:59.804767 sc-supertree-2024.2.29.post1/.gitignore
--rw-r--r--   0        0        0     1502 2023-10-25 05:51:31.315332 sc-supertree-2024.2.29.post1/LICENSE
--rw-r--r--   0        0        0     4241 2024-02-29 00:40:26.460457 sc-supertree-2024.2.29.post1/README.md
--rw-r--r--   0        0        0       36 2024-02-19 04:33:19.845791 sc-supertree-2024.2.29.post1/mypy.ini
--rw-r--r--   0        0        0      561 2024-02-26 00:01:35.128189 sc-supertree-2024.2.29.post1/noxfile.py
--rw-r--r--   0        0        0     1930 2024-02-28 06:20:05.020070 sc-supertree-2024.2.29.post1/pyproject.toml
--rw-r--r--   0        0        0      888 2024-02-29 00:49:45.629494 sc-supertree-2024.2.29.post1/src/sc_supertree/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-28 06:00:40.149406 sc-supertree-2024.2.29.post1/src/sc_supertree/cli.py
--rw-r--r--   0        0        0        0 2024-02-28 06:00:40.150406 sc-supertree-2024.2.29.post1/src/sc_supertree/py.typed
--rw-r--r--   0        0        0    21934 2024-02-28 06:00:40.151406 sc-supertree-2024.2.29.post1/src/sc_supertree/scs.py
--rw-r--r--   0        0        0      340 2024-02-28 04:09:45.748669 sc-supertree-2024.2.29.post1/tests/helpers.py
--rw-r--r--   0        0        0     5696 2024-02-28 04:57:21.858347 sc-supertree-2024.2.29.post1/tests/test_cli.py
--rw-r--r--   0        0        0     7221 2024-02-22 05:18:03.960880 sc-supertree-2024.2.29.post1/tests/test_data/dcm_iq_expected.tre
--rw-r--r--   0        0        0    55450 2024-02-22 05:18:28.050929 sc-supertree-2024.2.29.post1/tests/test_data/dcm_iq_source.tre
--rw-r--r--   0        0        0    47673 2024-02-23 04:16:34.761509 sc-supertree-2024.2.29.post1/tests/test_data/dcm_model_tree.tre
--rw-r--r--   0        0        0    55450 2024-02-16 05:58:47.739528 sc-supertree-2024.2.29.post1/tests/test_data/dcm_source_trees.tre
--rw-r--r--   0        0        0      597 2024-02-26 00:01:08.897349 sc-supertree-2024.2.29.post1/tests/test_data/supertriplets_expected.tre
--rw-r--r--   0        0        0    22636 2024-02-26 00:34:32.732502 sc-supertree-2024.2.29.post1/tests/test_data/supertriplets_source.tre
--rw-r--r--   0        0        0     5522 2024-02-28 04:57:21.861346 sc-supertree-2024.2.29.post1/tests/test_spectral_cluster_supertree.py
--rw-r--r--   0        0        0     5919 1970-01-01 00:00:00.000000 sc-supertree-2024.2.29.post1/PKG-INFO
+-rw-r--r--   0        0        0      693 2024-02-16 00:58:41.000000 sc-supertree-2024.5.6/.github/dependabot.yml
+-rw-r--r--   0        0        0     1502 2024-02-20 06:24:43.000000 sc-supertree-2024.5.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2753 2024-02-16 00:43:49.000000 sc-supertree-2024.5.6/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     2053 2024-02-26 00:02:31.000000 sc-supertree-2024.5.6/.github/workflows/linters.yml
+-rw-r--r--   0        0        0      762 2024-02-20 06:25:19.000000 sc-supertree-2024.5.6/.github/workflows/type_check.yml
+-rw-r--r--   0        0        0     3096 2024-02-13 05:59:59.000000 sc-supertree-2024.5.6/.gitignore
+-rw-r--r--   0        0        0     1502 2023-10-25 05:51:31.000000 sc-supertree-2024.5.6/LICENSE
+-rw-r--r--   0        0        0     4427 2024-05-06 05:00:38.529986 sc-supertree-2024.5.6/README.md
+-rw-r--r--   0        0        0       36 2024-02-19 04:33:19.000000 sc-supertree-2024.5.6/mypy.ini
+-rw-r--r--   0        0        0      561 2024-02-26 00:01:35.000000 sc-supertree-2024.5.6/noxfile.py
+-rw-r--r--   0        0        0     1925 2024-05-06 04:56:05.818437 sc-supertree-2024.5.6/pyproject.toml
+-rw-r--r--   0        0        0      881 2024-05-06 05:00:38.473630 sc-supertree-2024.5.6/src/sc_supertree/__init__.py
+-rw-r--r--   0        0        0     1137 2024-02-28 06:00:40.000000 sc-supertree-2024.5.6/src/sc_supertree/cli.py
+-rw-r--r--   0        0        0        0 2024-02-28 06:00:40.000000 sc-supertree-2024.5.6/src/sc_supertree/py.typed
+-rw-r--r--   0        0        0    21935 2024-04-22 05:27:22.521472 sc-supertree-2024.5.6/src/sc_supertree/scs.py
+-rw-r--r--   0        0        0      340 2024-02-28 04:09:45.000000 sc-supertree-2024.5.6/tests/helpers.py
+-rw-r--r--   0        0        0     5696 2024-02-28 04:57:21.000000 sc-supertree-2024.5.6/tests/test_cli.py
+-rw-r--r--   0        0        0     7221 2024-02-22 05:18:03.000000 sc-supertree-2024.5.6/tests/test_data/dcm_iq_expected.tre
+-rw-r--r--   0        0        0    55450 2024-02-22 05:18:28.000000 sc-supertree-2024.5.6/tests/test_data/dcm_iq_source.tre
+-rw-r--r--   0        0        0    47673 2024-02-23 04:16:34.000000 sc-supertree-2024.5.6/tests/test_data/dcm_model_tree.tre
+-rw-r--r--   0        0        0    55450 2024-02-16 05:58:47.000000 sc-supertree-2024.5.6/tests/test_data/dcm_source_trees.tre
+-rw-r--r--   0        0        0      597 2024-02-26 00:01:08.000000 sc-supertree-2024.5.6/tests/test_data/supertriplets_expected.tre
+-rw-r--r--   0        0        0    22636 2024-02-26 00:34:32.000000 sc-supertree-2024.5.6/tests/test_data/supertriplets_source.tre
+-rw-r--r--   0        0        0     5522 2024-02-28 04:57:21.000000 sc-supertree-2024.5.6/tests/test_spectral_cluster_supertree.py
+-rw-r--r--   0        0        0     6093 1970-01-01 00:00:00.000000 sc-supertree-2024.5.6/PKG-INFO
```

### Comparing `sc-supertree-2024.2.29.post1/.github/dependabot.yml` & `sc-supertree-2024.5.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/.github/workflows/ci.yml` & `sc-supertree-2024.5.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/.github/workflows/codeql.yml` & `sc-supertree-2024.5.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/.github/workflows/linters.yml` & `sc-supertree-2024.5.6/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/.github/workflows/type_check.yml` & `sc-supertree-2024.5.6/.github/workflows/type_check.yml`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/.gitignore` & `sc-supertree-2024.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/LICENSE` & `sc-supertree-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/README.md` & `sc-supertree-2024.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![PyPI Version](https://img.shields.io/pypi/v/sc-supertree)](https://pypi.org/project/sc-supertree/)
 [![Python Version](https://img.shields.io/pypi/pyversions/sc-supertree)](https://pypi.org/project/sc-supertree/)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![CI](https://github.com/rmcar17/SpectralClusterSupertree/workflows/CI/badge.svg)](https://github.com/rmcar17/SpectralClusterSupertree/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rmcar17/SpectralClusterSupertree/badge.svg?branch=main)](https://coveralls.io/github/rmcar17/SpectralClusterSupertree?branch=main)
 [![License](https://img.shields.io/github/license/rmcar17/SpectralClusterSupertree)](https://github.com/rmcar17/SpectralClusterSupertree/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/667189656.svg)](https://zenodo.org/badge/latestdoi/667189656)
 
 Spectral Cluster Supertree is a state-of-the-art algorithm for constructing rooted supertrees from collections of rooted source trees.
 
 Spectral Cluster Supertree can be used on Newick formatted trees in Python in conjunction with [cogent3](https://github.com/cogent3/cogent3)'s tree objects, or invoked from the command line.
 
 Spectral Cluster Supertree can employ a number of weighting strategies that take into account the depths of nodes in the trees, as well as branch lengths. A user can specify weights of trees to add bias to some of the source trees if desired.
 
@@ -32,43 +33,43 @@
 supertree = construct_supertree(source_trees, pcg_weighting="branch")
 
 supertree.write("supertree_file.tre")
 ```
 
 ### CLI
 
-In your environment which has spectral-cluster-supertree installed:
+In your environment which has `sc-supertree` installed:
 
 ```bash
 scs -i SOURCE_TREE_FILE -o SUPERTREE_FILE -p PCG_WEIGHTING_STRATEGY
 ```
 
 The ```-i``` and ```-o``` options for the input and output files are required.
 
-The ```-p``` *proper cluster graph* weighting strategy option must be one of ```ONE|DEPTH|BRANCH```. It defaults to ```BRANCH``` when not provided (not recommended when some trees are missing branch lenghts - see below).
+The ```-p``` *proper cluster graph* weighting strategy option must be one of ```ONE|DEPTH|BRANCH```. It defaults to ```BRANCH``` when not provided (not recommended when some trees are missing branch lengths - see below). Tree weights are not supported through the command line.
 
 ## Weighting Strategies
 
 ### Proper Cluster Graph Weighting
 
-Spectral Cluster Supertree recursively paritions the complete set of taxa to form a supertree. The core component of the algorithm involves partitioning the *proper cluster graph* through spectral clustering when the source trees are not consistent.
+Spectral Cluster Supertree recursively partitions the complete set of taxa to form a supertree. The core component of the algorithm involves partitioning the *proper cluster graph* through spectral clustering when the source trees are not consistent.
 
 The *proper cluster graph* has the set of all taxa in the source trees as its vertices, and an edge connects two taxa if they appear together on the same side of the root in any of the source trees (such pairs of taxa are called **proper clusters**). Let $lca$ be the lowest common ancestor of a proper cluster. Each edge is weighted according to the specified strategy:
 
 - **one** - The number of trees in which the pair of taxa appear as a proper cluster in.
 - **depth** - The sum of the depths of the $lca$ of the proper cluster in all of the source trees.
-- **branch** - The sum of the root to $lca$ branch lengths of the proper cluster in all of the source trees. If branch lengths are missing defaults to one (equivalent to depth). Do not use if some trees are missing branch lengths.
+- **branch** - The sum of the root to $lca$ branch lengths of the proper cluster in all of the source trees. If branch lengths are missing defaults to one (equivalent to depth). Do not use if source trees contain a mix of some trees with branch lengths and some without.
 
-The **branch** weighting strategy is recommened where branch lengths are available. Otherwise, the **depth** weighting strategy is recommended over the **one** weighting strategy.
+The **branch** weighting strategy is recommended when branch lengths are available. Otherwise, the **depth** weighting strategy is recommended over the **one** weighting strategy.
 
 ### Tree Weighting
 
-In addition to the above, users may associate trees with weights to bias the results towards specific trees. Prior to the summation of the weights for an edge in the *proper cluster graph*, they are multiplied by the weight of the corresponding tree. The weight of each tree defaults to one if not specified.
+In addition to the above, users may associate trees with weights to bias the results towards specific trees. Prior to the summation of the weights for an edge in the *proper cluster graph*, they are each multiplied by the weight of the corresponding tree. The weight of each tree defaults to one if not specified.
 
-An example is shown below, without the tree weights the alogrithm would randomly return either triple.
+An example is shown below, without the tree weights the algorithm would randomly return either triple.
 
 ```python
 >>> from sc_supertree import construct_supertree
 >>> from cogent3 import make_tree
 >>> tree_1 = make_tree("(a,(b,c))")
 >>> tree_2 = make_tree("(c,(b,a))")
 >>> print(construct_supertree([tree_1, tree_2], weights=[1, 1.5]))
```

### Comparing `sc-supertree-2024.2.29.post1/noxfile.py` & `sc-supertree-2024.5.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/pyproject.toml` & `sc-supertree-2024.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Topic :: Scientific/Engineering :: Bio-Informatics",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["click ==8.1.7", "numpy ==1.26.4", "cogent3 ==2024.2.5a1", "scikit-learn ==1.4.1.post1"]
+dependencies = ["click ==8.1.7", "numpy ==1.26.4", "cogent3 ==2024.2.5a1", "scikit-learn ==1.4.2"]
 keywords = [
   "supertree",
   "phylogeny",
   "biology",
   "bioinformatics",
 ]
 license = {file = "LICENSE"}
@@ -34,18 +34,18 @@
 "Source Code" = "https://github.com/rmcar17/SpectralClusterSupertree"
 
 [project.scripts]
 scs = "sc_supertree.cli:scs"
 
 [project.optional-dependencies]
 dev = [
-  "black==24.2.0",
+  "black==24.4.2",
   "isort==5.13.2",
   "click==8.1.7",
-  "mypy==1.8.0",
+  "mypy==1.10.0",
   "docformatter",
   "flit",
   "pytest",
   "pytest-cov",
   "pytest-xdist",
   "nox",
 ]
```

### Comparing `sc-supertree-2024.2.29.post1/src/sc_supertree/__init__.py` & `sc-supertree-2024.5.6/src/sc_supertree/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 A scalable and accurate algorithm for merging rooted phylogenetic trees.
 """
 
 __all__ = ["load_trees", "construct_supertree"]
 __copyright__ = "Copyright 2023, Robert McArthur"
 __license__ = "BSD"
-__version__ = "2024.2.29.post1"
+__version__ = "2024.5.6"
 
 import os
 
 from cogent3 import TreeNode, make_tree
 
 from sc_supertree.scs import construct_supertree
```

### Comparing `sc-supertree-2024.2.29.post1/src/sc_supertree/cli.py` & `sc-supertree-2024.5.6/src/sc_supertree/cli.py`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/src/sc_supertree/scs.py` & `sc-supertree-2024.5.6/src/sc_supertree/scs.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         return tree
 
     pcg_vertices: PcgVertexSet = set((name,) for name in all_names)
 
     (
         pcg_edges,
         pcg_weights,
-        taxa_ocurrences,
+        taxa_occurrences,
         taxa_co_occurrences,
     ) = _proper_cluster_graph_edges(
         pcg_vertices,
         trees,
         weights,
         pcg_weighting,
     )
@@ -103,15 +103,15 @@
     if len(components) == 1:
         if contract_edges:
             # Modifies the proper cluster graph inplace
             _contract_proper_cluster_graph(
                 pcg_vertices,
                 pcg_edges,
                 pcg_weights,
-                taxa_ocurrences,
+                taxa_occurrences,
                 taxa_co_occurrences,
             )
         components = spectral_cluster_graph(pcg_vertices, pcg_weights, random_state)
 
     # The child trees corresponding to the components of the graph
     child_trees: list[TreeNode] = []
 
@@ -119,15 +119,15 @@
         component = _component_to_names_set(pcg_component)
         # Trivial case for if the size of the component is <=2
         # Simply add a tree expressing that
         if len(component) <= 2:
             child_trees.append(_tip_names_to_tree(component))
             continue
 
-        # Otherwise, need to induce the trees on each compoment
+        # Otherwise, need to induce the trees on each component
         # and recursively call SCS
 
         # Note, inducing could possible remove trees.
         new_induced_trees, new_weights = _generate_induced_trees_with_weights(
             component, trees, weights
         )
 
@@ -201,15 +201,15 @@
         The weights of the edges of the proper cluster graph.
     random_state : np.random.RandomState
         Random number generation for spectral clustering.
 
     Returns
     -------
     list[PcgVertexSet]
-        The bipartion of taxa of the proper cluster graph.
+        The bipartition of taxa of the proper cluster graph.
     """
     sc = SpectralClustering(
         2,
         affinity="precomputed",
         assign_labels="kmeans",
         n_jobs=1,
         random_state=random_state,
@@ -241,15 +241,15 @@
     taxa_co_occurrences: dict[EdgeTuple, int],
 ) -> None:
     """Contracts the proper cluster graph.
 
     This method operates in-place.
 
     Given the proper cluster graph, contract every edge where
-    two taxa always appear together. i.e. the number of co-occurences
+    two taxa always appear together. i.e. the number of co-occurrences
     as a proper cluster is equal to the maximum number of times either
     taxa appears in any of the source trees.
 
     The vertices for the contracted edges is a tuple containing
     the taxa in the old vertices as elements (sorted).
 
     The weights for the parallel classes of edges formed through
@@ -285,15 +285,15 @@
             u, v = pair
             max_edges[u].add(v)
             max_edges[v].add(u)
 
     # The components of the new graph are the new vertices after contraction
     contractions = _get_graph_components(max_vertices, max_edges)
 
-    # Find the new vertices in processeded_contractions
+    # Find the new vertices in processed_contractions
     processed_contractions: list[PcgVertex] = []
     for contraction in contractions:
         processed: list[Taxa] = []
         for vertex in contraction:
             processed.extend(vertex)
         processed_contractions.append(tuple_sorted(processed))
 
@@ -327,15 +327,15 @@
                 )
 
                 # There may be multiple edges to a vertex outside of the contraction
                 if new_edge_pair not in new_edge_weights:
                     new_edge_weights[new_edge_pair] = []
                 new_edge_weights[new_edge_pair].append(edge_weights[old_edge])
 
-                # Delete the edge and edge weight with the neighbout
+                # Delete the edge and edge weight with the neighbour
                 edges[neighbour].remove(vertex)
                 del edge_weights[old_edge]
             # Handled all neighbours of the vertex,
             # can now delete the edges for this vertex
             del edges[vertex]
 
     # Can safely add the new vertices
@@ -530,18 +530,18 @@
     edge_weights: dict[EdgeTuple, float],
     taxa_co_occurrences: dict[EdgeTuple, int],
     tree: PhyloNode,
     tree_weight: float,
     length: float,
     length_function: Callable[[float, PhyloNode], float],
 ) -> list[PcgVertex]:
-    """Recusrive helper to construct the proper cluster graph from the tree in a DFS fashion.
+    """Recursive helper to construct the proper cluster graph from the tree in a DFS fashion.
 
     As all pairs of that are a descendant of an internal but on opposite sides have
-    the same wait, performing a DFS minimisises computational cost of constructing
+    the same wait, performing a DFS minimises computational cost of constructing
     the proper cluster graph.
 
     Parameters
     ----------
     edges : PcgEdgeMap
         The current edges of the proper cluster graph (modified in-place).
     edge_weights : dict[EdgeTuple, float]
```

### Comparing `sc-supertree-2024.2.29.post1/tests/test_cli.py` & `sc-supertree-2024.5.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/dcm_iq_expected.tre` & `sc-supertree-2024.5.6/tests/test_data/dcm_iq_expected.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/dcm_iq_source.tre` & `sc-supertree-2024.5.6/tests/test_data/dcm_iq_source.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/dcm_model_tree.tre` & `sc-supertree-2024.5.6/tests/test_data/dcm_model_tree.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/dcm_source_trees.tre` & `sc-supertree-2024.5.6/tests/test_data/dcm_source_trees.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/supertriplets_expected.tre` & `sc-supertree-2024.5.6/tests/test_data/supertriplets_expected.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_data/supertriplets_source.tre` & `sc-supertree-2024.5.6/tests/test_data/supertriplets_source.tre`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/tests/test_spectral_cluster_supertree.py` & `sc-supertree-2024.5.6/tests/test_spectral_cluster_supertree.py`

 * *Files identical despite different names*

### Comparing `sc-supertree-2024.2.29.post1/PKG-INFO` & `sc-supertree-2024.5.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-supertree
-Version: 2024.2.29.post1
+Version: 2024.5.6
 Summary: Spectral Cluster Supertree
 Keywords: supertree,phylogeny,biology,bioinformatics
 Author: Robert McArthur
 Requires-Python: >=3.10,<3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -14,19 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click ==8.1.7
 Requires-Dist: numpy ==1.26.4
 Requires-Dist: cogent3 ==2024.2.5a1
-Requires-Dist: scikit-learn ==1.4.1.post1
-Requires-Dist: black==24.2.0 ; extra == "dev"
+Requires-Dist: scikit-learn ==1.4.2
+Requires-Dist: black==24.4.2 ; extra == "dev"
 Requires-Dist: isort==5.13.2 ; extra == "dev"
 Requires-Dist: click==8.1.7 ; extra == "dev"
-Requires-Dist: mypy==1.8.0 ; extra == "dev"
+Requires-Dist: mypy==1.10.0 ; extra == "dev"
 Requires-Dist: docformatter ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
@@ -43,14 +43,15 @@
 [![PyPI Version](https://img.shields.io/pypi/v/sc-supertree)](https://pypi.org/project/sc-supertree/)
 [![Python Version](https://img.shields.io/pypi/pyversions/sc-supertree)](https://pypi.org/project/sc-supertree/)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![CI](https://github.com/rmcar17/SpectralClusterSupertree/workflows/CI/badge.svg)](https://github.com/rmcar17/SpectralClusterSupertree/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rmcar17/SpectralClusterSupertree/badge.svg?branch=main)](https://coveralls.io/github/rmcar17/SpectralClusterSupertree?branch=main)
 [![License](https://img.shields.io/github/license/rmcar17/SpectralClusterSupertree)](https://github.com/rmcar17/SpectralClusterSupertree/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/667189656.svg)](https://zenodo.org/badge/latestdoi/667189656)
 
 Spectral Cluster Supertree is a state-of-the-art algorithm for constructing rooted supertrees from collections of rooted source trees.
 
 Spectral Cluster Supertree can be used on Newick formatted trees in Python in conjunction with [cogent3](https://github.com/cogent3/cogent3)'s tree objects, or invoked from the command line.
 
 Spectral Cluster Supertree can employ a number of weighting strategies that take into account the depths of nodes in the trees, as well as branch lengths. A user can specify weights of trees to add bias to some of the source trees if desired.
 
@@ -72,43 +73,43 @@
 supertree = construct_supertree(source_trees, pcg_weighting="branch")
 
 supertree.write("supertree_file.tre")
 ```
 
 ### CLI
 
-In your environment which has spectral-cluster-supertree installed:
+In your environment which has `sc-supertree` installed:
 
 ```bash
 scs -i SOURCE_TREE_FILE -o SUPERTREE_FILE -p PCG_WEIGHTING_STRATEGY
 ```
 
 The ```-i``` and ```-o``` options for the input and output files are required.
 
-The ```-p``` *proper cluster graph* weighting strategy option must be one of ```ONE|DEPTH|BRANCH```. It defaults to ```BRANCH``` when not provided (not recommended when some trees are missing branch lenghts - see below).
+The ```-p``` *proper cluster graph* weighting strategy option must be one of ```ONE|DEPTH|BRANCH```. It defaults to ```BRANCH``` when not provided (not recommended when some trees are missing branch lengths - see below). Tree weights are not supported through the command line.
 
 ## Weighting Strategies
 
 ### Proper Cluster Graph Weighting
 
-Spectral Cluster Supertree recursively paritions the complete set of taxa to form a supertree. The core component of the algorithm involves partitioning the *proper cluster graph* through spectral clustering when the source trees are not consistent.
+Spectral Cluster Supertree recursively partitions the complete set of taxa to form a supertree. The core component of the algorithm involves partitioning the *proper cluster graph* through spectral clustering when the source trees are not consistent.
 
 The *proper cluster graph* has the set of all taxa in the source trees as its vertices, and an edge connects two taxa if they appear together on the same side of the root in any of the source trees (such pairs of taxa are called **proper clusters**). Let $lca$ be the lowest common ancestor of a proper cluster. Each edge is weighted according to the specified strategy:
 
 - **one** - The number of trees in which the pair of taxa appear as a proper cluster in.
 - **depth** - The sum of the depths of the $lca$ of the proper cluster in all of the source trees.
-- **branch** - The sum of the root to $lca$ branch lengths of the proper cluster in all of the source trees. If branch lengths are missing defaults to one (equivalent to depth). Do not use if some trees are missing branch lengths.
+- **branch** - The sum of the root to $lca$ branch lengths of the proper cluster in all of the source trees. If branch lengths are missing defaults to one (equivalent to depth). Do not use if source trees contain a mix of some trees with branch lengths and some without.
 
-The **branch** weighting strategy is recommened where branch lengths are available. Otherwise, the **depth** weighting strategy is recommended over the **one** weighting strategy.
+The **branch** weighting strategy is recommended when branch lengths are available. Otherwise, the **depth** weighting strategy is recommended over the **one** weighting strategy.
 
 ### Tree Weighting
 
-In addition to the above, users may associate trees with weights to bias the results towards specific trees. Prior to the summation of the weights for an edge in the *proper cluster graph*, they are multiplied by the weight of the corresponding tree. The weight of each tree defaults to one if not specified.
+In addition to the above, users may associate trees with weights to bias the results towards specific trees. Prior to the summation of the weights for an edge in the *proper cluster graph*, they are each multiplied by the weight of the corresponding tree. The weight of each tree defaults to one if not specified.
 
-An example is shown below, without the tree weights the alogrithm would randomly return either triple.
+An example is shown below, without the tree weights the algorithm would randomly return either triple.
 
 ```python
 >>> from sc_supertree import construct_supertree
 >>> from cogent3 import make_tree
 >>> tree_1 = make_tree("(a,(b,c))")
 >>> tree_2 = make_tree("(c,(b,a))")
 >>> print(construct_supertree([tree_1, tree_2], weights=[1, 1.5]))
```

