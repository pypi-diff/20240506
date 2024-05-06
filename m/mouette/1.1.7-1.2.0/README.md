# Comparing `tmp/mouette-1.1.7.tar.gz` & `tmp/mouette-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mouette-1.1.7.tar", last modified: Tue Feb 13 16:02:11 2024, max compression
+gzip compressed data, was "mouette-1.2.0.tar", last modified: Mon May  6 09:10:37 2024, max compression
```

## Comparing `mouette-1.1.7.tar` & `mouette-1.2.0.tar`

### file list

```diff
@@ -1,123 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/
--rw-rw-r--   0 root         (0) root         (0)     1075 2023-06-01 07:15:45.000000 mouette-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1956 2024-02-13 16:02:11.585801 mouette-1.1.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1698 2023-06-01 07:15:45.000000 mouette-1.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.573801 mouette-1.1.7/mouette/
--rw-rw-r--   0 root         (0) root         (0)      623 2024-01-31 13:55:01.000000 mouette-1.1.7/mouette/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.577801 mouette-1.1.7/mouette/attributes/
--rw-rw-r--   0 root         (0) root         (0)      181 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/attributes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3709 2024-01-31 13:58:17.000000 mouette-1.1.7/mouette/attributes/glob.py
--rw-rw-r--   0 root         (0) root         (0)     4296 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/attributes/interpolate.py
--rw-rw-r--   0 root         (0) root         (0)     3142 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/attributes/misc_cells.py
--rw-rw-r--   0 root         (0) root         (0)     3090 2024-01-31 15:25:34.000000 mouette-1.1.7/mouette/attributes/misc_corners.py
--rw-rw-r--   0 root         (0) root         (0)     3627 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/attributes/misc_edges.py
--rw-rw-r--   0 root         (0) root         (0)     8500 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/attributes/misc_faces.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/attributes/misc_vertices.py
--rw-rw-r--   0 root         (0) root         (0)     1172 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.577801 mouette-1.1.7/mouette/geometry/
--rw-rw-r--   0 root         (0) root         (0)    15644 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/geometry/SphericalHarmonics.py
--rw-rw-r--   0 root         (0) root         (0)      134 2023-07-18 13:39:55.000000 mouette-1.1.7/mouette/geometry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10482 2024-01-20 09:59:27.000000 mouette-1.1.7/mouette/geometry/aabb.py
--rw-rw-r--   0 root         (0) root         (0)     7061 2024-02-13 10:11:12.000000 mouette-1.1.7/mouette/geometry/geometry.py
--rw-rw-r--   0 root         (0) root         (0)     2408 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/geometry/rotations.py
--rw-rw-r--   0 root         (0) root         (0)     4623 2024-01-31 13:59:00.000000 mouette-1.1.7/mouette/geometry/transform.py
--rw-rw-r--   0 root         (0) root         (0)     1902 2023-07-12 21:22:48.000000 mouette-1.1.7/mouette/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.577801 mouette-1.1.7/mouette/mesh/
--rw-rw-r--   0 root         (0) root         (0)      214 2024-02-13 13:05:47.000000 mouette-1.1.7/mouette/mesh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.577801 mouette-1.1.7/mouette/mesh/datatypes/
--rw-rw-r--   0 root         (0) root         (0)      216 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      574 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/base.py
--rw-rw-r--   0 root         (0) root         (0)     5250 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/linear.py
--rw-rw-r--   0 root         (0) root         (0)      904 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/pointcloud.py
--rw-rw-r--   0 root         (0) root         (0)    20192 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/mesh/datatypes/surface.py
--rw-rw-r--   0 root         (0) root         (0)     1767 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/type_checks.py
--rw-rw-r--   0 root         (0) root         (0)    20556 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/datatypes/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/mesh/io/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/io/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14541 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/io/geogram_ascii.py
--rw-rw-r--   0 root         (0) root         (0)     1330 2023-12-26 20:25:27.000000 mouette-1.1.7/mouette/mesh/io/io.py
--rw-rw-r--   0 root         (0) root         (0)     4999 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/io/medit.py
--rw-rw-r--   0 root         (0) root         (0)     4209 2023-12-26 19:10:04.000000 mouette-1.1.7/mouette/mesh/io/obj.py
--rw-rw-r--   0 root         (0) root         (0)     2191 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/io/off.py
--rw-rw-r--   0 root         (0) root         (0)     1834 2023-12-26 21:23:28.000000 mouette-1.1.7/mouette/mesh/io/stl.py
--rw-rw-r--   0 root         (0) root         (0)     1494 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/mesh/io/tet.py
--rw-rw-r--   0 root         (0) root         (0)     1420 2023-07-02 20:05:44.000000 mouette-1.1.7/mouette/mesh/io/xyz.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-02-13 15:35:46.000000 mouette-1.1.7/mouette/mesh/mesh.py
--rw-rw-r--   0 root         (0) root         (0)    12499 2024-02-13 15:50:06.000000 mouette-1.1.7/mouette/mesh/mesh_attributes.py
--rw-rw-r--   0 root         (0) root         (0)    10987 2024-02-13 15:59:57.000000 mouette-1.1.7/mouette/mesh/mesh_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/operators/
--rw-rw-r--   0 root         (0) root         (0)       83 2023-11-07 09:46:27.000000 mouette-1.1.7/mouette/operators/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3220 2023-11-07 09:46:27.000000 mouette-1.1.7/mouette/operators/adjacency.py
--rw-rw-r--   0 root         (0) root         (0)     2851 2023-11-07 09:46:27.000000 mouette-1.1.7/mouette/operators/gradient.py
--rw-rw-r--   0 root         (0) root         (0)    10333 2023-10-14 11:01:41.000000 mouette-1.1.7/mouette/operators/laplacian_op.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/optimize/
--rw-rw-r--   0 root         (0) root         (0)       77 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/optimize/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1639 2023-10-14 11:01:41.000000 mouette-1.1.7/mouette/optimize/eigensolve.py
--rw-rw-r--   0 root         (0) root         (0)    12823 2023-12-21 13:23:19.000000 mouette-1.1.7/mouette/optimize/levenberg_marquardt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/procedural/
--rw-rw-r--   0 root         (0) root         (0)      278 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/procedural/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1745 2024-02-13 12:55:48.000000 mouette-1.1.7/mouette/procedural/cylinder.py
--rw-rw-r--   0 root         (0) root         (0)     1567 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/procedural/hexahedra.py
--rw-rw-r--   0 root         (0) root         (0)     3091 2024-02-13 12:58:49.000000 mouette-1.1.7/mouette/procedural/platonic.py
--rw-rw-r--   0 root         (0) root         (0)     2787 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/procedural/rings.py
--rw-rw-r--   0 root         (0) root         (0)     3778 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/procedural/sphere.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/processing/
--rw-rw-r--   0 root         (0) root         (0)      707 2023-12-21 12:16:48.000000 mouette-1.1.7/mouette/processing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4182 2023-12-21 13:35:50.000000 mouette-1.1.7/mouette/processing/border.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.581801 mouette-1.1.7/mouette/processing/combinatorics/
--rw-rw-r--   0 root         (0) root         (0)       63 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/combinatorics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17363 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/combinatorics/cutting.py
--rw-rw-r--   0 root         (0) root         (0)     8418 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/combinatorics/subdivide.py
--rw-rw-r--   0 root         (0) root         (0)     8925 2023-10-14 11:01:41.000000 mouette-1.1.7/mouette/processing/connection.py
--rw-rw-r--   0 root         (0) root         (0)     4921 2023-11-07 09:46:27.000000 mouette-1.1.7/mouette/processing/expmap.py
--rw-rw-r--   0 root         (0) root         (0)     9206 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/features.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/mouette/processing/framefield/
--rw-rw-r--   0 root         (0) root         (0)       92 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/framefield/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1782 2023-10-14 11:01:41.000000 mouette-1.1.7/mouette/processing/framefield/base.py
--rw-rw-r--   0 root         (0) root         (0)    13700 2023-12-21 13:25:02.000000 mouette-1.1.7/mouette/processing/framefield/cells.py
--rw-rw-r--   0 root         (0) root         (0)     4009 2023-12-21 13:29:12.000000 mouette-1.1.7/mouette/processing/framefield/curvature_faces.py
--rw-rw-r--   0 root         (0) root         (0)     8496 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/framefield/curvature_vertex.py
--rw-rw-r--   0 root         (0) root         (0)    14720 2023-11-07 09:46:27.000000 mouette-1.1.7/mouette/processing/framefield/faces2d.py
--rw-rw-r--   0 root         (0) root         (0)    10853 2023-12-21 13:25:59.000000 mouette-1.1.7/mouette/processing/framefield/framefield.py
--rw-rw-r--   0 root         (0) root         (0)    18195 2023-07-12 21:22:48.000000 mouette-1.1.7/mouette/processing/framefield/vertex2d.py
--rw-rw-r--   0 root         (0) root         (0)    12386 2023-12-21 13:24:25.000000 mouette-1.1.7/mouette/processing/framefield/vertex3d.py
--rw-rw-r--   0 root         (0) root         (0)     2936 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/mouette/processing/parametrization/
--rw-rw-r--   0 root         (0) root         (0)      250 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/parametrization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1534 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/parametrization/base.py
--rw-rw-r--   0 root         (0) root         (0)     9241 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/parametrization/cone_param.py
--rw-rw-r--   0 root         (0) root         (0)    10003 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/parametrization/cotan_emb.py
--rw-rw-r--   0 root         (0) root         (0)    12940 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/parametrization/distortion.py
--rw-rw-r--   0 root         (0) root         (0)    12791 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/parametrization/ff_integration.py
--rw-rw-r--   0 root         (0) root         (0)     5991 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/parametrization/lscm.py
--rw-rw-r--   0 root         (0) root         (0)     5526 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/parametrization/tutte.py
--rw-rw-r--   0 root         (0) root         (0)     8822 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/paths.py
--rw-rw-r--   0 root         (0) root         (0)     5279 2024-01-31 14:25:31.000000 mouette-1.1.7/mouette/processing/sampling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/mouette/processing/space_partition/
--rw-rw-r--   0 root         (0) root         (0)       30 2023-07-06 09:26:07.000000 mouette-1.1.7/mouette/processing/space_partition/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6230 2023-07-18 13:59:34.000000 mouette-1.1.7/mouette/processing/space_partition/quadtree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/mouette/processing/trees/
--rw-rw-r--   0 root         (0) root         (0)      198 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/trees/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3413 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/trees/base.py
--rw-rw-r--   0 root         (0) root         (0)     3329 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/trees/cell_sp.py
--rw-rw-r--   0 root         (0) root         (0)     8401 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/trees/edge_sp.py
--rw-rw-r--   0 root         (0) root         (0)     3505 2023-06-29 20:38:41.000000 mouette-1.1.7/mouette/processing/trees/face_sp.py
--rw-rw-r--   0 root         (0) root         (0)      451 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/processing/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.585801 mouette-1.1.7/mouette/utils/
--rw-rw-r--   0 root         (0) root         (0)      222 2023-12-21 13:23:09.000000 mouette-1.1.7/mouette/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2159 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/utils/argument_check.py
--rw-rw-r--   0 root         (0) root         (0)     1744 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/utils/iterators.py
--rw-rw-r--   0 root         (0) root         (0)     1476 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/utils/maths.py
--rw-rw-r--   0 root         (0) root         (0)      281 2023-12-21 13:27:28.000000 mouette-1.1.7/mouette/utils/osqp_lin_solve.py
--rw-rw-r--   0 root         (0) root         (0)     2031 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/utils/priority_queue.py
--rw-rw-r--   0 root         (0) root         (0)     8788 2023-06-01 07:15:45.000000 mouette-1.1.7/mouette/utils/unionfind.py
--rw-rw-r--   0 root         (0) root         (0)     1106 2023-12-21 13:26:02.000000 mouette-1.1.7/mouette/utils/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 16:02:11.577801 mouette-1.1.7/mouette.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1956 2024-02-13 16:02:11.000000 mouette-1.1.7/mouette.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3343 2024-02-13 16:02:11.000000 mouette-1.1.7/mouette.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-13 16:02:11.000000 mouette-1.1.7/mouette.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-02-13 16:02:11.000000 mouette-1.1.7/mouette.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-13 16:02:11.000000 mouette-1.1.7/mouette.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      756 2024-02-13 16:01:17.000000 mouette-1.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-13 16:02:11.585801 mouette-1.1.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      578 2024-02-13 16:01:16.000000 mouette-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/
+-rw-rw-r--   0 root         (0) root         (0)     1075 2024-03-06 14:42:58.000000 mouette-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-05-06 09:10:37.841672 mouette-1.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1698 2024-03-06 14:42:58.000000 mouette-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.837672 mouette-1.2.0/mouette/
+-rw-rw-r--   0 root         (0) root         (0)      665 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/attributes/
+-rw-rw-r--   0 root         (0) root         (0)      292 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/attributes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3733 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/attributes/glob.py
+-rw-rw-r--   0 root         (0) root         (0)     4312 2024-05-03 08:08:25.000000 mouette-1.2.0/mouette/attributes/interpolate.py
+-rw-rw-r--   0 root         (0) root         (0)     3144 2024-05-03 11:48:22.000000 mouette-1.2.0/mouette/attributes/misc_cells.py
+-rw-rw-r--   0 root         (0) root         (0)     3097 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/attributes/misc_corners.py
+-rw-rw-r--   0 root         (0) root         (0)     3655 2024-05-02 22:41:20.000000 mouette-1.2.0/mouette/attributes/misc_edges.py
+-rw-rw-r--   0 root         (0) root         (0)     8499 2024-05-03 11:46:26.000000 mouette-1.2.0/mouette/attributes/misc_faces.py
+-rw-rw-r--   0 root         (0) root         (0)     6884 2024-05-02 21:22:46.000000 mouette-1.2.0/mouette/attributes/misc_vertices.py
+-rw-rw-r--   0 root         (0) root         (0)     3671 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/attributes/uv_export.py
+-rw-rw-r--   0 root         (0) root         (0)     1173 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/geometry/
+-rw-rw-r--   0 root         (0) root         (0)    15644 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/geometry/SphericalHarmonics.py
+-rw-rw-r--   0 root         (0) root         (0)      134 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/geometry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10482 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/geometry/aabb.py
+-rw-rw-r--   0 root         (0) root         (0)     9449 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/geometry/geometry.py
+-rw-rw-r--   0 root         (0) root         (0)     2408 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/geometry/rotations.py
+-rw-rw-r--   0 root         (0) root         (0)     4623 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/geometry/transform.py
+-rw-rw-r--   0 root         (0) root         (0)     1902 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/geometry/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/mesh/
+-rw-rw-r--   0 root         (0) root         (0)      185 2024-05-02 15:17:00.000000 mouette-1.2.0/mouette/mesh/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7769 2024-05-03 18:50:39.000000 mouette-1.2.0/mouette/mesh/data_container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/mesh/datatypes/
+-rw-rw-r--   0 root         (0) root         (0)      216 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/datatypes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      574 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/datatypes/base.py
+-rw-rw-r--   0 root         (0) root         (0)     4903 2024-05-03 09:59:23.000000 mouette-1.2.0/mouette/mesh/datatypes/linear.py
+-rw-rw-r--   0 root         (0) root         (0)      904 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/datatypes/pointcloud.py
+-rw-rw-r--   0 root         (0) root         (0)    21667 2024-05-03 18:45:25.000000 mouette-1.2.0/mouette/mesh/datatypes/surface.py
+-rw-rw-r--   0 root         (0) root         (0)     1767 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/datatypes/type_checks.py
+-rw-rw-r--   0 root         (0) root         (0)    20769 2024-05-03 11:46:24.000000 mouette-1.2.0/mouette/mesh/datatypes/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/mesh/io/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/io/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14524 2024-05-02 15:14:17.000000 mouette-1.2.0/mouette/mesh/io/geogram_ascii.py
+-rw-rw-r--   0 root         (0) root         (0)     1424 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/mesh/io/io.py
+-rw-rw-r--   0 root         (0) root         (0)     4829 2024-05-02 14:45:45.000000 mouette-1.2.0/mouette/mesh/io/medit.py
+-rw-rw-r--   0 root         (0) root         (0)     4259 2024-05-02 15:03:52.000000 mouette-1.2.0/mouette/mesh/io/obj.py
+-rw-rw-r--   0 root         (0) root         (0)     2287 2024-05-02 15:25:24.000000 mouette-1.2.0/mouette/mesh/io/off.py
+-rw-rw-r--   0 root         (0) root         (0)     1260 2024-05-02 14:40:54.000000 mouette-1.2.0/mouette/mesh/io/ply.py
+-rw-rw-r--   0 root         (0) root         (0)     3257 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/mesh/io/stl.py
+-rw-rw-r--   0 root         (0) root         (0)     1494 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/mesh/io/tet.py
+-rw-rw-r--   0 root         (0) root         (0)     1420 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/mesh/io/xyz.py
+-rw-rw-r--   0 root         (0) root         (0)     6633 2024-05-03 07:46:25.000000 mouette-1.2.0/mouette/mesh/mesh.py
+-rw-rw-r--   0 root         (0) root         (0)    12499 2024-05-02 14:28:28.000000 mouette-1.2.0/mouette/mesh/mesh_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)     9572 2024-05-03 18:32:13.000000 mouette-1.2.0/mouette/mesh/mesh_data.py
+-rw-rw-r--   0 root         (0) root         (0)     8569 2024-05-03 11:48:24.000000 mouette-1.2.0/mouette/mesh/subdivision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/operators/
+-rw-rw-r--   0 root         (0) root         (0)       83 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/operators/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3220 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/operators/adjacency.py
+-rw-rw-r--   0 root         (0) root         (0)     2919 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/operators/gradient.py
+-rw-rw-r--   0 root         (0) root         (0)    10361 2024-05-03 07:48:02.000000 mouette-1.2.0/mouette/operators/laplacian_op.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/optimize/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/optimize/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1639 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/optimize/eigensolve.py
+-rw-rw-r--   0 root         (0) root         (0)    12823 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/optimize/levenberg_marquardt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/procedural/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/procedural/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2559 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/procedural/flat.py
+-rw-rw-r--   0 root         (0) root         (0)     2787 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/procedural/rings.py
+-rw-rw-r--   0 root         (0) root         (0)    13798 2024-05-03 18:31:44.000000 mouette-1.2.0/mouette/procedural/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     1650 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/procedural/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/processing/
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4293 2024-05-03 18:54:51.000000 mouette-1.2.0/mouette/processing/border.py
+-rw-rw-r--   0 root         (0) root         (0)     8879 2024-05-03 14:48:16.000000 mouette-1.2.0/mouette/processing/connection.py
+-rw-rw-r--   0 root         (0) root         (0)    17485 2024-05-03 14:48:51.000000 mouette-1.2.0/mouette/processing/cutting.py
+-rw-rw-r--   0 root         (0) root         (0)     4923 2024-05-02 21:22:04.000000 mouette-1.2.0/mouette/processing/expmap.py
+-rw-rw-r--   0 root         (0) root         (0)     8811 2024-05-03 19:00:02.000000 mouette-1.2.0/mouette/processing/features.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/processing/framefield/
+-rw-rw-r--   0 root         (0) root         (0)       92 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/processing/framefield/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1782 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/framefield/base.py
+-rw-rw-r--   0 root         (0) root         (0)    13703 2024-05-03 11:48:33.000000 mouette-1.2.0/mouette/processing/framefield/cells.py
+-rw-rw-r--   0 root         (0) root         (0)     4011 2024-05-03 07:54:44.000000 mouette-1.2.0/mouette/processing/framefield/curvature_faces.py
+-rw-rw-r--   0 root         (0) root         (0)     8420 2024-05-03 07:50:18.000000 mouette-1.2.0/mouette/processing/framefield/curvature_vertex.py
+-rw-rw-r--   0 root         (0) root         (0)    14725 2024-05-03 11:47:49.000000 mouette-1.2.0/mouette/processing/framefield/faces2d.py
+-rw-rw-r--   0 root         (0) root         (0)    10854 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/framefield/framefield.py
+-rw-rw-r--   0 root         (0) root         (0)    18197 2024-05-03 14:46:56.000000 mouette-1.2.0/mouette/processing/framefield/vertex2d.py
+-rw-rw-r--   0 root         (0) root         (0)    12388 2024-05-03 11:48:41.000000 mouette-1.2.0/mouette/processing/framefield/vertex3d.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/processing/parametrization/
+-rw-rw-r--   0 root         (0) root         (0)      307 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1537 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/base.py
+-rw-rw-r--   0 root         (0) root         (0)     9244 2024-05-03 07:51:53.000000 mouette-1.2.0/mouette/processing/parametrization/cone_param.py
+-rw-rw-r--   0 root         (0) root         (0)    10009 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/cotan_emb.py
+-rw-rw-r--   0 root         (0) root         (0)    12916 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/distortion.py
+-rw-rw-r--   0 root         (0) root         (0)    12773 2024-05-03 07:52:22.000000 mouette-1.2.0/mouette/processing/parametrization/ff_integration.py
+-rw-rw-r--   0 root         (0) root         (0)     5990 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/lscm.py
+-rw-rw-r--   0 root         (0) root         (0)     5532 2024-05-03 11:41:54.000000 mouette-1.2.0/mouette/processing/parametrization/tutte.py
+-rw-rw-r--   0 root         (0) root         (0)     8979 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/processing/parametrization/winslow.py
+-rw-rw-r--   0 root         (0) root         (0)     8825 2024-05-02 21:22:10.000000 mouette-1.2.0/mouette/processing/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/processing/trees/
+-rw-rw-r--   0 root         (0) root         (0)      198 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/processing/trees/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3413 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/processing/trees/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3329 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/processing/trees/cell_sp.py
+-rw-rw-r--   0 root         (0) root         (0)     8403 2024-05-02 21:22:24.000000 mouette-1.2.0/mouette/processing/trees/edge_sp.py
+-rw-rw-r--   0 root         (0) root         (0)     3514 2024-05-03 07:54:07.000000 mouette-1.2.0/mouette/processing/trees/face_sp.py
+-rw-rw-r--   0 root         (0) root         (0)      451 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/processing/worker.py
+-rw-rw-r--   0 root         (0) root         (0)     8449 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/sampling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/space_partition/
+-rw-rw-r--   0 root         (0) root         (0)       30 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/space_partition/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6227 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/space_partition/quadtree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/splines/
+-rw-rw-r--   0 root         (0) root         (0)       77 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/splines/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      951 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/splines/bezier_curve.py
+-rw-rw-r--   0 root         (0) root         (0)     1306 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/splines/bezier_surface.py
+-rw-rw-r--   0 root         (0) root         (0)      716 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/splines/evaluate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.841672 mouette-1.2.0/mouette/utils/
+-rw-rw-r--   0 root         (0) root         (0)      222 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2159 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/argument_check.py
+-rw-rw-r--   0 root         (0) root         (0)     1744 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/iterators.py
+-rw-rw-r--   0 root         (0) root         (0)     1476 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/maths.py
+-rw-rw-r--   0 root         (0) root         (0)      281 2024-05-02 14:21:29.000000 mouette-1.2.0/mouette/utils/osqp_lin_solve.py
+-rw-rw-r--   0 root         (0) root         (0)     2031 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/priority_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     8788 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/unionfind.py
+-rw-rw-r--   0 root         (0) root         (0)     1106 2024-03-06 14:42:58.000000 mouette-1.2.0/mouette/utils/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:10:37.837672 mouette-1.2.0/mouette.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-05-06 09:10:37.000000 mouette-1.2.0/mouette.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3452 2024-05-06 09:10:37.000000 mouette-1.2.0/mouette.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:10:37.000000 mouette-1.2.0/mouette.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-06 09:10:37.000000 mouette-1.2.0/mouette.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-06 09:10:37.000000 mouette-1.2.0/mouette.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      784 2024-05-03 19:06:41.000000 mouette-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 09:10:37.841672 mouette-1.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      597 2024-05-03 19:06:43.000000 mouette-1.2.0/setup.py
```

### Comparing `mouette-1.1.7/LICENSE` & `mouette-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/PKG-INFO` & `mouette-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouette
-Version: 1.1.7
+Version: 1.2.0
 Summary: Mesh, Tools and Geometry Processing
 Home-page: https://github.com/GCoiffier/mouette
 Author: GCoiffier
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mouette-1.1.7/README.md` & `mouette-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/__init__.py` & `mouette-1.2.0/mouette/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from . import mesh
 from . import attributes
 from . import procedural
 from . import operators
 from . import geometry
 from . import processing
 from . import optimize
+from . import sampling
+from . import space_partition
+from . import splines
 
 from .processing import framefield
 from .processing import parametrization
-from .processing import sampling
 
 from .geometry.vector import Vec
 from .geometry import transform
 from .utils import Logger
 from .processing.worker import Worker
 from .mesh.mesh_attributes import ArrayAttribute, Attribute
```

### Comparing `mouette-1.1.7/mouette/attributes/glob.py` & `mouette-1.2.0/mouette/attributes/glob.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,28 @@
     """
     
     v = len(mesh.vertices)
     e = len(mesh.edges)
     f = len(mesh.faces)
     return v-e+f
 
-@allowed_mesh_types(SurfaceMesh)
-def genus(mesh : SurfaceMesh) -> int:
-    """Computes the genus g of a mesh.
-    The genus is the number of "holes" a surface contains. It is linked to the euler characteristic X by
-    X = 2 - 2g
+# @allowed_mesh_types(SurfaceMesh)
+# def genus(mesh : SurfaceMesh) -> int:
+#     """Computes the genus g of a mesh.
+#     The genus is the number of "holes" a surface contains. It is linked to the euler characteristic X by
+#     X = 2 - 2g
 
-    Parameters:
-        mesh (Mesh): the mesh
+#     Parameters:
+#         mesh (Mesh): the mesh
 
-    Returns:
-        (int): the Euler characteristic
-    """
-    X = euler_characteristic(mesh)
-    return 1 - X//2
+#     Returns:
+#         (int): the Euler characteristic
+#     """
+#     X = euler_characteristic(mesh)
+#     return 1 - X//2
 
 @forbidden_mesh_types(PointCloud)
 def mean_edge_length(mesh : Mesh, n : int = None) -> float:
     """
     Estimation of mean edge length
 
     Parameters:
```

### Comparing `mouette-1.1.7/mouette/attributes/interpolate.py` & `mouette-1.2.0/mouette/attributes/interpolate.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,28 @@
         Exception: fails if 'weight' is not in {'uniform', 'area', 'angle'}
     """
     if weight not in {'uniform', 'area', 'angle'}:
         raise Exception(f"interpolate_vertices_to_faces: weight argument '{weight}' not recognized.\nPossibilites are {'uniform', 'area', 'angle'}.")
 
     if weight=="uniform":
         for v in mesh.id_vertices:
-            for f in mesh.connectivity.vertex_to_face(v):
+            for f in mesh.connectivity.vertex_to_faces(v):
                 vattr[v] = vattr[v] + fattr[f]
         for v in mesh.id_vertices:
-            vattr[v] /= mesh.connectivity.n_VtoF(v)
+            vattr[v] /= len(mesh.connectivity.vertex_to_faces(v))
     
     elif weight=="area":
         if mesh.faces.has_attribute("area"):
             area = mesh.faces.get_attribute("area")
         else:
             area = face_area(mesh, persistent=False)
         total_area = np.zeros(len(mesh.vertices))
         for v in mesh.id_vertices:
             total_area[v] = 0.
-            for f in mesh.connectivity.vertex_to_face(v):
+            for f in mesh.connectivity.vertex_to_faces(v):
                 vattr[v] = vattr[v] + fattr[f] * area[f]
                 total_area[v] = total_area[v] + area[f]
         for v in mesh.id_vertices:
             vattr[v] /= total_area[v]
 
     elif weight=="angle":
         if mesh.face_corners.has_attribute("angles"):
```

### Comparing `mouette-1.1.7/mouette/attributes/misc_cells.py` & `mouette-1.2.0/mouette/attributes/misc_cells.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,11 +67,11 @@
     """
     if persistent:
         bndf = mesh.cells.create_attribute(name, int, dense=dense)
     else:
         bndf = ArrayAttribute(int, len(mesh.cells)) if dense else Attribute(int)
 
     for iF in mesh.id_faces:
-        if len(mesh.connectivity.face_to_cell(iF))==1 : 
-            iC = mesh.connectivity.face_to_cell(iF)[0]
+        if len(mesh.connectivity.face_to_cells(iF))==1 : 
+            iC = mesh.connectivity.face_to_cells(iF)[0]
             bndf[iC] += 1
     return bndf
```

### Comparing `mouette-1.1.7/mouette/attributes/misc_corners.py` & `mouette-1.2.0/mouette/attributes/misc_corners.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     else:
         cot = ArrayAttribute(float, len(mesh.face_corners)) if dense else Attribute(float)
 
     if mesh.face_corners.has_attribute("angles"):
         # Compute cotan from angles
         angles = mesh.face_corners.get_attribute("angles")
         for c in mesh.id_corners:
-            cot[c] = math.cotan(angles[c])
+            cot[c] = -np.tan(angles[c] + np.pi/2)
     else:
         for i, (iA,iB,iC) in enumerate(mesh.faces):
             pA, pB, pC = (mesh.vertices[_i] for _i in (iA,iB,iC))
             cot[3*i] = geom.cotan(pC, pA, pB)
             cot[3*i+1] = geom.cotan(pA, pB, pC)
             cot[3*i+2] = geom.cotan(pB, pC, pA)
     return cot
```

### Comparing `mouette-1.1.7/mouette/attributes/misc_edges.py` & `mouette-1.2.0/mouette/attributes/misc_edges.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     Note:
         See Curvature Frame Fields for their aggregation on triangles or vertices
     """
 
     data = np.zeros((len(mesh.edges), 3,3), dtype=np.float64)
     for e, (A,B) in enumerate(mesh.edges):
-        T1,T2 = mesh.half_edges.edge_to_triangles(A,B)
+        T1,T2 = mesh.connectivity.edge_to_faces(A,B)
         if T1 is not None and T2 is not None:
             _,_,n1 = geom.face_basis(*(mesh.vertices[u] for u in mesh.faces[T1]))
             _,_,n2 = geom.face_basis(*(mesh.vertices[u] for u in mesh.faces[T2]))
             # angle = geom.signed_angle_2vec3D(n1,n2,n2-n1)
             angle = geom.angle_2vec3D(n1,n2)
             edge = Vec.normalized(mesh.vertices[B] - mesh.vertices[A])
             data[e,:,:] = angle * np.outer(edge,edge)
@@ -66,16 +66,16 @@
 
     if mesh.face_corners.has_attribute("cotan"):
         cot = mesh.face_corners.get_attribute("cotan")
     else:
         cot = cotangent(mesh,persistent=persistent)
 
     for e,(A,B) in enumerate(mesh.edges):
-        T,iA,iB = mesh.half_edges.adj(A,B)
+        T,iA,iB = mesh.connectivity.direct_face(A,B,True)
         if T is not None:
             cnr = mesh.connectivity.face_to_first_corner(T)+3-iA-iB
             cw[e] += cot[cnr]/2
-        T,iB,iA = mesh.half_edges.adj(B,A)
+        T,iB,iA = mesh.connectivity.direct_face(B,A,True)
         if T is not None:
             cnr = mesh.connectivity.face_to_first_corner(T)+3-iA-iB
             cw[e] += cot[cnr]/2
     return cw
```

### Comparing `mouette-1.1.7/mouette/attributes/misc_faces.py` & `mouette-1.2.0/mouette/attributes/misc_faces.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,22 +124,22 @@
 
     Returns:
         Attribute: one bool per faces. If not persistent, returns a set.
     """
     
     near = set()
     for e in mesh.boundary_edges:
-        T1,T2 = mesh.half_edges.edge_to_triangles(*mesh.edges[e])
+        T1,T2 = mesh.connectivity.edge_to_faces(*mesh.edges[e])
         if T1 is None: near.add(T2)
         else: near.add(T1)
     for _ in range(dist-1):
         new_near = set()
         for T in mesh.id_faces:
             if T in near : continue
-            for T2 in mesh.connectivity.face_to_face(T):
+            for T2 in mesh.connectivity.face_to_faces(T):
                 if T2 in near: new_near.add(T)
         near = near | new_near
     
     if persistent:
         near_attr = mesh.faces.create_attribute(name, bool, dense=dense)
     else:
         near_attr = ArrayAttribute(bool, len(mesh.faces)) if dense else Attribute(bool)
```

### Comparing `mouette-1.1.7/mouette/attributes/misc_vertices.py` & `mouette-1.2.0/mouette/attributes/misc_vertices.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,21 +131,21 @@
     """
     if persistent:
         bnormals = mesh.vertices.create_attribute(name, float, 3, dense=dense)
     else:
         bnormals = ArrayAttribute(float, len(mesh.vertices), 3) if dense else Attribute(float, 3)
 
     for v in mesh.boundary_vertices:
-        v0 = mesh.connectivity.vertex_to_vertex(v)[0]
-        v1 = mesh.connectivity.vertex_to_vertex(v)[-1]
+        v0 = mesh.connectivity.vertex_to_vertices(v)[0]
+        v1 = mesh.connectivity.vertex_to_vertices(v)[-1]
         P,P0,P1 = (mesh.vertices[u] for u in (v,v0,v1))
         E0 = P - P0
         E1 = P1 - P
-        T0,_,_ = mesh.half_edges.adj(v0,v)
-        if T0 is None: T0,_,_ = mesh.half_edges.adj(v,v0)
-        T1,_,_ = mesh.half_edges.adj(v,v1)
-        if T1 is None: T1,_,_ = mesh.half_edges.adj(v1,v)
+        T0 = mesh.connectivity.direct_face(v0,v)
+        if T0 is None: T0 = mesh.connectivity.direct_face(v,v0)
+        T1 = mesh.connectivity.direct_face(v,v1)
+        if T1 is None: T1 = mesh.connectivity.direct_face(v1,v)
         _,_,N0 = geom.face_basis(*mesh.pt_of_face(T0))
         _,_,N1 = geom.face_basis(*mesh.pt_of_face(T1))
         bnormals[v] = geom.cross(E0,N0) + geom.cross(E1,N1)
         bnormals[v] = Vec.normalized(bnormals[v])
     return bnormals
```

### Comparing `mouette-1.1.7/mouette/config.py` & `mouette-1.2.0/mouette/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 """
 Whether to export edges as 'l <v> <v>' fields in .obj file format
 """
 export_edges_in_obj = True
 
 """
-/!\ If set to true, this will compute the half edge structure on the mesh (which can cause a lot of computations)
+/!\\ If set to true, this will compute the half edge structure on the mesh (which can cause a lot of computations)
 """
 sort_neighborhoods = True
 
 """
 When creating an attribute that already exists on a mesh, mouette prints a warning in the console and returns the attribute currently carrying this name.
 If this flag is set to True, no warning is printed. We then assume that you know what you are doing
 """
```

### Comparing `mouette-1.1.7/mouette/geometry/SphericalHarmonics.py` & `mouette-1.2.0/mouette/geometry/SphericalHarmonics.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/geometry/aabb.py` & `mouette-1.2.0/mouette/geometry/aabb.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/geometry/geometry.py` & `mouette-1.2.0/mouette/geometry/geometry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,115 @@
 from .vector import Vec
 import numpy as np
 import math
 from typing import Union
 
-def sign0(x : float):
-    """sign of x
-        1 if x >= 0
-        -1 if x < 0
+def sign0(x: float):
+    """
+    $$\\text{sign0}(x)=\\begin{cases} 
+        1 \\text{ if } x\\geqslant0 \\\\
+        -1 \\text{ if } x<0
+    \\end{cases}$$
 
     Parameters:
         x (float): input number
 
     Returns:
-        [float]: the sign of x
+        float: the sign of x
     """
     if x>=0: return 1
     return -1
 
-def sign(x : float):
-    """sign of x
-        1 if x > 0
-        -1 if x < 0
-        0 if x = 0
+def sign(x: float):
+    """
+    $$\\text{sign}(x)=\\begin{cases} 
+        0 \\text{ if } x=0 \\\\
+        1 \\text{ if } x>0 \\\\
+        -1 \\text{ if } x<0
+    \\end{cases}$$
 
     Parameters:
         x (float): input number
 
     Returns:
-        [float]: x/|x|
+        float: x/|x| and 0 for x=0
     """
     if x>0: return 1
     elif x<0 : return -1
     return 0
 
-def norm(x : np.ndarray):
+def norm(x: np.ndarray) -> float:
+    """Euclidean norm of vector x, defined as $\\sqrt{x^Tx}$
+
+    Args:
+        x (np.ndarray): vector
+
+    Returns:
+        float: Euclidean norm
+    """
     return np.sqrt(np.dot(x.flatten(), x.flatten()))
 
-def dot(A,B):
+def dot(A: np.ndarray, B: np.ndarray) -> float:
+    """dot product $A^TB$ between two vectors
+
+    Args:
+        A (np.ndarray): first vector
+        B (np.ndarray): second vector
+
+    Returns:
+        float: dot product
+    """
     return np.dot(A,B)
 
-def distance(a : np.ndarray, b : np.ndarray):
-    return norm(b-a)
+def distance(A: Vec, B: Vec) -> float:
+    """Euclidean distance between A and B, defined as $||B-A|| = \\sqrt{(B-A)^T(B-A)}$
+
+    Args:
+        a (Vec): first point
+        b (Vec): second point
+
+    Returns:
+        float: distance
+    """
+    return norm(B-A)
+
+def cross(A: Vec, B: Vec) -> Vec:
+    """Cross product of vectors A and B
 
-def cross(v1,v2):
+    Args:
+        A (Vec): Size 3 vector
+        B (Vec): Size 3 vector
+        
+    Returns:
+        Vec: cross product AxB
+    """
     return Vec(
-        v1[1]*v2[2] - v1[2] * v2[1],
-        v2[0]*v1[2] - v2[2] * v1[0],
-        v1[0]*v2[1] - v1[1] * v2[0]
+        A[1]*B[2] - A[2] * B[1],
+        B[0]*A[2] - B[2] * A[0],
+        A[0]*B[1] - A[1] * B[0]
     )
 
-def cotan(A:Vec, B:Vec, C:Vec):
-    """ 
-    A,B,C three points in R^3
-    returns the cotangent of the angle from BA to BC
+def cotan(A: Vec, B: Vec, C: Vec) -> float:
+    """cotangent of the angle $\\hat{ABC}$
+    Parameters:
+        A (Vec): point A
+        B (Vec): point B
+        C (Vec): point C
+
+    Returns:
+        float: the cotangent
     """
     A, B, C = Vec(A), Vec(B), Vec(C)
     BA = Vec.normalized(A-B)
     BC = Vec.normalized(C-B)
     cosine = np.dot(BA,BC)
     sine = norm(cross(BA,BC))
     return cosine/sine
 
-def angle_3pts(A:Vec, B:Vec, C:Vec) -> float:
+def angle_3pts(A: Vec, B: Vec, C: Vec) -> float:
     """Angle ABC between three points
 
     Parameters:
         A (Vec): first point
         B (Vec): central point
         C (Vec): second point
 
@@ -75,15 +119,15 @@
     BA = Vec(A)-Vec(B)
     BC = Vec(C)-Vec(B)
     s = cross(BA,BC).norm()
     c = dot(BA,BC)
     return math.atan2(s, c)
 
 
-def signed_angle_2vec3D(V1:Vec, V2:Vec, N:Vec) -> float:
+def signed_angle_2vec3D(V1: Vec, V2: Vec, N: Vec) -> float:
     """Signed angle between two vectors with orientation given by normal N
 
     Parameters:
         V1 (Vec): First vector
         V2 (Vec): Second vector
         N (Vec): reference normal direction
 
@@ -106,39 +150,94 @@
 
     Returns:
         float: the angle
     """
     return signed_angle_2vec3D(A-B, C-B, N)
 
 def angle_2vec2D(V1:Vec, V2:Vec) -> float:
+    """Angle between two **2D** vectors
+
+    Args:
+        V1 (Vec): first vector
+        V2 (Vec): second vector
+
+    Returns:
+        float: the angle
+    """
     return math.atan2(V2.y, V2.x) - math.atan2(V1.y, V1.x)
 
 def angle_2vec3D(V1:Vec, V2:Vec) -> float:
+    """Angle between two **3D** vectors
+
+    Args:
+        V1 (Vec): first vector
+        V2 (Vec): second vector
+
+    Returns:
+        float: the angle
+    """
     C = cross(V1,V2)
     return math.atan2(C.norm(), dot(V1,V2))
 
 def face_basis(*f):
-    """ 
+    """
     Orthonormal basis of face
     Given three points A,B,C, returns a basis such that the first vector is along direction AB and third vector is normal to the plane ABC
+
+    Args:
+        A,B,C: three points (in a list or not)
+
+    Returns:
+        Vec,Vec,Vec: an orthonormal 3D basis of the face
     """
     if len(f)==1: f = f[0]
     pA,pB,pC = (x for x in f)
     X = Vec.normalized(pB-pA)
     Z = Vec.normalized(cross(X, pC-pA))
     Y = Vec.normalized(cross(Z,X))
     return X,Y,Z
 
-def triangle_area(A:Vec, B:Vec, C:Vec) -> float :
+def triangle_area(A: Vec, B: Vec, C: Vec) -> float:
+    """Area of 3D triangle ABC
+
+    Args:
+        A (Vec): first point
+        B (Vec): second point
+        C (Vec): third point
+
+    Returns:
+        float: area
+    """
     return cross(B-A,C-A).norm()/2
 
-def triangle_area_2D(A:Vec, B:Vec, C:Vec) -> float :
+def triangle_area_2D(A: Vec, B: Vec, C: Vec) -> float:
+    """Area of 2D triangle ABC
+
+    Args:
+        A (Vec): first point
+        B (Vec): second point
+        C (Vec): third point
+
+    Returns:
+        float: area
+    """
     return abs(det_2x2(B-A,C-A)/2)
 
 def quad_area(A:Vec, B:Vec, C:Vec, D:Vec) -> float:
+    """Area of the quad ABCD
+
+    Args:
+        A (Vec): first point
+        B (Vec): second point
+        C (Vec): third point
+        D (Vec): fourth point
+
+    Returns:
+        float: area
+    """
     return (triangle_area(A,B,C) + triangle_area(A,C,D) + triangle_area(B,C,D) + triangle_area(B,D,A))/2
 
 def det_2x2(A:Union[complex,np.ndarray], B:Union[complex,np.ndarray]) -> float:
     """Computes a 2x2 determinant
 
     Parameters:
         A (Union[complex,np.ndarray]): first column vector. Can also be a complex number
@@ -157,15 +256,15 @@
         bx,by = B[0], B[1]
     return ax*by - ay*bx
 
 def det_3x3(*args) -> float:
     """Computes a 3x3 using the rule of Sarrus
     
     Parameters:
-        Either a 3*3 numpy array representing a matrix, or 3 3*1 numpy array representing three column vectors
+        args: Either a 3x3 numpy array representing a matrix, or 3 3x1 numpy array representing three column vectors
 
     Returns:
         float: the determinant
     """
     if len(args)==1:
         mat = args[0]
         assert mat.shape == (3,3)
@@ -177,30 +276,42 @@
         mat[0,2] * mat[1,0] * mat[2,1] - \
         mat[0,0] * mat[1,2] * mat[2,1] - \
         mat[0,1] * mat[1,0] * mat[2,2] - \
         mat[0,2] * mat[1,1] * mat[2,0]
     return d
 
 def intersect_2lines2D(p1 : Vec, d1 : Vec, p2: Vec, d2 : Vec) -> Vec:
+    """Computes the intersection of two lines in the plane
+
+    Args:
+        p1 (Vec): point on the first line
+        d1 (Vec): direction vector of the first line
+        p2 (Vec): point on the second line
+        d2 (Vec): direction vector of the second line
+
+    Returns:
+        Vec: the intersection point. None if lines are parallel
+    """
     p1,d1,p2,d2 = (u[:2] for u in (p1,d1,p2,d2))
     if abs(det_2x2(d1,d2))<1e-12 : return None #parallel lines
     n2 = Vec(d2.y, -d2.x)
     t = dot(p2-p1,n2)/dot(d1,n2)
     return p1+t*d1
 
 def circumcenter(v1 : Vec, v2 : Vec, v3: Vec) -> Vec:
     """Circumcenter of the triangle formed by three points in space
 
-    /!\ circumcenter of triangle (v1,v2,v3) may not lay inside the triangle
-
     Parameters:
         v1 (Vec): first point
         v2 (Vec): second point
         v3 (Vec): third point
 
+    Warning:
+        Circumcenter of triangle (v1,v2,v3) may not lay inside the triangle
+
     Returns:
         Vec: coordinates of the circumcenter
     """
     p1 = (v1+v2)/2
     p2 = (v1+v3)/2
     d1 = v2-v1
     d2 = v3-v1
```

### Comparing `mouette-1.1.7/mouette/geometry/rotations.py` & `mouette-1.2.0/mouette/geometry/rotations.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/geometry/transform.py` & `mouette-1.2.0/mouette/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/geometry/vector.py` & `mouette-1.2.0/mouette/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/base.py` & `mouette-1.2.0/mouette/mesh/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/linear.py` & `mouette-1.2.0/mouette/mesh/datatypes/linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """
         return range(len(self.edges))
 
     class _Connectivity:
         """
         Connectivity handler class. Allows connectivity queries on the object, like neighbours of a vertex, etc.
 
-        Connectivity is computed lazily only when needed in the code. For instance, the first call to `mesh.connectivity.vertex_to_vertex` will generate the vertex_to_vertex array, so that the next call will not perform any computation but a lookup in the array.
+        Connectivity is computed lazily only when needed in the code. For instance, the first call to `mesh.connectivity.vertex_to_vertices` will generate the vertex_to_vertices dictionnary, so that the next call will not perform any computation but a lookup in the array.
         """
         
         def __init__(self, master):
             self.mesh = master
 
             self._edge_id : dict = None # (v1, v2) -> edge | None
             self._adjV2V : dict = None # vertex -> vertex
@@ -53,26 +53,26 @@
             """
             Resets connectivity. 
             The next query in the code will regenerate internal arrays.
             """
             self._edge_id = None
             self._adjV2V = None
 
-        def _compute_vertex_adj(self):
+        def _compute_connectivity(self):
             self._adjV2V = dict([(i,set()) for i in self.mesh.id_vertices ])
 
             for (A,B) in self.mesh.edges:
                 assert A != B # should not be possible
                 self._adjV2V[A].add(B)
                 self._adjV2V[B].add(A)
                     
             for U in self.mesh.id_vertices:
                 self._adjV2V[U] = list(self._adjV2V[U])
 
-        def _compute_edge_adj(self):
+        def _compute_edge_id(self):
             self._edge_id = dict()
             for iE,E in enumerate(self.mesh.edges):
                 key = utils.keyify(E)
                 self._edge_id[key] = iE
 
         def edge_id(self, V1:int, V2:int)->int:
             """
@@ -83,15 +83,15 @@
                 V1 (int): first vertex of the edge
                 V2 (int): second vertex of the edge
 
             Returns:
                 int: the id of edge (V1,V2), or `None` if the edge does not exist.
             """
             if self._edge_id is None:
-                self._compute_edge_adj()
+                self._compute_edge_id()
             key = utils.keyify(V1,V2)
             return self._edge_id.get(key, None)
 
         def other_edge_end(self, E:int, V:int) -> int:
             """
             Vertex at the opposite end of edge `E` from vertex `V`.
             Returns `None` if `V` is not adjacent to edge `E`
@@ -104,63 +104,48 @@
                 int: the vertex `W` such that `E` is the edge `(V,W)`. Returns `None` if `V` is not adjacent to edge `E`
             """
             A,B = self.mesh.edges[E]
             if V==A: return B
             if V==B: return A
             return None
 
-        ##### Vertex to Vertex #####
+        ##### Vertex to elements
 
-        def vertex_to_vertex(self, V : int) -> list:
+        def vertex_to_vertices(self, V: int) -> list:
             """
             Neighborhood of vertex `V` in terms of vertices.
 
             Args:
                 V (int): vertex id
 
             Returns:
                 list: list of vertices `W` such that `(V,W)` is a valid edge in the polyline.
             """
             if self._adjV2V is None : 
-                self._compute_vertex_adj()
+                self._compute_connectivity()
             return self._adjV2V[V]
 
-        def n_VtoV(self, V : int) -> int:
-            """
-            Size of the neighborhood of vertex `V`
-
-            Args:
-                V (int): vertex id
-
-            Returns:
-                int: `len(vertex_to_vertex(V))`
-            """
-            if self._adjV2V is None:
-                self._compute_vertex_adj()
-            return len(self._adjV2V[V])
-
-        ##### Vertex to Edges #####
-
-        def vertex_to_edge(self, V : int) -> list:
+        def vertex_to_edges(self, V: int) -> list:
             """
             Neighborhood of vertex `V` in terms of edges.
 
             Args:
                 V (int): vertex id
 
             Returns:
                 list: list of edges E such that V belongs to E.
             """
-            return [ self.edge_id(V, u) for u in self.vertex_to_vertex(V)]
+            return [ self.edge_id(V, u) for u in self.vertex_to_vertices(V)]
 
-        def n_VtoE(self, V : int) -> int:
-            """
-            Size of the neighborhood of vertex `V`
+
+        ##### Edge to elements
+
+        def edge_to_vertices(self, E: int) -> list:
+            """Returns the two vertex indices that are adjacent to edge `E
 
             Args:
-                V (int): vertex id
+                E (int): edge index
 
             Returns:
-                int: `len(vertex_to_edge(V))`
+                list: two vertex indices
             """
-            return self.n_VtoV(V)
-
+            return self.mesh.edges[E]
```

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/pointcloud.py` & `mouette-1.2.0/mouette/mesh/datatypes/pointcloud.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/surface.py` & `mouette-1.2.0/mouette/mesh/datatypes/surface.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,49 +2,46 @@
 from ..mesh_attributes import Attribute
 from .base import Mesh
 from .linear import PolyLine
 from ... import utils
 from ... import config
 
 class SurfaceMesh(Mesh):
-    """
-    A data structure for representing polygonal surfaces.
-
+    """A data structure for representing polygonal surfaces.
+    
     Attributes:
         vertices (DataContainer): the container for all vertices
         edges (DataContainer): the container for all edges
         faces (DataContainer): the container for all faces
         face_corners (DataContainer): the container for all corner of faces
 
         boundary_edges (list): list of all edges on the boundary
-        interior_edges (list): list of all interior edges (all edges \ boundary_edges)
+        interior_edges (list): list of all interior edges (all edges \\ boundary_edges)
         boundary_vertices (list): list of all vertices on the boundary
-        interior_vertices (list): list of all interior vertices (all vertices \ boundary_vertices)
+        interior_vertices (list): list of all interior vertices (all vertices \\ boundary_vertices)
 
         __str__: Representation of the object and its elements as a string.
     """
 
     def __init__(self, data : RawMeshData = None):
         Mesh.__init__(self, 2, data)
 
-        if self.is_triangular():
-            self.half_edges = SurfaceMesh._HalfEdgeStructure(self)
-        else:
-            self.half_edges = None
-
         self.connectivity = SurfaceMesh._Connectivity(self)
 
         # Boundary data
         self._boundary_edges : list = None
         self._interior_edges : list = None
 
-        self._is_vertex_on_border : Attribute = None 
+        self._is_vertex_on_border : Attribute = None
         self._boundary_vertices : list = None
         self._interior_vertices : list = None
 
+        self._is_triangular : bool = None
+        self._is_quad : bool = None
+
     def __str__(self):
         out = "mouette.mesh.SurfaceMesh object\n"
         out += "| {} vertices\n".format(len(self.vertices))
         out += "| {} edges\n".format(len(self.edges))
         out += "| {} faces\n".format(len(self.faces))
         return out
 
@@ -97,31 +94,38 @@
             fid (int): face id
 
         Returns:
             iterable: iterator of Vec objects representing point coordinates of vertices
         """
         return (self.vertices[_v] for _v in self.faces[fid])
 
+    def _compute_mesh_type(self):
+        self._is_triangular = True
+        self._is_quad = True
+        for f in self.faces:
+            self._is_triangular = self._is_triangular and len(f)==3
+            self._is_quad = self._is_quad and len(f)==4
+
     def is_triangular(self) -> bool:
         """
         Returns:
             bool: True if the mesh is triangular (all faces are triangles)
         """
-        for f in self.faces:
-            if len(f)!=3: return False
-        return True
+        if self._is_triangular is None:
+            self._compute_mesh_type()
+        return self._is_triangular
 
     def is_quad(self) -> bool:
         """
         Returns:
             bool: True if the mesh is quadrangular (all faces are quad)
         """
-        for f in self.faces:
-            if len(f) != 4: return False
-        return True
+        if self._is_quad is None:
+            self._compute_mesh_type()
+        return self._is_quad
 
     def recompute_edges(self):
         """Recomputes the set of edges according to the set of faces"""
         self.edges.clear()
         edge_set = set()
         for f in self.faces:
             nf = len(f)
@@ -175,17 +179,18 @@
         whether edge (u,v) is a boundary edge or not
 
         Args:
             u (int): vertex id
             v (int): vertex id
 
         Returns:
-            bool: whether edge (u,v) is a boundary edge or not
+            bool: whether edge (u,v) is a boundary edge or not. Returns False if (u,v) is not a valid edge.
         """
-        return self.half_edges.adj(u,v)[0] is None or self.half_edges.adj(v,u)[0] is None
+        if self.connectivity.edge_id(u,v) is None: return False
+        return self.connectivity.direct_face(u,v) is None or self.connectivity.direct_face(v,u) is None
 
     def is_vertex_on_border(self, u:int) -> bool:
         """
         whether vertex `u` is a boundary vertex or not.
 
         Args:
             u (int): vertex id
@@ -217,329 +222,309 @@
     
     @property
     def interior_vertices(self):
         if self._interior_vertices is None:
             self._compute_interior_boundary_vertices()
         return self._interior_vertices
 
-    ###### Half Edges ######
-
-    class _HalfEdgeStructure:
-        def __init__(self, master):
-            self.mesh : SurfaceMesh = master
-            self._half_edges : dict = None
-
-        def clear(self):
-            """
-            Resets connectivity. 
-            The next query in the code will regenerate internal arrays.
-            """
-            self._half_edges : dict = None
-
-        def _compute_half_edges(self):
-            self._half_edges = dict()
-            for i,F in enumerate(self.mesh.faces):
-                n = len(F)
-                for v in range(n):
-                    self._half_edges[ (F[v], F[(v+1)%n] ) ] = (i,v,(v+1)%n)
-
-        def __iter__(self):
-            if self._half_edges is None:
-                self._compute_half_edges()
-            return self._half_edges.__iter__()
-
-        def adj(self, u : int, v : int):
-            """Pair (u,v) of vertex -> triangle to the left of edge (u,v) if edge (u,v) exists, None otherwise
-            Also returns local indexes of u and v in the triangle (and None if (u,v) does not exists)
-            
-            Calling this function with edge (v,u) yield the triangle of the other side of the edge
-            """
-            if self._half_edges is None:
-                self._compute_half_edges()
-            if (u,v) in self._half_edges:
-                return self._half_edges[(u,v)]
-            return None,None,None
-
-        def opposite(self, u : int, v : int, T : int):
-            """Given a pair of vertices (u,v) and a face T, returns the face (and local indexes of u and v) on the other side of edge (u,v)
-
-            if (u,v) are not two vertices of the face T, returns None
-            """
-            T1,u1,v1 = self.adj(u,v)
-            T2,v2,u2 = self.adj(v,u)
-            if T1==T:
-                return T2,u2,v2
-            if T2==T:
-                return T1,u1,v1
-            return None,None,None
-
-        def edge_to_triangles(self, u, v):
-            return self.adj(u,v)[0], self.adj(v,u)[0]
-
-        def common_edge(self,iF1,iF2):
-            F1 = self.mesh.faces[iF1]
-            n = len(F1)
-            for i in range(n):
-                A,B = F1[i], F1[(i+1)%n]
-                if self.opposite(A,B,iF1)[0]==iF2:
-                    return utils.keyify(A,B)
-            return None,None
-
-        def next_around(self, v : int, u: int):
-            """ 
-            Turning clockwise in the neighbourhood of vertex v, finds the vertex after u.
-            Returns None is such a vertex does not exist (reach boundary)
-            """
-            T, iV, iU = self.adj(v,u)
-            if T is None: return None
-            return self.mesh.ith_vertex_of_face(T, 3-iV-iU)
-
-        def prev_around(self, v, u):
-            """ 
-            Turning counter clockwise in the neighbourhood of vertex v, finds the vertex after u.
-            Returns None is such a vertex does not exist (reach boundary)
-            """
-            T, iU, iV = self.adj(u,v)
-            if T is None: return None
-            return self.mesh.ith_vertex_of_face(T, 3-iV-iU)
-
-    ###### connectivity ######
+    ###### Connectivity ######
 
     class _Connectivity(PolyLine._Connectivity):
 
         def __init__(self, master):
             super().__init__(master)
 
-            self._adjV2F : dict = dict() # vertex -> triangle
-            # V2F is not None because connectivity is built on the fly at each query
-            
-            self._adjF2F : dict = None # triangle -> triangle
-            self._adjVF2Cn : dict = None # vertex,face -> corner
-            self._adjCn2F : dict = None # corner -> face
-            self._adjF2Cn : dict = None # face -> first corner
-
-            self._face_id : dict = None
+            self._half_edges : dict = None # (v1,v2) -> (corner, previous, next, opposite, face, i1, i2)
+            self._Cn2he      : dict = None # corner -> (v1,v2)
+            self._adjVF2Cn   : dict = None # vertex,face -> corner
+            self._adjV2Cn    : dict = None # vertex -> corners
+            self._adjF2Cn    : dict = None # face -> corners
+            self._face_id    : dict = None # (list of vertices) -> face
         
         def clear(self):
             """
             Resets connectivity. 
             The next query in the code will regenerate internal arrays.
             """
             super().clear()
-            self._adjV2F : dict = dict() # vertex -> triangle            
-            self._adjF2F : dict = None # triangle -> triangle
-            self._adjVF2Cn : dict = None # vertex,face -> corner
-            self._adjCn2F : dict = None # corner -> face
-            self._adjF2Cn : dict = None # face -> first corner
-            self._face_id : dict = None     
+            self._half_edges : dict = None # (v1,v2) -> (corner, previous, next, opposite, face, i1, i2)
+            self._Cn2he      : dict = None # corner -> (v1,v2)
+            self._adjVF2Cn   : dict = None # vertex,face -> corner
+            self._adjV2Cn    : dict = None # vertex -> corners
+            self._adjF2Cn    : dict = None # face -> first corner
+            self._face_id    : dict = None # (list of vertices) -> face
+
+        def _compute_face_ids(self):
+            self._face_id = dict()
+            for iF, F in enumerate(self.mesh.faces):
+                self._face_id[utils.keyify(F)] = iF
 
-        def face_id(self, a, b, c):
+        def face_id(self, *args) -> int:
+            """ The id of a face
+            Args:
+                int*: integers representing indices of vertices of the face (not necessarily in the correct order)
+
+            Returns:
+                int: A face index or None if the given tuple is invalid
+            """
             if self._face_id is None:
-                self._compute_vertex_adj()
-            key = utils.keyify(a,b,c)
+                self._compute_face_ids()
+            key = utils.keyify(*args)
             return self._face_id.get(key, None)
 
-        def _compute_vertex_adj(self):
-            super()._compute_vertex_adj()
-
-            self._adjV2F = dict([(i,set()) for i in self.mesh.id_vertices])
-            self._face_id = dict()
+        def _compute_connectivity(self):
+            super()._compute_connectivity()
 
+            ### Compute corner connectivity dictionnaries
+            self._adjV2Cn = dict([(i,set()) for i in self.mesh.id_vertices])
+            self._adjVF2Cn = dict()
+            self._adjF2Cn = dict()
+            for iC in self.mesh.id_corners:
+                v,f = self.mesh.face_corners.element(iC), self.mesh.face_corners.adj(iC)
+                self._adjV2Cn[v].add(iC)
+                self._adjVF2Cn[(v,f)] = iC
+                if f not in self._adjF2Cn:
+                    self._adjF2Cn[f] = iC
+            for v in self.mesh.id_vertices:
+                # recast sets as list for indexing and sorting
+                self._adjV2Cn[v] = list(self._adjV2Cn[v])
+                
+            ### Compute half edges
+            self._half_edges = dict()
+            self._Cn2he = dict()
             for iF,F in enumerate(self.mesh.faces):
-                key = utils.keyify(F)
-                self._face_id[key] = iF
-                for V in F:
-                    self._adjV2F[V].add(iF)
+                n = len(F)
+                for iV in range(n):
+                    P, Pprev, Pnext = F[iV], F[(iV-1)%n], F[(iV+1)%n]
+                    iC, iCprev, iCnext = (self._adjVF2Cn[(p,iF)] for p in (P,Pprev,Pnext)) 
+                    self._half_edges[ (P, Pnext) ] = [iC, iCprev, iCnext, None, iF, iV, (iV+1)%n]
+                    self._Cn2he[iC] = (P,Pnext)
+            for (A,B) in self._half_edges.keys():
+                iC1 = self._half_edges.get((A,B), [None])[0] # index of corner if it exists, else None 
+                iC2 = self._half_edges.get((B,A), [None])[0]
+                if iC1 is not None and iC2 is not None:
+                    # iC1 and iC2 are opposite corners
+                    self._half_edges[(A,B)][3] = iC2
+                    self._half_edges[(B,A)][3] = iC1
 
-            for U in self.mesh.id_vertices:
-                self._adjV2F[U] = list(self._adjV2F[U])
-            
-            # Neighborhood should be sorted to have a clockwise order
+            ### Sorting vertex neighborhoods
             if config.sort_neighborhoods and isinstance(self.mesh, SurfaceMesh):
+                # Neighborhood should be sorted to have a clockwise order
+                # Ignore sorting for volume meshes
                 self._sort_vertex_neighborhoods()
-
+            
         def _sort_vertex_neighborhoods(self):
-            for A in self.mesh.interior_vertices:
-                if not self._adjV2V[A] : continue # no adjacent vertices to sort
-                indexV, indexF = dict(), dict()
-                B = self._adjV2V[A][0]
-                T = self.mesh.half_edges.adj(A,B)[0]
-                indexV[B] = 0
-                indexF[T] = 0
-                for i in range(len(self._adjV2V[A])):
-                    B = self.mesh.half_edges.next_around(A,B) # B before T since root triangle is handled outside of the loop
-                    T = self.mesh.half_edges.adj(A,B)[0]
-                    indexV[B] = i+1
-                    indexF[T] = i+1
-
-                self._adjV2V[A].sort(key = lambda u : indexV[u])
-                self._adjV2F[A].sort(key = lambda u : indexF[u])
-
-            for A in self.mesh.boundary_vertices:
-                if not self._adjV2V[A] : continue # not adjacent vertices to sort
-                indexV,indexF = dict(), dict()
-                B = self._adjV2V[A][0]
+            for A in self.mesh.id_vertices:
+                corners_A = self._adjV2Cn[A]
+                if len(corners_A)==0: continue
+                sort_index = dict([(c,0) for c in corners_A])
                 ind = 0
-                indexV[B] = ind
-                while self.mesh.half_edges.adj(B,A)[0] is not None:
-                    T = self.mesh.half_edges.adj(B,A)[0] # T before B because root triangle is not handled outside of the loop
-                    B = self.mesh.half_edges.prev_around(A,B)
-                    ind-=1
-                    indexV[B] = ind
-                    indexF[T] = ind
-                # reset and go the other way around
-                B = self._adjV2V[A][0]
-                ind = 0
-                while self.mesh.half_edges.adj(A,B)[0] is not None:
-                    T = self.mesh.half_edges.adj(A,B)[0] # T before B because root triangle is not handled outside of the loop
-                    B = self.mesh.half_edges.next_around(A,B)
-                    ind +=1
-                    indexV[B] = ind
-                    indexF[T] = ind
-                    
-                self._adjV2V[A].sort(key = lambda u : indexV[u])
-                self._adjV2F[A].sort(key = lambda u : indexF[u]) 
-        
-        def _compute_face_adj(self):
-            self._adjF2F = dict([(t, []) for t in self.mesh.id_faces])
-            for (A,B) in self.mesh.edges:
-                F1, _, _ = self.mesh.half_edges.adj(A,B)
-                F2, _, _ = self.mesh.half_edges.adj(B,A)
-                if F1 is not None and F2 is not None:
-                    self._adjF2F[F1].append(F2)
-                    self._adjF2F[F2].append(F1)
+                is_boundary = False
+                Cn = corners_A[0]
+                for _ in range(len(sort_index)):
+                    sort_index[Cn] = ind 
+                    ind -= 1 
+                    Cn = self.opposite_corner(self.previous_corner(Cn))
+                    if Cn is None: 
+                        is_boundary = True
+                        break
+                if is_boundary:
+                    # also go counter clockwise 
+                    ind = 0
+                    Cn = corners_A[0]
+                    for _ in range(len(sort_index)):
+                        sort_index[Cn] = ind 
+                        ind +=1
+                        Cn = self.opposite_corner(Cn)
+                        if Cn is None : break
+                        Cn = self.next_corner(Cn)
+                self._adjV2Cn[A].sort(key = lambda c : sort_index[c])
+                sort_indexV = dict()
+                for v in self._adjV2V[A]:
+                    # all vertices have an associated corner except the last one (opposite half edge does not exist on boundary)
+                    sort_indexV[v] = sort_index.get(self.half_edge_to_corner(A,v), -float("inf"))
+                self._adjV2V[A].sort(key = lambda v : sort_indexV[v])
 
-        def _compute_corner_adj(self):
-            self._adjVF2Cn = dict()
-            self._adjCn2F = dict()
-            self._adjF2Cn = dict()
-            c = 0
-            for iF,F in enumerate(self.mesh.faces):
-                self._adjF2Cn[iF] = c
-                for v in F:
-                    assert self.mesh.face_corners[c] == v
-                    self._adjVF2Cn[(v,iF)] = c
-                    self._adjCn2F[c] = iF
-                    c += 1
+        ##### Vertices to elements
 
-        ##### Vertex to Faces #####
-
-        def vertex_to_face(self, V:int) -> list:
+        def vertex_to_faces(self, V: int) -> list:
             """
             Neighborhood of vertex `V` in terms of faces.
 
             Args:
                 V (int): vertex id
 
             Returns:
                 list: list of faces `F` such that `V` is a vertex of `F`.
             """
-            L = self._adjV2F.get(V, None)
-            if L is None :
-                self._compute_vertex_adj()
-            return self._adjV2F[V]
-        
-        def n_VtoF(self, V:int) -> int:
-            """
-            Size of the face neighborhood of vertex `V`
-
-            Args:
-                V (int): vertex id
-
-            Returns:
-                int: `len(vertex_to_face(V))`
-            """
-            L = self._adjV2F.get(V, None)
-            if L is None:
-                self._adjV2F[V] = []
-                for iT,T in enumerate(self.mesh.faces):
-                    if V in T:
-                        self._adjV2F[V].append(iT)
-            return len(self._adjV2F[V])
-
-        ##### Corners #####
+            return [self.corner_to_face(iC) for iC in self.vertex_to_corners(V)]
 
-        def vertex_to_corner(self, V:int) -> list:
+        def vertex_to_corners(self, V: int) -> list:
             """
             List of face corners that correspond to vertex `V`
 
             Args:
                 V (int): vertex id
 
             Returns:
                 list: the list of corners `C` such that `mesh.corners[C]==V`
             """
-            L = self._adjV2F.get(V, None)
-            if L is None:
-                self._adjV2F[V] = []
-                for iT,T in enumerate(self.mesh.faces):
-                    if V in T:
-                        self._adjV2F[V].append(iT)
-            return [self.vertex_to_corner_in_face(V,_f) for _f in self.vertex_to_face(V)]
-
-        def vertex_to_corner_in_face(self, V:int, F:int) -> int:
+            if self._adjV2Cn is None :
+                self._compute_connectivity()
+            return self._adjV2Cn.get(V, None)
+        
+        def vertex_to_corner_in_face(self, V: int, F: int) -> int:
             """
             The corner `C` corresponding to vertex `V` in face `F`.
 
             Args:
                 V (int): vertex id
                 F (int): face id
 
             Returns:
                 int: corner id, or `None` if `V` is not a vertex of `F`.
             """
             if self._adjVF2Cn is None:
-                self._compute_corner_adj()
+                self._compute_connectivity()
             return self._adjVF2Cn.get((V,F), None)
+        
+        #### Corner to element
+        
+        def previous_corner(self, C: int) -> int:
+            """Previous corner of `C` around its associated face
+
+            Args:
+                C (int): corner index
+
+            Returns:
+                int: index of the previous corner
+            """
+            if self._half_edges is None:
+                self._compute_connectivity()
+            key = self._Cn2he.get(C,None)
+            if key is None: return None
+            return self._half_edges[key][1]
+
+        def next_corner(self, C:int) -> int:
+            """Next corner of `C` around its associated face
+
+            Args:
+                C (int): corner index
+
+            Returns:
+                int: index of the next corner
+            """
+            if self._half_edges is None:
+                self._compute_connectivity()
+            key = self._Cn2he.get(C,None)
+            if key is None: return None
+            return self._half_edges[key][2]
+
+        def opposite_corner(self, C: int) -> int:
+            """Opposite corner of `C` in terms of half edges. 
+            If `C.vertex = A` and `C.next.vertex = B`, then returns the corner D such that `D.vertex = B` and `D.vertex.next = A`
+
+            Args:
+                C (int): corner index
+
+            Returns:
+                int: index of the opposite corner
+            """
+            if self._half_edges is None:
+                self._compute_connectivity()
+            key = self._Cn2he.get(C,None)
+            if key is None: return None
+            return self._half_edges[key][3]
+
+        def corner_to_half_edge(self, C: int) -> int:
+            if self._Cn2he is None:
+                self._compute_connectivity()
+            return self._Cn2he.get(C,None)
 
-        def corner_to_face(self,C:int)->int:
+        def corner_to_face(self, C: int) -> int:
             """
             The face inside which corner `C` belongs.
 
             Args:
                 C (int): corner id
 
             Returns:
-                int: face id or `None` if `C` is not a valid corner
+                int: face id
             """
-            if self._adjCn2F is None:
-                self._compute_corner_adj()
-            return self._adjCn2F.get(C,None)
+            return self.mesh.face_corners.adj(C)
         
-        def face_to_first_corner(self,F:int)->int:
-            """
-            One corner `C` of the face `F` (the first in order of appearance in the `face_corners` container)
+        #### Edge to element
+        
+        def half_edge_to_corner(self, u: int, v: int) -> int:
+            return self._half_edges.get((u,v), [None])[0]
+
+        def direct_face(self, u: int, v: int, return_inds: bool = False):
+            """Pair (u,v) of vertex -> triangle to the left of edge (u,v) if edge (u,v) exists, None otherwise
+            Also returns local indexes of u and v in the triangle (and None if (u,v) does not exists)
+            
+            Calling this function with edge (v,u) yield the triangle of the other side of the edge
 
             Args:
-                F (int): face id
+                u (int): first vertex index
+                v (int): second vertex index
+                return_inds (bool, optional): Whether to return local indices of u and v in the face. Defaults to False.
 
             Returns:
-                int: corner id
+                int | None | tuple[int,int,int] | tuple[None,None,None]: index of a face or None. If return_inds is True, tuple made of index of face and local indices of u and v in face. 
             """
-            if self._adjF2Cn is None:
-                self._compute_corner_adj()
-            return self._adjF2Cn[F]
+            if self._half_edges is None:
+                self._compute_connectivity()
+            if (u,v) in self._half_edges:
+                if return_inds: return self._half_edges[(u,v)][4:]
+                return self._half_edges[(u,v)][4]
+            else:
+                if return_inds: return None,None,None
+                return None
+
+        def edge_to_faces(self, u: int, v: int):
+            return self.direct_face(u,v), self.direct_face(v,u)
 
-        def face_to_corners(self,F:int)->list:
+        def opposite_face(self, u : int, v : int, T : int, return_inds: bool = False):
+            """Given a pair of vertices (u,v) and a face T, returns the face (and local indexes of u and v) on the other side of edge (u,v)
+
+            if (u,v) are not two vertices of the face T, returns None
             """
-            list of corners of face `F`
+            if return_inds:
+                T1, u1, v1 = self.direct_face(u,v, True)
+                T2, v2, u2 = self.direct_face(v,u, True)
+                if T1==T: return T2,u2,v2
+                if T2==T: return T1,u1,v1
+                return None,None,None
+            else:
+                T1, T2 = self.direct_face(u,v), self.direct_face(v,u)
+                if T==T1: return T2
+                if T==T2: return T1
+                return None
+
+        def common_edge(self, iF1: int, iF2: int):
+            """Returns the two vertices (u,v) of the edge that separates faces iF1 and iF2 if it exists, and (None,None) otherwise.
 
             Args:
-                F (int): face id
+                iF1 (int): first face index
+                iF2 (int): second face index
 
             Returns:
-                list: list of corners of face `F`
+                (u,v) pair of vertex indices, or (None,None)
             """
-            if self._adjF2Cn is None:
-                self._compute_corner_adj()
-            return [self._adjF2Cn[F] + _i for _i in range(len(self.mesh.faces[F]))]
+            F1 = self.mesh.faces[iF1]
+            n = len(F1)
+            for i in range(n):
+                A,B = F1[i], F1[(i+1)%n]
+                if self.opposite_face(A,B,iF1)==iF2:
+                    return utils.keyify(A,B)
+            return None,None
 
-        ##### Faces to Vertex #####
+        ##### Face to element
 
-        def face_to_vertex(self, F:int) -> list:
+        def face_to_vertices(self, F:int) -> list:
             """
             Neighborhood of face `F` in terms of vertices.
 
             Note:
                 Equivalent to `mesh.faces[F]`
 
             Args:
@@ -560,38 +545,63 @@
             Returns:
                 int
             """
             for (i,v) in enumerate(self.mesh.faces[F]):
                 if v==V: return i
             return None
         
-        ##### Face to Edge ######
-
-        def face_to_edge(self, F:int) -> list:
+        def face_to_edges(self, F:int) -> list:
             """
             List of edges that bound face `F`.
 
             Args:
                 F (int): face id
 
             Returns:
                 list: list of edges `E` such that `E` is a boundary edge of face `F`
             """
             lF = self.mesh.faces[F]
             n = len(lF)
             return [self.edge_id(lF[i],lF[(i+1)%n]) for i in range(n)]
 
-        ###### Face to face ######
+        def face_to_first_corner(self, F: int) -> int:
+            """
+            One corner `C` of the face `F` (the first in order of appearance in the `face_corners` container)
+
+            Args:
+                F (int): face id
 
-        def face_to_face(self, F:int) -> list:
+            Returns:
+                int: corner id
             """
-            Neighborhood of face `F` in terms of vertices.
+            if self._adjF2Cn is None:
+                self._compute_connectivity()
+            return self._adjF2Cn[F]
+
+        def face_to_corners(self, F: int) -> list:
+            """
+            list of corners of face `F`
+
+            Args:
+                F (int): face id
+
+            Returns:
+                list: list of corners of face `F`
+            """
+            if self._adjF2Cn is None:
+                self._compute_connectivity()
+            return [self._adjF2Cn[F] + _i for _i in range(len(self.mesh.faces[F]))]
+
+        def face_to_faces(self, F:int) -> list:
+            """
+            List of faces that are adjacent to face `F
 
             Args:
                 F (int): face id
 
             Returns:
                 list: list of faces `G` that are adjacent to `F`
             """
-            if self._adjF2F is None:
-                self._compute_face_adj()
-            return self._adjF2F[F]
+            if self._adjF2Cn is None:
+                self._compute_connectivity()
+            opposites = [self.opposite_corner(C) for C in self.face_to_corners(F)]
+            return [self.corner_to_face(Op) for Op in opposites if Op is not None]
```

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/type_checks.py` & `mouette-1.2.0/mouette/mesh/datatypes/type_checks.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/datatypes/volume.py` & `mouette-1.2.0/mouette/mesh/datatypes/volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..mesh_data import RawMeshData
 from ..mesh_attributes import Attribute
 from .base import Mesh
-from .surface import SurfaceMesh
+from .surface import PolyLine, SurfaceMesh
 from ...utils import keyify
 from ...geometry.geometry import det_3x3
 from ... import config
 
 import numpy as np
 
 class VolumeMesh(Mesh):
@@ -38,38 +38,45 @@
         out += "| {} faces\n".format(len(self.faces))
         out += "| {} cells\n".format(len(self.cells))
         return out
 
     @property
     def id_vertices(self):
         """
-        Shortcut for range(len(self.vertices))
+        Shortcut for `range(len(self.vertices))`
         """
         return range(len(self.vertices))
 
     @property
     def id_edges(self):
         """
-        Shortcut for range(len(self.edges))
+        Shortcut for `range(len(self.edges))`
         """
         return range(len(self.edges))
 
     @property
     def id_faces(self):
         """
-        Shortcut for range(len(self.faces))
+        Shortcut for `range(len(self.faces))`
         """
         return range(len(self.faces))
 
     @property
     def id_cells(self):
         """
-        Shortcut for range(len(self.cells))
+        Shortcut for `range(len(self.cells))`
         """
         return range(len(self.cells))
+    
+    @property
+    def id_corners(self):
+        """
+        Shortcut for `range(len(self.face_corners))`
+        """
+        return range(len(self.face_corners))
 
     @property
     def boundary_mesh(self):
         return self.boundary_connectivity.mesh
 
     def _compute_interior_boundary_faces(self):
         self._interior_faces = []
@@ -105,27 +112,36 @@
         for e in self.id_edges:
             if self._is_edge_on_border[e]:
                 self._boundary_edges.append(e)
             else:
                 self._interior_edges.append(e)
 
     def is_face_on_border(self, *args) -> bool:
+        """Simple test to determine if a given face is on the boundary of the mesh.
+        
+        Parameters:
+            Either an integer index representing a face, or n integer indices representing the vertices
+            
+        Returns:
+            bool: Returns True is the given face exists and is on the boundary of the mesh
+        """
         if len(args)==1:
-            n = self.connectivity.n_F2C(args[0])
+            n = len(self.connectivity.face_to_cells(args[0]))
         else:
-            n = self.connectivity.n_F2C(self.connectivity.face_id(*args))
+            n = len(self.connectivity.face_to_cells(self.connectivity.face_id(*args)))
         return n<2
     
     def is_vertex_on_border(self, V) -> bool:
         if self._is_vertex_on_border is None:
             self._compute_interior_boundary_vertices()
         return self._is_vertex_on_border[V]
     
     def is_edge_on_border(self, *args) -> bool:
-        """
+        """Simple test to determine if a given edge is on the boundary of the mesh.
+
         Parameters:
             Either an integer index representing an edge, or two integer indices representing two (adjacent) vertices
 
         Returns:
             bool: Returns True if the given edge is on the boundary of the mesh.
         """
         if self._is_edge_on_border is None:
@@ -205,16 +221,16 @@
             self._adjC2F : dict = None
             self._adjF2C : dict = None
 
             self._adjE2F : dict = None
             self._adjE2C : dict = None
             self._adjC2E : dict = None
 
-        def _compute_vertex_adj(self):
-            super()._compute_vertex_adj()
+        def _compute_connectivity(self):
+            super()._compute_connectivity()
             
             self._adjV2C = dict([(i,set()) for i in self.mesh.id_vertices ])
             for iC,C in enumerate(self.mesh.cells):
                 for V in C:
                     self._adjV2C[V].add(iC)
 
             for U in self.mesh.id_vertices:
@@ -244,15 +260,15 @@
             else:
                 self._adjC2C = self.mesh.cell_faces.create_attribute("adjacent_cell", int, 1, default_value= config.NOT_AN_ID)
                 for iC, cell in enumerate(self.mesh.cells):
                     v0,v1,v2,v3 = cell
                     # face fi does not contain vertex vi
                     f0,f1,f2,f3 = self.face_id(v1,v3,v2), self.face_id(v0,v2,v3), self.face_id(v3,v1,v0), self.face_id(v0,v1,v2)
                     for iF, F in enumerate((f0,f1,f2,f3)):
-                        for iC2 in self.face_to_cell(F):
+                        for iC2 in self.face_to_cells(F):
                             if iC2 != iC: self._adjC2C[(iC,iF)] = iC2
                             
 
         def _compute_cell_adj(self):
             self._adjC2F = dict([(i,[]) for i in self.mesh.id_cells ])
             self._adjF2C = dict([(i,[]) for i in self.mesh.id_faces ])
 
@@ -273,22 +289,22 @@
                                 self._adjC2F[iC].add(iF)
                                 self._adjF2C[iF].append(iC)
             for iC in self.mesh.id_cells:
                 self._adjC2F[iC] = list(self._adjC2F[iC])
             for iF in self.mesh.id_faces:
                 self._adjF2C[iF] = list(self._adjF2C[iF])
 
-        def _compute_edge_adj(self):
-            super()._compute_edge_adj() # for edge_id computation
+        def _compute_edge_id(self):
+            super()._compute_edge_id() # for edge_id computation
             self._adjE2F = dict([(e, []) for e in self.mesh.id_edges])
             self._adjE2C = dict([(e, set()) for e in self.mesh.id_edges])
 
             for f in self.mesh.id_faces:
-                c = set(self.face_to_cell(f))
-                for e in self.face_to_edge(f):
+                c = set(self.face_to_cells(f))
+                for e in self.face_to_edges(f):
                     self._adjE2F[e].append(f)
                     self._adjE2C[e] |= c
             for e in self.mesh.id_edges:
                 self._adjE2C[e] = list(self._adjE2C[e])
             
             if config.sort_neighborhoods:
                 self._sort_edge_neighborhoods()
@@ -332,17 +348,17 @@
                     p2 = [x for x in self.mesh.cells[iC] if x not in (A,B,p2)][0]
                 self._adjE2C[e].sort(key= lambda c : keys_cell[c])
                 self._adjE2F[e].sort(key= lambda f : keys_face[f])
 
         ##### Faces - Cells #####
 
         def n_F2C(self, F):
-            return len(self.face_to_cell(F))
+            return len(self.face_to_cells(F))
 
-        def face_to_cell(self, iF):
+        def face_to_cells(self, iF):
             if self._adjF2C is None:
                 self._compute_cell_adj()
             return self._adjF2C[iF]
 
         def cell_to_face(self, iC):
             if self._adjC2F is None:
                 self._compute_cell_adj()
@@ -352,29 +368,29 @@
 
         def cell_to_cell(self, iC):
             if self._adjC2C is None:
                 self._compute_adjacent_cell()
             return [ self._adjC2C[(iC,i)] for i in range(len(self.mesh.cells[iC])) if self._adjC2C[(iC,i)] != config.NOT_AN_ID]
 
         def other_face_side(self, C, F):
-            if len(self.face_to_cell(F)) != 2 : return None
-            C1,C2 = self.face_to_cell(F)
+            if len(self.face_to_cells(F)) != 2 : return None
+            C1,C2 = self.face_to_cells(F)
             if C==C1: return C2
             if C==C2 : return C1
             return None
         
         def common_face(self, C1, C2):
             common_vert = set(self.mesh.cells[C1]).intersection(self.mesh.cells[C2])
             if len(common_vert) != 3: return None
             return self.face_id(*common_vert)
 
         ##### Vertex - Cell #####
         def vertex_to_cell(self, V):
             if self._adjV2C is None:
-                self._compute_vertex_adj()
+                self._compute_connectivity()
             return self._adjV2C[V]
         
         def cell_to_vertex(self, C):
             return self.mesh.cells[C]
         
         def in_cell_index(self, C, V):
             """Index of vertex V in cell C. None if V is not in cell C
@@ -401,15 +417,15 @@
         ##### Edge - face #####
 
         # face_to_edge already defined in parent class SurfaceMesh.connectivity
         # edge_to_face is not since SurfaceMesh takes advantage of the half edge structure
         
         def edge_to_face(self, e):
             if self._adjE2F is None:
-                self._compute_edge_adj()
+                self._compute_edge_id()
             return self._adjE2F[e]
 
         ##### Edge - Cells #####
 
         def cell_to_edge(self, c):
             if self._adjC2E is None:
                 self._adjC2E = dict()
@@ -423,15 +439,15 @@
                         e = self.edge_id(A,B)
                         if e is not None:
                             self._adjC2E[c].append(e)
             return self._adjC2E[c]
 
         def edge_to_cell(self,e):
             if self._adjE2C is None:
-                self._compute_edge_adj()
+                self._compute_edge_id()
             return self._adjE2C[e]
 
     class _BoundaryConnectivity(SurfaceMesh._Connectivity):
 
         def __init__(self, master):
             self.complete_mesh = master
 
@@ -474,63 +490,49 @@
             for i,v in enumerate(vertex_set):
                 boundary.vertices.append(self.complete_mesh.vertices[v])
                 self.m2b_vertex[v] = i
                 self.b2m_vertex[i] = v
 
             # generate set of faces and check for orientation
             for iF in bnd_faces:
-                iC = self.complete_mesh.connectivity.face_to_cell(iF)[0]
+                iC = self.complete_mesh.connectivity.face_to_cells(iF)[0]
                 pA,pB,pC = (self.complete_mesh.vertices[_x] for _x in self.complete_mesh.faces[iF])
                 bA,bB,bC = (self.m2b_vertex[v] for v in self.complete_mesh.faces[iF])
                 D = [x for x in self.complete_mesh.cells[iC] if x not in self.complete_mesh.faces[iF]][0] # fourth point in cell but not on face
                 pD = self.complete_mesh.vertices[D]
                 if det_3x3(pA-pD,pB-pD,pC-pD)>0:
                     boundary.faces.append((bA,bB,bC))
                 else:
                     boundary.faces.append((bA,bC,bB))
             return SurfaceMesh(boundary)
         
-        ##### Vertex to Vertex #####
+        ##### Vertex to elements #####
 
-        def vertex_to_vertex(self, V : int):
+        def vertex_to_vertices(self, V : int):
             Vb = self.m2b_vertex.get(V,None)
             if Vb is None: return []
-            return [self.b2m_vertex[_v] for _v in super().vertex_to_vertex(Vb)]
+            return [self.b2m_vertex[_v] for _v in super().vertex_to_vertices(Vb)]
         
-        def n_VtoV(self, V : int):
-            Vb = self.m2b_vertex.get(V,None)
-            if Vb is None: return 0
-            return super().n_VtoV(Vb)
-
-        ##### Vertex to Edges #####
-
-        def vertex_to_edge(self, V : int) :
+        def vertex_to_edges(self, V : int) :
             Vb = self.m2b_vertex.get(V,None)
             if Vb is None: return []
-            edges = [self.edge_id(Vb,Wb) for Wb in super().vertex_to_vertex(Vb)]
+            edges = [self.edge_id(Vb,Wb) for Wb in super().vertex_to_vertices(Vb)]
             return [self.b2m_edge[e] for e in edges]
 
-        ##### Vertex to faces #####
-
-        def n_VtoF(self, V):
-            Vb = self.m2b_vertex.get(V, None)
-            if Vb is None: return 0
-            return super().n_VtoF(Vb)
-
-        def vertex_to_face(self, V):
+        def vertex_to_faces(self, V):
             Vb = self.m2b_vertex.get(V,None)
             if Vb is None: return
-            return [self.b2m_face[f] for f in super().vertex_to_face(Vb)]
+            return [self.b2m_face[f] for f in super().vertex_to_faces(Vb)]
 
         def vertex_to_face_quad(self, V):
             raise NotImplementedError
             
-        ##### faces to Vertex #####
+        ##### Faces to elements #####
 
-        def face_to_vertex(self, F):
+        def face_to_vertices(self, F):
             Fb = self.m2b_face.get(F,None)
             if Fb is None : return []
             return list(self.mesh.faces[Fb])
 
         def in_face_index(self, F, V):
             """Index of vertex V in face F. None if V is not in face F
 
@@ -541,20 +543,16 @@
             Returns:
                 int
             """
             Fb,Vb = self.m2b_face.get(F,None), self.m2b_vertex.get(V,None)
             if Fb is None or Vb is None : return None
             return super().in_face_index(Fb,Vb)
         
-        ##### face to Edge ######
-
-        def face_to_edge(self, F):
+        def face_to_edges(self, F):
             Fb = self.m2b_face.get(F,None)
             if Fb is None: return []
-            return  [self.b2m_edge[_e] for _e in super().face_to_edge(Fb)]
-
-        ###### face to face ######
+            return  [self.b2m_edge[_e] for _e in super().face_to_edges(Fb)]
 
-        def face_to_face(self, F):
+        def face_to_faces(self, F):
             Fb = self.m2b_face.get(F,None)
             if Fb is None: return []
-            return [self.b2m_face[_f] for _f in super().face_to_face(Fb)]
+            return [self.b2m_face[_f] for _f in super().face_to_faces(Fb)]
```

### Comparing `mouette-1.1.7/mouette/mesh/io/geogram_ascii.py` & `mouette-1.2.0/mouette/mesh/io/geogram_ascii.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,35 +175,34 @@
         elif chk.container == Chunk.Container.FACE_CORNERS and chk.name == "\"GEO::Mesh::facet_corners::corner_vertex\"":
             assert chk.n_data==1
             for i in range(container_sizes[Chunk.Container.FACES]):
                 ncf = n_corner_in_facet[i]
                 ptr = facet_ptr[i]
                 face = [chk.data[ptr+_i] for _i in range(ncf)]
                 outmesh.faces.append(face)
-                outmesh.face_corners += face
+                outmesh.face_corners += [(x,i) for x in face]
 
         elif chk.container == Chunk.Container.FACE_CORNERS and chk.name == "\"GEO::Mesh::facet_corners::corner_adjacent_facet\"":
             assert chk.n_data==1
-            #chk.name = "corner_adjacent_face"
-            adj_vert = outmesh.face_corners.create_attribute("corner_adjacent_facet", int, default_value=NOT_AN_ID)
-            import_attribute(chk, adj_vert)
+            adj_corner = outmesh.face_corners.create_attribute("opposite_face", int, default_value=NOT_AN_ID)
+            import_attribute(chk, adj_corner)
 
         elif chk.container == Chunk.Container.CELL_CORNERS and chk.name == "\"GEO::Mesh::cell_corners::corner_vertex\"":
             assert chk.n_data==1
             for i in range(container_sizes[Chunk.Container.CELLS]):
                 ncc = n_corner_in_cell[i]
                 ptr = cell_ptr[i]
                 cell = [chk.data[ptr+_i] for _i in range(ncc)]
                 outmesh.cells.append(cell)
-                outmesh.cell_corners += cell
+                outmesh.cell_corners += [(x,i) for x in cell]
 
         elif chk.container == Chunk.Container.CELL_FACETS and chk.name == "\"GEO::Mesh::cell_facets::adjacent_cell\"":
             assert chk.n_data==1
             # chk.name = "adjacent_cell"
-            adj_cell = outmesh.cell_faces.create_attribute("adjacent_cell", int, default_value=NOT_AN_ID)
+            adj_cell = outmesh.cell_faces.create_attribute("opposite_cell", int, default_value=NOT_AN_ID)
             adj_cell._expand(container_sizes[Chunk.Container.CELL_FACETS])
             import_attribute(chk, adj_cell)
 
         else: # user defined attribute
             container = {
                 Chunk.Container.VERTICES : outmesh.vertices,
                 Chunk.Container.EDGES : outmesh.edges,
```

### Comparing `mouette-1.1.7/mouette/mesh/io/io.py` & `mouette-1.2.0/mouette/mesh/io/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from .geogram_ascii import import_geogram_ascii, export_geogram_ascii
 from .obj import import_obj, export_obj
 from .medit import import_medit, export_medit
 from .off import import_off, export_off
 from .xyz import import_xyz, export_xyz
 from .tet import import_tet, export_tet
 from .stl import import_stl, export_stl
+from .ply import import_ply, export_ply
 
 def read_by_extension(filename : str):
     ext = get_extension(filename)
     import_fun = {
         "geogram_ascii" : import_geogram_ascii,
         "obj" : import_obj,
         "mesh" : import_medit,
         "off" : import_off,
         "xyz" : import_xyz,
         "tet" : import_tet,
         "stl" : import_stl,
+        "ply" : import_ply
     }.get(ext.lower(), None)
     if import_fun is None:
         raise Exception("Unsupported file extension '{}'".format(ext))
     data = import_fun(filename)
     return data
 
 def write_by_extension(mesh : "RawMeshData", filename : str):
@@ -29,11 +31,12 @@
         "geogram_ascii" : export_geogram_ascii,
         "obj" : export_obj,
         "mesh" : export_medit,
         "off" : export_off,
         "xyz" : export_xyz,
         "tet" : export_tet,
         "stl" : export_stl,
+        "ply" : export_ply
     }.get(ext.lower(), None)
     if export_fun is None:
         raise Exception("Unsupported file extension '{}'".format(ext))
     export_fun(mesh, filename)
```

### Comparing `mouette-1.1.7/mouette/mesh/io/medit.py` & `mouette-1.2.0/mouette/mesh/io/medit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from ..datatypes import *
 from ..mesh_data import RawMeshData
 from collections import deque
 
-def parse_field(data : deque, container, nlines, nelem, corner_container=None):
+def parse_field(data : deque, container, nlines, nelem):
     for _ in range(nlines):
         line = data.popleft().split()
         d = [int(u.strip())-1 for u in line][:nelem]
         container.append(d)
-        if corner_container is not None:
-            corner_container += d
 
 def import_medit(path):
     obj = RawMeshData()
     data = deque()
     with open(path, 'r' ) as meditf:
         data = deque([x.strip() for x in meditf.readlines()])
                 
@@ -30,27 +28,27 @@
 
         elif line=="Edges":
             ne = int(data.popleft())
             parse_field(data, obj.edges, ne, 2)
 
         elif line=="Triangles":
             nt = int(data.popleft())
-            parse_field(data, obj.faces, nt, 3, obj.face_corners)
+            parse_field(data, obj.faces, nt, 3)
 
         elif line=="Quadrilaterals":
             nq = int(data.popleft())
-            parse_field(data, obj.faces,  nq, 4, obj.face_corners)
+            parse_field(data, obj.faces,  nq, 4)
 
         elif line=="Tetrahedra":
             nc = int(data.popleft())
-            parse_field(data, obj.cells, nc, 4, obj.cell_corners)
+            parse_field(data, obj.cells, nc, 4)
         
         elif line=="Hexahedra":
             nc = int(data.popleft())
-            parse_field(data, obj.cells, nc, 6, obj.cell_corners)
+            parse_field(data, obj.cells, nc, 6)
 
     return obj
 
 def count_cells(mesh : RawMeshData):
     cell_count = [0,0,0]
     # 0 = hexahedra
     # 1 = tetrahedra
```

### Comparing `mouette-1.1.7/mouette/mesh/io/obj.py` & `mouette-1.2.0/mouette/mesh/io/obj.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,25 +40,25 @@
             v1,v2 = int(toks[1])-1, int(toks[2])-1
             e = keyify(v1,v2)
             obj.edges.append(e)
 
     normals_attr = obj.vertices.create_attribute("normals", float, 3)
     uv_attr = obj.face_corners.create_attribute("uv_coords", float, 2)
     ic = 0
-    for f in faces:
+    for iF,F in enumerate(faces):
         face = []
-        for (vid,tid,nid) in f:
+        for (vid,tid,nid) in F:
             face.append(vid)
             if nid!=-1:
                 normals_attr[vid] = normals[nid]
             if tid!=-1:
                 uv_attr[ic] = uv_coords[tid]
             ic += 1
         obj.faces.append(face)
-        obj.face_corners += face
+        obj.face_corners += [(v,iF) for v in face]
     if normals_attr.empty() : obj.vertices.delete_attribute("normals")
     if uv_attr.empty(): obj.face_corners.delete_attribute("uv_coords")
     return obj
 
 def export_obj(mesh, path):
     has_texcoords_vert = mesh.vertices.has_attribute("uv_coords") and not mesh.vertices.get_attribute("uv_coords").empty()
     has_texcoords_corners = mesh.face_corners.has_attribute("uv_coords") and not mesh.face_corners.get_attribute("uv_coords").empty()
@@ -70,15 +70,15 @@
 
         if has_texcoords_corners:
             texcoords = mesh.face_corners.get_attribute("uv_coords").as_array(len(mesh.face_corners))
             for tex in texcoords:
                 ofile.write('vt '+' '.join([str(vt) for vt in tex])+'\n')
                     
         elif has_texcoords_vert:
-            texcoords = mesh.vertices.get_attribute("uv_coords").as_array()
+            texcoords = mesh.vertices.get_attribute("uv_coords").as_array(len(mesh.vertices))
             for tex in texcoords:
                 ofile.write('vt '+' '.join([str(vt) for vt in tex])+'\n')
 
         if has_normals :
             normals = mesh.vertices.get_attribute("normals")
             for i in mesh.id_vertices:
                 nrm = normals[i]
```

### Comparing `mouette-1.1.7/mouette/mesh/io/off.py` & `mouette-1.2.0/mouette/mesh/io/off.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,28 @@
     for _ in range(nv):
         vertex = [float(u) for u in data.popleft()]
         output.vertices.append(Vec(vertex))
 
     for _ in range(nf):
         simplex = data.popleft()
         nvi = int(simplex[0])
+        nf,nc = 0,0
         if nvi==3:
             face = [int(u) for u in simplex[1:nvi+1]]
             output.faces.append(face)
-            output.face_corners += face
+            output.face_corners += [(x,nf) for x in face]
+            nf += 1
         elif nvi==2:
             a,b = simplex[1], simplex[2]
             output.edges.append((min(a,b), max(a,b)))
         elif nvi==4:
             cell = [int(u) for u in simplex[1:nvi+1]]
             output.cells.append(cell)
-            output.cell_corners += cell
+            output.cell_corners += [(x,nc) for x in cell]
+            nc += 1
     return output
 
 def export_off(mesh, path):
     with open( path, 'w' ) as ofile:
         ofile.write("OFF\n")
         nums = "{} {} {}\n".format(len(mesh.vertices), len(mesh.faces), len(mesh.edges))
         ofile.write(nums)
```

### Comparing `mouette-1.1.7/mouette/mesh/io/stl.py` & `mouette-1.2.0/mouette/mesh/io/stl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,62 @@
 import stl_reader
 import struct
 from ..mesh_data import RawMeshData
+from collections import deque
+
+def is_stl_ascii(path : str):
+    try:
+        with open(path, 'r', encoding="utf-8") as f:
+            return "solid" in f.readline().strip().split()
+    except Exception as e:
+        return False
 
 def import_stl(path : str):
-    vertices, faces =  stl_reader.read(path)
-    data = RawMeshData()
-    data.vertices += list(vertices)
-    data.faces += list(faces)
-    return data
+    if is_stl_ascii(path):
+        return _import_stl_ascii(path)
+    else:
+        vertices, faces =  stl_reader.read(path)
+        out = RawMeshData()
+        out.vertices += list(vertices)
+        out.faces += list(faces)
+        return out
+
+def _import_stl_ascii(path : str):
+    data = deque()
+    with open(path, "r", encoding="utf-8") as stlf:
+        data = deque([x.strip().split() for x in stlf.readlines()])
+    
+    out = RawMeshData()
+    normals = out.faces.create_attribute("normals", float, 3)
+    iF = 0
+    while data:
+        line = data.popleft()
+        if line[0]=="solid": continue
+        
+        elif line[0]=="facet":
+            assert line[1] == "normal"
+            normals[iF] = [float(x) for x in line[2:]]
+            out_loop = data.popleft()
+            assert out_loop[0] == "outer"
+            vertices = []
+            for _ in range(3):
+                v = data.popleft()
+                assert v[0] == "vertex"
+                vertices.append([float(x) for x in v[1:]])
+            end_loop = data.popleft()
+            assert end_loop[0] == "endloop"
+            endfacet = data.popleft()
+            assert endfacet[0] == "endfacet"
+
+            out.vertices += vertices
+            out.faces.append((3*iF,3*iF+1,3*iF+2))
+            iF += 1
+
+        elif line[0] == "endsolid": continue
+    return out
 
 # Exporter adapted from https://gist.github.com/ryansturmer/9329299
 # License: MIT License 
 
 def export_stl(mesh, path :str):
     if not hasattr(mesh, "faces"):
         print("[Warning] no faces detected in the object. Nothing to write. Returning.")
```

### Comparing `mouette-1.1.7/mouette/mesh/io/tet.py` & `mouette-1.2.0/mouette/mesh/io/tet.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/io/xyz.py` & `mouette-1.2.0/mouette/mesh/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/mesh.py` & `mouette-1.2.0/mouette/mesh/mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,13 @@
 from .mesh_data import RawMeshData
 from .datatypes import Mesh, PointCloud, PolyLine, SurfaceMesh, VolumeMesh
 from .io.io import read_by_extension, write_by_extension
 
 import numpy as np
 
-def new_point_cloud() -> PointCloud: 
-    """
-    Create a new empty point cloud
-
-    Returns:
-        PointCloud
-    """
-    return PointCloud()
-    
-def new_polyline() -> PolyLine:
-    """
-    Creates a new empty poly line
-
-    Returns:
-        PolyLine
-    """
-    return PolyLine()
-
-def new_surface() -> SurfaceMesh:
-    """
-    Creates a new empty surface mesh
-
-    Returns:
-        SurfaceMesh
-    """
-    return SurfaceMesh()
-
-def new_volume() -> VolumeMesh:
-    """
-    Creates a new empty volume mesh
-
-    Returns:
-        VolumeMesh
-    """
-    return VolumeMesh()
-
-
 def _instanciate_raw_mesh_data(mesh_data : RawMeshData, dim : int = None) -> Mesh:
     mesh_data.prepare()
     if dim is None: dim = -1
     dim = max(dim, mesh_data.dimensionality)
     if dim==0: return PointCloud(mesh_data)
     if dim==1: return PolyLine(mesh_data)
     if dim==2: return SurfaceMesh(mesh_data)
@@ -117,21 +80,20 @@
         if np.any(F>=n_vert): raise Exception("Face indices should be between 0 and n_vertices")
         m.faces += list(F)
     if C is not None:
         if np.any(C>=n_vert): raise Exception("Cell indices should be between 0 and n_vertices")
         m.cells += list(C)
     return _instanciate_raw_mesh_data(m)
 
-def copy(mesh : Mesh, copy_attributes=False, copy_connectivity=False, copy_half_edges=False) -> Mesh:
+def copy(mesh : Mesh, copy_attributes=False, copy_connectivity=False) -> Mesh:
     """Makes a copy of the input mesh
 
     Parameters:
         mesh (Mesh): input mesh
         copy_attributes (bool, optional): whether to also copy attributes data. Defaults to False.
-        copy_half_edges (bool, optional): whether to also copy pre-computed half-edge structure for connectivity. Defaults to False.
     Returns:
         Mesh: a hard copy of the given mesh
     """
     from copy import deepcopy
     copy_mesh = type(mesh)() # instanciate a new mesh of the same type
 
     if copy_attributes:
@@ -139,29 +101,32 @@
         if hasattr(mesh, "edges") : copy_mesh.edges = deepcopy(mesh.edges)
         if hasattr(mesh, "faces") :
             copy_mesh.faces = deepcopy(mesh.faces)
             copy_mesh.face_corners = deepcopy(mesh.face_corners)
         if hasattr(mesh, "cells"):
             copy_mesh.cells = deepcopy(mesh.cells)
             copy_mesh.cell_corners = deepcopy(mesh.cell_corners)
+            copy_mesh.cell_faces = deepcopy(mesh.cell_faces)
     else:
         # copy only _cont data of each container (connectivity data and not attribute data)
         copy_mesh.vertices._data = deepcopy(mesh.vertices._data)
         if hasattr(mesh, "edges"): copy_mesh.edges._data = deepcopy(mesh.edges._data)
         if hasattr(mesh, "faces") : 
             copy_mesh.faces._data = deepcopy(mesh.faces._data)
-            copy_mesh.face_corners._data = deepcopy(mesh.face_corners._data)
+            copy_mesh.face_corners._elem = deepcopy(mesh.face_corners._elem)
+            copy_mesh.face_corners._adj = deepcopy(mesh.face_corners._adj)
         if hasattr(mesh, "cells") : 
             copy_mesh.cells._data = deepcopy(mesh.cells._data)
-            copy_mesh.cell_corners._data = deepcopy(mesh.cell_corners._data)
+            copy_mesh.cell_corners._elem = deepcopy(mesh.cell_corners._elem)
+            copy_mesh.cell_corners._adj = deepcopy(mesh.cell_corners._adj)
+            copy_mesh.cell_faces._elem = deepcopy(mesh.cell_faces._elem)
+            copy_mesh.cell_faces._adj = deepcopy(mesh.cell_faces._adj)
         # _cont of face_corners and cell_corners are always empty
     if copy_connectivity and hasattr(mesh, "connectivity"):
         copy_mesh.connectivity = mesh.connectivity
-    if copy_half_edges and hasattr(mesh, "half_edges"):
-        copy_mesh.half_edges = mesh.half_edges
     return copy_mesh
 
 def merge(mesh_list : list) -> Mesh:
     """Merges a list of independents meshes as a unique mesh.
 
     Parameters:
         mesh_list (list): the list of meshes. If empty, this function returns None
```

### Comparing `mouette-1.1.7/mouette/mesh/mesh_attributes.py` & `mouette-1.2.0/mouette/mesh/mesh_attributes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/mesh/mesh_data.py` & `mouette-1.2.0/mouette/optimize/levenberg_marquardt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,307 +1,311 @@
 import numpy as np
+from osqp import OSQP
+from dataclasses import dataclass
+import scipy.sparse as sp
+from types import FunctionType
+
+from tqdm import tqdm, trange
+from tqdm.utils import _term_move_up
+prefix = _term_move_up() + '\r'
 
-from .mesh_attributes import Attribute, ArrayAttribute
-from ..geometry import Vec
-from .. import utils
-from .. import config
-import itertools
-import warnings
-from .. import config
+from ..utils import Logger, get_osqp_lin_solver
+from .. import geometry as geom
 
-
-class DataContainer:
+@dataclass
+class LMParameters:
     """
-    A DataContainer is a container class for all simplicial elements of the same type in an instance (for example, vertices, edges or faces).
-    It stores relevant information about the combinatorics (in the _data field) as well as various attributes onto the elements (in the _attr field)
+    Hyper parameters for the Levenberg-Marquardt algorithm
     """
+    N_ITER_MAX    : int   = 1000 # stopping criterion on maximal number of iterations
+    ENERGY_MIN    : float = 1e-7 # stopping criterion for reaching zero
+    MIN_STEP_NORM : float = 1e-5 # stopping criterio, on ||x_n - x_{n-1}||
+    MIN_GRAD_NORM : float = 1e-5 # stopping criterion on gradient projected on constraints
+    MIN_DELTA_E   : float = 1e-5 # stopping criterion
+    MU_MAX        : float = 1e8  # stopping criterion on mu going to +infty
+    MU_MIN        : float = 1e-8 # minimal value for mu
+    alpha         : float = 0.5  # if iteration is a success, mu = alpha * mu
+    beta          : float = 2.   # if iteration fails, mu = beta * mu
+
+@dataclass
+class LMVerboseOptions:
+    logger_verbose : bool = True  # main verbose for mouette logging
+    solver_verbose : bool = False # prints outputs of OSQP solver
+    use_tqdm       : bool = True  # progression bar using tqdm
+    log_frequency  : int  = 1     # display an info message every 'log_frequency' iterations
+
+@dataclass
+class LMFunction:
+    name : str # name of the function
+    fun  : FunctionType # x -> f(x), J(x) where J is the jacobian
+    fun_noJ : FunctionType = None # x -> f(x) without jacobian
+    weight : float = 1. # multiplicative weight
+
+    def call(self, X):
+        F,J = self.fun(X)
+        return self.weight*F, self.weight*J
 
-    def __init__(self, data : list = None, attributes : dict = None, id : str = ""):
-        self.id = id
-        if data is None:
-            self._data = []
-        else:
-            self._data = list(data)
-        
-        # self._attr : dict of str->Attribute
-        if attributes is None:
-            self._attr = dict()
-        else:
-            assert isinstance(attributes, dict)
-            self._attr = attributes 
-    
-    def __getitem__(self, key):
-        return self._data[key]
+    def call_noJ(self,X):
+        return self.weight*self.fun_noJ(X)
 
-    def __setitem__(self, key, value):
-        try:
-            self._data[key] = value
-        except Exception as e:
-            warnings.warn(f"Error in attribute '{key}' : {e}")
-            raise Exception("Aborting")
-
-    def __iter__(self):
-        return self._data.__iter__()
-
-    def __repr__(self):
-        return self._data.__repr__()
-
-    def __str__(self):
-        return str(self._data) + "\nAttributes: "+str(self._attr.keys())
-
-    @property
-    def size(self):
-        return len(self._data)
-
-    def __len__(self):
-        return len(self._data)
-
-    def empty(self):
-        return not self._data
-
-    def clear(self):
-        self._data = []
-        self._attr = dict()
-
-    @property
-    def attributes(self):
-        return self._attr.keys()
-
-    def create_attribute(self, name, data_type, elem_size=1, dense=False, default_value=None) -> Attribute:
-        # If 'name' already exists in the attribute dict, the corresponding attribute will be overridden
-        if name in self._attr and not config.disable_duplicate_attribute_warning:
-            warnings.warn(f"Warning ! Attribute '{name}' already exists on {self.id}")
-        else:
-            if dense:
-                self._attr[name] = ArrayAttribute(data_type, len(self), elem_size=elem_size, default_value=default_value)
-            else:
-                self._attr[name] = Attribute(data_type, elem_size=elem_size, default_value=default_value)
-        return self._attr[name]
+class LevenbergMarquardt(Logger):
+    """
+    Levenberg-Marquardt algorithm for non-linear least-square minimization.
 
-    def register_array_as_attribute(self, name, data, default_value=None):
-         # If 'name' already exists in the attribute dict, the corresponding attribute will be overridden
-        if name in self._attr and not config.disable_duplicate_attribute_warning:
-            warnings.warn(f"Warning ! Attribute '{name}' already exists on {self.id}")
-        else:
-            if len(data.shape)==1: 
-                data = data[:,np.newaxis] # change array of size (n,) to size (n,1)
-            try:
-                n_elem = data.shape[0]
-                elem_size = data.shape[1]
-                assert n_elem == len(self)
-            except Exception as e:
-                raise Exception(f"data array has invalid shape {data.shape}")
-            self._attr[name] = ArrayAttribute(type(data[0,0].item()), n_elem, elem_size=elem_size, default_value=default_value)
-            self._attr[name]._data = data
-
-    def delete_attribute(self, name):
-        if name in self._attr:
-            del self._attr[name]
-
-    def has_attribute(self, name) -> bool:
-        return name in self._attr
-
-    def get_attribute(self, name) -> Attribute :
-        if name not in self._attr:
-            raise Exception("Attribute does not exist")
-        return self._attr[name]
-
-    def append(self,val):
-        self._data.append(val)
-        for attr in self._attr.values():
-            attr._expand(1)
-
-    def __iadd__(self,other):
-        if isinstance(other, list) or isinstance(other,tuple) or isinstance(other, set):
-            self._data += list(other)
-            for attr in self._attr.values():
-                attr._expand(len(other))
-        elif isinstance(other,DataContainer):
-            self._data += other._data
-            for attr in self._attr.values():
-                attr._expand(other.n_elem)
-        else:
-            raise Exception("Could not append data container of type {} onto an attribute".format(type(other)))
-        return self
+    References:
+        [1] https://en.wikipedia.org/wiki/Levenberg%E2%80%93Marquardt_algorithm
+        [2] Constrained Levenberg-Marquardt Method with global complexity bounds, Marumo et al.
+    """
 
+    def __init__(self,
+        HP : LMParameters = LMParameters(), 
+        verbose : LMVerboseOptions = LMVerboseOptions(),
+        **kwargs):
+        super().__init__("LMopt",verbose.logger_verbose)
+        self.verbose_options = verbose
+        self.HP = HP
+
+        self.X = None # variables
+
+        ### Linear Constraints
+        self._cstM = None
+        self._cstL = None
+        self._cstU = None
 
-class RawMeshData:
-    """
-    A base container class to store all the data relative to a mesh.
-    It is not made to be used outside of the library, and serves an intermediate between io parsers and instantiated (and typed) mesh classes.
-    """
+        ### Metric matrix
+        self._W : sp.csc_matrix = None
 
-    def __init__(self, mesh=None):
-        self.vertices = DataContainer(id="vertices") if mesh is None else mesh.vertices
-        self.edges = DataContainer(id="edges") if (mesh is None or not hasattr(mesh,"edges")) else mesh.edges
-
-        self.faces = DataContainer(id="faces") if (mesh is None or not hasattr(mesh,"faces")) else mesh.faces
-        self.face_corners = DataContainer(id="face_corners") if (mesh is None or not hasattr(mesh,"face_corners")) else mesh.face_corners
-       
-        self.cells = DataContainer(id="cells") if (mesh is None or not hasattr(mesh,"cells")) else mesh.cells
-        self.cell_corners = DataContainer(id="cell_corners") if (mesh is None or not hasattr(mesh,"cell_corners")) else mesh.cell_corners
-        self.cell_faces = DataContainer(id="cell_faces") if (mesh is None or not hasattr(mesh,"cell_faces")) else mesh.cell_faces
-
-        self._dimensionality : int = None
-        self._prepared : bool = False
-    
-    @property
-    def id_vertices(self):
-        """
-        Shortcut for range(len(self.vertices))
-        """
-        return range(len(self.vertices))
+        ### Function to optimize
+        self._functions = []
 
-    @property
-    def id_edges(self):
-        """
-        Shortcut for range(len(self.edges))
-        """
-        return range(len(self.edges))
+        ### Others
+        self._stop_criterion_instance = None # OSQP instance to compute projected gradient norm
+        
+        ### Additionnal parameters
+        self._linsys_solver = kwargs.get("lin_solver", get_osqp_lin_solver())
 
-    @property
-    def id_faces(self):
+    def register_constraints(self, A : sp.spmatrix, l : np.ndarray = None, u : np.ndarray = None):
         """
-        Shortcut for range(len(self.faces))
+        Adds linear constraints to the optimization problem :
+
+        min_X ||F(X)||² s.t.  l <= AX <= u
+
+        Args:
+            cstMat (sp.spmatrix): constraint matrix, either dense or sparse
+            cstL (np.ndarray, optional): vector l. Defaults to None.
+            cstR (np.ndarray, optional): vector u. Defaults to None.
         """
-        return range(len(self.faces))
 
-    @property
-    def id_cells(self):
+        if isinstance(A, sp.spmatrix):
+            self._cstM = A.tocsc()
+        elif isinstance(A, np.ndarray):
+            assert len(A.shape)==2 # we make sure A is indeed a matrix
+            self._cstM = sp.csc_matrix(A)
+        self._cstL = l
+        self._cstU = u
+
+    def register_function(self, fun, fun_noJ=None, weight:float=1., name:str=None):
         """
-        Shortcut for range(len(self.cells))
+        Adds a function to minimize.
+
+        Args:
+            fun (python callable): A function taking a single argument X (np.array) returning a vector of values F and a (sparse or dense) jacobian matrix J
+
+            fun_noJ (python callable, optional): The same function that avoids the computation of the jacobian for speed purposes. If not provided, will use the function provided above and ignore the jacobian.
+
+            weight (float, optional): real weight to be applied to the function. Defaults to 1..
+            
+            name (str, optional): Name of the function in the logs. If not specified, the function will be given a default name.
         """
-        return range(len(self.cells))
+        if name is None:
+            name = f"fun{len(self._functions)}"
+        if fun_noJ is None:
+            fun_noJ = lambda x : fun(x)[0]
+        self._functions.append( LMFunction(name, fun, fun_noJ, weight) )
+
+    def set_metric_matrix(self, W : sp.spmatrix):
+        # TODO : some assertions on the matrix
+        self._W = W.tocsc()
 
-    @property
-    def dimensionality(self) -> int:
+    def energy(self, X, jac=True, which=None):
+        funs_to_call = self._functions if which is None else [fun for fun in self._functions if fun.name in which]
+        if jac:
+            F,J = [],[]
+            for f in funs_to_call:
+                fi,ji = f.call(X)
+                F.append(fi)
+                J.append(ji)
+            return F,J
+        return [f.call_noJ(X) for f in funs_to_call]
+
+    def optimize(self, x_init: np.ndarray) -> float:
         """
-        Dimensionality of the manifold represented by the data.
-        If only vertices -> 0
-        If vertices and edges (embedded graph) -> 1
-        If faces (surface manifold) -> 2
-        If cells (volume manifold) -> 3
+        Alias of the 'run' method.
+
+        Args:
+            x_init (np.ndarray): initial values for the variables.
 
         Returns:
-            int
+            float: final value of the energy
         """
-        if self._dimensionality is None:
-            self._compute_dimensionality()
-        return self._dimensionality
-
-    def _compute_dimensionality(self):
-        if not self.cells.empty():
-            self._dimensionality = 3
-        elif not self.faces.empty():
-            self._dimensionality = 2
-        elif not self.edges.empty():
-            self._dimensionality = 1
-        else:
-            self._dimensionality = 0
+        return self.run(x_init)
 
-    def prepare(self) -> None:
+    def run(self, x_init : np.ndarray):
         """
-        Prepares the data to have the correct format.
-        On vertices : casts to M.Vec
-        On edges : sorts edge tuples to satisfy edge convention (smallest index first)
-        On faces : nothing
-        On cells : nothing
+        Runs the optimizer
 
-        if option is set in config, adds to the edge container all the edges implicitly defined by the faces
-        """
-        if self._prepared : return
+        Args:
+            x_init (np.ndarray): initial values for the variables.
 
-        # call completion before preparation
-        if config.complete_faces_from_cells:
-            self._complete_faces_from_cells()
-
-        # call edge completion ***after*** face completion
-        if config.complete_edges_from_faces : 
-            self._complete_edges_from_faces() 
-
-        self._prepare_vertices()
-        self._prepare_edges()
-        self._prepare_faces()
-        self._prepare_face_corners()
-        self._prepare_cells()
-        self._compute_dimensionality()
-        self._prepared = True
-
-    def _prepare_vertices(self):
-        for iv in self.id_vertices:
-            self.vertices[iv] = Vec(self.vertices[iv])
-
-    def _prepare_edges(self):
-        N = len(self.vertices)
-
-        def is_valid(a,b):
-            return a!=b and 0<=a<N and 0<=b<N
-
-        # Filter invalid edges (like (x,x)) and make the other immutable
-        edges_invalid = any((not is_valid(a,b) for a,b in self.edges))
-        if edges_invalid:
-            # Rebuild the edge container
-            new_edges = DataContainer(id="edges")
-            new_attrs = dict()
-            old_attrs = dict()
-            for attr_name in self.edges.attributes:
-                old_attrs[attr_name] = self.edges.get_attribute(attr_name)
-                new_attrs[attr_name] = new_edges.create_attribute(attr_name, old_attrs[attr_name].type, old_attrs[attr_name].elemsize)
-            n = 0
-            for ie in self.id_edges:
-                a,b = self.edges[ie]
-                if is_valid(a,b):
-                    new_edges.append(utils.keyify(a,b))
-                    for name in new_attrs:
-                        if ie in old_attrs[name]: # keep sparsity of the attribute
-                            new_attrs[name][n] = old_attrs[name][ie]
-                    n+=1
-            self.edges = new_edges
-        else:
-            for ie in self.id_edges:
-                self.edges[ie] = utils.keyify(self.edges[ie])
+        Returns:
+            float: final value of the energy
+        """
 
-    def _prepare_faces(self):
-        pass
-        # for iF in self.id_faces:
-        #     self.faces[iF] = tuple(self.faces[iF])
+        self.X = x_init # variable vector
         
+        if self.HP.N_ITER_MAX <= 0 :
+            # return current energy
+            en = self.energy(x_init, jac=False)
+            return 0.5*sum(np.dot(e,e) for e in en)
+
+        if not self._functions: 
+            # No functions to optimize
+            self.log("No function to optimize.")
+            return 0.
+
+        if self._W is None:
+            # Metric matrix is Id by default (classical L2 norm)
+            self._W = sp.identity(x_init.size, format="csc")
+
+        mu = 1.
+        mu_avg = mu
+        update = True
+        grad_norm = None
+        step_norm = 0.
+        RelDeltaE = 0.
+
+        # iterable for optimization steps
+        if self.verbose_options.logger_verbose and self.verbose_options.use_tqdm:
+            print()
+            iterobj = trange(self.HP.N_ITER_MAX, total=self.HP.N_ITER_MAX, position=1, leave=False, ncols=100, unit="")
+        else:
+            iterobj = range(self.HP.N_ITER_MAX)
 
-    def _prepare_face_corners(self):
-        nc = len(self.face_corners)
-        nf = sum([len(f) for f in self.faces])
-        if nc == 0 or nc!= nf : 
-            # corners were not generated
-            self.face_corners._data = []
-            for f in self.faces:
-                self.face_corners._data += list(f)
-
-    def _prepare_cells(self):
-        pass
+        try:
+            # Iteration loop
+            for it in iterobj:                
 
-    def _complete_edges_from_faces(self):
-        if self.faces.empty() : return # nothing to do
-        
-        # Create hard edges attribute for already existing edges
-        hard_edges = self.edges.create_attribute("hard_edges", bool)
-        for e in self.id_edges: hard_edges[e] = True
-        
-        edge_set = set([utils.keyify(e) for e in self.edges])
-        for f in self.faces:
-            nf = len(f)
-            for i in range(nf):
-                edge = utils.keyify(f[i], f[(i+1)%nf])
-                if edge not in edge_set:
-                    edge_set.add(edge)
-                    self.edges.append(edge)
-
-    def _complete_faces_from_cells(self):
-        if self.cells.empty() : return # nothing to do
-        face_set = set([utils.keyify(f) for f in self.faces])
-        for C in self.cells:
-            if len(C)>4:
-                continue
-            for F in itertools.combinations(C,3): # all possibilities of 3-uples among the tetrahedron
-                face = utils.keyify(F)
-                if face not in face_set:
-                    face_set.add(face)
-                    self.faces.append(F)
+                if update: # energy only changes if we performed a step last iteration
+                    flist, Jlist = self.energy(self.X)
+                    Jx = sp.vstack(Jlist).tocsr()
+                    fx = np.concatenate(flist)
+                    Jt = Jx.transpose()
+                    JtJ = Jt.dot(Jx)
+                    q = Jt.dot(fx) # gradient
+
+                    Ex = np.dot(fx,fx)/2
+
+                    if Ex<self.HP.ENERGY_MIN:
+                        return self._end_optimization(Ex, "Ex < Ex_min") # zero found
+                    if np.isnan(Ex):
+                        return self._end_optimization(Ex, "NaN value in energy")
+                    if np.isposinf(Ex):
+                        mu = self.HP.beta*mu
+                        update=False
+                        continue
+                    grad_stop, grad_norm = self._stop_criterion_projgrad(q)
+                    if grad_stop:
+                        return self._end_optimization(Ex, "projected grad norm on constraints < min_grad_norm")
+
+                if mu>self.HP.MU_MAX:
+                    return self._end_optimization(Ex, "mu > mu_max")
+                    
+                gamma = mu * np.sqrt(2*Ex)
+                osqp_instance = OSQP()
+                if self._cstM is not None:
+                    # OSQP solve inside iteration loop computes the increment x_{n-1} - x_n, so constraints have to be shifted
+                    xCst = self._cstM @ self.X
+                    cstL = self._cstL - xCst
+                    cstU = self._cstU - xCst
+                else:
+                    cstL,cstU = None, None
+                osqp_instance.setup(JtJ + gamma*self._W, q=q, A=self._cstM, l=cstL, u=cstU,
+                    verbose=self.verbose_options.solver_verbose,
+                    eps_abs=1e-3, eps_rel=1e-3,
+                    max_iter=100, polish=True, check_termination=10, 
+                    adaptive_rho=True, linsys_solver= self._linsys_solver)
+                s = osqp_instance.solve().x # computed increment
+
+                if s[0] is not None:
+                    ms = fx + Jx.dot(s)
+                    ms = np.dot(ms,ms)/2 + gamma*np.dot(s,s)/2
+                    fxs = self.energy(self.X + s, jac=False)
+                    fxs = np.concatenate(fxs)
+                    Exs = np.dot(fxs,fxs)/2
+
+                update = (s is not None) and (Exs <= ms)  # whether to make a step (True) or increase mu (False)
+                if update:
+                    RelDeltaE = abs(Exs-Ex)/Ex
+                    if RelDeltaE < self.HP.MIN_DELTA_E :
+                        return self._end_optimization(Ex, "Relative progression of energy < ΔE_min")
+                    self.X += s
+                    step_norm = geom.norm(s)
+                    if step_norm < self.HP.MIN_STEP_NORM :
+                        return self._end_optimization(Ex, "Step norm < min_step_norm")
+                    mu, mu_avg = max(self.HP.MU_MIN, self.HP.alpha*mu_avg), mu
+                else:
+                    mu = self.HP.beta*mu
+
+                if self.verbose_options.logger_verbose and self.verbose_options.log_frequency >0 and it%self.verbose_options.log_frequency==0:
+                    energies = [np.dot(_f,_f)/2 for _f in flist]
+                    if self.verbose_options.use_tqdm:
+                        tqdm_log = prefix
+                        if len(self._functions)>1:
+                            for n,e in zip([f.name for f in self._functions], energies):
+                                tqdm_log+="{}: {:.2E} | ".format(n,e)
+                            tqdm_log += "Total: {:.2E} | Grad: {:.2E} | ".format(Ex, grad_norm)
+                        else:
+                            tqdm_log += "{}: {:.2E} | Grad: {:.2E} | ".format(self._functions[0].name, Ex, grad_norm)
+                        tqdm_log += "ΔE {:.2E} | Step {:.2E} | Mu: {:.2E}".format(RelDeltaE, step_norm, mu)
+                        tqdm_log += " " * 10
+                        tqdm.write(prefix)
+                        tqdm.write(tqdm_log)
+                    else:
+                        log = f"{it+1}/{self.HP.N_ITER_MAX} | "
+                        if len(self._functions)>1:
+                            for n,e in zip([f.name for f in self._functions], energies):
+                                log+="{}: {:.2E} | ".format(n,e)
+                            log += "Total: {:.2E} | Grad: {:.2E} | ".format(Ex, grad_norm)
+                        else:
+                            log += "{}: {:.2E} | Grad: {:.2E} | ".format(self._functions[0].name, Ex, grad_norm)
+                        log += "ΔE {:.2E} | Step {:.2E} | Mu: {:.2E}".format(RelDeltaE, step_norm, mu)
+                        print(log)
+                    
+        except KeyboardInterrupt:
+            self.log("Manual interruption")
+        return self._end_optimization(Ex, "max iteration reached")
+
+    def _stop_criterion_projgrad(self, G):
+        # Projected gradient on the orthogonal of space spanned by constraints should have small norm
+        if self._cstM is None:
+            xnorm = np.sqrt(np.dot(G,G))
+        else:
+            n = self._cstM.shape[1]
+            if self._stop_criterion_instance is None:
+                self._stop_criterion_instance = OSQP()
+                self._stop_criterion_instance.setup(
+                    sp.eye(n,format=("csc")), q=-2*G, A = self._cstM, l = self._cstL, u = self._cstU,
+                    verbose=self.verbose_options.solver_verbose)
+            else:
+                self._stop_criterion_instance.update(q=-2*G)
+            x = self._stop_criterion_instance.solve().x
+            if x is None: return False, 0.
+            xnorm = np.sqrt(np.dot(x,x))
+        return xnorm<self.HP.MIN_GRAD_NORM, xnorm
+
+    def _end_optimization(self, energy, message):
+        if self.verbose:
+            if self.verbose_options.use_tqdm: print("\n")
+            self.log("End of optimization: "+message)
+            self.log(f"Final Energy: {energy:.4E}")
+            if self.verbose_options.use_tqdm: print("\n\r")
+        return energy
```

### Comparing `mouette-1.1.7/mouette/operators/adjacency.py` & `mouette-1.2.0/mouette/operators/adjacency.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/operators/gradient.py` & `mouette-1.2.0/mouette/operators/gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 from ..geometry import *
 from ..processing.connection import SurfaceConnectionFaces
 from ..mesh.datatypes import *
 from ..attributes.misc_faces import face_area
 
 @allowed_mesh_types(SurfaceMesh)
-def gradient(mesh : SurfaceMesh, conn : SurfaceConnectionFaces, as_complex: bool =True) -> sp.csc_matrix:
+def gradient(mesh: SurfaceMesh, conn: SurfaceConnectionFaces = None, as_complex: bool = True) -> sp.csc_matrix:
     """
     Computes the gradient operator, i.e. a [F| x |V| matrix G such that for any scalar function f defined over vertices of a surface mesh, Gf is its gradient inside faces.
 
     Gf maps to each face of the mesh either a vector of R^2 or a complex number representing the gradient vector inside this face in local base.
 
     Args:
         mesh (SurfaceMesh): The input mesh
-        conn (SurfaceConnectionFaces): Connection objects specifying local bases of faces.
+        conn (SurfaceConnectionFaces, optional): Connection objects specifying local bases of faces. Will be computed if not provided. Defaults to None.
         as_complex (bool, optional): whether the output is |F| complex values of 2|F| float values
 
     Raises:
         Exception: Fails if the mesh is not a triangulation
     
     Returns:
         scipy.sparse.csc_matrix: Gradient operator
```

### Comparing `mouette-1.1.7/mouette/operators/laplacian_op.py` & `mouette-1.2.0/mouette/operators/laplacian_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         data[k] = x
         rows[k] = i
         cols[k] = j
         return k+1
 
     k = 0
     for l in mesh.id_vertices:
-        adj = mesh.connectivity.vertex_to_vertex(l)
+        adj = mesh.connectivity.vertex_to_vertices(l)
         k = add(k,l,l,len(adj))
         for b in adj:
             k = add(k, l, b, -1)
     return sp.csc_matrix((data, (rows,cols)), shape=(n,n))
 
 
 @allowed_mesh_types(SurfaceMesh)
@@ -129,16 +129,16 @@
     Returns:
         sp.csc_matrix
     """
     m = len(mesh.edges)
     cotan = cotangent(mesh, persistent=False)
     coeffs = np.zeros(m)
     for ie,(u,v) in enumerate(mesh.edges):
-        T1,uT1,vT1 = mesh.half_edges.adj(u,v)
-        T2,vT2,uT2 = mesh.half_edges.adj(v,u)
+        T1,uT1,vT1 = mesh.connectivity.direct_face(u,v,True)
+        T2,vT2,uT2 = mesh.connectivity.direct_face(v,u,True)
         cT1,cT2 = 0., 0.
         if T1 is not None : 
             w = mesh.faces[T1][3-uT1-vT1]
             c = mesh.connectivity.vertex_to_corner_in_face(w,T1)
             cT1 = cotan[c]
         if T2 is not None : 
             w = mesh.faces[T2][3-uT2-vT2]
@@ -193,21 +193,21 @@
 
     n = len(mesh.faces)
     m = len(mesh.edges)
 
     Nabla = sp.lil_matrix((m,n), dtype=complex if connection else np.float32) # gradient matrix
     if connection is not None:
         for ie,(ei,ej) in enumerate(mesh.edges):
-            T1,T2 = mesh.half_edges.edge_to_triangles(ei,ej)
+            T1,T2 = mesh.connectivity.edge_to_faces(ei,ej)
             if T1 is not None and T2 is not None:
                 Nabla[ie,T1] = -1
                 Nabla[ie,T2] = cmath.rect(1, order*connection.transport(T1,T2))
     else:
          for ie,(ei,ej) in enumerate(mesh.edges):
-            T1,T2 = mesh.half_edges.edge_to_triangles(ei,ej)
+            T1,T2 = mesh.connectivity.edge_to_faces(ei,ej)
             if T1 is not None and T2 is not None:
                 Nabla[ie,T1] = -1
                 Nabla[ie,T2] = 1
     Nabla = Nabla.tocsc()
     Nabla_star = Nabla.conj().transpose()
     if cotan:
         D = cotan_edge_diagonal(mesh)
```

### Comparing `mouette-1.1.7/mouette/optimize/eigensolve.py` & `mouette-1.2.0/mouette/optimize/eigensolve.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/procedural/cylinder.py` & `mouette-1.2.0/mouette/procedural/transform.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import numpy as np
-
-from ..geometry import *
-from ..attributes import mean_edge_length
 from ..mesh.datatypes import *
 from ..mesh.mesh_data import RawMeshData
-from ..mesh.mesh import merge
+from ..mesh.mesh import merge, _instanciate_raw_mesh_data
+
+from ..attributes import face_barycenter
+
+from .shapes import cylinder, icosphere
+from ..attributes import mean_edge_length
+
+def spherify_vertices(points : PointCloud, radius : float = 1e-2, n_subdiv=1) -> SurfaceMesh:
+    """Transforms vertices of a point cloud as icospheres
+
+    Args:
+        points (PointCloud): the input point cloud
+        radius (float, optional): radius of each sphere. Defaults to 1e-2.
+        n_subdiv (int, optional): number of subdivisions of the icospheres. Defaults to 1.
+
+    Returns:
+        SurfaceMesh
+    """
+    spheres = []
+    if isinstance(points, Mesh):
+        what = points.vertices
+    else:
+        what = points
+    for P in what:
+        mp = icosphere(n_subdiv, P, radius)
+        spheres.append(mp)
+    return merge(spheres)
 
-def cylinder(P1 : Vec, P2 : Vec, radius: float = 1., N=50, fill_caps=True) -> SurfaceMesh:
-    cy = RawMeshData()
-    axis = Vec.normalized(P2-P1)
-    t = Vec(axis.y, -axis.x, 0.) # tangent vector
-    if t.norm()<1e-6:
-        t = Vec(0, axis.z, -axis.y) # another tangent vector
-    t = Vec.normalized(t)
-    for P in (P1,P2):
-        for i in range(N):
-            Pi = P + radius * rotate_around_axis(t, axis, 2*np.pi*i/N)
-            cy.vertices.append(Pi)
-    # caps
-    if fill_caps:
-        cy.vertices += [P1,P2]
-        for i in range(N):
-            cy.faces.append((i,(i+1)%N,2*N))
-            cy.faces.append((i+N,2*N+1, (i+1)%N+N))
-    # side of cylinder
-    for i in range(N):
-        cy.faces.append((i,  N+i, (i+1)%N))
-        cy.faces.append((N+i, N+(i+1)%N, (i+1)%N))
-    return SurfaceMesh(cy)
 
 @forbidden_mesh_types(PointCloud)
 def cylindrify_edges( mesh : PolyLine, radius: float = 5e-2, N=50) -> SurfaceMesh:
     """ Transforms edges of a polyline as cylinder surface
 
     Parameters:
         mesh (PolyLine): the input mesh
```

### Comparing `mouette-1.1.7/mouette/procedural/rings.py` & `mouette-1.2.0/mouette/procedural/rings.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/processing/__init__.py` & `mouette-1.2.0/mouette/processing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """
 M.processing
 submodule for algorithms applied on meshes
 """
 
 from .misc import *
-from .combinatorics.subdivide import *
-from .combinatorics.cutting import SingularityCutter
+from .cutting import SingularityCutter
 from .features import FeatureEdgeDetector
-from .space_partition import QuadTree
 from .expmap import DiscreteExponentialMap
 
 from .paths import shortest_path, shortest_path_to_border, shortest_path_to_vertex_set
 from .border import extract_border_cycle, extract_border_cycle_all, extract_curve_boundary, extract_surface_boundary
 
 from . import trees
-from . import sampling
 from .parametrization import distortion
 from .connection import SurfaceConnectionFaces, SurfaceConnectionVertices, FlatConnectionVertices, FlatConnectionFaces
```

### Comparing `mouette-1.1.7/mouette/processing/border.py` & `mouette-1.2.0/mouette/processing/border.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,27 @@
     if len(mesh.boundary_vertices)==0 : return []
     if starting_point is None:
         starting_point = mesh.boundary_vertices[0]
     if not mesh.is_vertex_on_border(starting_point) : 
         raise Exception("Starting point (vertex {}) is not on mesh border".format(starting_point))
 
     vborder, eborder = [starting_point], []
-    point1, point2 = starting_point, mesh.connectivity.vertex_to_vertex(starting_point)[0]
-    
-    while point2 != starting_point:
+    point1, point2 = starting_point, mesh.connectivity.vertex_to_vertices(starting_point)[0]
+    nvisited = 0
+    MAX_VISITED = len(mesh.vertices)
+        
+    while point2 != starting_point and nvisited < MAX_VISITED:
         # while we have not come back to origin
         vborder.append(point2)
         eborder.append(mesh.connectivity.edge_id(point1, point2))
-        for v in mesh.connectivity.vertex_to_vertex(point2):
+        for v in mesh.connectivity.vertex_to_vertices(point2):
             if mesh.is_vertex_on_border(v) and v!=point1:
                 point1, point2 = point2, v
                 break
+        nvisited += 1
     eborder.append(mesh.connectivity.edge_id(point1, point2)) # add last edge to close the cycle
     return vborder, eborder
 
 @allowed_mesh_types(SurfaceMesh)
 def extract_border_cycle_all(mesh : SurfaceMesh) -> list:
     """
     Extracts all the border cycles of a mesh and returns a list of list of vertices
```

### Comparing `mouette-1.1.7/mouette/processing/combinatorics/cutting.py` & `mouette-1.2.0/mouette/processing/cutting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from ..worker import Worker
+from .worker import Worker
 
-from ...geometry import distance
-from ...mesh.datatypes import *
-from ...mesh.mesh_data import RawMeshData
-from ...mesh.mesh_attributes import *
-from ...utils import keyify, UnionFind, PriorityQueue
-from ..paths import shortest_path, shortest_path_to_border, shortest_path_to_vertex_set
-from ..trees import FaceSpanningForest
-from ... import attributes
+from ..geometry import distance
+from ..mesh.datatypes import *
+from ..mesh.mesh_data import RawMeshData
+from ..mesh.mesh_attributes import *
+from ..utils import keyify, UnionFind, PriorityQueue
+from .paths import shortest_path, shortest_path_to_border, shortest_path_to_vertex_set
+from .trees import FaceSpanningForest
+from .. import attributes
 from collections import deque
 
 class SingularityCutter(Worker):
     """
     Given some indexes in the mesh, performs optimal cuts connecting all these vertices with the boundary.
     """
 
@@ -122,15 +122,14 @@
             l = 0
             for i in range(1, len(path)):
                 A,B = path[i-1], path[i]
                 l += self.edge_lengths[self.input_mesh.connectivity.edge_id(A,B)]
             return l
             
         # Compute all edge paths between singularities (and border)
-
         path_btw_singus = dict()
         for i,a in enumerate(self.singularities):
             paths_a = shortest_path(self.input_mesh, a, set(self.singularities[i:]), weights=self.edge_lengths)
             for b in paths_a:
                 path_btw_singus[keyify(a,b)] = paths_a[b]
             if mesh_has_border:
                 path_btw_singus[(BORDER,a)] = shortest_path_to_border(self.input_mesh, a, weights=self.edge_lengths)
@@ -191,15 +190,15 @@
             v,prev = queue.popleft()
             if visited[v] : continue
             visited[v] = True
             parent[v] = prev
             if prev is not None:
                 e = self.input_mesh.connectivity.edge_id(v,prev)
                 edge_flags[e] = True
-            for e in self.input_mesh.connectivity.vertex_to_edge(v):
+            for e in self.input_mesh.connectivity.vertex_to_edges(v):
                 if e in self.feat_detector.feature_edges:
                     nv = self.input_mesh.connectivity.other_edge_end(e,v)
                     if not visited[nv]:
                         queue.append((nv,v))
 
         return edge_flags
 
@@ -232,18 +231,18 @@
             # Heuristic for distance between two faces
             return distance(barycenters[f1], barycenters[f2])
 
         while not queue.empty():
             iF = queue.get().x
             if fvisited[iF] : continue
             fvisited[iF] = True                
-            for e in self.input_mesh.connectivity.face_to_edge(iF):
+            for e in self.input_mesh.connectivity.face_to_edges(iF):
                 v1,v2 = self.input_mesh.edges[e]
                 if forbidden_edges[e] : continue # edge is on the singularity spanning tree
-                iF2 = self.input_mesh.half_edges.opposite(v1,v2,iF)[0]
+                iF2 = self.input_mesh.connectivity.opposite_face(v1,v2,iF)
                 if iF2 is not None: 
                     d = face_distance(iF,iF2)
                     if dist[iF2] > dist[iF] + d :
                         dist[iF2] = dist[iF] + d
                         path[iF2] = e
                     if not fvisited[iF2] :
                         queue.push(iF2, dist[iF2])
@@ -266,18 +265,18 @@
             # Heuristic for distance between two faces
             return distance(barycenters[f1], barycenters[f2])
 
         while not queue.empty():
             iF = queue.get().x
             if fvisited[iF] : continue
             fvisited[iF] = True        
-            for e in self.input_mesh.connectivity.face_to_edge(iF):
+            for e in self.input_mesh.connectivity.face_to_edges(iF):
                 v1,v2 = self.input_mesh.edges[e]
                 if forbidden_edges[e] : continue # edge is on the singularity spanning tree
-                iF2 = self.input_mesh.half_edges.opposite(v1,v2,iF)[0]
+                iF2 = self.input_mesh.connectivity.opposite_face(v1,v2,iF)
                 if iF2 is not None:
                     u,v = set(self.input_mesh.faces[iF]) & set(self.input_mesh.faces[iF2])
                     blocked = self.input_mesh.connectivity.edge_id(u,v) in self.feat_detector.feature_edges and regions.connected(iF,iF2)
                     if not blocked:
                         d = face_distance(iF,iF2)
                         if dist[iF2] > dist[iF] + d :
                             dist[iF2] = dist[iF] + d
@@ -338,58 +337,60 @@
         self._cut_graph = PolyLine(self._cut_graph)
 
     def _build_mesh_with_cuts(self):
         self._output_mesh = RawMeshData()
         uf = UnionFind(range(3*len(self.input_mesh.faces)))
         duplicate_vertices = dict([(v, set()) for v in self.input_mesh.id_vertices])
 
-        # First, no faces are adjacent
+        # At first, no faces are adjacent
+        kF = 0
         for iF,F in enumerate(self.input_mesh.faces):
             nF = len(F)
-            self._output_mesh.faces.append([nF*iF+_i for _i in range(nF)])
+            self._output_mesh.faces.append([kF+_i for _i in range(nF)])
             for iv,v in enumerate(F):
                 pv = self.input_mesh.vertices[v]
                 self._output_mesh.vertices.append(pv)
-                duplicate_vertices[v].add(nF*iF+iv)
+                duplicate_vertices[v].add(kF+iv)
+            kF += nF
 
         # Fusion vertices along edges that are not a cut
         for e in self.input_mesh.interior_edges:
             a,b = self.input_mesh.edges[e]
             if e not in self.cut_edges:
-                F1, iA1, iB1 = self.input_mesh.half_edges.adj(a,b)
-                F2, iB2, iA2 = self.input_mesh.half_edges.adj(b,a)
+                F1, iA1, iB1 = self.input_mesh.connectivity.direct_face(a,b,True)
+                F2, iB2, iA2 = self.input_mesh.connectivity.direct_face(b,a,True)
                 uf.union(self._output_mesh.faces[F1][iA1], self._output_mesh.faces[F2][iA2])
                 uf.union(self._output_mesh.faces[F1][iB1], self._output_mesh.faces[F2][iB2])
 
         for i,F in enumerate(self._output_mesh.faces):
-            self._output_mesh.faces[i] = [uf.find(a) for a in F]
-
-        # Reorder vertices to get rid of non connected duplicates
+            self._output_mesh.faces[i] = [uf.find(v) for v in F]
+            
+        # Reorder vertices to [0,n-1] and get rid of non connected duplicates
         imap = dict()
         i=0
         for F in self._output_mesh.faces:
-            for u in F:
-                if u not in imap:
-                    imap[u]=i # assign new index to u
-                    i+=1
+            for v in F:
+                if v in imap: continue
+                imap[v]=i # assign new index to first version of vertex u met
+                i+=1
 
         for iF,F in enumerate(self._output_mesh.faces):
             self._output_mesh.faces[iF] = [imap[v] for v in F]
         order_verts = [None]*len(imap)
 
         for u in range(len(self._output_mesh.vertices)):
-            if u in imap:
-                order_verts[imap[u]] = self._output_mesh.vertices[u]
+            if u not in imap: continue
+            order_verts[imap[u]] = self._output_mesh.vertices[u]
         self._output_mesh.vertices.clear()
         self._output_mesh.vertices += order_verts
+        self._output_mesh = SurfaceMesh(self._output_mesh)
         
         # get rid of duplicated and isolated vertices in map
         for v in duplicate_vertices:
             duplicate_vertices[v] = {imap[uf.find(u)] for u in duplicate_vertices[v]}
 
         # inverse duplicate_vertices to get self.ref_vertex
         self.ref_vertex = dict()
         for v in duplicate_vertices:
             for u in duplicate_vertices[v]:
                 self.ref_vertex[u] = v
 
-        self._output_mesh = SurfaceMesh(self._output_mesh)
```

### Comparing `mouette-1.1.7/mouette/processing/combinatorics/subdivide.py` & `mouette-1.2.0/mouette/mesh/subdivision.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from ...mesh.datatypes import *
-from ...mesh.mesh_data import RawMeshData
-from ...mesh.mesh import _instanciate_raw_mesh_data
-from ...geometry import Vec
-from ...utils import keyify, Logger
+from .datatypes import *
+from .mesh_data import RawMeshData
+from .mesh import _instanciate_raw_mesh_data
+from ..geometry import Vec
+from ..utils import keyify, Logger
 
 ### Polyline Subdivision ###
 
 @allowed_mesh_types(PolyLine)
 def split_edge(mesh : PolyLine, n : int) -> PolyLine:
     A,B = mesh.edges[n]
     C = len(mesh.vertices)
@@ -87,32 +87,35 @@
         self.triangulate()
 
         for _ in range(n):
             newMeshData = RawMeshData()
             newMeshData.vertices += self.mesh.vertices
             # cut every edge in half
             half = dict()
-            for e in self.mesh.id_edges:
-                A,B = self.mesh.edges[e]
+            for (A,B) in self.mesh.edges:
                 C = len(newMeshData.vertices)
                 pC = (self.mesh.vertices[A] + self.mesh.vertices[B])/2
                 newMeshData.vertices.append(pC)
                 half[keyify(A,B)]=C
             for f in self.mesh.id_faces:
                 A,B,C = self.mesh.faces[f]
                 mAB = half[keyify(A,B)]
                 mBC = half[keyify(B,C)]
                 mCA = half[keyify(C,A)]
-                for new_tris in [
+                for new_tri in [
                     (mAB,mBC,mCA),
                     (A,mAB,mCA),
                     (B,mBC,mAB),
                     (C,mCA,mBC)
                 ]:
-                    newMeshData.faces.append(new_tris)
+                    newMeshData.faces.append(new_tri)
+                for new_edge in [
+                    (A,mAB),(mAB,B),(B,mBC),(mBC,C),(C,mCA),(mCA,A), (mAB,mBC),(mBC,mCA),(mCA,mAB)
+                ]:
+                    newMeshData.edges.append(keyify(new_edge))
             self.mesh = newMeshData
 
     @allowed_mesh_types(SurfaceMesh)
     def subdivide_triangles_6(self, repeat:int = 1) -> SurfaceMesh:
         """Subdivides triangles of a mesh in 6 triangles by adding a point at the barycenter and three middles of edges.
             If the mesh is not triangulated, will triangulate the mesh first.
 
@@ -214,15 +217,15 @@
         f = self.mesh.faces[face_id]
         if len(f) != 3 : return
         A,B,C = f
         icenter = len(self.mesh.vertices)
         pcenter = sum([Vec(self.mesh.vertices[a]) for a in f ])/3 # barycenter
         self.mesh.vertices.append(pcenter)
         
-        for c in self.conn.face_to_cell(face_id):
+        for c in self.conn.face_to_cells(face_id):
             iF = self.conn.in_cell_face_index(c,face_id)
             new_cells = []
             for i in range(4):
                 if i==iF : continue # opposite point in tet from face
                 cell = [_x for _x in self.mesh.cells[c]]
                 cell[i] = icenter
                 new_cells.append(cell)
```

### Comparing `mouette-1.1.7/mouette/processing/connection.py` & `mouette-1.2.0/mouette/processing/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,44 +81,42 @@
         self._transport = dict()
 
         for u in range(n_vert):
             # find basis vector -> first edge
             P = Vec(self.mesh.vertices[u])
             N = self.vnormals[u]
             # extract basis edge
-            v = self.mesh.connectivity.vertex_to_vertex(u)[0]
-            E = self.mesh.vertices[v] - P
+            vert_u = self.mesh.connectivity.vertex_to_vertices(u)[::-1]
+            E = self.mesh.vertices[vert_u[0]] - P
             X = Vec.normalized(E - np.dot(E,N)*N) # project on tangent plane
             self._baseX[u] = X
             self._baseY[u] = geom.cross(N,X)
 
-            vert_u = self.mesh.connectivity.vertex_to_vertex(u)
-            
             # initialize angles of every edge in this basis
             ang = 0.
             if u in self.feat.feature_vertices:
                 dfct = self.feat.corners[u] * 2 * np.pi / self.feat.corner_order # target defect (multiple of pi/order)
                 for v in vert_u:
-                    T = self.mesh.half_edges.adj(u,v)[0]
+                    T = self.mesh.connectivity.direct_face(u,v)
                     self._transport[(u,v)] = ang * dfct / self.total_angle[u]
                     c = self.mesh.connectivity.vertex_to_corner_in_face(u,T)
                     if c is None: continue
                     ang += self.angles[c]
             else:
                 # normal vertex in interior -> flatten to 2pi
-                for v in vert_u :
-                    T = self.mesh.half_edges.adj(u,v)[0]
+                for v in vert_u:
+                    T = self.mesh.connectivity.direct_face(u,v)
                     self._transport[(u,v)] = ang * 2 * np.pi / self.total_angle[u]
                     c = self.mesh.connectivity.vertex_to_corner_in_face(u,T)
                     ang += self.angles[c]
 
 class FlatConnectionVertices(SurfaceConnection):
     """
     Surface connection on vertices where all local bases are taken as the canonical basis ([1 0 0], [0 1 0]).
-    /!\ This only makes sense if the considered surface is embedded in R^2, meaning that there is no curvature.
+    /!\\ This only makes sense if the considered surface is embedded in R^2, meaning that there is no curvature.
 
     Args:
         mesh (SurfaceMesh): the supporting mesh
     """
 
     @allowed_mesh_types(SurfaceMesh)
     def __init__(self, mesh : SurfaceMesh):
@@ -176,26 +174,26 @@
             self._baseY[id_face] = Y
 
         #### Initialize Parallel Transport
         for e in self.mesh.interior_edges:
             A,B = self.mesh.edges[e]
             pA,pB = self.mesh.vertices[A], self.mesh.vertices[B]
             E = geom.Vec(pB-pA)
-            T1,T2 = self.mesh.half_edges.edge_to_triangles(A,B)
+            T1,T2 = self.mesh.connectivity.edge_to_faces(A,B)
             X1,Y1 = self._baseX[T1], self._baseY[T1]
             X2,Y2 = self._baseX[T2], self._baseY[T2]
             angle1 = math.atan2( geom.dot(E,Y1), geom.dot(E,X1))
             angle2 = math.atan2( geom.dot(E,Y2), geom.dot(E,X2))
             self._transport[(T1,T2)] = angle1 - angle2
             self._transport[(T2,T1)] = angle2 - angle1
 
 class FlatConnectionFaces(SurfaceConnection):
     """
     Surface connection on faces where all local bases are taken as the canonical basis ([1 0 0], [0 1 0]).
-    /!\ This only makes sense if the considered surface is embedded in R^2, meaning that there is no curvature.
+    /!\\ This only makes sense if the considered surface is embedded in R^2, meaning that there is no curvature.
 
     Args:
         mesh (SurfaceMesh): the supporting mesh
     """
 
     @allowed_mesh_types(SurfaceMesh)
     def __init__(self, mesh : SurfaceMesh):
```

### Comparing `mouette-1.1.7/mouette/processing/expmap.py` & `mouette-1.2.0/mouette/processing/expmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         while not q.empty():
             front = q.get()
             v,rad = front.x, front.priority
             if rad>=self.radius : continue # ignore since too far from origin
             if v in visited : continue # vertex was already set
             visited.add(v)
-            for nv in self.mesh.connectivity.vertex_to_vertex(v):
+            for nv in self.mesh.connectivity.vertex_to_vertices(v):
                 dv = dist[v] + geom.distance(self.mesh.vertices[v], self.mesh.vertices[nv])
                 if dist.get(nv, float("inf")) > dv:
                     dist[nv] = dv
                     E = self.mesh.vertices[nv] - self.mesh.vertices[v]
                     E = self.conn.project(E, v)
                     rot[nv] = rot[v] + self.conn.transport(v,nv) - self.conn.transport(nv,v) + pi
                     self._map[u][nv] = self._map[u][v] + geom.rotate_2d(E, rot[v])
```

### Comparing `mouette-1.1.7/mouette/processing/features.py` & `mouette-1.2.0/mouette/processing/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.feature_graph : PolyLine = None
         self.only_border: bool = only_border # whether to ignore every feature edge that is not a boundary
         self.flag_corners: bool = flag_corners # whether to also flag the angle value of each feature vertex
         self.corner_order: int = corner_order
         self.compute_feature_graph: bool = compute_feature_graph
         
         self.border_cycles : list = None # result of 'M.processing.extract_border_cycle_all'
-        
+
         self.fnormals : Attribute = None # face normals
 
         # Following data structures will be filled
         self.feature_vertices : set = None # indexes of feature vertices
         self.feature_edges : set = None # indexes of feature edges
         self.feature_degrees : Attribute = None # degree of each feature vertex in the feature graph
         self.local_feat_edges : dict = None # vertex -> list of local indices of edges that are feature edges
@@ -78,23 +78,17 @@
             A, B = mesh.edges[e]
             self.feature_graph.edges.append((fvert[A],fvert[B]))
         self.feature_graph = PolyLine(self.feature_graph)
  
 ##### Feature detection subfunctions #####
 
     def _add_border_to_features(self, mesh : SurfaceMesh, feature_attr : Attribute) -> Attribute:
-        if len(mesh.boundary_vertices)==0 : return feature_attr # no border
-        border_cycles = extract_border_cycle_all(mesh)
-        for border in border_cycles:
-            nb = len(border)
-            for i in range(nb):
-                a,v,b = border[i-1], border[i], border[(i+1)%nb]
-                av,vb = mesh.connectivity.edge_id(a,v), mesh.connectivity.edge_id(v,b)
-                feature_attr[av] = True
-                feature_attr[vb] = True
+        if len(mesh.boundary_edges)==0 : return feature_attr # no border
+        for e in mesh.boundary_edges:
+            feature_attr[e] = True
         return feature_attr
 
     def _add_hard_edges_to_features(self, mesh : SurfaceMesh, feature_attr : Attribute) -> Attribute:
         """The mesh may already define a set of "hard" edges, for instance if it was imported from a file where edges were specified.
         These edges should be registered as features, but we filter them if their curvature is too small.
 
         Parameters:
@@ -104,16 +98,15 @@
             Attribute: the modified feature flag
         """
         if self.only_border : return feature_attr
         DOT_THRESHOLD = 0.2
         if mesh.edges.has_attribute("hard_edges"):
             for e in mesh.edges.get_attribute("hard_edges"):
                 A,B = mesh.edges[e]
-                T1,_,_ = mesh.half_edges.adj(A,B)
-                T2,_,_ = mesh.half_edges.adj(B,A)
+                T1,T2 = mesh.connectivity.edge_to_faces(A,B)
                 if T1 is None or T2 is None : continue
                 N1,N2 = self.fnormals[T1], self.fnormals[T2]
                 # we filter hard edge also depending on their angles. if marked but flat, the edge is ignored
                 if geometry.dot(N1,N2) < 1 - DOT_THRESHOLD and not mesh.is_edge_on_border(*mesh.edges[e]):
                     feature_attr[e] = True
         return feature_attr
 
@@ -125,31 +118,30 @@
 
         Returns:
             Attribute: the modified feature flag
         """
         if self.only_border : return feature_attr
         DOT_THRESHOLD = 0.5
         for e, (A,B) in enumerate(mesh.edges):
-            T1,_,_ = mesh.half_edges.adj(A,B)
-            T2,_,_ = mesh.half_edges.adj(B,A)
+            T1,T2 = mesh.connectivity.edge_to_faces(A,B)
             if T1 is None or T2 is None : continue
             N1,N2 = self.fnormals[T1], self.fnormals[T2]
             if geometry.dot(N1,N2) < DOT_THRESHOLD:
                 feature_attr[e] = True
         return feature_attr
     
     def _flag_corners(self, mesh : SurfaceMesh):
         if mesh.vertices.has_attribute("corners"):
             self.corners = mesh.vertices.get_attribute("corners")
         else:
             self.corners = mesh.vertices.create_attribute("corners", int)
         angles = corner_angles(mesh, persistent=False)
         for v in self.feature_vertices:
             angle_v = 0.
-            for T in mesh.connectivity.vertex_to_face(v):
+            for T in mesh.connectivity.vertex_to_faces(v):
                 c = mesh.connectivity.vertex_to_corner_in_face(v,T)
                 angle_v += angles[c]
             if abs(angle_v) <  2*pi/self.corner_order:
                 self.corners[v] = 1 if angle_v>=0 else -1
             else:
                 self.corners[v] = round(angle_v * self.corner_order / ( 2 * pi))
 
@@ -188,15 +180,15 @@
             self.feature_edges.add(e)
             self.feature_vertices.add(A)
             self.feature_vertices.add(B)
         
         self.log("Build local feature edges indices")
         for v in self.feature_vertices:
             self.local_feat_edges[v] = []
-            for i, ev in enumerate(mesh.connectivity.vertex_to_edge(v)):
+            for i, ev in enumerate(mesh.connectivity.vertex_to_edges(v)):
                 if feature[ev] :
                     self.local_feat_edges[v].append(i)
 
         for e in self.feature_edges:
             A,B = mesh.edges[e]
             self.feature_degrees[A] += 1
             self.feature_degrees[B] += 1
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/base.py` & `mouette-1.2.0/mouette/processing/framefield/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/processing/framefield/cells.py` & `mouette-1.2.0/mouette/processing/framefield/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             if abs(NF.z)<0.99:
                 axis = Vec.normalized(axis) * math.atan2(axis.norm(), NF.z)
                 face_bases_sh[iF] = SphericalHarmonics.from_vec3(axis)
             else:
                 face_bases_sh[iF] = Vec(0., 0., 0., 0., 1., 0., 0., 0., 0.)
         for iFb in self._boundary_mesh.id_faces:
             iF = self.mesh.boundary_connectivity.b2m_face[iFb]
-            iC = self.mesh.connectivity.face_to_cell(iF)[0]
+            iC = self.mesh.connectivity.face_to_cells(iF)[0]
             f,a = SphericalHarmonics.project_to_frame(face_bases_sh[iFb])
             self.var[9*iC:9*(iC+1)] += a
             self.frames[iC] *= f
         
         # normalization
         for iC in self._cell_on_bnd:
             nrm = geom.norm(self.var[9*iC:9*(iC+1)])
@@ -162,15 +162,15 @@
             if self._cell_on_bnd[iC]==0:
                 frame, a = SphericalHarmonics.project_to_frame(self.var[9*iC:9*(iC+1)], stop_threshold=1e-3)
                 self.var[9*iC:9*(iC+1)] = a
                 self.frames[iC] = frame
 
         for iFb in tqdm(self._boundary_mesh.id_faces, desc="normalize2"):
             iF = self.mesh.boundary_connectivity.b2m_face[iFb]
-            iC = self.mesh.connectivity.face_to_cell(iF)[0]
+            iC = self.mesh.connectivity.face_to_cells(iF)[0]
             # if self.cell_on_bnd[iC]!=1 : continue
             nrml = self._fnormals[iFb]
             frame, a = SphericalHarmonics.project_to_frame(self.var[9*iC:9*(iC+1)], stop_threshold=1e-3, nrml_cstr=nrml)
             self.var[9*iC:9*(iC+1)] = a
             self.frames[iC] = frame
             
     def _laplacian(self):
@@ -192,15 +192,15 @@
                 cols += [9*iC + _c for _c in range(9)]
                 coeffs += [1]*9
                 cstrRHS += [self.var[9*iC+_c] for _c in range(9)]
                 ncstr += 9
 
         for iFb in self._boundary_mesh.id_faces:
             iF = self.mesh.boundary_connectivity.b2m_face[iFb]
-            iC = self.mesh.connectivity.face_to_cell(iF)[0]
+            iC = self.mesh.connectivity.face_to_cells(iF)[0]
             if self._cell_on_bnd[iC] != 1 : 
                 continue
             axis = geom.cross(Z, self._fnormals[iFb])
             angle = geom.angle_2vec3D(Z, self._fnormals[iFb])
             if axis.norm()>1e-8: 
                 axis = Vec.normalized(axis) * angle
             nrml_frame = SphericalHarmonics.from_vec3(axis)
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/curvature_faces.py` & `mouette-1.2.0/mouette/processing/framefield/curvature_faces.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         super().__init__(supporting_mesh, 4, features, verbose, **kwargs)
         self.curv_mat_faces : np.ndarray = None # shape (|T|,3,3)
 
     def _initialize_curvature(self):
         curv_mat_edges = curvature_matrices(self.mesh)
         adj_e = dict([(e,set()) for e in self.mesh.id_edges])
         for T in self.mesh.id_faces:
-            for T2 in self.mesh.connectivity.face_to_face(T):
-                for e in self.mesh.connectivity.face_to_edge(T2):
+            for T2 in self.mesh.connectivity.face_to_faces(T):
+                for e in self.mesh.connectivity.face_to_edges(T2):
                     adj_e[e].add(T)
 
         self.curv_mat_faces = np.zeros((len(self.mesh.faces),3,3))
         for e in self.mesh.id_edges:
             for T in adj_e[e]:
                 self.curv_mat_faces[T] += curv_mat_edges[e]
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/curvature_vertex.py` & `mouette-1.2.0/mouette/processing/framefield/curvature_vertex.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,41 +5,39 @@
 from ... import geometry as geom
 from ...utils.maths import *
 from ... import operators
 
 import numpy as np
 import scipy.sparse as sp
 from scipy.sparse import linalg
-try:
-    from numba import jit, prange
-    
-    @jit(parallel=True, nopython=True)
-    def aggregate_mats(curvV, curvE, areas, iV,iE, n):
-        nvert = curvV.shape[0]
-        total_area = np.zeros(nvert, dtype=np.float64)
-        for i in prange(n):
-            v,e = iV[i], iE[i]
-            curvV[v,:,:] += areas[e]*curvE[e,:,:]
-            total_area[v] += areas[e]
-        for v in prange(nvert):
-            curvV[v,:,:] /= total_area[v]
-        return curvV
-
-except ImportError:
-
-    def aggregate_mats(curvV, curvE, areas, iV,iE, n):
-        nvert = curvV.shape[0]
-        total_area = np.zeros(nvert, dtype=np.float64)
-        for i in range(n):
-            v,e = iV[i], iE[i]
-            curvV[v,:,:] += areas[e]*curvE[e,:,:]
-            total_area[v] += areas[e]
-        for v in range(nvert):
-            curvV[v,:,:] /= total_area[v]
-        return curvV
+from numba import jit, prange
+
+@jit(parallel=True, nopython=True)
+def aggregate_mats(curvV, curvE, areas, iV,iE, n):
+    nvert = curvV.shape[0]
+    total_area = np.zeros(nvert, dtype=np.float64)
+    for i in prange(n):
+        v,e = iV[i], iE[i]
+        curvV[v,:,:] += areas[e]*curvE[e,:,:]
+        total_area[v] += areas[e]
+    for v in prange(nvert):
+        curvV[v,:,:] /= total_area[v]
+    return curvV
+
+# version without numba
+# def aggregate_mats(curvV, curvE, areas, iV,iE, n):
+#     nvert = curvV.shape[0]
+#     total_area = np.zeros(nvert, dtype=np.float64)
+#     for i in range(n):
+#         v,e = iV[i], iE[i]
+#         curvV[v,:,:] += areas[e]*curvE[e,:,:]
+#         total_area[v] += areas[e]
+#     for v in range(nvert):
+#         curvV[v,:,:] /= total_area[v]
+#     return curvV
 
 class PrincipalDirectionsVertices(_BaseFrameField2DVertices):
     """
     Principal curvature direction estimation using a frame field on vertices.
 
     Implementation based on 'Restricted Delaunay Triangulations and Normal Cycle',  David Cohen-Steiner and Jean-Marie Morvan, 2003
     """
@@ -101,15 +99,15 @@
     def _initialize_curv_matrices(self):
         self.log("Aggregate curvature matrices on patches")
         curv_mat_edges = attributes.curvature_matrices(self.mesh)
         self.curv_mat_vert = np.zeros((len(self.mesh.vertices),3,3), dtype=np.float64)
         row,col = self.M.nonzero()
         areas = np.zeros(len(self.mesh.edges), dtype=np.float64)
         for e,(a,b) in enumerate(self.mesh.edges):
-            areas[e] = sum([self.face_areas[_T] for _T in self.mesh.half_edges.edge_to_triangles(a,b) if _T is not None])/2
+            areas[e] = sum([self.face_areas[_T] for _T in self.mesh.connectivity.edge_to_faces(a,b) if _T is not None])/2
         self.curv_mat_vert = aggregate_mats(self.curv_mat_vert, curv_mat_edges, areas, row, col, self.M.count_nonzero())
 
     def initialize(self):
         self._initialize_attributes()
         self._build_patch_connectivity_matrix()
         self._initialize_curv_matrices()
         self._initialize_variables()
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/faces2d.py` & `mouette-1.2.0/mouette/processing/framefield/faces2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def _initialize_variables(self):
         self.var = np.zeros(len(self.mesh.faces), dtype=complex)
 
         # fix orientation on features
         for e in self.feat.feature_edges:
             e1,e2 = self.mesh.edges[e] # the edge on border
             edge = self.mesh.vertices[e2] - self.mesh.vertices[e1]
-            for T in self.mesh.half_edges.edge_to_triangles(e1,e2):
+            for T in self.mesh.connectivity.edge_to_faces(e1,e2):
                 if T is None: continue # edge may be on boundary
                 X,Y = self.conn.base(T)
                 c = complex(edge.dot(X), edge.dot(Y)) # compute edge in local basis coordinates (edge.dot(Z) = 0 -> complex number for 2D vector)
                 self.var[T] = (c/abs(c))**4 # c^4 is the same for all four directions of the cross
 
     def _compute_attach_weight(self, A, fail_value=1e-3):
         # A is area weight matrix
@@ -106,15 +106,15 @@
             edge_rot.clear()
         else:
             edge_rot = self.mesh.edges.create_attribute("angles", float, 1, dense=True)
             # the rotation induced by the frame field on every edge
             # if edge is uv, positive orientation is from T(uv) to T(vu)
 
         for ie,(A,B) in enumerate(self.mesh.edges):
-            T1,T2 = self.mesh.half_edges.edge_to_triangles(A,B)
+            T1,T2 = self.mesh.connectivity.edge_to_faces(A,B)
             if T1 is None or T2 is None: continue
             f1,f2 = self.var[T1], self.var[T2] # representation complex for T1 and T2
             
             # parallel transport
             E = self.mesh.vertices[B] - self.mesh.vertices[A]
             X1,Y1 = self.conn.base(T1)
             X2,Y2 = self.conn.base(T2)
@@ -132,15 +132,15 @@
             singuls = self.mesh.vertices.get_attribute(singul_attr_name)
             singuls.clear()
         else:
             singuls = self.mesh.vertices.create_attribute(singul_attr_name, float)
         
         for v in self.mesh.id_vertices:
             angle = self.defect[v]
-            for e in self.mesh.connectivity.vertex_to_edge(v):
+            for e in self.mesh.connectivity.vertex_to_edges(v):
                 u = self.mesh.connectivity.other_edge_end(e,v)
                 angle += edge_rot[e] if u<v else -edge_rot[e]
             if abs(angle)>ZERO_THRESHOLD:
                 singuls[v] = angle*2/pi
 
     def export_as_mesh(self) -> PolyLine:
         """
@@ -196,15 +196,15 @@
         if len(self.feat.feature_vertices)>0: # We have a border / feature elements -> linear solve
             # Build fixed and variable indexes
             self.log("Feature element detected (border and/or feature edges)")
 
             fixed = self.mesh.faces.create_attribute("fixed", bool)
             for ie in self.feat.feature_edges:
                 u,v = self.mesh.edges[ie]
-                T1,T2 = self.mesh.half_edges.edge_to_triangles(u,v)
+                T1,T2 = self.mesh.connectivity.edge_to_faces(u,v)
                 if T1 is not None: fixed[T1] = True
                 if T2 is not None: fixed[T2] = True
             freeInds,fixedInds = [],[]
             for T in self.mesh.id_faces:
                 if fixed[T] : fixedInds.append(T)
                 else: freeInds.append(T)
               
@@ -280,22 +280,22 @@
         ### Optimize for rotations between frames
         n_cstr = len(self.mesh.vertices)
         n_rot = len(self.mesh.edges)
         CstMat = sp.lil_matrix((n_cstr,n_rot))
         CstX = np.zeros(n_cstr)
         r = 0
         for v in self.mesh.interior_vertices:
-            for e in self.mesh.connectivity.vertex_to_edge(v):
+            for e in self.mesh.connectivity.vertex_to_edges(v):
                 v2 = self.mesh.connectivity.other_edge_end(e,v)
                 CstMat[r,e] = 1 if v<v2 else -1
             CstX[r] = self.defect[v] - self.singus[v] * 2 * pi / self.order
             r += 1
 
         for v in self.mesh.boundary_vertices:
-            for v2 in self.mesh.connectivity.vertex_to_vertex(v):
+            for v2 in self.mesh.connectivity.vertex_to_vertices(v):
                 if self.mesh.is_edge_on_border(v,v2): continue
                 e = self.mesh.connectivity.edge_id(v,v2)
                 CstMat[r,e] = 1 if v<v2 else -1
             CstX[r] = self.defect[v] - (2 - self.feat.corners[v]) * 2 * pi / self.order
             r += 1
         
         instance = OSQP()
@@ -303,28 +303,28 @@
         res = instance.solve()
         if res.info.status != "solved":
             raise Exception(f"Solver exited with status '{res.info.status}'. Check validity of singularity indices (Poincarré-Hopf condition)")
         self.rotations = res.x
 
         ### Now rebuild frame field along a tree
         for _e0 in self.feat.feature_edges : break # get a feature edge
-        root = [T for T in self.mesh.half_edges.edge_to_triangles(*self.mesh.edges[_e0]) if T is not None][0]
+        root = [T for T in self.mesh.connectivity.edge_to_faces(*self.mesh.edges[_e0]) if T is not None][0]
         tree = trees.FaceSpanningTree(self.mesh, root)()
         for face,parent in tree.traverse():
             if parent is None: # root
                 self.var[face] = complex(1., 0.)
                 continue
             zp = self.var[parent]
-            ea,eb = self.mesh.half_edges.common_edge(parent,face)
+            ea,eb = self.mesh.connectivity.common_edge(parent,face)
             ea,eb = min(ea,eb),max(ea,eb)
             e = self.mesh.connectivity.edge_id(ea,eb)
             X1,Y1 = self.conn.base(parent)
             X2,Y2 = self.conn.base(face)
             # T1 -> T2 : angle of e in basis of T2 - angle of e in basis of T1
             E = self.mesh.vertices[eb] - self.mesh.vertices[ea]
             angle1 = atan2( geom.dot(E,Y1), geom.dot(E,X1))
             angle2 = atan2( geom.dot(E,Y2), geom.dot(E,X2))
             pt = utils.maths.principal_angle(angle2 - angle1)
-            w = self.rotations[e] if self.mesh.half_edges.adj(ea,eb)[0]==parent else -self.rotations[e]
+            w = self.rotations[e] if self.mesh.connectivity.direct_face(ea,eb)==parent else -self.rotations[e]
             zf = zp * cmath.rect(1, 4*(w + pt))
             self.var[face] = zf
         self.smoothed = True
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/framefield.py` & `mouette-1.2.0/mouette/processing/framefield/framefield.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         smooth_normals : Whether to initialize the frame field as a mean of adjacent feature edges (True), or following one of the edges (False). has no effect for frame field on faces. Defaults to True.
 
         verbose (bool, optional): verbose mode. Defaults to False.
         
         singularity_indices (Attribute, optional): custom singularity indices for the frame field. If provided, will use the algorithm described in [3] to get the smoothest frame field with these singularities.
             If elements is "vertices", the attribute should be indexed by the faces (where singularities appear)
             If elements is "faces", the attribute should be indexed by the vertices
-            /!\ Indices should respect the Poincarré-Hopf theorem. Defaults to None.
+            /!\\ Indices should respect the Poincarré-Hopf theorem. Defaults to None.
         
         custom_connection (SurfaceConnection, optional): custom connection object to be used for parallel transport. If not provided, a connection will be automatically computed (see SurfaceConnection class). Defaults to None.
         
         custom_feature (FeatureEdgeDetector, optional): custom feature edges to be used in frame field optimization. If not provided, feature edges will be automatically detected. If the 'features' flag is set to False, features of this object are ignored. Defaults to None.
 
     Raises:
         InvalidRangeArgumentError: 'order' should be >= 1
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/vertex2d.py` & `mouette-1.2.0/mouette/processing/framefield/vertex2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from .base import FrameField
 from ...mesh.mesh_attributes import ArrayAttribute, Attribute, Attribute
 from ...mesh.datatypes import *
 from ... import operators, utils, attributes, processing
 from...utils import maths
 from ..features import FeatureEdgeDetector
-from ..connection import SurfaceConnectionVertices
+from ..connection import SurfaceConnectionVertices, FlatConnectionVertices
 from ... import geometry as geom
 from ...optimize import inverse_power_method
 
 from math import pi
-from copy import copy
 import numpy as np
 import cmath
 import scipy.sparse as sp
 from scipy.sparse import linalg
 from osqp import OSQP
 
 class _BaseFrameField2DVertices(FrameField):
```

### Comparing `mouette-1.1.7/mouette/processing/framefield/vertex3d.py` & `mouette-1.2.0/mouette/processing/framefield/vertex3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,18 +239,18 @@
         bary_tri = attributes.face_barycenter(self.mesh, persistent=False)
 
         n = 0
         for Tri in self.mesh.id_faces:
             if abs(self.singuls[Tri])>1e-2:
                 # triangle is singular
                 if self.mesh.is_face_on_border(Tri):
-                    Tet = self.mesh.connectivity.face_to_cell(Tri)[0]
+                    Tet = self.mesh.connectivity.face_to_cells(Tri)[0]
                     singu_graph.vertices += [bary_tri[Tri], bary_tet[Tet]]
                 else:
-                    T1, T2 = self.mesh.connectivity.face_to_cell(Tri)
+                    T1, T2 = self.mesh.connectivity.face_to_cells(Tri)
                     singu_graph.vertices += [bary_tet[T1], bary_tet[T2]]
                 singu_graph.edges.append((2*n, 2*n+1))
                 singuls_on_graph[n] = self.singuls[Tri]
                 n += 1
         return singu_graph
 
     def export_as_mesh(self) -> SurfaceMesh:
```

### Comparing `mouette-1.1.7/mouette/processing/misc.py` & `mouette-1.2.0/mouette/processing/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ..mesh.datatypes import *
+from ..mesh.subdivision import SurfaceSubdivision
 from ..attributes.misc_vertices import degree
 from ..operators.laplacian_op import laplacian
 from ..geometry import distance
-from .combinatorics import SurfaceSubdivision
 
 import numpy as np
 import scipy.sparse as sp
 
 @allowed_mesh_types(SurfaceMesh)
 def split_double_boundary_edges_triangles(mesh : SurfaceMesh) -> SurfaceMesh:
     """
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/base.py` & `mouette-1.2.0/mouette/processing/parametrization/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         mesh : SurfaceMesh, 
         verbose : bool = True, 
         **kwargs
     ):
         super().__init__(name, verbose)
         self.mesh : SurfaceMesh = mesh
         self.save_on_corners : bool = kwargs.get("save_on_corners", True)
-        self.uvs : ArrayAttribute = kwargs.get("uv_attr", None) # attribute on corners or faces
+        self.uvs : ArrayAttribute = kwargs.get("uv_attr", None) # attribute on corners or vertices
 
         self._flat_mesh : SurfaceMesh = None
 
     @abstractmethod
     def run(self):
         pass
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/cone_param.py` & `mouette-1.2.0/mouette/processing/parametrization/cone_param.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self._frames = np.zeros(len(self.mesh.faces), dtype=complex)
 
         ## Determine the root of the tree traversal. Should be a boundary face if possible
         tree_root = 0  
         edge_root = None # A boundary edge to be aligned vertically or horizontally
         if len(self.mesh.boundary_edges)>0:
             edge_root = self.mesh.boundary_edges[0]
-            tree_root = [_T for _T in self.mesh.half_edges.edge_to_triangles(*self.mesh.edges[edge_root]) if _T is not None][0]
+            tree_root = [_T for _T in self.mesh.connectivity.edge_to_faces(*self.mesh.edges[edge_root]) if _T is not None][0]
 
         ## Perform tree traversal and integrate the scale factor
         tree = FaceSpanningTree(self.mesh, starting_face=tree_root, forbidden_edges=self._cutter.cut_edges)() # traverse the faces but avoid seams
         for face,parent in tree.traverse():
             if parent is None: # the tree root
                 if edge_root is None:
                     self._frames[face] = complex(1.,0.)
@@ -95,38 +95,38 @@
                     A,B = self.mesh.edges[edge_root]
                     E = self.mesh.vertices[B] - self.mesh.vertices[A]
                     X,Y = self._conn.base(face)
                     c = complex(E.dot(X), E.dot(Y)) # edge in local basis coordinates
                     self._frames[face] = c/abs(c) # the edge gives the global frame reference
                 continue
 
-            A,B = self.mesh.half_edges.common_edge(face,parent)
+            A,B = self.mesh.connectivity.common_edge(face,parent)
             e = self.mesh.connectivity.edge_id(A,B)
             w = cot[e]* (self._scale_factor[B] - self._scale_factor[A])
-            if self.mesh.half_edges.adj(A,B)[0]==face: 
+            if self.mesh.connectivity.direct_face(A,B)==face: 
                 w*=-1 # w is an oriented dual 1-form
             pt = self._conn.transport(face,parent)
             self._frames[face] = cmath.rect(1, w+pt) * self._frames[parent]
 
 
         self.log("Compute scaled edges in parameter space")
         scale_edges = np.zeros(2*len(self.cut_mesh.edges), dtype=float)
         cot = attributes.cotan_weights(self.cut_mesh, dense=True, persistent=False)
         for e,(A,B) in enumerate(self.cut_mesh.edges):
             rA,rB = self._cutter.ref_vertex[A], self._cutter.ref_vertex[B]
             E = self.mesh.vertices[rB] - self.mesh.vertices[rA]
             sce = np.exp( (self._scale_factor[rA] + self._scale_factor[rB])/2) # discrete scale factor of edge
             if self.cut_mesh.is_edge_on_border(A,B):
-                T = [_T for _T in self.cut_mesh.half_edges.edge_to_triangles(A,B) if _T is not None][0]
+                T = [_T for _T in self.cut_mesh.connectivity.edge_to_faces(A,B) if _T is not None][0]
                 X,Y = self._conn.base(T)
                 ET = complex(X.dot(E), Y.dot(E))
                 ET = ET / self._frames[T]
                 scale_edges[2*e:2*e+2] = cot[e] * sce * Vec(ET.real, ET.imag)
             else:
-                T1,T2 = self.cut_mesh.half_edges.edge_to_triangles(A,B)
+                T1,T2 = self.cut_mesh.connectivity.edge_to_faces(A,B)
                 X1,Y1 = self._conn.base(T1)
                 ET1 = complex(X1.dot(E), Y1.dot(E))
                 ET1 = ET1 / self._frames[T1]
                 X2,Y2 = self._conn.base(T2)
                 ET2 = complex(X2.dot(E), Y2.dot(E))
                 ET2 = ET2 / self._frames[T2]
                 mean = (ET1+ET2)/2
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/cotan_emb.py` & `mouette-1.2.0/mouette/processing/parametrization/cotan_emb.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     return 0.5 * x/ (y**0.75)
 
 class CotanEmbedding(BaseParametrization):
     """
     Given a parametrization of a disk where boundary is fixed, we can optimize the difference between unsigned and signed areas of triangles to compute a parametrization that is foldover-free.
 
     References:
-        Embedding a triangular graph within a given boundary, Xu et al. (2011)
+        [1] _Embedding a triangular graph within a given boundary_, Xu et al. (2011)
     """
 
     @allowed_mesh_types(SurfaceMesh)
     def __init__(self, mesh : SurfaceMesh, uv_attr: Attribute, verbose:bool=True, **kwargs):
         """
         Initializing the CotanEmbedding parametrization tool.
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/distortion.py` & `mouette-1.2.0/mouette/processing/parametrization/distortion.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,15 @@
 
                 sig = np.linalg.svd(J, compute_uv=False) # eigenvalues
                 detJ = np.linalg.det(J)
                 
                 if abs(detJ)<1e-8:
                     raise ZeroDivisionError
 
-                normJ = np.linalg.norm(J)
-
-                confDistT = ((normJ**2)/detJ)/2
+                confDistT = (np.trace(np.transpose(J) * J)/detJ)/2
                 self._conformal[T] = confDistT
                 conformalDist += confDistT * area[T] / xy_area
 
                 detJ *= scale_ratio
                 self._det[T] = detJ
                 
                 authDistT = ( detJ + 1 / detJ)/2
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/ff_integration.py` & `mouette-1.2.0/mouette/processing/parametrization/ff_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .base import BaseParametrization
 
 from ...mesh.datatypes import SurfaceMesh,PolyLine
 from ...mesh.mesh_attributes import Attribute
 from ...mesh.mesh import copy
 
-from ..combinatorics.cutting import SingularityCutter
+from ..cutting import SingularityCutter
 from ..connection import SurfaceConnectionFaces
 from ..features import FeatureEdgeDetector
 from ..framefield import FrameField
 from ..trees import FaceSpanningTree
 from ...import attributes
 
 from ... import geometry as geom
@@ -87,15 +87,15 @@
             angles = [utils.maths.angle_diff( cmath.phase(rp), cmath.phase(rf) - self._conn.transport(face,parent)) for rf in utils.maths.roots(self.frame_field[face], 4)]
             abs_angles = [abs(_a) for _a in angles]
             self._matching[face] = np.argmin(abs_angles)
 
     def _compute_jumps(self):
         self.jumps = self.mesh.edges.create_attribute("jump", int)
         for e in self._cutter.cut_edges:
-            T1,T2 = self.mesh.half_edges.edge_to_triangles(*self.mesh.edges[e])
+            T1,T2 = self.mesh.connectivity.edge_to_faces(*self.mesh.edges[e])
             if T1 is None or T2 is None : continue # boundary edge -> no jump
             ff1, ff2 = self.get_ff_dir(T1), self.get_ff_dir(T2)
             jump = utils.maths.angle_diff( cmath.phase(ff1), cmath.phase(ff2) - self._conn.transport(T2,T1))
             self.jumps[e] = round(2*jump/np.pi)%4 # integer multiple of pi/2
 
     def _integrate(self):
         nvar = 4*len(self.mesh.faces) # one 2x2 Jacobian per face
@@ -112,15 +112,15 @@
         rows,cols,vals = [], [], []
         irow = 0
         
         ## Build jump constraint matrix
         for e in self.mesh.id_edges:
             je = self.jumps[e]
             A,B = self.mesh.edges[e]
-            T1,T2 = self.mesh.half_edges.edge_to_triangles(A,B)
+            T1,T2 = self.mesh.connectivity.edge_to_faces(A,B)
             if T1 is None or T2 is None : continue # boundary edge
             E = self.mesh.vertices[B] - self.mesh.vertices[A]
             E1 = self._conn.project(E,T1)
             E2 = self._conn.project(E,T2)
             
             # J1 E1 = R^{je} J2 E2
             rows += [irow, irow,   irow+1, irow+1]
@@ -142,15 +142,15 @@
                 vals += [E2.x, E2.y, -E2.x, -E2.y]
             irow += 2
         
         ## Feature edge alignment
         for e in self._feat.feature_edges:
             A,B = self.mesh.edges[e]
             E = self.mesh.vertices[B] - self.mesh.vertices[A] 
-            for T in self.mesh.half_edges.edge_to_triangles(A,B):
+            for T in self.mesh.connectivity.edge_to_faces(A,B):
                 if T is None: continue
                 ET = Vec.normalized(self._conn.project(E,T))
                 zT = self.get_ff_dir(T)
                 zT = Vec(zT.real, zT.imag)
                 # determine the orientation of the feature (horizontal or vertical) in parameter space depending on the matching
                 dtp = round(abs(ET.dot(zT)))
                 rows += [irow, irow]
@@ -218,15 +218,15 @@
                 # build the root
                 pA,pB,pC = build_triangle(T)
                 self.uvs[3*T+0] = pA
                 self.uvs[3*T+1] = pB
                 self.uvs[3*T+2] = pC
                 continue
 
-            A,B = self.mesh.half_edges.common_edge(T,parent) # common vertices
+            A,B = self.mesh.connectivity.common_edge(T,parent) # common vertices
             iA,iB = (self.mesh.connectivity.in_face_index(parent,_u) for _u in (A,B))
             jA,jB = (self.mesh.connectivity.in_face_index(T,_u) for _u in (A,B))
             jC = 3-jA-jB
             
             pA,pB = self.uvs[3*parent+iA], self.uvs[3*parent+iB]
             q = build_triangle(T)
             qA,qB,qC = q[jA], q[jB], q[jC]
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/lscm.py` & `mouette-1.2.0/mouette/processing/parametrization/lscm.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 class LSCM(BaseParametrization):
     """
     Least-Square Conformal Map algorithm for computing a parametrization of a mesh.
     /!\\ The mesh should have the topology of a disk.
     Computed UVs are stored in the self.uvs container
 
     References:
-        - [1] Least Squares Conformal Maps for Automatic Texture Atlas Generation, Levy et al. (2002)
-        - [2] Spectral Conformal Parameterization, Mullen et al. (2008)
-        - See also : Intrinsic Parameterizations of Surface Meshes, Desbrun et al. (2002)
+        - [1] _Least Squares Conformal Maps for Automatic Texture Atlas Generation_, Levy et al. (2002)
+        - [2] _Spectral Conformal Parameterization_, Mullen et al. (2008)
+        - [3] _Intrinsic Parameterizations of Surface Meshes_, Desbrun et al. (2002)
     """
 
     @allowed_mesh_types(SurfaceMesh)
     def __init__(self, mesh : SurfaceMesh, verbose : bool=True, **kwargs):
         """
         Initializes the LSCM parametrization tool.
```

### Comparing `mouette-1.1.7/mouette/processing/parametrization/tutte.py` & `mouette-1.2.0/mouette/processing/parametrization/tutte.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 class TutteEmbedding(BaseParametrization):
     """
     Tutte's embedding parametrization method for a disk inside a fixed boundary.
     The parametrization is locally injective (Floater, 1997) provided the boundary is convex.
 
     References:
-        [1] How to draw a graph, Tutte, 1963.
+        [1] _How to draw a graph_, Tutte, 1963.
         
-        [2] Parametrization and smooth approximation of surface triangulations, Floater, 1996.
+        [2] _Parametrization and smooth approximation of surface triangulations_, Floater, 1996.
     """
 
     class BoundaryMode(Enum):
         """
         Enum that represents the shape of the boundary curve.
         """
         CIRCLE = 0
@@ -81,18 +81,18 @@
 
         U = linalg.spsolve(LI, -LB.dot(Ubnd))
         V = linalg.spsolve(LI, -LB.dot(Vbnd))
 
         if self.save_on_corners:
             self.uvs = self.mesh.face_corners.create_attribute("uv_coords", float, 2, dense=True)
             for i,v in enumerate(freeInds):
-                for c in self.mesh.connectivity.vertex_to_corner(v):
+                for c in self.mesh.connectivity.vertex_to_corners(v):
                     self.uvs[c] = Vec(U[i], V[i])
             for i,v in enumerate(bndInds):
-                for c in self.mesh.connectivity.vertex_to_corner(v):
+                for c in self.mesh.connectivity.vertex_to_corners(v):
                     self.uvs[c] = Vec(Ubnd[i], Vbnd[i])
         else:
             self.uvs = self.mesh.vertices.create_attribute("uv_coords", float, 2, dense=True)
             for i,v in enumerate(freeInds):
                 self.uvs[v] = Vec(U[i], V[i])
             for i,v in enumerate(bndInds):
                 self.uvs[v] = Vec(Ubnd[i], Vbnd[i])
```

### Comparing `mouette-1.1.7/mouette/processing/paths.py` & `mouette-1.2.0/mouette/processing/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     # Run Dijkstra's algorithm
     queue.push(start, 0.)
     while not queue.empty():
         v = queue.get().x
         if visited[v] : continue
         visited[v] = True
-        for nv in mesh.connectivity.vertex_to_vertex(v):
+        for nv in mesh.connectivity.vertex_to_vertices(v):
             d = distance[v] + edge_length(v,nv)
             if distance[nv] > d:
                 distance[nv] = d
                 path[nv] = v
             if not visited[nv]:
                 queue.push(nv, distance[nv])
     
@@ -228,8 +228,8 @@
     Returns:
        list: The list of vertices on shortest path
        If export_path_mesh is set to True, also returns a Polyline
     """
     if len(mesh.boundary_vertices)==0:
         raise Exception("Mesh has no border")
     
-    return shortest_path_to_vertex_set(mesh, start, mesh.boundary_vertices, weights, export_path_mesh)[1] # ignore first argument (id of vertex)
+    return shortest_path_to_vertex_set(mesh, start, mesh.boundary_vertices, weights, export_path_mesh)[1:] # ignore first argument (id of vertex)
```

### Comparing `mouette-1.1.7/mouette/processing/space_partition/quadtree.py` & `mouette-1.2.0/mouette/space_partition/quadtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ...mesh.datatypes import *
-from ...mesh.mesh_data import DataContainer, RawMeshData
-from ...geometry import Vec, BB2D
+from ..mesh.datatypes import *
+from ..mesh.mesh_data import DataContainer, RawMeshData
+from ..geometry import Vec, BB2D
 import numpy as np
 
 from dataclasses import dataclass
 from enum import Enum
 
 # class SpacePartitionTree:
```

### Comparing `mouette-1.1.7/mouette/processing/trees/base.py` & `mouette-1.2.0/mouette/processing/trees/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/processing/trees/cell_sp.py` & `mouette-1.2.0/mouette/processing/trees/cell_sp.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/processing/trees/edge_sp.py` & `mouette-1.2.0/mouette/processing/trees/edge_sp.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def compute(self):
         dist_to_root = [float("inf") for v in self.mesh.id_vertices]
         seen = [False for v in self.mesh.id_vertices]
         queue = deque()
 
         def put_neighbours_in_queue(v):
-            for nv in self.mesh.connectivity.vertex_to_vertex(v):
+            for nv in self.mesh.connectivity.vertex_to_vertices(v):
                 if (not seen[nv]) and (not self._avoid_edge(v,nv)):
                     queue.append((v,nv))
         
         put_neighbours_in_queue(self.root)
         dist_to_root[self.root] = 0
         seen[self.root] = True
```

### Comparing `mouette-1.1.7/mouette/processing/trees/face_sp.py` & `mouette-1.2.0/mouette/processing/trees/face_sp.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
     def compute(self):
         dist_to_root = [float("inf") for v in self.mesh.id_faces]
         seen = [False for v in self.mesh.id_faces]
         queue = deque()
 
         def put_neighbours_in_queue(f):
-            for e in self.mesh.connectivity.face_to_edge(f):
+            for e in self.mesh.connectivity.face_to_edges(f):
                 if e not in self.forbidden_edges:
                     a,b = self.mesh.edges[e]
-                    nf = self.mesh.half_edges.opposite(a,b,f)[0]
+                    nf = self.mesh.connectivity.opposite_face(a,b,f)
                     if (nf is not None) and (not seen[nf]):
                         queue.append((f,nf))
         
         put_neighbours_in_queue(self.root)
         dist_to_root[self.root] = 0
         seen[self.root] = True
 
@@ -61,15 +61,15 @@
                 self.children[p].append(f)
                 self.edges.append( keyify(p,f))
         super().compute() # sets the 'computed' flag
 
     def build_tree_as_polyline(self):
         output = PolyLine()
         if self.mesh.faces.has_attribute("barycenter"):
-            bary = self.mesh.faces.attribute("barycenter")
+            bary = self.mesh.faces.get_attribute("barycenter")
         else:
             bary = face_barycenter(self.mesh)
         for iF in self.mesh.id_faces:
             output.vertices.append(bary[iF])
             if self.parent[iF] is not None:
                 output.edges.append([iF, self.parent[iF]])
         return output
```

### Comparing `mouette-1.1.7/mouette/utils/argument_check.py` & `mouette-1.2.0/mouette/utils/argument_check.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/utils/iterators.py` & `mouette-1.2.0/mouette/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/utils/maths.py` & `mouette-1.2.0/mouette/utils/maths.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/utils/priority_queue.py` & `mouette-1.2.0/mouette/utils/priority_queue.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/utils/unionfind.py` & `mouette-1.2.0/mouette/utils/unionfind.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette/utils/utilities.py` & `mouette-1.2.0/mouette/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.7/mouette.egg-info/PKG-INFO` & `mouette-1.2.0/mouette.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouette
-Version: 1.1.7
+Version: 1.2.0
 Summary: Mesh, Tools and Geometry Processing
 Home-page: https://github.com/GCoiffier/mouette
 Author: GCoiffier
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mouette-1.1.7/mouette.egg-info/SOURCES.txt` & `mouette-1.2.0/mouette.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 mouette/__init__.py
 mouette/config.py
+mouette/sampling.py
 mouette.egg-info/PKG-INFO
 mouette.egg-info/SOURCES.txt
 mouette.egg-info/dependency_links.txt
 mouette.egg-info/requires.txt
 mouette.egg-info/top_level.txt
 mouette/attributes/__init__.py
 mouette/attributes/glob.py
 mouette/attributes/interpolate.py
 mouette/attributes/misc_cells.py
 mouette/attributes/misc_corners.py
 mouette/attributes/misc_edges.py
 mouette/attributes/misc_faces.py
 mouette/attributes/misc_vertices.py
+mouette/attributes/uv_export.py
 mouette/geometry/SphericalHarmonics.py
 mouette/geometry/__init__.py
 mouette/geometry/aabb.py
 mouette/geometry/geometry.py
 mouette/geometry/rotations.py
 mouette/geometry/transform.py
 mouette/geometry/vector.py
 mouette/mesh/__init__.py
+mouette/mesh/data_container.py
 mouette/mesh/mesh.py
 mouette/mesh/mesh_attributes.py
 mouette/mesh/mesh_data.py
+mouette/mesh/subdivision.py
 mouette/mesh/datatypes/__init__.py
 mouette/mesh/datatypes/base.py
 mouette/mesh/datatypes/linear.py
 mouette/mesh/datatypes/pointcloud.py
 mouette/mesh/datatypes/surface.py
 mouette/mesh/datatypes/type_checks.py
 mouette/mesh/datatypes/volume.py
 mouette/mesh/io/__init__.py
 mouette/mesh/io/geogram_ascii.py
 mouette/mesh/io/io.py
 mouette/mesh/io/medit.py
 mouette/mesh/io/obj.py
 mouette/mesh/io/off.py
+mouette/mesh/io/ply.py
 mouette/mesh/io/stl.py
 mouette/mesh/io/tet.py
 mouette/mesh/io/xyz.py
 mouette/operators/__init__.py
 mouette/operators/adjacency.py
 mouette/operators/gradient.py
 mouette/operators/laplacian_op.py
 mouette/optimize/__init__.py
 mouette/optimize/eigensolve.py
 mouette/optimize/levenberg_marquardt.py
 mouette/procedural/__init__.py
-mouette/procedural/cylinder.py
-mouette/procedural/hexahedra.py
-mouette/procedural/platonic.py
+mouette/procedural/flat.py
 mouette/procedural/rings.py
-mouette/procedural/sphere.py
+mouette/procedural/shapes.py
+mouette/procedural/transform.py
 mouette/processing/__init__.py
 mouette/processing/border.py
 mouette/processing/connection.py
+mouette/processing/cutting.py
 mouette/processing/expmap.py
 mouette/processing/features.py
 mouette/processing/misc.py
 mouette/processing/paths.py
-mouette/processing/sampling.py
 mouette/processing/worker.py
-mouette/processing/combinatorics/__init__.py
-mouette/processing/combinatorics/cutting.py
-mouette/processing/combinatorics/subdivide.py
 mouette/processing/framefield/__init__.py
 mouette/processing/framefield/base.py
 mouette/processing/framefield/cells.py
 mouette/processing/framefield/curvature_faces.py
 mouette/processing/framefield/curvature_vertex.py
 mouette/processing/framefield/faces2d.py
 mouette/processing/framefield/framefield.py
@@ -82,21 +83,26 @@
 mouette/processing/parametrization/base.py
 mouette/processing/parametrization/cone_param.py
 mouette/processing/parametrization/cotan_emb.py
 mouette/processing/parametrization/distortion.py
 mouette/processing/parametrization/ff_integration.py
 mouette/processing/parametrization/lscm.py
 mouette/processing/parametrization/tutte.py
-mouette/processing/space_partition/__init__.py
-mouette/processing/space_partition/quadtree.py
+mouette/processing/parametrization/winslow.py
 mouette/processing/trees/__init__.py
 mouette/processing/trees/base.py
 mouette/processing/trees/cell_sp.py
 mouette/processing/trees/edge_sp.py
 mouette/processing/trees/face_sp.py
+mouette/space_partition/__init__.py
+mouette/space_partition/quadtree.py
+mouette/splines/__init__.py
+mouette/splines/bezier_curve.py
+mouette/splines/bezier_surface.py
+mouette/splines/evaluate.py
 mouette/utils/__init__.py
 mouette/utils/argument_check.py
 mouette/utils/iterators.py
 mouette/utils/maths.py
 mouette/utils/osqp_lin_solve.py
 mouette/utils/priority_queue.py
 mouette/utils/unionfind.py
```

### Comparing `mouette-1.1.7/pyproject.toml` & `mouette-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "osqp"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mouette"
-version = "1.1.7"
+version = "1.2.0"
 authors = [
   { name="Guillaume Coiffier" },
 ]
 description = "Geometry Processing and mesh handling in python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
@@ -28,13 +28,15 @@
 dependencies = [
   "aenum",
   "tqdm",
   "numpy",
   "scipy",
   "osqp",
   "mkdocstrings[python]>=0.18",
+  "stl-reader",
+  "plyfile"
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/GCoiffier/mouette"
 "Documentation" = "https://GCoiffier.github.io/mouette"
```

### Comparing `mouette-1.1.7/setup.py` & `mouette-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as file_handle:
     long_description = file_handle.read()
 
 setuptools.setup(
     name="mouette",
-    version='1.1.7',
+    version='1.2.0',
     author="GCoiffier",
     description="Mesh, Tools and Geometry Processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GCoiffier/mouette",
     license="MIT",
     packages=setuptools.find_packages(),
     install_requires=[
         "aenum",
         'numpy',
-        'stl-reader',
         'scipy',
         'osqp',
         'tqdm',
+        'stl-reader',
+        "plyfile",
     ]
 )
```

