# Comparing `tmp/wntrfr-1.1.0.1.1.tar.gz` & `tmp/wntrfr-1.1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wntrfr-1.1.0.1.1.tar", last modified: Tue Apr 23 00:30:47 2024, max compression
+gzip compressed data, was "wntrfr-1.1.0.1.2.tar", last modified: Mon May  6 21:21:07 2024, max compression
```

## Comparing `wntrfr-1.1.0.1.1.tar` & `wntrfr-1.1.0.1.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/
--rw-rw-rw-   0        0        0     4787 2024-04-12 18:43:38.000000 wntrfr-1.1.0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0      343 2024-04-18 00:54:57.000000 wntrfr-1.1.0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4707 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.1/README.md
--rw-rw-rw-   0        0        0      210 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 00:30:47.996694 wntrfr-1.1.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4384 2024-04-13 00:40:09.000000 wntrfr-1.1.0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.907229 wntrfr-1.1.0.1.1/wntrfr/
--rw-rw-rw-   0        0        0      572 2024-04-23 00:30:40.000000 wntrfr-1.1.0.1.1/wntrfr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.914737 wntrfr-1.1.0.1.1/wntrfr/epanet/
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.915732 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/
--rw-rw-rw-   0        0        0   302216 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet.dylib
--rw-rw-rw-   0        0        0   325828 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet22.dylib
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.917738 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/
--rw-rw-rw-   0        0        0   385808 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet22_amd64.so
--rw-rw-rw-   0        0        0   505379 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet2_amd64.so
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.923747 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/
--rw-rw-rw-   0        0        0     8758 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.bas
--rw-rw-rw-   0        0        0     4106 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.def
--rw-rw-rw-   0        0        0   217088 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.dll
--rw-rw-rw-   0        0        0    22614 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.lib
--rw-rw-rw-   0        0        0     9910 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.pas
--rw-rw-rw-   0        0        0   349184 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_amd64.dll
--rw-rw-rw-   0        0        0   285696 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_win32.dll
--rw-rw-rw-   0        0        0   315904 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2_amd64.dll
--rw-rw-rw-   0        0        0      249 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/__init__.py
--rw-rw-rw-   0        0        0     7865 2024-04-12 18:43:46.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/exceptions.py
--rw-rw-rw-   0        0        0   152460 2024-04-23 00:30:11.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/io.py
--rw-rw-rw-   0        0        0    27944 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/toolkit.py
--rw-rw-rw-   0        0        0    46112 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/epanet/util.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.924749 wntrfr-1.1.0.1.1/wntrfr/gis/
--rw-rw-rw-   0        0        0      271 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/__init__.py
--rw-rw-rw-   0        0        0    12741 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/geospatial.py
--rw-rw-rw-   0        0        0    19214 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/gis/network.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.927744 wntrfr-1.1.0.1.1/wntrfr/graphics/
--rw-rw-rw-   0        0        0      394 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/__init__.py
--rw-rw-rw-   0        0        0     1779 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/color.py
--rw-rw-rw-   0        0        0     6745 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/curve.py
--rw-rw-rw-   0        0        0     3543 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/layer.py
--rw-rw-rw-   0        0        0    31670 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/graphics/network.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.932167 wntrfr-1.1.0.1.1/wntrfr/metrics/
--rw-rw-rw-   0        0        0      939 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/__init__.py
--rw-rw-rw-   0        0        0    15315 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/economic.py
--rw-rw-rw-   0        0        0    15710 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/hydraulic.py
--rw-rw-rw-   0        0        0     2761 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/misc.py
--rw-rw-rw-   0        0        0    16807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/topographic.py
--rw-rw-rw-   0        0        0     5236 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/metrics/water_security.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.937692 wntrfr-1.1.0.1.1/wntrfr/morph/
--rw-rw-rw-   0        0        0      573 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/__init__.py
--rw-rw-rw-   0        0        0    12684 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/link.py
--rw-rw-rw-   0        0        0    11032 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/node.py
--rw-rw-rw-   0        0        0    16912 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/morph/skel.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.946694 wntrfr-1.1.0.1.1/wntrfr/network/
--rw-rw-rw-   0        0        0      874 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/__init__.py
--rw-rw-rw-   0        0        0    25793 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/base.py
--rw-rw-rw-   0        0        0    83473 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/controls.py
--rw-rw-rw-   0        0        0    83834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/elements.py
--rw-rw-rw-   0        0        0    24487 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/io.py
--rw-rw-rw-   0        0        0     2311 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/layer.py
--rw-rw-rw-   0        0        0    88834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/model.py
--rw-rw-rw-   0        0        0    31476 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/network/options.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.951691 wntrfr-1.1.0.1.1/wntrfr/scenario/
--rw-rw-rw-   0        0        0      222 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/__init__.py
--rw-rw-rw-   0        0        0     7818 2024-04-13 00:44:11.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/earthquake.py
--rw-rw-rw-   0        0        0     3706 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/scenario/fragility_curve.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.960690 wntrfr-1.1.0.1.1/wntrfr/sim/
--rw-rw-rw-   0        0        0      329 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.972690 wntrfr-1.1.0.1.1/wntrfr/sim/aml/
--rw-rw-rw-   0        0        0      254 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/__init__.py
--rw-rw-rw-   0        0        0    16045 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/aml.py
--rw-rw-rw-   0        0        0    14245 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.cpp
--rw-rw-rw-   0        0        0     3707 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.hpp
--rw-rw-rw-   0        0        0      938 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.i
--rw-rw-rw-   0        0        0     2121 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.py
--rw-rw-rw-   0        0        0   359034 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator_wrap.cpp
--rw-rw-rw-   0        0        0    37825 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/expr.py
--rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/aml/numpy.i
--rw-rw-rw-   0        0        0    76807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/core.py
--rw-rw-rw-   0        0        0     5097 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/epanet.py
--rw-rw-rw-   0        0        0    14911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/hydraulics.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.980690 wntrfr-1.1.0.1.1/wntrfr/sim/models/
--rw-rw-rw-   0        0        0      108 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/__init__.py
--rw-rw-rw-   0        0        0      911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/constants.py
--rw-rw-rw-   0        0        0    29038 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/constraint.py
--rw-rw-rw-   0        0        0    17287 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/param.py
--rw-rw-rw-   0        0        0      938 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/utils.py
--rw-rw-rw-   0        0        0     2412 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/models/var.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.985690 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/
--rw-rw-rw-   0        0        0      148 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/__init__.py
--rw-rw-rw-   0        0        0     1647 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.cpp
--rw-rw-rw-   0        0        0      332 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.hpp
--rw-rw-rw-   0        0        0      634 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.i
--rw-rw-rw-   0        0        0     2129 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.py
--rw-rw-rw-   0        0        0   154827 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp
--rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/numpy.i
--rw-rw-rw-   0        0        0      415 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.1/wntrfr/sim/results.py
--rw-rw-rw-   0        0        0     7259 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/sim/solvers.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.993694 wntrfr-1.1.0.1.1/wntrfr/utils/
--rw-rw-rw-   0        0        0       93 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.1/wntrfr/utils/__init__.py
--rw-rw-rw-   0        0        0     1058 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/doc_inheritor.py
--rw-rw-rw-   0        0        0     1167 2024-04-13 00:45:48.000000 wntrfr-1.1.0.1.1/wntrfr/utils/logger.py
--rw-rw-rw-   0        0        0     1876 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/ordered_set.py
--rw-rw-rw-   0        0        0      972 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.1/wntrfr/utils/polynomial_interpolation.py
-drwxrwxrwx   0        0        0        0 2024-04-23 00:30:47.910229 wntrfr-1.1.0.1.1/wntrfr.egg-info/
--rw-rw-rw-   0        0        0     4707 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2787 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 00:30:27.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 00:30:46.000000 wntrfr-1.1.0.1.1/wntrfr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.932556 wntrfr-1.1.0.1.2/
+-rw-rw-rw-   0        0        0     4787 2024-04-12 18:43:38.000000 wntrfr-1.1.0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0      343 2024-04-18 00:54:57.000000 wntrfr-1.1.0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4707 2024-05-06 21:21:07.932556 wntrfr-1.1.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.2/README.md
+-rw-rw-rw-   0        0        0      210 2024-04-12 18:43:39.000000 wntrfr-1.1.0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 21:21:07.934558 wntrfr-1.1.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     4384 2024-04-13 00:40:09.000000 wntrfr-1.1.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.850328 wntrfr-1.1.0.1.2/wntrfr/
+-rw-rw-rw-   0        0        0      572 2024-05-06 21:18:24.000000 wntrfr-1.1.0.1.2/wntrfr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.860303 wntrfr-1.1.0.1.2/wntrfr/epanet/
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.862303 wntrfr-1.1.0.1.2/wntrfr/epanet/Darwin/
+-rw-rw-rw-   0        0        0   302216 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Darwin/libepanet.dylib
+-rw-rw-rw-   0        0        0   325828 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Darwin/libepanet22.dylib
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.864303 wntrfr-1.1.0.1.2/wntrfr/epanet/Linux/
+-rw-rw-rw-   0        0        0   385808 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Linux/libepanet22_amd64.so
+-rw-rw-rw-   0        0        0   505379 2024-04-12 18:43:47.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Linux/libepanet2_amd64.so
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.874303 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/
+-rw-rw-rw-   0        0        0     8758 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.bas
+-rw-rw-rw-   0        0        0     4106 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.def
+-rw-rw-rw-   0        0        0   217088 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.dll
+-rw-rw-rw-   0        0        0    22614 2024-04-12 18:43:53.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.lib
+-rw-rw-rw-   0        0        0     9910 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.pas
+-rw-rw-rw-   0        0        0   349184 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet22_amd64.dll
+-rw-rw-rw-   0        0        0   285696 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet22_win32.dll
+-rw-rw-rw-   0        0        0   315904 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2_amd64.dll
+-rw-rw-rw-   0        0        0      249 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/__init__.py
+-rw-rw-rw-   0        0        0     7865 2024-04-12 18:43:46.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/exceptions.py
+-rw-rw-rw-   0        0        0   152462 2024-05-06 21:11:29.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/io.py
+-rw-rw-rw-   0        0        0    27944 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/toolkit.py
+-rw-rw-rw-   0        0        0    46112 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/epanet/util.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.877303 wntrfr-1.1.0.1.2/wntrfr/gis/
+-rw-rw-rw-   0        0        0      271 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/gis/__init__.py
+-rw-rw-rw-   0        0        0    12741 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/gis/geospatial.py
+-rw-rw-rw-   0        0        0    19214 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/gis/network.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.881304 wntrfr-1.1.0.1.2/wntrfr/graphics/
+-rw-rw-rw-   0        0        0      394 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/graphics/__init__.py
+-rw-rw-rw-   0        0        0     1779 2024-04-12 18:43:54.000000 wntrfr-1.1.0.1.2/wntrfr/graphics/color.py
+-rw-rw-rw-   0        0        0     6745 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/graphics/curve.py
+-rw-rw-rw-   0        0        0     3543 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/graphics/layer.py
+-rw-rw-rw-   0        0        0    31670 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/graphics/network.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.886307 wntrfr-1.1.0.1.2/wntrfr/metrics/
+-rw-rw-rw-   0        0        0      939 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/__init__.py
+-rw-rw-rw-   0        0        0    15315 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/economic.py
+-rw-rw-rw-   0        0        0    15710 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/hydraulic.py
+-rw-rw-rw-   0        0        0     2761 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/misc.py
+-rw-rw-rw-   0        0        0    16807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/topographic.py
+-rw-rw-rw-   0        0        0     5236 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/metrics/water_security.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.890304 wntrfr-1.1.0.1.2/wntrfr/morph/
+-rw-rw-rw-   0        0        0      573 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/morph/__init__.py
+-rw-rw-rw-   0        0        0    12684 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/morph/link.py
+-rw-rw-rw-   0        0        0    11032 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/morph/node.py
+-rw-rw-rw-   0        0        0    16912 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/morph/skel.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.899390 wntrfr-1.1.0.1.2/wntrfr/network/
+-rw-rw-rw-   0        0        0      874 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/__init__.py
+-rw-rw-rw-   0        0        0    25793 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/base.py
+-rw-rw-rw-   0        0        0    83473 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/controls.py
+-rw-rw-rw-   0        0        0    83834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/elements.py
+-rw-rw-rw-   0        0        0    24487 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/io.py
+-rw-rw-rw-   0        0        0     2311 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/layer.py
+-rw-rw-rw-   0        0        0    88834 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/model.py
+-rw-rw-rw-   0        0        0    31476 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/network/options.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.901390 wntrfr-1.1.0.1.2/wntrfr/scenario/
+-rw-rw-rw-   0        0        0      222 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/scenario/__init__.py
+-rw-rw-rw-   0        0        0     7818 2024-04-13 00:44:11.000000 wntrfr-1.1.0.1.2/wntrfr/scenario/earthquake.py
+-rw-rw-rw-   0        0        0     3706 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/scenario/fragility_curve.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.907409 wntrfr-1.1.0.1.2/wntrfr/sim/
+-rw-rw-rw-   0        0        0      329 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.914394 wntrfr-1.1.0.1.2/wntrfr/sim/aml/
+-rw-rw-rw-   0        0        0      254 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/__init__.py
+-rw-rw-rw-   0        0        0    16045 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/aml.py
+-rw-rw-rw-   0        0        0    14245 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.cpp
+-rw-rw-rw-   0        0        0     3707 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.hpp
+-rw-rw-rw-   0        0        0      938 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.i
+-rw-rw-rw-   0        0        0     2121 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.py
+-rw-rw-rw-   0        0        0   359034 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator_wrap.cpp
+-rw-rw-rw-   0        0        0    37825 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/expr.py
+-rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/aml/numpy.i
+-rw-rw-rw-   0        0        0    76807 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/core.py
+-rw-rw-rw-   0        0        0     5097 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/epanet.py
+-rw-rw-rw-   0        0        0    14911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/hydraulics.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.920397 wntrfr-1.1.0.1.2/wntrfr/sim/models/
+-rw-rw-rw-   0        0        0      108 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/__init__.py
+-rw-rw-rw-   0        0        0      911 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/constants.py
+-rw-rw-rw-   0        0        0    29038 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/constraint.py
+-rw-rw-rw-   0        0        0    17287 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/param.py
+-rw-rw-rw-   0        0        0      938 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/utils.py
+-rw-rw-rw-   0        0        0     2412 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/models/var.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.926538 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/
+-rw-rw-rw-   0        0        0      148 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/__init__.py
+-rw-rw-rw-   0        0        0     1647 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.cpp
+-rw-rw-rw-   0        0        0      332 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.hpp
+-rw-rw-rw-   0        0        0      634 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.i
+-rw-rw-rw-   0        0        0     2129 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.py
+-rw-rw-rw-   0        0        0   154827 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation_wrap.cpp
+-rw-rw-rw-   0        0        0   109668 2024-04-12 18:43:57.000000 wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/numpy.i
+-rw-rw-rw-   0        0        0      415 2024-04-12 18:43:56.000000 wntrfr-1.1.0.1.2/wntrfr/sim/results.py
+-rw-rw-rw-   0        0        0     7259 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/sim/solvers.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.930538 wntrfr-1.1.0.1.2/wntrfr/utils/
+-rw-rw-rw-   0        0        0       93 2024-04-13 00:24:14.000000 wntrfr-1.1.0.1.2/wntrfr/utils/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.2/wntrfr/utils/doc_inheritor.py
+-rw-rw-rw-   0        0        0     1167 2024-04-13 00:45:48.000000 wntrfr-1.1.0.1.2/wntrfr/utils/logger.py
+-rw-rw-rw-   0        0        0     1876 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.2/wntrfr/utils/ordered_set.py
+-rw-rw-rw-   0        0        0      972 2024-04-12 18:44:01.000000 wntrfr-1.1.0.1.2/wntrfr/utils/polynomial_interpolation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:21:07.854304 wntrfr-1.1.0.1.2/wntrfr.egg-info/
+-rw-rw-rw-   0        0        0     4707 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2787 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 21:20:57.000000 wntrfr-1.1.0.1.2/wntrfr.egg-info/top_level.txt
```

### Comparing `wntrfr-1.1.0.1.1/LICENSE.md` & `wntrfr-1.1.0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/PKG-INFO` & `wntrfr-1.1.0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wntrfr
-Version: 1.1.0.1.1
+Version: 1.1.0.1.2
 Summary: Water Network Tool for Resilience
 Home-page: https://github.com/snaeimi/WNTR
 Author: WNTR Developers
 Maintainer-email: snaeimi@udel.edu
 License: Revised BSD
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `wntrfr-1.1.0.1.1/README.md` & `wntrfr-1.1.0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/setup.py` & `wntrfr-1.1.0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/__init__.py` & `wntrfr-1.1.0.1.2/wntrfr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from wntrfr import metrics
 from wntrfr import sim
 from wntrfr import scenario
 from wntrfr import graphics
 from wntrfr import gis
 from wntrfr import utils
 
-__version__ = '1.1.0.1.1'
+__version__ = '1.1.0.1.2'
 
 __copyright__ = """Copyright 2023 National Technology & Engineering 
 Solutions of Sandia, LLC (NTESS). Under the terms of Contract DE-NA0003525 
 with NTESS, the U.S. Government retains certain rights in this software."""
 
 __license__ = "Revised BSD License"
```

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet.dylib` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Darwin/libepanet.dylib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Darwin/libepanet22.dylib` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Darwin/libepanet22.dylib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet22_amd64.so` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Linux/libepanet22_amd64.so`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Linux/libepanet2_amd64.so` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Linux/libepanet2_amd64.so`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.bas` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.bas`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.def` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.def`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.dll` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.lib` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.lib`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2.pas` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2.pas`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_amd64.dll` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet22_amd64.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet22_win32.dll` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet22_win32.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/Windows/epanet2_amd64.dll` & `wntrfr-1.1.0.1.2/wntrfr/epanet/Windows/epanet2_amd64.dll`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/exceptions.py` & `wntrfr-1.1.0.1.2/wntrfr/epanet/exceptions.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/io.py` & `wntrfr-1.1.0.1.2/wntrfr/epanet/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 import warnings
 from collections import OrderedDict
 
 import numpy as np
 import pandas as pd
 import six
-import wntr
+import wntrfr
 import wntrfr.network
 from wntrfr.network.base import Link
 from wntrfr.network.controls import (AndCondition, Comparison, Control,
                                    ControlAction, OrCondition, Rule,
                                    SimTimeCondition, TimeOfDayCondition,
                                    ValueCondition, _ControlType)
 from wntrfr.network.elements import Junction, Pipe, Pump, Reservoir, Tank, Valve
```

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/toolkit.py` & `wntrfr-1.1.0.1.2/wntrfr/epanet/toolkit.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/epanet/util.py` & `wntrfr-1.1.0.1.2/wntrfr/epanet/util.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/gis/geospatial.py` & `wntrfr-1.1.0.1.2/wntrfr/gis/geospatial.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/gis/network.py` & `wntrfr-1.1.0.1.2/wntrfr/gis/network.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/graphics/color.py` & `wntrfr-1.1.0.1.2/wntrfr/graphics/color.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/graphics/curve.py` & `wntrfr-1.1.0.1.2/wntrfr/graphics/curve.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/graphics/layer.py` & `wntrfr-1.1.0.1.2/wntrfr/graphics/layer.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/graphics/network.py` & `wntrfr-1.1.0.1.2/wntrfr/graphics/network.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/__init__.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/economic.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/economic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/hydraulic.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/hydraulic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/misc.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/misc.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/topographic.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/topographic.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/metrics/water_security.py` & `wntrfr-1.1.0.1.2/wntrfr/metrics/water_security.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/morph/__init__.py` & `wntrfr-1.1.0.1.2/wntrfr/morph/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/morph/link.py` & `wntrfr-1.1.0.1.2/wntrfr/morph/link.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/morph/node.py` & `wntrfr-1.1.0.1.2/wntrfr/morph/node.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/morph/skel.py` & `wntrfr-1.1.0.1.2/wntrfr/morph/skel.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/__init__.py` & `wntrfr-1.1.0.1.2/wntrfr/network/__init__.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/base.py` & `wntrfr-1.1.0.1.2/wntrfr/network/base.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/controls.py` & `wntrfr-1.1.0.1.2/wntrfr/network/controls.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/elements.py` & `wntrfr-1.1.0.1.2/wntrfr/network/elements.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/io.py` & `wntrfr-1.1.0.1.2/wntrfr/network/io.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/layer.py` & `wntrfr-1.1.0.1.2/wntrfr/network/layer.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/model.py` & `wntrfr-1.1.0.1.2/wntrfr/network/model.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/network/options.py` & `wntrfr-1.1.0.1.2/wntrfr/network/options.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/scenario/earthquake.py` & `wntrfr-1.1.0.1.2/wntrfr/scenario/earthquake.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/scenario/fragility_curve.py` & `wntrfr-1.1.0.1.2/wntrfr/scenario/fragility_curve.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/aml.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/aml.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.cpp` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.hpp` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.hpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.i` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/evaluator_wrap.cpp` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/evaluator_wrap.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/expr.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/expr.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/aml/numpy.i` & `wntrfr-1.1.0.1.2/wntrfr/sim/aml/numpy.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/core.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/core.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/epanet.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/epanet.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/hydraulics.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/hydraulics.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/models/constants.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/models/constants.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/models/constraint.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/models/constraint.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/models/param.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/models/param.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/models/utils.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/models/utils.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/models/var.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/models/var.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.cpp` & `wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.i` & `wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/network_isolation_wrap.cpp` & `wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/network_isolation_wrap.cpp`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/network_isolation/numpy.i` & `wntrfr-1.1.0.1.2/wntrfr/sim/network_isolation/numpy.i`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/sim/solvers.py` & `wntrfr-1.1.0.1.2/wntrfr/sim/solvers.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/utils/doc_inheritor.py` & `wntrfr-1.1.0.1.2/wntrfr/utils/doc_inheritor.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/utils/logger.py` & `wntrfr-1.1.0.1.2/wntrfr/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/utils/ordered_set.py` & `wntrfr-1.1.0.1.2/wntrfr/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr/utils/polynomial_interpolation.py` & `wntrfr-1.1.0.1.2/wntrfr/utils/polynomial_interpolation.py`

 * *Files identical despite different names*

### Comparing `wntrfr-1.1.0.1.1/wntrfr.egg-info/PKG-INFO` & `wntrfr-1.1.0.1.2/wntrfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wntrfr
-Version: 1.1.0.1.1
+Version: 1.1.0.1.2
 Summary: Water Network Tool for Resilience
 Home-page: https://github.com/snaeimi/WNTR
 Author: WNTR Developers
 Maintainer-email: snaeimi@udel.edu
 License: Revised BSD
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `wntrfr-1.1.0.1.1/wntrfr.egg-info/SOURCES.txt` & `wntrfr-1.1.0.1.2/wntrfr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

