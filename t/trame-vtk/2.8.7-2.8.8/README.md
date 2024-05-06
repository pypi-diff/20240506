# Comparing `tmp/trame-vtk-2.8.7.tar.gz` & `tmp/trame-vtk-2.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.8.7.tar", last modified: Thu May  2 14:02:57 2024, max compression
+gzip compressed data, was "trame-vtk-2.8.8.tar", last modified: Mon May  6 21:42:02 2024, max compression
```

## Comparing `trame-vtk-2.8.7.tar` & `trame-vtk-2.8.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/
--rw-r--r--   0 root         (0) root         (0)     1504 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12924 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12189 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.730570 trame-vtk-2.8.7/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/tools/vtksz2html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1655508 2024-05-02 14:02:55.000000 trame-vtk-2.8.7/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.738570 trame-vtk-2.8.7/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7043 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.738570 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5356 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    24014 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.738570 trame-vtk-2.8.7/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     6729 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.742570 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.742570 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13036 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/cache.py
--rw-r--r--   0 root         (0) root         (0)     6976 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/export.py
--rw-r--r--   0 root         (0) root         (0)     5829 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5387 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1528 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     6059 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5436 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      914 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     4050 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/trame_vtk/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)   936161 2024-05-02 14:02:55.000000 trame-vtk-2.8.7/trame_vtk/tools/static_viewer.html
--rw-r--r--   0 root         (0) root         (0)     1713 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/tools/vtksz2html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.746570 trame-vtk-2.8.7/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35119 2024-05-02 14:02:51.000000 trame-vtk-2.8.7/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:02:57.734570 trame-vtk-2.8.7/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12924 2024-05-02 14:02:57.000000 trame-vtk-2.8.7/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-02 14:02:57.000000 trame-vtk-2.8.7/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 14:02:57.000000 trame-vtk-2.8.7/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-02 14:02:57.000000 trame-vtk-2.8.7/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-02 14:02:57.000000 trame-vtk-2.8.7/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.824043 trame-vtk-2.8.8/
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12924 2024-05-06 21:42:02.824043 trame-vtk-2.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12189 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-06 21:42:02.824043 trame-vtk-2.8.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.808043 trame-vtk-2.8.8/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.808043 trame-vtk-2.8.8/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.808043 trame-vtk-2.8.8/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.808043 trame-vtk-2.8.8/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.808043 trame-vtk-2.8.8/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.812043 trame-vtk-2.8.8/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.812043 trame-vtk-2.8.8/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.812043 trame-vtk-2.8.8/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1655508 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.812043 trame-vtk-2.8.8/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7043 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.816043 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    24014 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.816043 trame-vtk-2.8.8/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     6729 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.816043 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.820043 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13036 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/cache.py
+-rw-r--r--   0 root         (0) root         (0)     6976 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5387 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     4050 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.820043 trame-vtk-2.8.8/trame_vtk/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   936224 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/tools/static_viewer.html
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/tools/vtksz2html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.820043 trame-vtk-2.8.8/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.824043 trame-vtk-2.8.8/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35119 2024-05-06 21:42:00.000000 trame-vtk-2.8.8/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 21:42:02.812043 trame-vtk-2.8.8/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12924 2024-05-06 21:42:02.000000 trame-vtk-2.8.8/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-06 21:42:02.000000 trame-vtk-2.8.8/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 21:42:02.000000 trame-vtk-2.8.8/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 21:42:02.000000 trame-vtk-2.8.8/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-06 21:42:02.000000 trame-vtk-2.8.8/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.8.7/LICENSE` & `trame-vtk-2.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/PKG-INFO` & `trame-vtk-2.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.8.7
+Version: 2.8.8
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.8.7/README.rst` & `trame-vtk-2.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/setup.cfg` & `trame-vtk-2.8.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.8.7
+version = 2.8.8
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.8.7/trame_vtk/LICENSE` & `trame-vtk-2.8.8/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.8.8/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.8.8/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/export.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/export.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.8.8/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/tools/static_viewer.html` & `trame-vtk-2.8.8/trame_vtk/tools/static_viewer.html`

 * *Files 0% similar despite different names*

```diff
@@ -58257,255 +58257,258 @@
 000e3900: 6f72 6465 722d 7261 6469 7573 3a20 3130  order-radius: 10
 000e3910: 7078 3b5c 6e20 202d 7765 626b 6974 2d75  px;\n  -webkit-u
 000e3920: 7365 722d 7365 6c65 6374 3a20 6e6f 6e65  ser-select: none
 000e3930: 3b5c 6e20 2020 2020 2d6d 6f7a 2d75 7365  ;\n     -moz-use
 000e3940: 722d 7365 6c65 6374 3a20 6e6f 6e65 3b5c  r-select: none;\
 000e3950: 6e20 2020 2020 2020 2020 2075 7365 722d  n          user-
 000e3960: 7365 6c65 6374 3a20 6e6f 6e65 3b5c 6e7d  select: none;\n}
-000e3970: 5c6e 222c 2222 5d29 2c75 2e6c 6f63 616c  \n",""]),u.local
-000e3980: 733d 7b66 756c 6c53 6372 6565 6e3a 2276  s={fullScreen:"v
-000e3990: 6965 7765 722d 6d6f 6475 6c65 2d66 756c  iewer-module-ful
-000e39a0: 6c53 6372 6565 6e5f 6262 6b39 5922 2c66  lScreen_bbk9Y",f
-000e39b0: 756c 6c50 6172 656e 7453 697a 653a 2276  ullParentSize:"v
-000e39c0: 6965 7765 722d 6d6f 6475 6c65 2d66 756c  iewer-module-ful
-000e39d0: 6c50 6172 656e 7453 697a 655f 4554 6f70  lParentSize_ETop
-000e39e0: 4f22 2c62 6967 4669 6c65 4472 6f70 3a22  O",bigFileDrop:"
-000e39f0: 7669 6577 6572 2d6d 6f64 756c 652d 6269  viewer-module-bi
-000e3a00: 6746 696c 6544 726f 705f 6171 4367 6822  gFileDrop_aqCgh"
-000e3a10: 2c70 726f 6772 6573 733a 2276 6965 7765  ,progress:"viewe
-000e3a20: 722d 6d6f 6475 6c65 2d70 726f 6772 6573  r-module-progres
-000e3a30: 735f 6359 6a51 4a22 7d2c 742e 5a3d 757d  s_cYjQJ"},t.Z=u}
-000e3a40: 2c33 3936 3a66 756e 6374 696f 6e28 652c  ,396:function(e,
-000e3a50: 742c 6e29 7b76 6172 2072 3d6e 2833 3430  t,n){var r=n(340
-000e3a60: 292c 6f3d 6e28 3930 3329 3b76 6f69 6420  ),o=n(903);void 
-000e3a70: 303d 3d3d 6f2e 4f66 666c 696e 654c 6f63  0===o.OfflineLoc
-000e3a80: 616c 5669 6577 2626 286f 2e4f 6666 6c69  alView&&(o.Offli
-000e3a90: 6e65 4c6f 6361 6c56 6965 773d 7229 2c65  neLocalView=r),e
-000e3aa0: 2e65 7870 6f72 7473 3d72 7d2c 3839 323a  .exports=r},892:
-000e3ab0: 6675 6e63 7469 6f6e 2865 297b 2275 7365  function(e){"use
-000e3ac0: 2073 7472 6963 7422 3b76 6172 2074 3d5b   strict";var t=[
-000e3ad0: 5d3b 6675 6e63 7469 6f6e 206e 2865 297b  ];function n(e){
-000e3ae0: 666f 7228 7661 7220 6e3d 2d31 2c72 3d30  for(var n=-1,r=0
-000e3af0: 3b72 3c74 2e6c 656e 6774 683b 722b 2b29  ;r<t.length;r++)
-000e3b00: 6966 2874 5b72 5d2e 6964 656e 7469 6669  if(t[r].identifi
-000e3b10: 6572 3d3d 3d65 297b 6e3d 723b 6272 6561  er===e){n=r;brea
-000e3b20: 6b7d 7265 7475 726e 206e 7d66 756e 6374  k}return n}funct
-000e3b30: 696f 6e20 7228 652c 7229 7b66 6f72 2876  ion r(e,r){for(v
-000e3b40: 6172 2061 3d7b 7d2c 693d 5b5d 2c73 3d30  ar a={},i=[],s=0
-000e3b50: 3b73 3c65 2e6c 656e 6774 683b 732b 2b29  ;s<e.length;s++)
-000e3b60: 7b76 6172 206c 3d65 5b73 5d2c 633d 722e  {var l=e[s],c=r.
-000e3b70: 6261 7365 3f6c 5b30 5d2b 722e 6261 7365  base?l[0]+r.base
-000e3b80: 3a6c 5b30 5d2c 753d 615b 635d 7c7c 302c  :l[0],u=a[c]||0,
-000e3b90: 643d 2222 2e63 6f6e 6361 7428 632c 2220  d="".concat(c," 
-000e3ba0: 2229 2e63 6f6e 6361 7428 7529 3b61 5b63  ").concat(u);a[c
-000e3bb0: 5d3d 752b 313b 7661 7220 703d 6e28 6429  ]=u+1;var p=n(d)
-000e3bc0: 2c66 3d7b 6373 733a 6c5b 315d 2c6d 6564  ,f={css:l[1],med
-000e3bd0: 6961 3a6c 5b32 5d2c 736f 7572 6365 4d61  ia:l[2],sourceMa
-000e3be0: 703a 6c5b 335d 2c73 7570 706f 7274 733a  p:l[3],supports:
-000e3bf0: 6c5b 345d 2c6c 6179 6572 3a6c 5b35 5d7d  l[4],layer:l[5]}
-000e3c00: 3b69 6628 2d31 213d 3d70 2974 5b70 5d2e  ;if(-1!==p)t[p].
-000e3c10: 7265 6665 7265 6e63 6573 2b2b 2c74 5b70  references++,t[p
-000e3c20: 5d2e 7570 6461 7465 7228 6629 3b65 6c73  ].updater(f);els
-000e3c30: 657b 7661 7220 673d 6f28 662c 7229 3b72  e{var g=o(f,r);r
-000e3c40: 2e62 7949 6e64 6578 3d73 2c74 2e73 706c  .byIndex=s,t.spl
-000e3c50: 6963 6528 732c 302c 7b69 6465 6e74 6966  ice(s,0,{identif
-000e3c60: 6965 723a 642c 7570 6461 7465 723a 672c  ier:d,updater:g,
-000e3c70: 7265 6665 7265 6e63 6573 3a31 7d29 7d69  references:1})}i
-000e3c80: 2e70 7573 6828 6429 7d72 6574 7572 6e20  .push(d)}return 
-000e3c90: 697d 6675 6e63 7469 6f6e 206f 2865 2c74  i}function o(e,t
-000e3ca0: 297b 7661 7220 6e3d 742e 646f 6d41 5049  ){var n=t.domAPI
-000e3cb0: 2874 293b 7265 7475 726e 206e 2e75 7064  (t);return n.upd
-000e3cc0: 6174 6528 6529 2c66 756e 6374 696f 6e28  ate(e),function(
-000e3cd0: 7429 7b69 6628 7429 7b69 6628 742e 6373  t){if(t){if(t.cs
-000e3ce0: 733d 3d3d 652e 6373 7326 2674 2e6d 6564  s===e.css&&t.med
-000e3cf0: 6961 3d3d 3d65 2e6d 6564 6961 2626 742e  ia===e.media&&t.
-000e3d00: 736f 7572 6365 4d61 703d 3d3d 652e 736f  sourceMap===e.so
-000e3d10: 7572 6365 4d61 7026 2674 2e73 7570 706f  urceMap&&t.suppo
-000e3d20: 7274 733d 3d3d 652e 7375 7070 6f72 7473  rts===e.supports
-000e3d30: 2626 742e 6c61 7965 723d 3d3d 652e 6c61  &&t.layer===e.la
-000e3d40: 7965 7229 7265 7475 726e 3b6e 2e75 7064  yer)return;n.upd
-000e3d50: 6174 6528 653d 7429 7d65 6c73 6520 6e2e  ate(e=t)}else n.
-000e3d60: 7265 6d6f 7665 2829 7d7d 652e 6578 706f  remove()}}e.expo
-000e3d70: 7274 733d 6675 6e63 7469 6f6e 2865 2c6f  rts=function(e,o
-000e3d80: 297b 7661 7220 613d 7228 653d 657c 7c5b  ){var a=r(e=e||[
-000e3d90: 5d2c 6f3d 6f7c 7c7b 7d29 3b72 6574 7572  ],o=o||{});retur
-000e3da0: 6e20 6675 6e63 7469 6f6e 2865 297b 653d  n function(e){e=
-000e3db0: 657c 7c5b 5d3b 666f 7228 7661 7220 693d  e||[];for(var i=
-000e3dc0: 303b 693c 612e 6c65 6e67 7468 3b69 2b2b  0;i<a.length;i++
-000e3dd0: 297b 7661 7220 733d 6e28 615b 695d 293b  ){var s=n(a[i]);
-000e3de0: 745b 735d 2e72 6566 6572 656e 6365 732d  t[s].references-
-000e3df0: 2d7d 666f 7228 7661 7220 6c3d 7228 652c  -}for(var l=r(e,
-000e3e00: 6f29 2c63 3d30 3b63 3c61 2e6c 656e 6774  o),c=0;c<a.lengt
-000e3e10: 683b 632b 2b29 7b76 6172 2075 3d6e 2861  h;c++){var u=n(a
-000e3e20: 5b63 5d29 3b30 3d3d 3d74 5b75 5d2e 7265  [c]);0===t[u].re
-000e3e30: 6665 7265 6e63 6573 2626 2874 5b75 5d2e  ferences&&(t[u].
-000e3e40: 7570 6461 7465 7228 292c 742e 7370 6c69  updater(),t.spli
-000e3e50: 6365 2875 2c31 2929 7d61 3d6c 7d7d 7d2c  ce(u,1))}a=l}}},
-000e3e60: 3331 313a 6675 6e63 7469 6f6e 2865 297b  311:function(e){
-000e3e70: 2275 7365 2073 7472 6963 7422 3b76 6172  "use strict";var
-000e3e80: 2074 3d7b 7d3b 652e 6578 706f 7274 733d   t={};e.exports=
-000e3e90: 6675 6e63 7469 6f6e 2865 2c6e 297b 7661  function(e,n){va
-000e3ea0: 7220 723d 6675 6e63 7469 6f6e 2865 297b  r r=function(e){
-000e3eb0: 6966 2876 6f69 6420 303d 3d3d 745b 655d  if(void 0===t[e]
-000e3ec0: 297b 7661 7220 6e3d 646f 6375 6d65 6e74  ){var n=document
-000e3ed0: 2e71 7565 7279 5365 6c65 6374 6f72 2865  .querySelector(e
-000e3ee0: 293b 6966 2877 696e 646f 772e 4854 4d4c  );if(window.HTML
-000e3ef0: 4946 7261 6d65 456c 656d 656e 7426 266e  IFrameElement&&n
-000e3f00: 2069 6e73 7461 6e63 656f 6620 7769 6e64   instanceof wind
-000e3f10: 6f77 2e48 544d 4c49 4672 616d 6545 6c65  ow.HTMLIFrameEle
-000e3f20: 6d65 6e74 2974 7279 7b6e 3d6e 2e63 6f6e  ment)try{n=n.con
-000e3f30: 7465 6e74 446f 6375 6d65 6e74 2e68 6561  tentDocument.hea
-000e3f40: 647d 6361 7463 6828 6529 7b6e 3d6e 756c  d}catch(e){n=nul
-000e3f50: 6c7d 745b 655d 3d6e 7d72 6574 7572 6e20  l}t[e]=n}return 
-000e3f60: 745b 655d 7d28 6529 3b69 6628 2172 2974  t[e]}(e);if(!r)t
-000e3f70: 6872 6f77 206e 6577 2045 7272 6f72 2822  hrow new Error("
-000e3f80: 436f 756c 646e 2774 2066 696e 6420 6120  Couldn't find a 
-000e3f90: 7374 796c 6520 7461 7267 6574 2e20 5468  style target. Th
-000e3fa0: 6973 2070 726f 6261 626c 7920 6d65 616e  is probably mean
-000e3fb0: 7320 7468 6174 2074 6865 2076 616c 7565  s that the value
-000e3fc0: 2066 6f72 2074 6865 2027 696e 7365 7274   for the 'insert
-000e3fd0: 2720 7061 7261 6d65 7465 7220 6973 2069  ' parameter is i
-000e3fe0: 6e76 616c 6964 2e22 293b 722e 6170 7065  nvalid.");r.appe
-000e3ff0: 6e64 4368 696c 6428 6e29 7d7d 2c36 303a  ndChild(n)}},60:
-000e4000: 6675 6e63 7469 6f6e 2865 297b 2275 7365  function(e){"use
-000e4010: 2073 7472 6963 7422 3b65 2e65 7870 6f72   strict";e.expor
-000e4020: 7473 3d66 756e 6374 696f 6e28 6529 7b76  ts=function(e){v
-000e4030: 6172 2074 3d64 6f63 756d 656e 742e 6372  ar t=document.cr
-000e4040: 6561 7465 456c 656d 656e 7428 2273 7479  eateElement("sty
-000e4050: 6c65 2229 3b72 6574 7572 6e20 652e 7365  le");return e.se
-000e4060: 7441 7474 7269 6275 7465 7328 742c 652e  tAttributes(t,e.
-000e4070: 6174 7472 6962 7574 6573 292c 652e 696e  attributes),e.in
-000e4080: 7365 7274 2874 2c65 2e6f 7074 696f 6e73  sert(t,e.options
-000e4090: 292c 747d 7d2c 3139 323a 6675 6e63 7469  ),t}},192:functi
-000e40a0: 6f6e 2865 2c74 2c6e 297b 2275 7365 2073  on(e,t,n){"use s
-000e40b0: 7472 6963 7422 3b65 2e65 7870 6f72 7473  trict";e.exports
-000e40c0: 3d66 756e 6374 696f 6e28 6529 7b76 6172  =function(e){var
-000e40d0: 2074 3d6e 2e6e 633b 7426 2665 2e73 6574   t=n.nc;t&&e.set
-000e40e0: 4174 7472 6962 7574 6528 226e 6f6e 6365  Attribute("nonce
-000e40f0: 222c 7429 7d7d 2c37 3630 3a66 756e 6374  ",t)}},760:funct
-000e4100: 696f 6e28 6529 7b22 7573 6520 7374 7269  ion(e){"use stri
-000e4110: 6374 223b 652e 6578 706f 7274 733d 6675  ct";e.exports=fu
-000e4120: 6e63 7469 6f6e 2865 297b 7661 7220 743d  nction(e){var t=
-000e4130: 652e 696e 7365 7274 5374 796c 6545 6c65  e.insertStyleEle
-000e4140: 6d65 6e74 2865 293b 7265 7475 726e 7b75  ment(e);return{u
-000e4150: 7064 6174 653a 6675 6e63 7469 6f6e 286e  pdate:function(n
-000e4160: 297b 2166 756e 6374 696f 6e28 652c 742c  ){!function(e,t,
-000e4170: 6e29 7b76 6172 2072 3d22 223b 6e2e 7375  n){var r="";n.su
-000e4180: 7070 6f72 7473 2626 2872 2b3d 2240 7375  pports&&(r+="@su
-000e4190: 7070 6f72 7473 2028 222e 636f 6e63 6174  pports (".concat
-000e41a0: 286e 2e73 7570 706f 7274 732c 2229 207b  (n.supports,") {
-000e41b0: 2229 292c 6e2e 6d65 6469 6126 2628 722b  ")),n.media&&(r+
-000e41c0: 3d22 406d 6564 6961 2022 2e63 6f6e 6361  ="@media ".conca
-000e41d0: 7428 6e2e 6d65 6469 612c 2220 7b22 2929  t(n.media," {"))
-000e41e0: 3b76 6172 206f 3d76 6f69 6420 3021 3d3d  ;var o=void 0!==
-000e41f0: 6e2e 6c61 7965 723b 6f26 2628 722b 3d22  n.layer;o&&(r+="
-000e4200: 406c 6179 6572 222e 636f 6e63 6174 286e  @layer".concat(n
-000e4210: 2e6c 6179 6572 2e6c 656e 6774 683e 303f  .layer.length>0?
-000e4220: 2220 222e 636f 6e63 6174 286e 2e6c 6179  " ".concat(n.lay
-000e4230: 6572 293a 2222 2c22 207b 2229 292c 722b  er):""," {")),r+
-000e4240: 3d6e 2e63 7373 2c6f 2626 2872 2b3d 227d  =n.css,o&&(r+="}
-000e4250: 2229 2c6e 2e6d 6564 6961 2626 2872 2b3d  "),n.media&&(r+=
-000e4260: 227d 2229 2c6e 2e73 7570 706f 7274 7326  "}"),n.supports&
-000e4270: 2628 722b 3d22 7d22 293b 7661 7220 613d  &(r+="}");var a=
-000e4280: 6e2e 736f 7572 6365 4d61 703b 6126 2622  n.sourceMap;a&&"
-000e4290: 756e 6465 6669 6e65 6422 213d 7479 7065  undefined"!=type
-000e42a0: 6f66 2062 746f 6126 2628 722b 3d22 5c6e  of btoa&&(r+="\n
-000e42b0: 2f2a 2320 736f 7572 6365 4d61 7070 696e  /*# sourceMappin
-000e42c0: 6755 524c 3d64 6174 613a 6170 706c 6963  gURL=data:applic
-000e42d0: 6174 696f 6e2f 6a73 6f6e 3b62 6173 6536  ation/json;base6
-000e42e0: 342c 222e 636f 6e63 6174 2862 746f 6128  4,".concat(btoa(
-000e42f0: 756e 6573 6361 7065 2865 6e63 6f64 6555  unescape(encodeU
-000e4300: 5249 436f 6d70 6f6e 656e 7428 4a53 4f4e  RIComponent(JSON
-000e4310: 2e73 7472 696e 6769 6679 2861 2929 2929  .stringify(a))))
-000e4320: 2c22 202a 2f22 2929 2c74 2e73 7479 6c65  ," */")),t.style
-000e4330: 5461 6754 7261 6e73 666f 726d 2872 2c65  TagTransform(r,e
-000e4340: 2c74 2e6f 7074 696f 6e73 297d 2874 2c65  ,t.options)}(t,e
-000e4350: 2c6e 297d 2c72 656d 6f76 653a 6675 6e63  ,n)},remove:func
-000e4360: 7469 6f6e 2829 7b21 6675 6e63 7469 6f6e  tion(){!function
-000e4370: 2865 297b 6966 286e 756c 6c3d 3d3d 652e  (e){if(null===e.
-000e4380: 7061 7265 6e74 4e6f 6465 2972 6574 7572  parentNode)retur
-000e4390: 6e21 313b 652e 7061 7265 6e74 4e6f 6465  n!1;e.parentNode
-000e43a0: 2e72 656d 6f76 6543 6869 6c64 2865 297d  .removeChild(e)}
-000e43b0: 2874 297d 7d7d 7d2c 3836 353a 6675 6e63  (t)}}}},865:func
-000e43c0: 7469 6f6e 2865 297b 2275 7365 2073 7472  tion(e){"use str
-000e43d0: 6963 7422 3b65 2e65 7870 6f72 7473 3d66  ict";e.exports=f
-000e43e0: 756e 6374 696f 6e28 652c 7429 7b69 6628  unction(e,t){if(
-000e43f0: 742e 7374 796c 6553 6865 6574 2974 2e73  t.styleSheet)t.s
-000e4400: 7479 6c65 5368 6565 742e 6373 7354 6578  tyleSheet.cssTex
-000e4410: 743d 653b 656c 7365 7b66 6f72 283b 742e  t=e;else{for(;t.
-000e4420: 6669 7273 7443 6869 6c64 3b29 742e 7265  firstChild;)t.re
-000e4430: 6d6f 7665 4368 696c 6428 742e 6669 7273  moveChild(t.firs
-000e4440: 7443 6869 6c64 293b 742e 6170 7065 6e64  tChild);t.append
-000e4450: 4368 696c 6428 646f 6375 6d65 6e74 2e63  Child(document.c
-000e4460: 7265 6174 6554 6578 744e 6f64 6528 6529  reateTextNode(e)
-000e4470: 297d 7d7d 2c33 3532 3a66 756e 6374 696f  )}}},352:functio
-000e4480: 6e28 652c 742c 6e29 7b22 7573 6520 7374  n(e,t,n){"use st
-000e4490: 7269 6374 223b 652e 6578 706f 7274 733d  rict";e.exports=
-000e44a0: 6e2e 702b 2231 3338 6537 6231 3436 3966  n.p+"138e7b1469f
-000e44b0: 3634 3135 3638 3130 612e 6a70 6722 7d2c  64156810a.jpg"},
-000e44c0: 3730 363a 6675 6e63 7469 6f6e 2829 7b7d  706:function(){}
-000e44d0: 7d2c 743d 7b7d 3b66 756e 6374 696f 6e20  },t={};function 
-000e44e0: 6e28 7229 7b76 6172 206f 3d74 5b72 5d3b  n(r){var o=t[r];
-000e44f0: 6966 2876 6f69 6420 3021 3d3d 6f29 7265  if(void 0!==o)re
-000e4500: 7475 726e 206f 2e65 7870 6f72 7473 3b76  turn o.exports;v
-000e4510: 6172 2061 3d74 5b72 5d3d 7b69 643a 722c  ar a=t[r]={id:r,
-000e4520: 6c6f 6164 6564 3a21 312c 6578 706f 7274  loaded:!1,export
-000e4530: 733a 7b7d 7d3b 7265 7475 726e 2065 5b72  s:{}};return e[r
-000e4540: 5d2e 6361 6c6c 2861 2e65 7870 6f72 7473  ].call(a.exports
-000e4550: 2c61 2c61 2e65 7870 6f72 7473 2c6e 292c  ,a,a.exports,n),
-000e4560: 612e 6c6f 6164 6564 3d21 302c 612e 6578  a.loaded=!0,a.ex
-000e4570: 706f 7274 737d 6e2e 6d3d 652c 6e2e 616d  ports}n.m=e,n.am
-000e4580: 6444 3d66 756e 6374 696f 6e28 297b 7468  dD=function(){th
-000e4590: 726f 7720 6e65 7720 4572 726f 7228 2264  row new Error("d
-000e45a0: 6566 696e 6520 6361 6e6e 6f74 2062 6520  efine cannot be 
-000e45b0: 7573 6564 2069 6e64 6972 6563 7422 297d  used indirect")}
-000e45c0: 2c6e 2e61 6d64 4f3d 7b7d 2c6e 2e6e 3d66  ,n.amdO={},n.n=f
-000e45d0: 756e 6374 696f 6e28 6529 7b76 6172 2074  unction(e){var t
-000e45e0: 3d65 2626 652e 5f5f 6573 4d6f 6475 6c65  =e&&e.__esModule
-000e45f0: 3f66 756e 6374 696f 6e28 297b 7265 7475  ?function(){retu
-000e4600: 726e 2065 2e64 6566 6175 6c74 7d3a 6675  rn e.default}:fu
-000e4610: 6e63 7469 6f6e 2829 7b72 6574 7572 6e20  nction(){return 
-000e4620: 657d 3b72 6574 7572 6e20 6e2e 6428 742c  e};return n.d(t,
-000e4630: 7b61 3a74 7d29 2c74 7d2c 6e2e 643d 6675  {a:t}),t},n.d=fu
-000e4640: 6e63 7469 6f6e 2865 2c74 297b 666f 7228  nction(e,t){for(
-000e4650: 7661 7220 7220 696e 2074 296e 2e6f 2874  var r in t)n.o(t
-000e4660: 2c72 2926 2621 6e2e 6f28 652c 7229 2626  ,r)&&!n.o(e,r)&&
-000e4670: 4f62 6a65 6374 2e64 6566 696e 6550 726f  Object.definePro
-000e4680: 7065 7274 7928 652c 722c 7b65 6e75 6d65  perty(e,r,{enume
-000e4690: 7261 626c 653a 2130 2c67 6574 3a74 5b72  rable:!0,get:t[r
-000e46a0: 5d7d 297d 2c6e 2e67 3d66 756e 6374 696f  ]})},n.g=functio
-000e46b0: 6e28 297b 6966 2822 6f62 6a65 6374 223d  n(){if("object"=
-000e46c0: 3d74 7970 656f 6620 676c 6f62 616c 5468  =typeof globalTh
-000e46d0: 6973 2972 6574 7572 6e20 676c 6f62 616c  is)return global
-000e46e0: 5468 6973 3b74 7279 7b72 6574 7572 6e20  This;try{return 
-000e46f0: 7468 6973 7c7c 6e65 7720 4675 6e63 7469  this||new Functi
-000e4700: 6f6e 2822 7265 7475 726e 2074 6869 7322  on("return this"
-000e4710: 2928 297d 6361 7463 6828 6529 7b69 6628  )()}catch(e){if(
-000e4720: 226f 626a 6563 7422 3d3d 7479 7065 6f66  "object"==typeof
-000e4730: 2077 696e 646f 7729 7265 7475 726e 2077   window)return w
-000e4740: 696e 646f 777d 7d28 292c 6e2e 6f3d 6675  indow}}(),n.o=fu
-000e4750: 6e63 7469 6f6e 2865 2c74 297b 7265 7475  nction(e,t){retu
-000e4760: 726e 204f 626a 6563 742e 7072 6f74 6f74  rn Object.protot
-000e4770: 7970 652e 6861 734f 776e 5072 6f70 6572  ype.hasOwnProper
-000e4780: 7479 2e63 616c 6c28 652c 7429 7d2c 6e2e  ty.call(e,t)},n.
-000e4790: 723d 6675 6e63 7469 6f6e 2865 297b 2275  r=function(e){"u
-000e47a0: 6e64 6566 696e 6564 2221 3d74 7970 656f  ndefined"!=typeo
-000e47b0: 6620 5379 6d62 6f6c 2626 5379 6d62 6f6c  f Symbol&&Symbol
-000e47c0: 2e74 6f53 7472 696e 6754 6167 2626 4f62  .toStringTag&&Ob
-000e47d0: 6a65 6374 2e64 6566 696e 6550 726f 7065  ject.definePrope
-000e47e0: 7274 7928 652c 5379 6d62 6f6c 2e74 6f53  rty(e,Symbol.toS
-000e47f0: 7472 696e 6754 6167 2c7b 7661 6c75 653a  tringTag,{value:
-000e4800: 224d 6f64 756c 6522 7d29 2c4f 626a 6563  "Module"}),Objec
-000e4810: 742e 6465 6669 6e65 5072 6f70 6572 7479  t.defineProperty
-000e4820: 2865 2c22 5f5f 6573 4d6f 6475 6c65 222c  (e,"__esModule",
-000e4830: 7b76 616c 7565 3a21 307d 297d 2c6e 2e6e  {value:!0})},n.n
-000e4840: 6d64 3d66 756e 6374 696f 6e28 6529 7b72  md=function(e){r
-000e4850: 6574 7572 6e20 652e 7061 7468 733d 5b5d  eturn e.paths=[]
-000e4860: 2c65 2e63 6869 6c64 7265 6e7c 7c28 652e  ,e.children||(e.
-000e4870: 6368 696c 6472 656e 3d5b 5d29 2c65 7d2c  children=[]),e},
-000e4880: 6e2e 703d 2222 2c6e 2e62 3d64 6f63 756d  n.p="",n.b=docum
-000e4890: 656e 742e 6261 7365 5552 497c 7c73 656c  ent.baseURI||sel
-000e48a0: 662e 6c6f 6361 7469 6f6e 2e68 7265 662c  f.location.href,
-000e48b0: 6e2e 6e63 3d76 6f69 6420 302c 6e28 3339  n.nc=void 0,n(39
-000e48c0: 3629 7d28 293b 0a3c 2f73 6372 6970 743e  6)}();.</script>
-000e48d0: 0a3c 2f62 6f64 793e 0a3c 2f68 746d 6c3e  .</body>.</html>
-000e48e0: 0a                                       .
+000e3970: 5c6e 5c6e 626f 6479 207b 5c6e 2020 6d61  \n\nbody {\n  ma
+000e3980: 7267 696e 3a20 303b 5c6e 7d5c 6e5c 6e68  rgin: 0;\n}\n\nh
+000e3990: 746d 6c20 7b20 5c6e 2020 6f76 6572 666c  tml { \n  overfl
+000e39a0: 6f77 3a20 6869 6464 656e 3b20 5c6e 7d5c  ow: hidden; \n}\
+000e39b0: 6e22 2c22 225d 292c 752e 6c6f 6361 6c73  n",""]),u.locals
+000e39c0: 3d7b 6675 6c6c 5363 7265 656e 3a22 7669  ={fullScreen:"vi
+000e39d0: 6577 6572 2d6d 6f64 756c 652d 6675 6c6c  ewer-module-full
+000e39e0: 5363 7265 656e 5f62 626b 3959 222c 6675  Screen_bbk9Y",fu
+000e39f0: 6c6c 5061 7265 6e74 5369 7a65 3a22 7669  llParentSize:"vi
+000e3a00: 6577 6572 2d6d 6f64 756c 652d 6675 6c6c  ewer-module-full
+000e3a10: 5061 7265 6e74 5369 7a65 5f45 546f 704f  ParentSize_ETopO
+000e3a20: 222c 6269 6746 696c 6544 726f 703a 2276  ",bigFileDrop:"v
+000e3a30: 6965 7765 722d 6d6f 6475 6c65 2d62 6967  iewer-module-big
+000e3a40: 4669 6c65 4472 6f70 5f61 7143 6768 222c  FileDrop_aqCgh",
+000e3a50: 7072 6f67 7265 7373 3a22 7669 6577 6572  progress:"viewer
+000e3a60: 2d6d 6f64 756c 652d 7072 6f67 7265 7373  -module-progress
+000e3a70: 5f63 596a 514a 227d 2c74 2e5a 3d75 7d2c  _cYjQJ"},t.Z=u},
+000e3a80: 3339 363a 6675 6e63 7469 6f6e 2865 2c74  396:function(e,t
+000e3a90: 2c6e 297b 7661 7220 723d 6e28 3334 3029  ,n){var r=n(340)
+000e3aa0: 2c6f 3d6e 2839 3033 293b 766f 6964 2030  ,o=n(903);void 0
+000e3ab0: 3d3d 3d6f 2e4f 6666 6c69 6e65 4c6f 6361  ===o.OfflineLoca
+000e3ac0: 6c56 6965 7726 2628 6f2e 4f66 666c 696e  lView&&(o.Offlin
+000e3ad0: 654c 6f63 616c 5669 6577 3d72 292c 652e  eLocalView=r),e.
+000e3ae0: 6578 706f 7274 733d 727d 2c38 3932 3a66  exports=r},892:f
+000e3af0: 756e 6374 696f 6e28 6529 7b22 7573 6520  unction(e){"use 
+000e3b00: 7374 7269 6374 223b 7661 7220 743d 5b5d  strict";var t=[]
+000e3b10: 3b66 756e 6374 696f 6e20 6e28 6529 7b66  ;function n(e){f
+000e3b20: 6f72 2876 6172 206e 3d2d 312c 723d 303b  or(var n=-1,r=0;
+000e3b30: 723c 742e 6c65 6e67 7468 3b72 2b2b 2969  r<t.length;r++)i
+000e3b40: 6628 745b 725d 2e69 6465 6e74 6966 6965  f(t[r].identifie
+000e3b50: 723d 3d3d 6529 7b6e 3d72 3b62 7265 616b  r===e){n=r;break
+000e3b60: 7d72 6574 7572 6e20 6e7d 6675 6e63 7469  }return n}functi
+000e3b70: 6f6e 2072 2865 2c72 297b 666f 7228 7661  on r(e,r){for(va
+000e3b80: 7220 613d 7b7d 2c69 3d5b 5d2c 733d 303b  r a={},i=[],s=0;
+000e3b90: 733c 652e 6c65 6e67 7468 3b73 2b2b 297b  s<e.length;s++){
+000e3ba0: 7661 7220 6c3d 655b 735d 2c63 3d72 2e62  var l=e[s],c=r.b
+000e3bb0: 6173 653f 6c5b 305d 2b72 2e62 6173 653a  ase?l[0]+r.base:
+000e3bc0: 6c5b 305d 2c75 3d61 5b63 5d7c 7c30 2c64  l[0],u=a[c]||0,d
+000e3bd0: 3d22 222e 636f 6e63 6174 2863 2c22 2022  ="".concat(c," "
+000e3be0: 292e 636f 6e63 6174 2875 293b 615b 635d  ).concat(u);a[c]
+000e3bf0: 3d75 2b31 3b76 6172 2070 3d6e 2864 292c  =u+1;var p=n(d),
+000e3c00: 663d 7b63 7373 3a6c 5b31 5d2c 6d65 6469  f={css:l[1],medi
+000e3c10: 613a 6c5b 325d 2c73 6f75 7263 654d 6170  a:l[2],sourceMap
+000e3c20: 3a6c 5b33 5d2c 7375 7070 6f72 7473 3a6c  :l[3],supports:l
+000e3c30: 5b34 5d2c 6c61 7965 723a 6c5b 355d 7d3b  [4],layer:l[5]};
+000e3c40: 6966 282d 3121 3d3d 7029 745b 705d 2e72  if(-1!==p)t[p].r
+000e3c50: 6566 6572 656e 6365 732b 2b2c 745b 705d  eferences++,t[p]
+000e3c60: 2e75 7064 6174 6572 2866 293b 656c 7365  .updater(f);else
+000e3c70: 7b76 6172 2067 3d6f 2866 2c72 293b 722e  {var g=o(f,r);r.
+000e3c80: 6279 496e 6465 783d 732c 742e 7370 6c69  byIndex=s,t.spli
+000e3c90: 6365 2873 2c30 2c7b 6964 656e 7469 6669  ce(s,0,{identifi
+000e3ca0: 6572 3a64 2c75 7064 6174 6572 3a67 2c72  er:d,updater:g,r
+000e3cb0: 6566 6572 656e 6365 733a 317d 297d 692e  eferences:1})}i.
+000e3cc0: 7075 7368 2864 297d 7265 7475 726e 2069  push(d)}return i
+000e3cd0: 7d66 756e 6374 696f 6e20 6f28 652c 7429  }function o(e,t)
+000e3ce0: 7b76 6172 206e 3d74 2e64 6f6d 4150 4928  {var n=t.domAPI(
+000e3cf0: 7429 3b72 6574 7572 6e20 6e2e 7570 6461  t);return n.upda
+000e3d00: 7465 2865 292c 6675 6e63 7469 6f6e 2874  te(e),function(t
+000e3d10: 297b 6966 2874 297b 6966 2874 2e63 7373  ){if(t){if(t.css
+000e3d20: 3d3d 3d65 2e63 7373 2626 742e 6d65 6469  ===e.css&&t.medi
+000e3d30: 613d 3d3d 652e 6d65 6469 6126 2674 2e73  a===e.media&&t.s
+000e3d40: 6f75 7263 654d 6170 3d3d 3d65 2e73 6f75  ourceMap===e.sou
+000e3d50: 7263 654d 6170 2626 742e 7375 7070 6f72  rceMap&&t.suppor
+000e3d60: 7473 3d3d 3d65 2e73 7570 706f 7274 7326  ts===e.supports&
+000e3d70: 2674 2e6c 6179 6572 3d3d 3d65 2e6c 6179  &t.layer===e.lay
+000e3d80: 6572 2972 6574 7572 6e3b 6e2e 7570 6461  er)return;n.upda
+000e3d90: 7465 2865 3d74 297d 656c 7365 206e 2e72  te(e=t)}else n.r
+000e3da0: 656d 6f76 6528 297d 7d65 2e65 7870 6f72  emove()}}e.expor
+000e3db0: 7473 3d66 756e 6374 696f 6e28 652c 6f29  ts=function(e,o)
+000e3dc0: 7b76 6172 2061 3d72 2865 3d65 7c7c 5b5d  {var a=r(e=e||[]
+000e3dd0: 2c6f 3d6f 7c7c 7b7d 293b 7265 7475 726e  ,o=o||{});return
+000e3de0: 2066 756e 6374 696f 6e28 6529 7b65 3d65   function(e){e=e
+000e3df0: 7c7c 5b5d 3b66 6f72 2876 6172 2069 3d30  ||[];for(var i=0
+000e3e00: 3b69 3c61 2e6c 656e 6774 683b 692b 2b29  ;i<a.length;i++)
+000e3e10: 7b76 6172 2073 3d6e 2861 5b69 5d29 3b74  {var s=n(a[i]);t
+000e3e20: 5b73 5d2e 7265 6665 7265 6e63 6573 2d2d  [s].references--
+000e3e30: 7d66 6f72 2876 6172 206c 3d72 2865 2c6f  }for(var l=r(e,o
+000e3e40: 292c 633d 303b 633c 612e 6c65 6e67 7468  ),c=0;c<a.length
+000e3e50: 3b63 2b2b 297b 7661 7220 753d 6e28 615b  ;c++){var u=n(a[
+000e3e60: 635d 293b 303d 3d3d 745b 755d 2e72 6566  c]);0===t[u].ref
+000e3e70: 6572 656e 6365 7326 2628 745b 755d 2e75  erences&&(t[u].u
+000e3e80: 7064 6174 6572 2829 2c74 2e73 706c 6963  pdater(),t.splic
+000e3e90: 6528 752c 3129 297d 613d 6c7d 7d7d 2c33  e(u,1))}a=l}}},3
+000e3ea0: 3131 3a66 756e 6374 696f 6e28 6529 7b22  11:function(e){"
+000e3eb0: 7573 6520 7374 7269 6374 223b 7661 7220  use strict";var 
+000e3ec0: 743d 7b7d 3b65 2e65 7870 6f72 7473 3d66  t={};e.exports=f
+000e3ed0: 756e 6374 696f 6e28 652c 6e29 7b76 6172  unction(e,n){var
+000e3ee0: 2072 3d66 756e 6374 696f 6e28 6529 7b69   r=function(e){i
+000e3ef0: 6628 766f 6964 2030 3d3d 3d74 5b65 5d29  f(void 0===t[e])
+000e3f00: 7b76 6172 206e 3d64 6f63 756d 656e 742e  {var n=document.
+000e3f10: 7175 6572 7953 656c 6563 746f 7228 6529  querySelector(e)
+000e3f20: 3b69 6628 7769 6e64 6f77 2e48 544d 4c49  ;if(window.HTMLI
+000e3f30: 4672 616d 6545 6c65 6d65 6e74 2626 6e20  FrameElement&&n 
+000e3f40: 696e 7374 616e 6365 6f66 2077 696e 646f  instanceof windo
+000e3f50: 772e 4854 4d4c 4946 7261 6d65 456c 656d  w.HTMLIFrameElem
+000e3f60: 656e 7429 7472 797b 6e3d 6e2e 636f 6e74  ent)try{n=n.cont
+000e3f70: 656e 7444 6f63 756d 656e 742e 6865 6164  entDocument.head
+000e3f80: 7d63 6174 6368 2865 297b 6e3d 6e75 6c6c  }catch(e){n=null
+000e3f90: 7d74 5b65 5d3d 6e7d 7265 7475 726e 2074  }t[e]=n}return t
+000e3fa0: 5b65 5d7d 2865 293b 6966 2821 7229 7468  [e]}(e);if(!r)th
+000e3fb0: 726f 7720 6e65 7720 4572 726f 7228 2243  row new Error("C
+000e3fc0: 6f75 6c64 6e27 7420 6669 6e64 2061 2073  ouldn't find a s
+000e3fd0: 7479 6c65 2074 6172 6765 742e 2054 6869  tyle target. Thi
+000e3fe0: 7320 7072 6f62 6162 6c79 206d 6561 6e73  s probably means
+000e3ff0: 2074 6861 7420 7468 6520 7661 6c75 6520   that the value 
+000e4000: 666f 7220 7468 6520 2769 6e73 6572 7427  for the 'insert'
+000e4010: 2070 6172 616d 6574 6572 2069 7320 696e   parameter is in
+000e4020: 7661 6c69 642e 2229 3b72 2e61 7070 656e  valid.");r.appen
+000e4030: 6443 6869 6c64 286e 297d 7d2c 3630 3a66  dChild(n)}},60:f
+000e4040: 756e 6374 696f 6e28 6529 7b22 7573 6520  unction(e){"use 
+000e4050: 7374 7269 6374 223b 652e 6578 706f 7274  strict";e.export
+000e4060: 733d 6675 6e63 7469 6f6e 2865 297b 7661  s=function(e){va
+000e4070: 7220 743d 646f 6375 6d65 6e74 2e63 7265  r t=document.cre
+000e4080: 6174 6545 6c65 6d65 6e74 2822 7374 796c  ateElement("styl
+000e4090: 6522 293b 7265 7475 726e 2065 2e73 6574  e");return e.set
+000e40a0: 4174 7472 6962 7574 6573 2874 2c65 2e61  Attributes(t,e.a
+000e40b0: 7474 7269 6275 7465 7329 2c65 2e69 6e73  ttributes),e.ins
+000e40c0: 6572 7428 742c 652e 6f70 7469 6f6e 7329  ert(t,e.options)
+000e40d0: 2c74 7d7d 2c31 3932 3a66 756e 6374 696f  ,t}},192:functio
+000e40e0: 6e28 652c 742c 6e29 7b22 7573 6520 7374  n(e,t,n){"use st
+000e40f0: 7269 6374 223b 652e 6578 706f 7274 733d  rict";e.exports=
+000e4100: 6675 6e63 7469 6f6e 2865 297b 7661 7220  function(e){var 
+000e4110: 743d 6e2e 6e63 3b74 2626 652e 7365 7441  t=n.nc;t&&e.setA
+000e4120: 7474 7269 6275 7465 2822 6e6f 6e63 6522  ttribute("nonce"
+000e4130: 2c74 297d 7d2c 3736 303a 6675 6e63 7469  ,t)}},760:functi
+000e4140: 6f6e 2865 297b 2275 7365 2073 7472 6963  on(e){"use stric
+000e4150: 7422 3b65 2e65 7870 6f72 7473 3d66 756e  t";e.exports=fun
+000e4160: 6374 696f 6e28 6529 7b76 6172 2074 3d65  ction(e){var t=e
+000e4170: 2e69 6e73 6572 7453 7479 6c65 456c 656d  .insertStyleElem
+000e4180: 656e 7428 6529 3b72 6574 7572 6e7b 7570  ent(e);return{up
+000e4190: 6461 7465 3a66 756e 6374 696f 6e28 6e29  date:function(n)
+000e41a0: 7b21 6675 6e63 7469 6f6e 2865 2c74 2c6e  {!function(e,t,n
+000e41b0: 297b 7661 7220 723d 2222 3b6e 2e73 7570  ){var r="";n.sup
+000e41c0: 706f 7274 7326 2628 722b 3d22 4073 7570  ports&&(r+="@sup
+000e41d0: 706f 7274 7320 2822 2e63 6f6e 6361 7428  ports (".concat(
+000e41e0: 6e2e 7375 7070 6f72 7473 2c22 2920 7b22  n.supports,") {"
+000e41f0: 2929 2c6e 2e6d 6564 6961 2626 2872 2b3d  )),n.media&&(r+=
+000e4200: 2240 6d65 6469 6120 222e 636f 6e63 6174  "@media ".concat
+000e4210: 286e 2e6d 6564 6961 2c22 207b 2229 293b  (n.media," {"));
+000e4220: 7661 7220 6f3d 766f 6964 2030 213d 3d6e  var o=void 0!==n
+000e4230: 2e6c 6179 6572 3b6f 2626 2872 2b3d 2240  .layer;o&&(r+="@
+000e4240: 6c61 7965 7222 2e63 6f6e 6361 7428 6e2e  layer".concat(n.
+000e4250: 6c61 7965 722e 6c65 6e67 7468 3e30 3f22  layer.length>0?"
+000e4260: 2022 2e63 6f6e 6361 7428 6e2e 6c61 7965   ".concat(n.laye
+000e4270: 7229 3a22 222c 2220 7b22 2929 2c72 2b3d  r):""," {")),r+=
+000e4280: 6e2e 6373 732c 6f26 2628 722b 3d22 7d22  n.css,o&&(r+="}"
+000e4290: 292c 6e2e 6d65 6469 6126 2628 722b 3d22  ),n.media&&(r+="
+000e42a0: 7d22 292c 6e2e 7375 7070 6f72 7473 2626  }"),n.supports&&
+000e42b0: 2872 2b3d 227d 2229 3b76 6172 2061 3d6e  (r+="}");var a=n
+000e42c0: 2e73 6f75 7263 654d 6170 3b61 2626 2275  .sourceMap;a&&"u
+000e42d0: 6e64 6566 696e 6564 2221 3d74 7970 656f  ndefined"!=typeo
+000e42e0: 6620 6274 6f61 2626 2872 2b3d 225c 6e2f  f btoa&&(r+="\n/
+000e42f0: 2a23 2073 6f75 7263 654d 6170 7069 6e67  *# sourceMapping
+000e4300: 5552 4c3d 6461 7461 3a61 7070 6c69 6361  URL=data:applica
+000e4310: 7469 6f6e 2f6a 736f 6e3b 6261 7365 3634  tion/json;base64
+000e4320: 2c22 2e63 6f6e 6361 7428 6274 6f61 2875  ,".concat(btoa(u
+000e4330: 6e65 7363 6170 6528 656e 636f 6465 5552  nescape(encodeUR
+000e4340: 4943 6f6d 706f 6e65 6e74 284a 534f 4e2e  IComponent(JSON.
+000e4350: 7374 7269 6e67 6966 7928 6129 2929 292c  stringify(a)))),
+000e4360: 2220 2a2f 2229 292c 742e 7374 796c 6554  " */")),t.styleT
+000e4370: 6167 5472 616e 7366 6f72 6d28 722c 652c  agTransform(r,e,
+000e4380: 742e 6f70 7469 6f6e 7329 7d28 742c 652c  t.options)}(t,e,
+000e4390: 6e29 7d2c 7265 6d6f 7665 3a66 756e 6374  n)},remove:funct
+000e43a0: 696f 6e28 297b 2166 756e 6374 696f 6e28  ion(){!function(
+000e43b0: 6529 7b69 6628 6e75 6c6c 3d3d 3d65 2e70  e){if(null===e.p
+000e43c0: 6172 656e 744e 6f64 6529 7265 7475 726e  arentNode)return
+000e43d0: 2131 3b65 2e70 6172 656e 744e 6f64 652e  !1;e.parentNode.
+000e43e0: 7265 6d6f 7665 4368 696c 6428 6529 7d28  removeChild(e)}(
+000e43f0: 7429 7d7d 7d7d 2c38 3635 3a66 756e 6374  t)}}}},865:funct
+000e4400: 696f 6e28 6529 7b22 7573 6520 7374 7269  ion(e){"use stri
+000e4410: 6374 223b 652e 6578 706f 7274 733d 6675  ct";e.exports=fu
+000e4420: 6e63 7469 6f6e 2865 2c74 297b 6966 2874  nction(e,t){if(t
+000e4430: 2e73 7479 6c65 5368 6565 7429 742e 7374  .styleSheet)t.st
+000e4440: 796c 6553 6865 6574 2e63 7373 5465 7874  yleSheet.cssText
+000e4450: 3d65 3b65 6c73 657b 666f 7228 3b74 2e66  =e;else{for(;t.f
+000e4460: 6972 7374 4368 696c 643b 2974 2e72 656d  irstChild;)t.rem
+000e4470: 6f76 6543 6869 6c64 2874 2e66 6972 7374  oveChild(t.first
+000e4480: 4368 696c 6429 3b74 2e61 7070 656e 6443  Child);t.appendC
+000e4490: 6869 6c64 2864 6f63 756d 656e 742e 6372  hild(document.cr
+000e44a0: 6561 7465 5465 7874 4e6f 6465 2865 2929  eateTextNode(e))
+000e44b0: 7d7d 7d2c 3335 323a 6675 6e63 7469 6f6e  }}},352:function
+000e44c0: 2865 2c74 2c6e 297b 2275 7365 2073 7472  (e,t,n){"use str
+000e44d0: 6963 7422 3b65 2e65 7870 6f72 7473 3d6e  ict";e.exports=n
+000e44e0: 2e70 2b22 3133 3865 3762 3134 3639 6636  .p+"138e7b1469f6
+000e44f0: 3431 3536 3831 3061 2e6a 7067 227d 2c37  4156810a.jpg"},7
+000e4500: 3036 3a66 756e 6374 696f 6e28 297b 7d7d  06:function(){}}
+000e4510: 2c74 3d7b 7d3b 6675 6e63 7469 6f6e 206e  ,t={};function n
+000e4520: 2872 297b 7661 7220 6f3d 745b 725d 3b69  (r){var o=t[r];i
+000e4530: 6628 766f 6964 2030 213d 3d6f 2972 6574  f(void 0!==o)ret
+000e4540: 7572 6e20 6f2e 6578 706f 7274 733b 7661  urn o.exports;va
+000e4550: 7220 613d 745b 725d 3d7b 6964 3a72 2c6c  r a=t[r]={id:r,l
+000e4560: 6f61 6465 643a 2131 2c65 7870 6f72 7473  oaded:!1,exports
+000e4570: 3a7b 7d7d 3b72 6574 7572 6e20 655b 725d  :{}};return e[r]
+000e4580: 2e63 616c 6c28 612e 6578 706f 7274 732c  .call(a.exports,
+000e4590: 612c 612e 6578 706f 7274 732c 6e29 2c61  a,a.exports,n),a
+000e45a0: 2e6c 6f61 6465 643d 2130 2c61 2e65 7870  .loaded=!0,a.exp
+000e45b0: 6f72 7473 7d6e 2e6d 3d65 2c6e 2e61 6d64  orts}n.m=e,n.amd
+000e45c0: 443d 6675 6e63 7469 6f6e 2829 7b74 6872  D=function(){thr
+000e45d0: 6f77 206e 6577 2045 7272 6f72 2822 6465  ow new Error("de
+000e45e0: 6669 6e65 2063 616e 6e6f 7420 6265 2075  fine cannot be u
+000e45f0: 7365 6420 696e 6469 7265 6374 2229 7d2c  sed indirect")},
+000e4600: 6e2e 616d 644f 3d7b 7d2c 6e2e 6e3d 6675  n.amdO={},n.n=fu
+000e4610: 6e63 7469 6f6e 2865 297b 7661 7220 743d  nction(e){var t=
+000e4620: 6526 2665 2e5f 5f65 734d 6f64 756c 653f  e&&e.__esModule?
+000e4630: 6675 6e63 7469 6f6e 2829 7b72 6574 7572  function(){retur
+000e4640: 6e20 652e 6465 6661 756c 747d 3a66 756e  n e.default}:fun
+000e4650: 6374 696f 6e28 297b 7265 7475 726e 2065  ction(){return e
+000e4660: 7d3b 7265 7475 726e 206e 2e64 2874 2c7b  };return n.d(t,{
+000e4670: 613a 747d 292c 747d 2c6e 2e64 3d66 756e  a:t}),t},n.d=fun
+000e4680: 6374 696f 6e28 652c 7429 7b66 6f72 2876  ction(e,t){for(v
+000e4690: 6172 2072 2069 6e20 7429 6e2e 6f28 742c  ar r in t)n.o(t,
+000e46a0: 7229 2626 216e 2e6f 2865 2c72 2926 264f  r)&&!n.o(e,r)&&O
+000e46b0: 626a 6563 742e 6465 6669 6e65 5072 6f70  bject.defineProp
+000e46c0: 6572 7479 2865 2c72 2c7b 656e 756d 6572  erty(e,r,{enumer
+000e46d0: 6162 6c65 3a21 302c 6765 743a 745b 725d  able:!0,get:t[r]
+000e46e0: 7d29 7d2c 6e2e 673d 6675 6e63 7469 6f6e  })},n.g=function
+000e46f0: 2829 7b69 6628 226f 626a 6563 7422 3d3d  (){if("object"==
+000e4700: 7479 7065 6f66 2067 6c6f 6261 6c54 6869  typeof globalThi
+000e4710: 7329 7265 7475 726e 2067 6c6f 6261 6c54  s)return globalT
+000e4720: 6869 733b 7472 797b 7265 7475 726e 2074  his;try{return t
+000e4730: 6869 737c 7c6e 6577 2046 756e 6374 696f  his||new Functio
+000e4740: 6e28 2272 6574 7572 6e20 7468 6973 2229  n("return this")
+000e4750: 2829 7d63 6174 6368 2865 297b 6966 2822  ()}catch(e){if("
+000e4760: 6f62 6a65 6374 223d 3d74 7970 656f 6620  object"==typeof 
+000e4770: 7769 6e64 6f77 2972 6574 7572 6e20 7769  window)return wi
+000e4780: 6e64 6f77 7d7d 2829 2c6e 2e6f 3d66 756e  ndow}}(),n.o=fun
+000e4790: 6374 696f 6e28 652c 7429 7b72 6574 7572  ction(e,t){retur
+000e47a0: 6e20 4f62 6a65 6374 2e70 726f 746f 7479  n Object.prototy
+000e47b0: 7065 2e68 6173 4f77 6e50 726f 7065 7274  pe.hasOwnPropert
+000e47c0: 792e 6361 6c6c 2865 2c74 297d 2c6e 2e72  y.call(e,t)},n.r
+000e47d0: 3d66 756e 6374 696f 6e28 6529 7b22 756e  =function(e){"un
+000e47e0: 6465 6669 6e65 6422 213d 7479 7065 6f66  defined"!=typeof
+000e47f0: 2053 796d 626f 6c26 2653 796d 626f 6c2e   Symbol&&Symbol.
+000e4800: 746f 5374 7269 6e67 5461 6726 264f 626a  toStringTag&&Obj
+000e4810: 6563 742e 6465 6669 6e65 5072 6f70 6572  ect.defineProper
+000e4820: 7479 2865 2c53 796d 626f 6c2e 746f 5374  ty(e,Symbol.toSt
+000e4830: 7269 6e67 5461 672c 7b76 616c 7565 3a22  ringTag,{value:"
+000e4840: 4d6f 6475 6c65 227d 292c 4f62 6a65 6374  Module"}),Object
+000e4850: 2e64 6566 696e 6550 726f 7065 7274 7928  .defineProperty(
+000e4860: 652c 225f 5f65 734d 6f64 756c 6522 2c7b  e,"__esModule",{
+000e4870: 7661 6c75 653a 2130 7d29 7d2c 6e2e 6e6d  value:!0})},n.nm
+000e4880: 643d 6675 6e63 7469 6f6e 2865 297b 7265  d=function(e){re
+000e4890: 7475 726e 2065 2e70 6174 6873 3d5b 5d2c  turn e.paths=[],
+000e48a0: 652e 6368 696c 6472 656e 7c7c 2865 2e63  e.children||(e.c
+000e48b0: 6869 6c64 7265 6e3d 5b5d 292c 657d 2c6e  hildren=[]),e},n
+000e48c0: 2e70 3d22 222c 6e2e 623d 646f 6375 6d65  .p="",n.b=docume
+000e48d0: 6e74 2e62 6173 6555 5249 7c7c 7365 6c66  nt.baseURI||self
+000e48e0: 2e6c 6f63 6174 696f 6e2e 6872 6566 2c6e  .location.href,n
+000e48f0: 2e6e 633d 766f 6964 2030 2c6e 2833 3936  .nc=void 0,n(396
+000e4900: 297d 2829 3b0a 3c2f 7363 7269 7074 3e0a  )}();.</script>.
+000e4910: 3c2f 626f 6479 3e0a 3c2f 6874 6d6c 3e0a  </body>.</html>.
```

### Comparing `trame-vtk-2.8.7/trame_vtk/tools/vtksz2html.py` & `trame-vtk-2.8.8/trame_vtk/tools/vtksz2html.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.8.8/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.8.8/trame_vtk/widgets/vtk/common.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.8.7/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.8.8/trame_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.8.7
+Version: 2.8.8
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.8.7/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.8.8/trame_vtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

