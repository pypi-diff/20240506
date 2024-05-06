# Comparing `tmp/nrel-bird-0.0.4.tar.gz` & `tmp/nrel_bird-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrel-bird-0.0.4.tar", last modified: Fri Mar  1 00:36:03 2024, max compression
+gzip compressed data, was "nrel_bird-0.0.5.tar", last modified: Mon May  6 16:09:26 2024, max compression
```

## Comparing `nrel-bird-0.0.4.tar` & `nrel_bird-0.0.5.tar`

### file list

```diff
@@ -1,128 +1,134 @@
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.257013 nrel-bird-0.0.4/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1523 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/LICENSE
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    10050 2024-03-01 00:36:03.256706 nrel-bird-0.0.4/PKG-INFO
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     9211 2024-03-01 00:33:39.000000 nrel-bird-0.0.4/README.md
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.242656 nrel-bird-0.0.4/bird/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      733 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/__init__.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.243509 nrel-bird-0.0.4/bird/meshing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12016 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/_mesh_tools.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4295 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/_stir_tank_reactor.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    17267 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.240710 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.244005 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1308 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      835 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1144 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.244331 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      803 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      550 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.244662 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1164 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      829 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.244987 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1215 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1669 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.245314 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1043 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      834 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.245639 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1216 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.245969 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1044 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      840 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.246289 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1125 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1163 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.246622 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1217 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.246936 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2769 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.247273 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2815 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.247591 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.247927 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1690 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.248251 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1969 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2572 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.248580 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.248917 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.249251 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.249585 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2273 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1938 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.249907 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1288 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.250236 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1289 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.250558 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.250883 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.251208 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.251529 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.251857 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.252183 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    26151 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/stir_tank_mesh.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.240897 nrel-bird-0.0.4/bird/meshing/stir_tank_mesh_templates/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.252350 nrel-bird-0.0.4/bird/meshing/stir_tank_mesh_templates/base_tank/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      824 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4337 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/meshing/stl_mesh_tools.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.252671 nrel-bird-0.0.4/bird/postProcess/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.252832 nrel-bird-0.0.4/bird/postProcess/computeQoI/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6108 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/postProcess/computeQoI/compute_QOI.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4573 2024-02-29 16:42:42.000000 nrel-bird-0.0.4/bird/postProcess/conditional_mean.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.253368 nrel-bird-0.0.4/bird/postProcess/data_early/
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    13092 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/postProcess/data_early/150rpm_1e8.csv
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    16781 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/postProcess/data_early/150rpm_5e7.csv
--rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    48787 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/postProcess/data_early/240rpm_1e8.csv
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     9024 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/postProcess/early_pred.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.241414 nrel-bird-0.0.4/bird/preprocess/
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.253761 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6539 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/main.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6003 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/main_rep.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.254089 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/util/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1803 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3839 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-03-01 00:31:36.000000 nrel-bird-0.0.4/bird/requirements.txt
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.255050 nrel-bird-0.0.4/bird/utilities/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7182 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/bubble_col_util.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      976 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/folderManagement.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1894 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/label_plot.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1194 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/mathtools.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4751 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/ofio.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1430 2024-02-29 16:42:44.000000 nrel-bird-0.0.4/bird/utilities/stl_plotting.py
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       56 2024-03-01 00:34:47.000000 nrel-bird-0.0.4/bird/version.py
-drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-03-01 00:36:03.256348 nrel-bird-0.0.4/nrel_bird.egg-info/
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    10050 2024-03-01 00:36:03.000000 nrel-bird-0.0.4/nrel_bird.egg-info/PKG-INFO
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4732 2024-03-01 00:36:03.000000 nrel-bird-0.0.4/nrel_bird.egg-info/SOURCES.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        1 2024-03-01 00:36:03.000000 nrel-bird-0.0.4/nrel_bird.egg-info/dependency_links.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-03-01 00:36:03.000000 nrel-bird-0.0.4/nrel_bird.egg-info/requires.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        5 2024-03-01 00:36:03.000000 nrel-bird-0.0.4/nrel_bird.egg-info/top_level.txt
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       38 2024-03-01 00:36:03.257075 nrel-bird-0.0.4/setup.cfg
--rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1446 2024-03-01 00:31:36.000000 nrel-bird-0.0.4/setup.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.624543 nrel_bird-0.0.5/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1523 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/LICENSE
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12888 2024-05-06 16:09:26.624232 nrel_bird-0.0.5/PKG-INFO
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12049 2024-05-06 15:49:30.000000 nrel_bird-0.0.5/README.md
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.605468 nrel_bird-0.0.5/bird/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      923 2024-05-06 14:51:11.000000 nrel_bird-0.0.5/bird/__init__.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.607144 nrel_bird-0.0.5/bird/meshing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12016 2024-05-06 14:57:17.000000 nrel_bird-0.0.5/bird/meshing/_mesh_tools.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4295 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/_stir_tank_reactor.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    17267 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.602645 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.607829 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1308 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      835 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1144 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.608201 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      803 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      550 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.608574 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1164 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      829 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.608929 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1215 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1669 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.609315 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1043 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      834 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.610001 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1216 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.610399 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1044 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      840 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.610797 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1125 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1163 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.611168 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1217 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.611508 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2769 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.611840 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2815 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3943 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.612170 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.612505 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1690 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.612882 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1969 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2572 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.613264 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.613609 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2247 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3176 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.613947 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2524 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3797 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.614299 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     2273 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1938 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.614627 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1288 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.614974 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1289 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.615297 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.615617 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1249 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1374 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.615963 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.616364 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1722 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1973 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.616708 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.617054 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1287 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1600 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7158 2024-05-06 14:57:17.000000 nrel_bird-0.0.5/bird/meshing/block_rect_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.602934 nrel_bird-0.0.5/bird/meshing/block_rect_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.617220 nrel_bird-0.0.5/bird/meshing/block_rect_mesh_templates/loopReactor/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      535 2024-05-06 14:34:40.000000 nrel_bird-0.0.5/bird/meshing/block_rect_mesh_templates/loopReactor/input.json
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.617390 nrel_bird-0.0.5/bird/meshing/block_rect_mesh_templates/sub_blocks/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      541 2024-05-06 15:19:34.000000 nrel_bird-0.0.5/bird/meshing/block_rect_mesh_templates/sub_blocks/input.json
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    26151 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/stir_tank_mesh.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.603139 nrel_bird-0.0.5/bird/meshing/stir_tank_mesh_templates/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.617556 nrel_bird-0.0.5/bird/meshing/stir_tank_mesh_templates/base_tank/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      824 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4337 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/meshing/stl_mesh_tools.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.617927 nrel_bird-0.0.5/bird/postProcess/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.618321 nrel_bird-0.0.5/bird/postProcess/computeQoI/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6108 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/postProcess/computeQoI/compute_QOI.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4573 2024-05-03 20:29:34.000000 nrel_bird-0.0.5/bird/postProcess/conditional_mean.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.619163 nrel_bird-0.0.5/bird/postProcess/data_early/
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    13092 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/postProcess/data_early/150rpm_1e8.csv
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    16781 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/postProcess/data_early/150rpm_5e7.csv
+-rwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    48787 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/postProcess/data_early/240rpm_1e8.csv
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     9024 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/postProcess/early_pred.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.603686 nrel_bird-0.0.5/bird/preprocess/
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.619619 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6539 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/main.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     6003 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/main_rep.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.619975 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/util/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1803 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     3839 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/requirements.txt
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.621307 nrel_bird-0.0.5/bird/utilities/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     7182 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/bubble_col_util.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)      976 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/folderManagement.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1894 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/label_plot.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1194 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/mathtools.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4751 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/ofio.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1430 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/bird/utilities/stl_plotting.py
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       56 2024-05-06 15:53:10.000000 nrel_bird-0.0.5/bird/version.py
+drwxr-xr-x   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        0 2024-05-06 16:09:26.623362 nrel_bird-0.0.5/nrel_bird.egg-info/
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)    12888 2024-05-06 16:09:26.000000 nrel_bird-0.0.5/nrel_bird.egg-info/PKG-INFO
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     4887 2024-05-06 16:09:26.000000 nrel_bird-0.0.5/nrel_bird.egg-info/SOURCES.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        1 2024-05-06 16:09:26.000000 nrel_bird-0.0.5/nrel_bird.egg-info/dependency_links.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       72 2024-05-06 16:09:26.000000 nrel_bird-0.0.5/nrel_bird.egg-info/requires.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)        5 2024-05-06 16:09:26.000000 nrel_bird-0.0.5/nrel_bird.egg-info/top_level.txt
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)       38 2024-05-06 16:09:26.624606 nrel_bird-0.0.5/setup.cfg
+-rw-r--r--   0 mhassana (786209005) NREL_NT\Domain Users (18434217)     1446 2024-05-03 20:29:35.000000 nrel_bird-0.0.5/setup.py
```

### Comparing `nrel-bird-0.0.4/LICENSE` & `nrel_bird-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/PKG-INFO` & `nrel_bird-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: nrel-bird
-Version: 0.0.4
-Summary: Bio Reactor Design (BiRD): a toolbox to simulate and analyze different designs of bioreactors in OpenFOAM
-Home-page: https://github.com/NREL/BioReactorDesign
-Author: Malik Hassanaly
-License: BSD 3-Clause
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: prettyPlot>=0.0.27
-Requires-Dist: ruamel_yaml
-Requires-Dist: numpy-stl
-Requires-Dist: scipy
-Requires-Dist: corner
-Requires-Dist: jax
-Requires-Dist: numpyro
-
 # <ins>Bi</ins>o <ins>R</ins>eactor <ins>D</ins>esign (BiRD) Toolbox [![bird-CI](https://github.com/NREL/BioReactorDesign/actions/workflows/ci.yml/badge.svg)](https://github.com/NREL/BioReactorDesign/actions/workflows/ci.yml) [![bird-pyversion](https://img.shields.io/pypi/pyversions/NREL-bird.svg)](https://pypi.org/project/NREL-bird/)  [![bird-pypi](https://badge.fury.io/py/nrel-bird.svg)](https://badge.fury.io/py/nrel-bird)
 
 ## Installation for developers
 
 ```bash
 conda create --name bird python=3.10
 conda activate bird
@@ -214,14 +189,63 @@
 options:
   -h, --help            show this help message and exit
   -i , --input_file     Input file for meshing and geometry parameters
   -t , --topo_file      Block description of the configuration
   -o , --output_folder 
                         Output folder for blockMeshDict
 ```
+
+
+### Block rectangular meshing
+
+Generates `blockMeshDict` in `system`
+
+```bash
+root=`pwd`
+caseFolder=bird/meshing/block_rect_cases_templates/case
+mesh_temp=bird/meshing/block_rect_mesh_templates/loopReactor
+
+python applications/write_block_rect_mesh.py -i $mesh_temp/input.json -o $caseFolder/system
+```
+
+Then activate openFoam environment (tested with OpenFoam9) and mesh with
+
+```bash
+cd $caseFolder
+blockMesh
+cd $root
+```
+
+Will generate this
+
+<p float="left">
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="250"/>
+</p>
+
+
+#### How to change the block rectangular geometry
+
+The geometry of the block cylindrical mesh is defined within a 3D domain (X,Y,Z). The blocks that represent the fluid domain are a subset of a block rectangular background domain. The fluid blocks are defined using the geometry corners. For the mesh shown above, the geometry corners are the red blocks shown below 
+
+<p float="left">
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loop_schematic.png" width="250"/>
+</p>
+ 
+The corners are defined in the `input.json`
+```
+"Geometry": {
+        "Fluids": [
+                [ [0,0,0], [9,0,0], [9,0,4], [0,0,4] ],
+                [ [0,1,4], [0,4,4], [0,4,0], [0,1,0] ]
+        ]
+}
+...
+```
+
+
 ## Postprocess
 
 ### Perform early prediction
 
 `python applications/earlyPredicition.py -df bird/postProcess/data_early`
 
 Generates
@@ -292,17 +316,47 @@
 Fix imports and format : `pip install black isort; bash fixFormat.sh`
 
 Spelling is checked but not automatically fixed using `codespell`
 
 
 ## References
 
-Coming soon
+Software record [SWR 24-35](https://www.osti.gov/biblio/2319227)
 
-SWR-24-35 "BiRD (BioReactorDesign)"
+To cite BioReactorDesign use these articles on [CO2 interphase mass transfer (open access)](https://arxiv.org/pdf/2404.19636) on [aerobic bioreactors](https://www.sciencedirect.com/science/article/pii/S0263876218304337) 
+and on [butanediol synthesis](https://www.sciencedirect.com/science/article/pii/S0263876223004689)
+```
+@article{hassanaly2024inverse,
+  title={Inverse modeling of bubble size dynamics for interphase mass transfer and gas holdup in CO2 bubble column reactors},
+  author={Hassanaly, Malik and Parra-Alvarez, John M. and Rahimi, Mohammad J. and Sitaraman, Hariswaran},
+  journal={Under Review},
+  year={2024},
+}
+
+
+@article{rahimi2018computational,
+  title={Computational fluid dynamics study of full-scale aerobic bioreactors: Evaluation of gas--liquid mass transfer, oxygen uptake, and dynamic oxygen distribution},
+  author={Rahimi, Mohammad J and Sitaraman, Hariswaran and Humbird, David and Stickel, Jonathan J},
+  journal={Chemical Engineering Research and Design},
+  volume={139},
+  pages={283--295},
+  year={2018},
+  publisher={Elsevier}
+}
+
+@article{sitaraman2023reacting,
+  title={A reacting multiphase computational flow model for 2, 3-butanediol synthesis in industrial-scale bioreactors},
+  author={Sitaraman, Hariswaran and Lischeske, James and Lu, Yimin and Stickel, Jonathan},
+  journal={Chemical Engineering Research and Design},
+  volume={197},
+  pages={38--52},
+  year={2023},
+  publisher={Elsevier}
+}
+```
 
 ## Acknowledgments
 
-This work was authored by the National Renewable Energy Laboratory (NREL), operated by Alliance for Sustainable Energy, LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This work was supported by funding from DOE's Bioenergy Technologies Office (BETO) program. The research was performed using computational resources sponsored by the Department of Energy's Office of Energy Efficiency and Renewable Energy and located at the National Renewable Energy Laboratory. The views expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S. Government retains and the publisher, by accepting the article for publication, acknowledges that the U.S. Government retains a nonexclusive, paid-up, irrevocable, worldwide license to publish or reproduce the published form of this work, or allow others to do so, for U.S. Government purposes.
+This work was authored by the National Renewable Energy Laboratory (NREL), operated by Alliance for Sustainable Energy, LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This work was supported by funding from DOE Bioenergy Technologies Office (BETO) [CO2RUe consortium](https://www.energy.gov/eere/co2rue). The research was performed using computational resources sponsored by the Department of Energy's Office of Energy Efficiency and Renewable Energy and located at the National Renewable Energy Laboratory. The views expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S. Government retains and the publisher, by accepting the article for publication, acknowledges that the U.S. Government retains a nonexclusive, paid-up, irrevocable, worldwide license to publish or reproduce the published form of this work, or allow others to do so, for U.S. Government purposes.
```

### Comparing `nrel-bird-0.0.4/bird/__init__.py` & `nrel_bird-0.0.5/bird/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 BIRD_POST_DIR = os.path.join(BIRD_DIR, "postProcess")
 BIRD_BLOCK_CYL_MESH_TEMP_DIR = os.path.join(
     BIRD_MESH_DIR, "block_cyl_mesh_templates"
 )
 BIRD_BLOCK_CYL_CASE_TEMP_DIR = os.path.join(
     BIRD_MESH_DIR, "block_cyl_case_templates"
 )
+BIRD_BLOCK_RECT_MESH_TEMP_DIR = os.path.join(
+    BIRD_MESH_DIR, "block_rect_mesh_templates"
+)
+BIRD_BLOCK_RECT_CASE_TEMP_DIR = os.path.join(
+    BIRD_MESH_DIR, "block_rect_case_templates"
+)
 BIRD_STIR_TANK_MESH_TEMP_DIR = os.path.join(
     BIRD_MESH_DIR, "stir_tank_mesh_templates"
 )
 BIRD_STIR_TANK_CASE_TEMP_DIR = os.path.join(
     BIRD_MESH_DIR, "stir_tank_case_templates"
 )
 BIRD_EARLY_PRED_DATA_DIR = os.path.join(BIRD_POST_DIR, "data_early")
```

### Comparing `nrel-bird-0.0.4/bird/meshing/_mesh_tools.py` & `nrel_bird-0.0.5/bird/meshing/_mesh_tools.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/_stir_tank_reactor.py` & `nrel_bird-0.0.5/bird/meshing/_stir_tank_reactor.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh.py` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/baseColumn_refineSparg/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/circle_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_slot/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/flatDonut_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple2/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple3/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple4_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple5/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/multiRing_simple_projected/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/sideSparger_widerBCR/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_flatDonut_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json` & `nrel_bird-0.0.5/bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/stir_tank_mesh.py` & `nrel_bird-0.0.5/bird/meshing/stir_tank_mesh.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml` & `nrel_bird-0.0.5/bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/meshing/stl_mesh_tools.py` & `nrel_bird-0.0.5/bird/meshing/stl_mesh_tools.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/computeQoI/compute_QOI.py` & `nrel_bird-0.0.5/bird/postProcess/computeQoI/compute_QOI.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/conditional_mean.py` & `nrel_bird-0.0.5/bird/postProcess/conditional_mean.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/data_early/150rpm_1e8.csv` & `nrel_bird-0.0.5/bird/postProcess/data_early/150rpm_1e8.csv`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/data_early/150rpm_5e7.csv` & `nrel_bird-0.0.5/bird/postProcess/data_early/150rpm_5e7.csv`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/data_early/240rpm_1e8.csv` & `nrel_bird-0.0.5/bird/postProcess/data_early/240rpm_1e8.csv`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/postProcess/early_pred.py` & `nrel_bird-0.0.5/bird/postProcess/early_pred.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/main.py` & `nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/main.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/main_rep.py` & `nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/main_rep.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py` & `nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/util/argument_inhomo.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py` & `nrel_bird-0.0.5/bird/preprocess/inhomogeneousBC/util/fromMomtoPdf.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/bubble_col_util.py` & `nrel_bird-0.0.5/bird/utilities/bubble_col_util.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/folderManagement.py` & `nrel_bird-0.0.5/bird/utilities/folderManagement.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/label_plot.py` & `nrel_bird-0.0.5/bird/utilities/label_plot.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/mathtools.py` & `nrel_bird-0.0.5/bird/utilities/mathtools.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/ofio.py` & `nrel_bird-0.0.5/bird/utilities/ofio.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/bird/utilities/stl_plotting.py` & `nrel_bird-0.0.5/bird/utilities/stl_plotting.py`

 * *Files identical despite different names*

### Comparing `nrel-bird-0.0.4/nrel_bird.egg-info/PKG-INFO` & `nrel_bird-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrel-bird
-Version: 0.0.4
+Version: 0.0.5
 Summary: Bio Reactor Design (BiRD): a toolbox to simulate and analyze different designs of bioreactors in OpenFOAM
 Home-page: https://github.com/NREL/BioReactorDesign
 Author: Malik Hassanaly
 License: BSD 3-Clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -214,14 +214,63 @@
 options:
   -h, --help            show this help message and exit
   -i , --input_file     Input file for meshing and geometry parameters
   -t , --topo_file      Block description of the configuration
   -o , --output_folder 
                         Output folder for blockMeshDict
 ```
+
+
+### Block rectangular meshing
+
+Generates `blockMeshDict` in `system`
+
+```bash
+root=`pwd`
+caseFolder=bird/meshing/block_rect_cases_templates/case
+mesh_temp=bird/meshing/block_rect_mesh_templates/loopReactor
+
+python applications/write_block_rect_mesh.py -i $mesh_temp/input.json -o $caseFolder/system
+```
+
+Then activate openFoam environment (tested with OpenFoam9) and mesh with
+
+```bash
+cd $caseFolder
+blockMesh
+cd $root
+```
+
+Will generate this
+
+<p float="left">
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/assets/loop_react.png" width="250"/>
+</p>
+
+
+#### How to change the block rectangular geometry
+
+The geometry of the block cylindrical mesh is defined within a 3D domain (X,Y,Z). The blocks that represent the fluid domain are a subset of a block rectangular background domain. The fluid blocks are defined using the geometry corners. For the mesh shown above, the geometry corners are the red blocks shown below 
+
+<p float="left">
+  <img src="https://raw.githubusercontent.com/NREL/BioReactorDesign/main/bird/meshing/block_rect_mesh_templates/loop_schematic.png" width="250"/>
+</p>
+ 
+The corners are defined in the `input.json`
+```
+"Geometry": {
+        "Fluids": [
+                [ [0,0,0], [9,0,0], [9,0,4], [0,0,4] ],
+                [ [0,1,4], [0,4,4], [0,4,0], [0,1,0] ]
+        ]
+}
+...
+```
+
+
 ## Postprocess
 
 ### Perform early prediction
 
 `python applications/earlyPredicition.py -df bird/postProcess/data_early`
 
 Generates
@@ -292,17 +341,47 @@
 Fix imports and format : `pip install black isort; bash fixFormat.sh`
 
 Spelling is checked but not automatically fixed using `codespell`
 
 
 ## References
 
-Coming soon
+Software record [SWR 24-35](https://www.osti.gov/biblio/2319227)
 
-SWR-24-35 "BiRD (BioReactorDesign)"
+To cite BioReactorDesign use these articles on [CO2 interphase mass transfer (open access)](https://arxiv.org/pdf/2404.19636) on [aerobic bioreactors](https://www.sciencedirect.com/science/article/pii/S0263876218304337) 
+and on [butanediol synthesis](https://www.sciencedirect.com/science/article/pii/S0263876223004689)
+```
+@article{hassanaly2024inverse,
+  title={Inverse modeling of bubble size dynamics for interphase mass transfer and gas holdup in CO2 bubble column reactors},
+  author={Hassanaly, Malik and Parra-Alvarez, John M. and Rahimi, Mohammad J. and Sitaraman, Hariswaran},
+  journal={Under Review},
+  year={2024},
+}
+
+
+@article{rahimi2018computational,
+  title={Computational fluid dynamics study of full-scale aerobic bioreactors: Evaluation of gas--liquid mass transfer, oxygen uptake, and dynamic oxygen distribution},
+  author={Rahimi, Mohammad J and Sitaraman, Hariswaran and Humbird, David and Stickel, Jonathan J},
+  journal={Chemical Engineering Research and Design},
+  volume={139},
+  pages={283--295},
+  year={2018},
+  publisher={Elsevier}
+}
+
+@article{sitaraman2023reacting,
+  title={A reacting multiphase computational flow model for 2, 3-butanediol synthesis in industrial-scale bioreactors},
+  author={Sitaraman, Hariswaran and Lischeske, James and Lu, Yimin and Stickel, Jonathan},
+  journal={Chemical Engineering Research and Design},
+  volume={197},
+  pages={38--52},
+  year={2023},
+  publisher={Elsevier}
+}
+```
 
 ## Acknowledgments
 
-This work was authored by the National Renewable Energy Laboratory (NREL), operated by Alliance for Sustainable Energy, LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This work was supported by funding from DOE's Bioenergy Technologies Office (BETO) program. The research was performed using computational resources sponsored by the Department of Energy's Office of Energy Efficiency and Renewable Energy and located at the National Renewable Energy Laboratory. The views expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S. Government retains and the publisher, by accepting the article for publication, acknowledges that the U.S. Government retains a nonexclusive, paid-up, irrevocable, worldwide license to publish or reproduce the published form of this work, or allow others to do so, for U.S. Government purposes.
+This work was authored by the National Renewable Energy Laboratory (NREL), operated by Alliance for Sustainable Energy, LLC, for the U.S. Department of Energy (DOE) under Contract No. DE-AC36-08GO28308. This work was supported by funding from DOE Bioenergy Technologies Office (BETO) [CO2RUe consortium](https://www.energy.gov/eere/co2rue). The research was performed using computational resources sponsored by the Department of Energy's Office of Energy Efficiency and Renewable Energy and located at the National Renewable Energy Laboratory. The views expressed in the article do not necessarily represent the views of the DOE or the U.S. Government. The U.S. Government retains and the publisher, by accepting the article for publication, acknowledges that the U.S. Government retains a nonexclusive, paid-up, irrevocable, worldwide license to publish or reproduce the published form of this work, or allow others to do so, for U.S. Government purposes.
```

### Comparing `nrel-bird-0.0.4/nrel_bird.egg-info/SOURCES.txt` & `nrel_bird-0.0.5/nrel_bird.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 bird/__init__.py
 bird/requirements.txt
 bird/version.py
 bird/meshing/_mesh_tools.py
 bird/meshing/_stir_tank_reactor.py
 bird/meshing/block_cyl_mesh.py
+bird/meshing/block_rect_mesh.py
 bird/meshing/stir_tank_mesh.py
 bird/meshing/stl_mesh_tools.py
 bird/meshing/block_cyl_mesh_templates/baseColumn/input.json
 bird/meshing/block_cyl_mesh_templates/baseColumn/input.yaml
 bird/meshing/block_cyl_mesh_templates/baseColumn/topology.json
 bird/meshing/block_cyl_mesh_templates/baseColumn_projected/input.json
 bird/meshing/block_cyl_mesh_templates/baseColumn_projected/topology.json
@@ -58,14 +59,16 @@
 bird/meshing/block_cyl_mesh_templates/template_multiRing/topology.json
 bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/input.json
 bird/meshing/block_cyl_mesh_templates/template_multiRing_coarse/topology.json
 bird/meshing/block_cyl_mesh_templates/template_sideSparger/input.json
 bird/meshing/block_cyl_mesh_templates/template_sideSparger/topology.json
 bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/input.json
 bird/meshing/block_cyl_mesh_templates/template_sideSparger_coarse/topology.json
+bird/meshing/block_rect_mesh_templates/loopReactor/input.json
+bird/meshing/block_rect_mesh_templates/sub_blocks/input.json
 bird/meshing/stir_tank_mesh_templates/base_tank/tank_par.yaml
 bird/postProcess/conditional_mean.py
 bird/postProcess/early_pred.py
 bird/postProcess/computeQoI/compute_QOI.py
 bird/postProcess/data_early/150rpm_1e8.csv
 bird/postProcess/data_early/150rpm_5e7.csv
 bird/postProcess/data_early/240rpm_1e8.csv
```

### Comparing `nrel-bird-0.0.4/setup.py` & `nrel_bird-0.0.5/setup.py`

 * *Files identical despite different names*

