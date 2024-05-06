# Comparing `tmp/fenics-ffcx-0.7.0.tar.gz` & `tmp/fenics_ffcx-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-ffcx-0.7.0.tar", last modified: Tue Nov 21 09:10:18 2023, max compression
+gzip compressed data, was "fenics_ffcx-0.8.0.tar", last modified: Mon May  6 08:00:44 2024, max compression
```

## Comparing `fenics-ffcx-0.7.0.tar` & `fenics_ffcx-0.8.0.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.231491 fenics-ffcx-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)    25212 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ChangeLog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/INSTALL
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-21 09:10:18.231491 fenics-ffcx-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.211491 fenics-ffcx-0.7.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/cmake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/cmake/ufcx.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/cmake/ufcxConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.215491 fenics-ffcx-0.7.0/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/BiharmonicHHJ.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/BiharmonicRegge.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/CellGeometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/ComplexPoisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/ExpressionInterpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/FacetIntegrals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/FacetRestrictionAD.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/HyperElasticity.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MassDG0.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MassHcurl_2D_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MassHdiv_2D_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MathFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Mini.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MixedCoefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MixedGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/MixedPoissonDual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Normals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Poisson1D.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/PoissonQuad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/ProjectionManifold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/ReactionDiffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/SpatialCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/StabilisedStokes.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/Symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/TraceElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/VectorConstant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/VectorPoisson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/demo/test_demos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.215491 fenics-ffcx-0.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.215491 fenics-ffcx-0.7.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.231491 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-21 09:10:18.000000 fenics-ffcx-0.7.0/fenics_ffcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.219491 fenics-ffcx-0.7.0/ffcx/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.223491 fenics-ffcx-0.7.0/ffcx/codegeneration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.227491 fenics-ffcx-0.7.0/ffcx/codegeneration/C/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/basix_custom_element_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/c_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/dofmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/dofmap_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/expressions_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/file_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/finite_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/finite_element_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/form_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/integrals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/C/integrals_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16363 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/codegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/expression_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/flop_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/integral_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)    24986 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/lnodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    15414 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/ufcx.h
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/codegeneration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/element_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/git_commit_hash.py.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.227491 fenics-ffcx-0.7.0/ffcx/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.227491 fenics-ffcx-0.7.0/ffcx/ir/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/factorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/modified_terminals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/valuenumbering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/analysis/visualise.py
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/elementtables.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/ir/representationutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/ffcx/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-11-21 09:10:18.231491 fenics-ffcx-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 09:10:18.227491 fenics-ffcx-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/Poisson.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_add_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_blocked_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10579 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_jit_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    36970 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_jit_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-21 09:10:10.000000 fenics-ffcx-0.7.0/test/test_lnodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.903079 fenics_ffcx-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)    25212 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ChangeLog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-06 08:00:44.903079 fenics_ffcx-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.887079 fenics_ffcx-0.8.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/cmake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/cmake/ufcx.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/cmake/ufcxConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.891079 fenics_ffcx-0.8.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/BiharmonicHHJ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/BiharmonicRegge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/CellGeometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/ComplexPoisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/ExpressionInterpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/FacetIntegrals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/FacetRestrictionAD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/HyperElasticity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MassAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MassDG0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MassHcurl_2D_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MassHdiv_2D_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MathFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MixedCoefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MixedGradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/MixedPoissonDual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Normals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Poisson1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/PoissonQuad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/ProjectionManifold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/ReactionDiffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/SpatialCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/StabilisedStokes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/Symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/TraceElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/VectorConstant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/VectorPoisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/demo/test_demos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.891079 fenics_ffcx-0.8.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.891079 fenics_ffcx-0.8.0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.903079 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:00:44.000000 fenics_ffcx-0.8.0/fenics_ffcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.895079 fenics_ffcx-0.8.0/ffcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.895079 fenics_ffcx-0.8.0/ffcx/codegeneration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.899079 fenics_ffcx-0.8.0/ffcx/codegeneration/C/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/basix_custom_element_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/c_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/dofmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/dofmap_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/expressions_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/file_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/finite_element_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/form_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/integrals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/integrals_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/C/quadrature_rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/codegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/expression_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/integral_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30730 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/lnodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/ufcx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/codegeneration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/element_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/git_commit_hash.py.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.899079 fenics_ffcx-0.8.0/ffcx/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.899079 fenics_ffcx-0.8.0/ffcx/ir/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/factorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/modified_terminals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/valuenumbering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/analysis/visualise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/elementtables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/ir/representationutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/ffcx/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:00:44.903079 fenics_ffcx-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:00:44.903079 fenics_ffcx-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/Poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_add_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_blocked_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_jit_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_jit_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_lnodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_submesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-06 08:00:36.000000 fenics_ffcx-0.8.0/test/test_tensor_product.py
```

### Comparing `fenics-ffcx-0.7.0/AUTHORS` & `fenics_ffcx-0.8.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     Andy R. Terrel
     email: aterrel@uchicago.edu
     www:   http://people.cs.uchicago.edu/~aterrel/
 
     Ivan Yashchuk
     email: ivan.yashchuk@aalto.fi
 
+    Matthew Scroggs
+    email: matthew.scroggs.14@ucl.ac.uk
+    www:   https://mscroggs.co.uk
 
 Credits for UFC
 ===============
 
 UFC was merged into FFC 2014-02-18. Below is the list of credits for
 UFC at the time of the merge.
```

### Comparing `fenics-ffcx-0.7.0/COPYING` & `fenics_ffcx-0.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/COPYING.LESSER` & `fenics_ffcx-0.8.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/ChangeLog.rst` & `fenics_ffcx-0.8.0/ChangeLog.rst`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/INSTALL` & `fenics_ffcx-0.8.0/INSTALL`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/README.md` & `fenics_ffcx-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # FFCx: The FEniCSx Form Compiler
 
 [![FFCx CI](https://github.com/FEniCS/ffcx/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/FEniCS/ffcx/actions/workflows/pythonapp.yml)
+[![Spack install](https://github.com/FEniCS/ffcx/actions/workflows/spack.yml/badge.svg)](https://github.com/FEniCS/ffcx/actions/workflows/spack.yml)
 [![Coverage Status](https://coveralls.io/repos/github/FEniCS/ffcx/badge.svg?branch=main)](https://coveralls.io/github/FEniCS/ffcx?branch=main)
 
 FFCx is a new version of the FEniCS Form Compiler. It is being actively
 developed and is compatible with DOLFINx.
 
 FFCx is a compiler for finite element variational forms. From a
 high-level description of the form in the Unified Form Language (UFL),
```

### Comparing `fenics-ffcx-0.7.0/cmake/CMakeLists.txt` & `fenics_ffcx-0.8.0/cmake/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.19)
 
-project(ufcx VERSION 0.7.0 DESCRIPTION "UFCx interface header for finite element kernels"
+project(ufcx VERSION 0.8.0 DESCRIPTION "UFCx interface header for finite element kernels"
   LANGUAGES C
   HOMEPAGE_URL https://github.com/fenics/ffcx)
 include(GNUInstallDirs)
 
 file(SHA1 ${PROJECT_SOURCE_DIR}/../ffcx/codegeneration/ufcx.h UFCX_HASH)
 message("Test hash: ${UFCX_HASH}")
```

### Comparing `fenics-ffcx-0.7.0/demo/BiharmonicHHJ.py` & `fenics_ffcx-0.8.0/demo/BiharmonicHHJ.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 # Copyright (C) 2016 Lizao Li
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Biharmonic equation in Hellan-Herrmann-Johnson (HHJ)
-# formulation.
+"""Biharmonis HHJ demo.
+
+The bilinear form a(u, v) and linear form L(v) for Biharmonic equation
+in Hellan-Herrmann-Johnson (HHJ) formulation.
+"""
+
 import basix.ufl
-from ufl import (Coefficient, FacetNormal, TestFunctions, TrialFunctions, dot,
-                 dS, ds, dx, grad, inner, jump, triangle)
+from ufl import (
+    Coefficient,
+    FacetNormal,
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    dot,
+    dS,
+    ds,
+    dx,
+    grad,
+    inner,
+    jump,
+)
 
-HHJ = basix.ufl.element('HHJ', "triangle", 2)
-P = basix.ufl.element('P', "triangle", 3)
+HHJ = basix.ufl.element("HHJ", "triangle", 2)
+P = basix.ufl.element("P", "triangle", 3)
 mixed_element = basix.ufl.mixed_element([HHJ, P])
-
-(sigma, u) = TrialFunctions(mixed_element)
-(tau, v) = TestFunctions(mixed_element)
-f = Coefficient(P)
+domain = Mesh(basix.ufl.element("P", "triangle", 1, shape=(2,)))
+mixed_space = FunctionSpace(domain, mixed_element)
+p_space = FunctionSpace(domain, P)
+
+(sigma, u) = TrialFunctions(mixed_space)
+(tau, v) = TestFunctions(mixed_space)
+f = Coefficient(p_space)
 
 
 def b(sigma, v):
-    n = FacetNormal(triangle)
-    return inner(sigma, grad(grad(v))) * dx \
-        - dot(dot(sigma('+'), n('+')), n('+')) * jump(grad(v), n) * dS \
+    """The form b."""
+    n = FacetNormal(domain)
+    return (
+        inner(sigma, grad(grad(v))) * dx
+        - dot(dot(sigma("+"), n("+")), n("+")) * jump(grad(v), n) * dS
         - dot(dot(sigma, n), n) * dot(grad(v), n) * ds
+    )
 
 
 a = inner(sigma, tau) * dx - b(tau, u) + b(sigma, v)
 L = f * v * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/ComplexPoisson.py` & `fenics_ffcx-0.8.0/demo/ComplexPoisson.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation using bilinear elements on bilinear mesh geometry.
+"""Complex Poisson demo.
+
+The bilinear form a(u, v) and linear form L(v) for
+Poisson's equation using bilinear elements on bilinear mesh geometry.
+"""
+
 import basix.ufl
-from ufl import (Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 dx, grad, inner)
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, dx, grad, inner
 
-coords = basix.ufl.element("P", "triangle", 2, shape=(2, ))
+coords = basix.ufl.element("P", "triangle", 2, shape=(2,))
 mesh = Mesh(coords)
 dx = dx(mesh)
 
 element = basix.ufl.element("P", mesh.ufl_cell().cellname(), 2)
 space = FunctionSpace(mesh, element)
 
 u = TrialFunction(space)
```

### Comparing `fenics-ffcx-0.7.0/demo/Components.py` & `fenics_ffcx-0.8.0/demo/Components.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# This example demonstrates how to create vectors component-wise
+"""Components demo.
+
+This example demonstrates how to create vectors component-wise.
+"""
+
 import basix.ufl
-from ufl import Coefficient, TestFunction, as_vector, dot, dx
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, as_vector, dx, inner
 
-element = basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3, ))
+element = basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3,))
+domain = Mesh(element)
+space = FunctionSpace(domain, element)
 
-v = TestFunction(element)
-f = Coefficient(element)
+v = TestFunction(space)
+f = Coefficient(space)
 
 # Create vector
 v0 = as_vector([v[0], v[1], 0.0])
 
 # Use created vector in linear form
-L = dot(f, v0) * dx
+L = inner(f, v0) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/Conditional.py` & `fenics_ffcx-0.8.0/demo/SpatialCoordinates.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010-2011 Kristian B. Oelgaard
+# Copyright (C) 2010 Kristian B. Oelgaard
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,32 +10,43 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# Illustration on how to use Conditional to define a source term
-import basix.ufl
-from ufl import (And, Constant, Not, Or, SpatialCoordinate, TestFunction,
-                 conditional, dx, ge, gt, le, lt, triangle)
-
-element = basix.ufl.element("Lagrange", "triangle", 2)
+"""Spatial coordinates demo.
 
-v = TestFunction(element)
-g = Constant(triangle)
+The bilinear form a(u, v) and linear form L(v) for Poisson's equation where
+spatial coordinates are used to define the source and boundary flux terms.
+"""
 
-x = SpatialCoordinate(triangle)
-c0 = conditional(le((x[0] - 0.33)**2 + (x[1] - 0.67)**2, 0.015), -1.0, 5.0)
-c = conditional(le((x[0] - 0.33)**2 + (x[1] - 0.67)**2, 0.025), c0, 0.0)
+import basix.ufl
+from ufl import (
+    FunctionSpace,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    TrialFunction,
+    ds,
+    dx,
+    exp,
+    grad,
+    inner,
+    sin,
+)
 
-t0 = And(ge(x[0], 0.55), le(x[0], 0.95))
-t1 = Or(lt(x[1], 0.05), gt(x[1], 0.45))
-t2 = And(t0, Not(t1))
-t = conditional(And(ge(x[1] - x[0] - 0.05 + 0.55, 0.0), t2), -1.0, 0.0)
+element = basix.ufl.element("Lagrange", "triangle", 2)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-k = conditional(gt(1, 0), g, g + 1)
+u = TrialFunction(space)
+v = TestFunction(space)
 
-f = c + t + k
+x = SpatialCoordinate(domain)
+d_x = x[0] - 0.5
+d_y = x[1] - 0.5
+f = 10.0 * exp(-(d_x * d_x + d_y * d_y) / 0.02)
+g = sin(5.0 * x[0])
 
-L = v * f * dx
+a = inner(grad(u), grad(v)) * dx
+L = inner(f, v) * dx + inner(g, v) * ds
```

### Comparing `fenics-ffcx-0.7.0/demo/ExpressionInterpolation.py` & `fenics_ffcx-0.8.0/demo/ExpressionInterpolation.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,55 +10,57 @@
 # FFC is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFC. If not, see <http://www.gnu.org/licenses/>.
-#
-# Defines an Expression which evaluates the several different functions at
-# a set of interpolation points
+"""Expression interpolation demo.
+
+Defines an Expression which evaluates the several different functions at
+a set of interpolation points.
+"""
 
 import basix
 import basix.ufl
-from ffcx.element_interface import QuadratureElement
 from ufl import Coefficient, FunctionSpace, Mesh, grad
 
 # Define mesh
 cell = "triangle"
-v_el = basix.ufl.element("Lagrange", cell, 1, shape=(2, ))
+v_el = basix.ufl.element("Lagrange", cell, 1, shape=(2,))
 mesh = Mesh(v_el)
 
 # Define mixed function space
 el = basix.ufl.element("P", cell, 2)
-el_int = basix.ufl.element("Discontinuous Lagrange", cell, 1, shape=(2, ))
+el_int = basix.ufl.element("Discontinuous Lagrange", cell, 1, shape=(2,))
 me = basix.ufl.mixed_element([el, el_int])
 V = FunctionSpace(mesh, me)
 u = Coefficient(V)
 
 # Define expressions on each sub-space
 du0 = grad(u[0])
 du1 = grad(u[1])
 
 # Define an expression using quadrature elements
 q_rule = "gauss_jacobi"
 q_degree = 3
-q_el = QuadratureElement(cell, (), q_rule, q_degree)
+q_el = basix.ufl.quadrature_element(cell, scheme=q_rule, degree=q_degree)
 Q = FunctionSpace(mesh, q_el)
 q = Coefficient(Q)
 powq = 3 * q**2
 
 # Extract basix cell type
 b_cell = basix.cell.string_to_type(cell)
 
 # Find quadrature points for quadrature element
 b_rule = basix.quadrature.string_to_type(q_rule)
 quadrature_points, _ = basix.quadrature.make_quadrature(b_cell, q_degree, rule=b_rule)
 
 # Get interpolation points for output space
 family = basix.finite_element.string_to_family("Lagrange", cell)
-b_element = basix.create_element(family, b_cell, 4, basix.LagrangeVariant.gll_warped, discontinuous=True)
+b_element = basix.create_element(
+    family, b_cell, 4, basix.LagrangeVariant.gll_warped, discontinuous=True
+)
 interpolation_points = b_element.points
 
 # Create expressions that can be used for interpolation
-expressions = [(du0, interpolation_points), (du1, interpolation_points),
-               (powq, quadrature_points)]
+expressions = [(du0, interpolation_points), (du1, interpolation_points), (powq, quadrature_points)]
```

### Comparing `fenics-ffcx-0.7.0/demo/FacetIntegrals.py` & `fenics_ffcx-0.8.0/demo/Normals.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2009-2010 Anders Logg
+# Copyright (C) 2009 Peter Brune
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,27 +10,29 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# First added:  2009-03-20
-# Last changed: 2011-03-08
-#
-# Simple example of a form defined over exterior and interior facets.
+"""Normals demo.
+
+This example demonstrates how to use the facet normals
+Merely project the normal onto a vector section.
+"""
+
 import basix.ufl
-from ufl import (FacetNormal, TestFunction, TrialFunction, avg, ds, dS, grad,
-                 inner, jump, triangle)
+from ufl import FacetNormal, FunctionSpace, Mesh, TestFunction, TrialFunction, ds, inner, triangle
+
+cell = triangle
 
-element = basix.ufl.element("Discontinuous Lagrange", "triangle", 1)
+element = basix.ufl.element("Lagrange", cell.cellname(), 1, shape=(2,))
+domain = Mesh(basix.ufl.element("Lagrange", cell.cellname(), 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-u = TrialFunction(element)
-v = TestFunction(element)
+n = FacetNormal(domain)
 
-n = FacetNormal(triangle)
+v = TrialFunction(space)
+u = TestFunction(space)
 
-a = u * v * ds \
-    + u('+') * v('-') * dS \
-    + inner(jump(u, n), avg(grad(v))) * dS \
-    + inner(avg(grad(u)), jump(v, n)) * dS
+a = inner(v, u) * ds
+L = inner(n, u) * ds
```

### Comparing `fenics-ffcx-0.7.0/demo/FacetRestrictionAD.py` & `fenics_ffcx-0.8.0/demo/ReactionDiffusion.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010 Garth N. Wells
+# Copyright (C) 2009 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,19 +10,26 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
+"""Reaction-diffusion demo.
+
+The bilinear form a(u, v) and linear form L(v) for a simple
+reaction-diffusion equation using simplified tuple notation.
+"""
+
 import basix.ufl
-from ufl import (Coefficient, TestFunction, TrialFunction, avg, derivative,
-                 dot, dS, dx, grad, inner)
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, dx, grad, inner
 
-element = basix.ufl.element("Discontinuous Lagrange", "triangle", 1)
+element = basix.ufl.element("Lagrange", "triangle", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-v = TestFunction(element)
-w = Coefficient(element)
-L = inner(grad(w), grad(v)) * dx - dot(avg(grad(w)), avg(grad(v))) * dS
+u = TrialFunction(space)
+v = TestFunction(space)
+f = Coefficient(space)
 
-u = TrialFunction(element)
-a = derivative(L, w, u)
+a = (inner(grad(u), grad(v)) + inner(u, v)) * dx
+L = inner(f, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/HyperElasticity.py` & `fenics_ffcx-0.8.0/demo/HyperElasticity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,85 @@
-#
 # Author: Martin Sandve Alnes
 # Date: 2008-12-22
-#
+# Modified by Garth N. Wells, 2009
+"""Hyper-elasticity demo."""
 
 import basix.ufl
-# Modified by Garth N. Wells, 2009
-from ufl import (Coefficient, Constant, FacetNormal, Identity,
-                 SpatialCoordinate, TestFunction, TrialFunction, derivative,
-                 det, diff, dot, ds, dx, exp, grad, inner, inv, tetrahedron,
-                 tr, variable)
+from ufl import (
+    Coefficient,
+    Constant,
+    FacetNormal,
+    FunctionSpace,
+    Identity,
+    Mesh,
+    SpatialCoordinate,
+    TestFunction,
+    TrialFunction,
+    derivative,
+    det,
+    diff,
+    ds,
+    dx,
+    exp,
+    grad,
+    inner,
+    inv,
+    tetrahedron,
+    tr,
+    variable,
+)
 
 # Cell and its properties
 cell = tetrahedron
-d = cell.geometric_dimension()
-N = FacetNormal(cell)
-x = SpatialCoordinate(cell)
+d = 3
 
 # Elements
-u_element = basix.ufl.element("P", cell.cellname(), 2, shape=(3, ))
+u_element = basix.ufl.element("P", cell.cellname(), 2, shape=(3,))
 p_element = basix.ufl.element("P", cell.cellname(), 1)
 A_element = basix.ufl.element("P", cell.cellname(), 1, shape=(3, 3))
 
+# Spaces
+domain = Mesh(basix.ufl.element("Lagrange", cell.cellname(), 1, shape=(3,)))
+u_space = FunctionSpace(domain, u_element)
+p_space = FunctionSpace(domain, p_element)
+A_space = FunctionSpace(domain, A_element)
+
+# Cell properties
+N = FacetNormal(domain)
+x = SpatialCoordinate(domain)
+
 # Test and trial functions
-v = TestFunction(u_element)
-w = TrialFunction(u_element)
+v = TestFunction(u_space)
+w = TrialFunction(u_space)
 
 # Displacement at current and two previous timesteps
-u = Coefficient(u_element)
-up = Coefficient(u_element)
-upp = Coefficient(u_element)
+u = Coefficient(u_space)
+up = Coefficient(u_space)
+upp = Coefficient(u_space)
 
 # Time parameters
-dt = Constant(cell)
+dt = Constant(domain)
 
 # Fiber field
-A = Coefficient(A_element)
+A = Coefficient(A_space)
 
 # External forces
-T = Coefficient(u_element)
-p0 = Coefficient(p_element)
+T = Coefficient(u_space)
+p0 = Coefficient(p_space)
 
 # Material parameters FIXME
-rho = Constant(cell)
-K = Constant(cell)
-c00 = Constant(cell)
-c11 = Constant(cell)
-c22 = Constant(cell)
+rho = Constant(domain)
+K = Constant(domain)
+c00 = Constant(domain)
+c11 = Constant(domain)
+c22 = Constant(domain)
 
 # Deformation gradient
-I = Identity(d)
-F = I + grad(u)
+Ident = Identity(d)
+F = Ident + grad(u)
 F = variable(F)
 Finv = inv(F)
 J = det(F)
 
 # Left Cauchy-Green deformation tensor
 B = F * F.T
 I1_B = tr(B)
@@ -63,34 +89,38 @@
 # Right Cauchy-Green deformation tensor
 C = F.T * F
 I1_C = tr(C)
 I2_C = (I1_C**2 - tr(C * C)) / 2
 I3_C = J**2
 
 # Green strain tensor
-E = (C - I) / 2
+E = (C - Ident) / 2
 
 # Mapping of strain in fiber directions
 Ef = A * E * A.T
 
 # Strain energy function W(Q(Ef))
-Q = c00 * Ef[0, 0]**2 + c11 * Ef[1, 1]**2 + c22 * Ef[2, 2]**2  # FIXME: insert some simple law here
+Q = (
+    c00 * Ef[0, 0] ** 2 + c11 * Ef[1, 1] ** 2 + c22 * Ef[2, 2] ** 2
+)  # FIXME: insert some simple law here
 W = (K / 2) * (exp(Q) - 1)  # + p stuff
 
 # First Piola-Kirchoff stress tensor
 P = diff(W, F)
 
 # Acceleration term discretized with finite differences
 k = dt / rho
-acc = (u - 2 * up + upp)
+acc = u - 2 * up + upp
 
 # Residual equation # FIXME: Can contain errors, not tested!
-a_F = inner(acc, v) * dx \
-    + k * inner(P, grad(v)) * dx \
-    - k * dot(J * Finv * T, v) * ds(0) \
-    - k * dot(J * Finv * p0 * N, v) * ds(1)
+a_F = (
+    inner(acc, v) * dx
+    + k * inner(P, grad(v)) * dx
+    - k * inner(J * Finv * T, v) * ds(0)
+    - k * inner(J * Finv * p0 * N, v) * ds(1)
+)
 
 # Jacobi matrix of residual equation
 a_J = derivative(a_F, u, w)
 
 # Export forms
 forms = [a_F, a_J]
```

### Comparing `fenics-ffcx-0.7.0/demo/MassDG0.py` & `fenics_ffcx-0.8.0/demo/MassHcurl_2D_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Igor Baratta
+# Copyright (C) 2004-2010 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,18 +10,20 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form for a mass matrix.
+"""H(curl) mass matrix demo."""
+
 import basix.ufl
-from ufl import TestFunction, TrialFunction, dx, inner
+from ufl import FunctionSpace, Mesh, TestFunction, TrialFunction, dx, inner
 
-element = basix.ufl.element("DG", "tetrahedron", 0)
+element = basix.ufl.element("N1curl", "triangle", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-v = TestFunction(element)
-u = TrialFunction(element)
+v = TestFunction(space)
+u = TrialFunction(space)
 
 a = inner(u, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/MassHcurl_2D_1.py` & `fenics_ffcx-0.8.0/demo/Poisson1D.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2004-2010 Anders Logg
+# Copyright (C) 2004-2007 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,16 +10,25 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
+"""1D Poisson demo.
+
+The bilinear form a(u, v) and linear form L(v) for Poisson's equation.
+"""
+
 import basix.ufl
-from ufl import TestFunction, TrialFunction, dx, inner
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, dx, grad, inner
 
-element = basix.ufl.element("N1curl", "triangle", 1)
+element = basix.ufl.element("Lagrange", "interval", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "interval", 1, shape=(1,)))
+space = FunctionSpace(domain, element)
 
-v = TestFunction(element)
-u = TrialFunction(element)
+u = TrialFunction(space)
+v = TestFunction(space)
+f = Coefficient(space)
 
-a = inner(v, u) * dx
+a = inner(grad(u), grad(v)) * dx
+L = inner(f, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/MassHdiv_2D_1.py` & `fenics_ffcx-0.8.0/demo/PoissonQuad.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010 Anders Logg
+# Copyright (C) 2016 Jan Blechta
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,16 +10,29 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
+"""Quadrilateral Poisson demo.
+
+The bilinear form a(u, v) and linear form L(v) for
+Poisson's equation using bilinear elements on bilinear mesh geometry.
+"""
+
 import basix.ufl
-from ufl import TestFunction, TrialFunction, dx, inner
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, dx, grad, inner
+
+coords = basix.ufl.element("P", "triangle", 2, shape=(2,))
+mesh = Mesh(coords)
+dx = dx(mesh)
 
-element = basix.ufl.element("BDM", "triangle", 1)
+element = basix.ufl.element("P", mesh.ufl_cell().cellname(), 2)
+space = FunctionSpace(mesh, element)
 
-v = TestFunction(element)
-u = TrialFunction(element)
+u = TrialFunction(space)
+v = TestFunction(space)
+f = Coefficient(space)
 
-a = inner(v, u) * dx
+a = inner(grad(u), grad(v)) * dx
+L = inner(f, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/MathFunctions.py` & `fenics_ffcx-0.8.0/demo/MathFunctions.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,36 +10,95 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# Test all algebra operators on Coefficients.
+"""Math function demo.
+
+Test all algebra operators on Coefficients.
+"""
+
 import basix.ufl
-from ufl import (Coefficient, acos, asin, atan, bessel_J, bessel_Y, cos, dx,
-                 erf, exp, ln, sin, sqrt, tan)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    acos,
+    asin,
+    atan,
+    bessel_J,
+    bessel_Y,
+    cos,
+    dx,
+    erf,
+    exp,
+    ln,
+    sin,
+    sqrt,
+    tan,
+)
 
 element = basix.ufl.element("Lagrange", "triangle", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-c0 = Coefficient(element)
-c1 = Coefficient(element)
+c0 = Coefficient(space)
+c1 = Coefficient(space)
 
 s0 = 3 * c0 - c1
 p0 = c0 * c1
 f0 = c0 / c1
 
-integrand = sqrt(c0) + sqrt(s0) + sqrt(p0) + sqrt(f0)\
-    + exp(c0) + exp(s0) + exp(p0) + exp(f0)\
-    + ln(c0) + ln(s0) + ln(p0) + ln(f0)\
-    + cos(c0) + cos(s0) + cos(p0) + cos(f0)\
-    + sin(c0) + sin(s0) + sin(p0) + sin(f0)\
-    + tan(c0) + tan(s0) + tan(p0) + tan(f0)\
-    + acos(c0) + acos(s0) + acos(p0) + acos(f0)\
-    + asin(c0) + asin(s0) + asin(p0) + asin(f0)\
-    + atan(c0) + atan(s0) + atan(p0) + atan(f0)\
-    + erf(c0) + erf(s0) + erf(p0) + erf(f0)\
-    + bessel_J(1, c0) + bessel_J(1, s0) + bessel_J(0, p0) + bessel_J(0, f0)\
-    + bessel_Y(1, c0) + bessel_Y(1, s0) + bessel_Y(0, p0) + bessel_Y(0, f0)
+integrand = (
+    sqrt(c0)
+    + sqrt(s0)
+    + sqrt(p0)
+    + sqrt(f0)
+    + exp(c0)
+    + exp(s0)
+    + exp(p0)
+    + exp(f0)
+    + ln(c0)
+    + ln(s0)
+    + ln(p0)
+    + ln(f0)
+    + cos(c0)
+    + cos(s0)
+    + cos(p0)
+    + cos(f0)
+    + sin(c0)
+    + sin(s0)
+    + sin(p0)
+    + sin(f0)
+    + tan(c0)
+    + tan(s0)
+    + tan(p0)
+    + tan(f0)
+    + acos(c0)
+    + acos(s0)
+    + acos(p0)
+    + acos(f0)
+    + asin(c0)
+    + asin(s0)
+    + asin(p0)
+    + asin(f0)
+    + atan(c0)
+    + atan(s0)
+    + atan(p0)
+    + atan(f0)
+    + erf(c0)
+    + erf(s0)
+    + erf(p0)
+    + erf(f0)
+    + bessel_J(1, c0)
+    + bessel_J(1, s0)
+    + bessel_J(0, p0)
+    + bessel_J(0, f0)
+    + bessel_Y(1, c0)
+    + bessel_Y(1, s0)
+    + bessel_Y(0, p0)
+    + bessel_Y(0, f0)
+)
 
 a = integrand * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/Mini.py` & `fenics_ffcx-0.8.0/demo/Mini.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# Illustration of vector sum of elements (EnrichedElement): The
-# bilinear form a(u, v) for the Stokes equations using a mixed
-# formulation involving the Mini element. The velocity element is
-# composed of a P1 element augmented by the cubic bubble function.
+"""Mini element demo.
+
+Illustration of vector sum of elements (EnrichedElement): The
+bilinear form a(u, v) for the Stokes equations using a mixed
+formulation involving the Mini element. The velocity element is
+composed of a P1 element augmented by the cubic bubble function.
+"""
+
 import basix.ufl
-from ufl import TestFunctions, TrialFunctions, div, dx, grad, inner
+from ufl import FunctionSpace, Mesh, TestFunctions, TrialFunctions, div, dx, grad, inner
 
 P1 = basix.ufl.element("Lagrange", "triangle", 1)
 B = basix.ufl.element("Bubble", "triangle", 3)
-V = basix.ufl.blocked_element(basix.ufl.enriched_element([P1, B]), shape=(2, ))
+V = basix.ufl.blocked_element(basix.ufl.enriched_element([P1, B]), shape=(2,))
 Q = basix.ufl.element("P", "triangle", 1)
 
-Mini = basix.ufl.mixed_element([V, Q])
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+Mini = FunctionSpace(domain, basix.ufl.mixed_element([V, Q]))
+
 (u, p) = TrialFunctions(Mini)
 (v, q) = TestFunctions(Mini)
 
-a = (inner(grad(u), grad(v)) - div(v) * p + div(u) * q) * dx
+a = (inner(grad(u), grad(v)) - inner(p, div(v)) + inner(div(u), q)) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/MixedCoefficient.py` & `fenics_ffcx-0.8.0/demo/TraceElement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
-
-# Copyright (C) 2016 Miklós Homolya
+# Copyright (C) 2015 Marie E. Rognes
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,21 +10,17 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# Mixed coefficient.
-import basix.ufl
-from ufl import Coefficients, dot, dS, dx
+"""Trace element demo."""
 
-DG = basix.ufl.element("DG", "triangle", 0, shape=(2, ))
-CG = basix.ufl.element("Lagrange", "triangle", 2)
-RT = basix.ufl.element("RT", "triangle", 3)
-
-element = basix.ufl.mixed_element([DG, CG, RT])
-
-f, g, h = Coefficients(element)
+import basix.ufl
+from ufl import FunctionSpace, Mesh, TestFunction, avg, dS, ds
 
-forms = [dot(f('+'), h('-')) * dS + g * dx]
+element = basix.ufl.element("HDiv Trace", "triangle", 0)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
+v = TestFunction(space)
+L = v * ds + avg(v) * dS
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fenics-ffcx-0.7.0/demo/MixedPoissonDual.py` & `fenics_ffcx-0.8.0/demo/MixedPoissonDual.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 # DOLFINx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with DOLFINx. If not, see <http://www.gnu.org/licenses/>.
-#
-# First added:  2014-01-29
-# Last changed: 2014-01-29
-#
-# The bilinear form a(u, v) and linear form L(v) for a two-field
-# (mixed) formulation of Poisson's equation
+"""Mixed Poisson dual demo.
+
+The bilinear form a(u, v) and linear form L(v) for a two-field
+(mixed) formulation of Poisson's equation.
+"""
+
 import basix.ufl
-from ufl import Coefficient, TestFunctions, TrialFunctions, dot, ds, dx, grad
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunctions, TrialFunctions, ds, dx, grad, inner
 
 DRT = basix.ufl.element("Discontinuous RT", "triangle", 2)
 P = basix.ufl.element("P", "triangle", 3)
 W = basix.ufl.mixed_element([DRT, P])
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, W)
 
-(sigma, u) = TrialFunctions(W)
-(tau, v) = TestFunctions(W)
+(sigma, u) = TrialFunctions(space)
+(tau, v) = TestFunctions(space)
 
 P1 = basix.ufl.element("P", "triangle", 1)
-f = Coefficient(P1)
-g = Coefficient(P1)
+space = FunctionSpace(domain, P1)
+f = Coefficient(space)
+g = Coefficient(space)
 
-a = (dot(sigma, tau) + dot(grad(u), tau) + dot(sigma, grad(v))) * dx
-L = - f * v * dx - g * v * ds
+a = (inner(sigma, tau) + inner(grad(u), tau) + inner(sigma, grad(v))) * dx
+L = -inner(f, v) * dx - inner(g, v) * ds
```

### Comparing `fenics-ffcx-0.7.0/demo/Normals.py` & `fenics_ffcx-0.8.0/test/Poisson.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2009 Peter Brune
+# Copyright (C) 2004-2007 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,23 +11,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
 #
-# This example demonstrates how to use the facet normals
-# Merely project the normal onto a vector section.
+"""The bilinear form a(u, v) and linear form L(v) for Poisson's equation.
+
+Compile this form with FFCx: ffcx Poisson.ufl.
+"""
+
 import basix.ufl
-from ufl import FacetNormal, TestFunction, TrialFunction, dot, ds, triangle
+from ufl import (
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dx,
+    grad,
+    inner,
+)
 
-cell = triangle
+mesh = Mesh(basix.ufl.element("P", "triangle", 2, shape=(2,)))
 
-element = basix.ufl.element("Lagrange", cell.cellname(), 1, shape=(2, ))
+e = basix.ufl.element("Lagrange", "triangle", 2)
+space = FunctionSpace(mesh, e)
 
-n = FacetNormal(cell)
+u = TrialFunction(space)
+v = TestFunction(space)
+f = Coefficient(space)
 
-v = TrialFunction(element)
-u = TestFunction(element)
+kappa1 = Constant(mesh, shape=(2, 2))
+kappa2 = Constant(mesh, shape=(2, 2))
 
-a = dot(v, u) * ds
-L = dot(n, u) * ds
+a = inner(kappa1, kappa2) * inner(grad(u), grad(v)) * dx
+L = f * v * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/Poisson1D.py` & `fenics_ffcx-0.8.0/demo/VectorPoisson.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2004-2007 Anders Logg
+# Copyright (C) 2010 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,21 +10,25 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation.
+"""Vector Poisson demo.
+
+The bilinear form a(u, v) and linear form L(v) for the vector-valued Poisson's equation.
+"""
+
 import basix.ufl
-from ufl import Coefficient, TestFunction, TrialFunction, dx, grad, inner
+from ufl import Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction, dx, grad, inner
 
-element = basix.ufl.element("Lagrange", "interval", 1)
+element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2,))
+domain = Mesh(element)
+space = FunctionSpace(domain, element)
 
-u = TrialFunction(element)
-v = TestFunction(element)
-f = Coefficient(element)
+u = TrialFunction(space)
+v = TestFunction(space)
+f = Coefficient(space)
 
 a = inner(grad(u), grad(v)) * dx
-L = f * v * dx
+L = inner(f, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/PoissonQuad.py` & `fenics_ffcx-0.8.0/demo/VectorConstant.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,27 +10,42 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation using bilinear elements on bilinear mesh geometry.
+"""Vector constant demo.
+
+The bilinear form a(u, v) and linear form L(v) for
+Poisson's equation using bilinear elements on bilinear mesh geometry.
+"""
+
 import basix.ufl
-from ufl import (Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 dx, grad, inner)
+from ufl import (
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dx,
+    grad,
+    inner,
+)
 
-coords = basix.ufl.element("P", "triangle", 2, shape=(2, ))
+coords = basix.ufl.element("P", "triangle", 2, shape=(2,))
 mesh = Mesh(coords)
 dx = dx(mesh)
 
 element = basix.ufl.element("P", mesh.ufl_cell().cellname(), 2)
 space = FunctionSpace(mesh, element)
 
 u = TrialFunction(space)
 v = TestFunction(space)
 f = Coefficient(space)
 
-a = inner(grad(u), grad(v)) * dx
-L = f * v * dx
+L = inner(f, v) * dx
+
+mu = Constant(mesh, shape=(3,))
+theta = -(mu[1] - 2) / mu[0] - (2 * (2 * mu[0] - 2) * (mu[0] - 1)) / (mu[0] * (mu[1] - 2))
+a = theta * inner(grad(u), grad(v)) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/ProjectionManifold.py` & `fenics_ffcx-0.8.0/demo/MassHdiv_2D_1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2012 Marie E. Rognes and David Ham
+# Copyright (C) 2010 Anders Logg
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,22 +10,20 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# This demo illustrates use of finite element spaces defined over
-# simplicies embedded in higher dimensions
+"""H(div) mass matrix demo."""
+
 import basix.ufl
-from ufl import TestFunctions, TrialFunctions, div, dx, inner
+from ufl import FunctionSpace, Mesh, TestFunction, TrialFunction, dx, inner
 
-# Define element over this domain
-V = basix.ufl.element("RT", "triangle", 1, gdim=3)
-Q = basix.ufl.element("DG", "triangle", 0, gdim=3)
-element = basix.ufl.mixed_element([V, Q])
+element = basix.ufl.element("BDM", "triangle", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-(u, p) = TrialFunctions(element)
-(v, q) = TestFunctions(element)
+v = TestFunction(space)
+u = TrialFunction(space)
 
-a = (inner(u, v) + div(u) * q + div(v) * p) * dx
+a = inner(u, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/SpatialCoordinates.py` & `fenics_ffcx-0.8.0/demo/ProjectionManifold.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010 Kristian B. Oelgaard
+# Copyright (C) 2012 Marie E. Rognes and David Ham
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,28 +10,27 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation where spatial coordinates are used to define the source
-# and boundary flux terms.
-import basix.ufl
-from ufl import (SpatialCoordinate, TestFunction, TrialFunction, ds, dx, exp,
-                 grad, inner, sin, triangle)
+"""Projection manifold demo.
 
-element = basix.ufl.element("Lagrange", "triangle", 2)
+This demo illustrates use of finite element spaces defined over
+simplicies embedded in higher dimensions.
+"""
+
+import basix.ufl
+from ufl import FunctionSpace, Mesh, TestFunctions, TrialFunctions, div, dx, inner
 
-u = TrialFunction(element)
-v = TestFunction(element)
+# Define element over this domain
+V = basix.ufl.element("RT", "triangle", 1)
+Q = basix.ufl.element("DG", "triangle", 0)
+element = basix.ufl.mixed_element([V, Q])
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(3,)))
+space = FunctionSpace(domain, element)
 
-x = SpatialCoordinate(triangle)
-d_x = x[0] - 0.5
-d_y = x[1] - 0.5
-f = 10.0 * exp(-(d_x * d_x + d_y * d_y) / 0.02)
-g = sin(5.0 * x[0])
+(u, p) = TrialFunctions(space)
+(v, q) = TestFunctions(space)
 
-a = inner(grad(u), grad(v)) * dx
-L = f * v * dx + g * v * ds
+a = (inner(u, v) + inner(div(u), q) + inner(p, div(v))) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/StabilisedStokes.py` & `fenics_ffcx-0.8.0/demo/StabilisedStokes.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,29 +10,46 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and Linear form L(v) for the Stokes
-# equations using a mixed formulation (equal-order stabilized).
+"""Stabilised Stokes demo.
+
+The bilinear form a(u, v) and Linear form L(v) for the Stokes
+equations using a mixed formulation (equal-order stabilized).
+"""
+
 import basix.ufl
-from ufl import (Coefficient, TestFunctions, TrialFunctions, div, dot, dx,
-                 grad, inner)
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunctions,
+    TrialFunctions,
+    div,
+    dot,
+    dx,
+    grad,
+    inner,
+)
 
-vector = basix.ufl.element("Lagrange", "triangle", 1, shape=(2, ))
+vector = basix.ufl.element("Lagrange", "triangle", 1, shape=(2,))
 scalar = basix.ufl.element("Lagrange", "triangle", 1)
 system = basix.ufl.mixed_element([vector, scalar])
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+system_space = FunctionSpace(domain, system)
+scalar_space = FunctionSpace(domain, scalar)
+vector_space = FunctionSpace(domain, vector)
 
-(u, p) = TrialFunctions(system)
-(v, q) = TestFunctions(system)
+(u, p) = TrialFunctions(system_space)
+(v, q) = TestFunctions(system_space)
 
-f = Coefficient(vector)
-h = Coefficient(scalar)
+f = Coefficient(vector_space)
+h = Coefficient(scalar_space)
 
 beta = 0.2
 delta = beta * h * h
 
 a = (inner(grad(u), grad(v)) - div(v) * p + div(u) * q + delta * dot(grad(p), grad(q))) * dx
 L = dot(f, v + delta * grad(q)) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/TraceElement.py` & `fenics_ffcx-0.8.0/demo/MixedCoefficient.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015 Marie E. Rognes
+# Copyright (C) 2016 Miklós Homolya
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,13 +10,23 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
+"""Mixed coefficient demo."""
+
 import basix.ufl
-from ufl import TestFunction, avg, ds, dS
+from ufl import Coefficients, FunctionSpace, Mesh, dot, dS, dx
+
+DG = basix.ufl.element("DG", "triangle", 0, shape=(2,))
+CG = basix.ufl.element("Lagrange", "triangle", 2)
+RT = basix.ufl.element("RT", "triangle", 3)
+
+element = basix.ufl.mixed_element([DG, CG, RT])
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
+
+f, g, h = Coefficients(space)
 
-element = basix.ufl.element("HDiv Trace", "triangle", 0)
-v = TestFunction(element)
-L = v * ds + avg(v) * dS
+forms = [dot(f("+"), h("-")) * dS + g * dx]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenics-ffcx-0.7.0/demo/VectorConstant.py` & `fenics_ffcx-0.8.0/demo/MassDG0.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016 Jan Blechta
+# Copyright (C) 2021 Igor Baratta
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,30 +10,23 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation using bilinear elements on bilinear mesh geometry.
-import basix.ufl
-from ufl import (Constant, Coefficient, FunctionSpace, Mesh, TestFunction, TrialFunction,
-                 dx, grad, inner)
+"""DG mass matrix demo.
 
-coords = basix.ufl.element("P", "triangle", 2, shape=(2, ))
-mesh = Mesh(coords)
-dx = dx(mesh)
+The bilinear form for a mass matrix.
+"""
 
-element = basix.ufl.element("P", mesh.ufl_cell().cellname(), 2)
-space = FunctionSpace(mesh, element)
+import basix.ufl
+from ufl import FunctionSpace, Mesh, TestFunction, TrialFunction, dx, inner
 
-u = TrialFunction(space)
-v = TestFunction(space)
-f = Coefficient(space)
+element = basix.ufl.element("DG", "tetrahedron", 0)
+domain = Mesh(basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3,)))
+space = FunctionSpace(domain, element)
 
-L = f * v * dx
+v = TestFunction(space)
+u = TrialFunction(space)
 
-mu = Constant(mesh, shape=(3,))
-theta = - (mu[1] - 2) / mu[0] - (2 * (2 * mu[0] - 2) * (mu[0] - 1)) / (mu[0] * (mu[1] - 2))
-a = theta * inner(grad(u), grad(v)) * dx
+a = inner(u, v) * dx
```

### Comparing `fenics-ffcx-0.7.0/demo/VectorPoisson.py` & `fenics_ffcx-0.8.0/demo/FacetRestrictionAD.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2010 Anders Logg
+# Copyright (C) 2010 Garth N. Wells
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,21 +10,34 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# the vector-valued Poisson's equation.
+"""Facet restriction demo."""
+
 import basix.ufl
-from ufl import Coefficient, TestFunction, TrialFunction, dx, grad, inner
+from ufl import (
+    Coefficient,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    avg,
+    derivative,
+    dS,
+    dx,
+    grad,
+    inner,
+)
 
-element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2, ))
+element = basix.ufl.element("Discontinuous Lagrange", "triangle", 1)
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
 
-u = TrialFunction(element)
-v = TestFunction(element)
-f = Coefficient(element)
+v = TestFunction(space)
+w = Coefficient(space)
+L = inner(grad(w), grad(v)) * dx - inner(avg(grad(w)), avg(grad(v))) * dS
 
-a = inner(grad(u), grad(v)) * dx
-L = inner(f, v) * dx
+u = TrialFunction(space)
+a = derivative(L, w, u)
```

### Comparing `fenics-ffcx-0.7.0/doc/Makefile` & `fenics_ffcx-0.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/doc/source/conf.py` & `fenics_ffcx-0.8.0/doc/source/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Configuration file for the Sphinx documentation builder.
-#
+"""Configuration file for the Sphinx documentation builder."""
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/stable/config
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
@@ -15,19 +14,19 @@
 # sys.path.insert(0, os.path.abspath('.'))
 import datetime
 
 import ffcx
 
 # -- Project information -----------------------------------------------------
 
-project = 'FEniCS Form Compiler X'
+project = "FEniCS Form Compiler X"
 now = datetime.datetime.now()
 date = now.date()
-copyright = f'{date.year}, FEniCS Project'
-author = 'FEniCS Project'
+copyright = f"{date.year}, FEniCS Project"
+author = "FEniCS Project"
 
 # The short X.Y version
 version = ffcx.__version__
 # The full version, including alpha/beta/rc tags
 release = ffcx.__version__
 
 
@@ -37,50 +36,50 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.doctest',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
@@ -92,15 +91,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
@@ -108,75 +107,87 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'FEniCSFormCompilerXdoc'
+htmlhelp_basename = "FEniCSFormCompilerXdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'FEniCSFormCompilerX.tex', 'FEniCS Form Compiler X Documentation',
-     'FEniCS Project', 'manual'),
+    (
+        master_doc,
+        "FEniCSFormCompilerX.tex",
+        "FEniCS Form Compiler X Documentation",
+        "FEniCS Project",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'fenicsformcompilerx', 'FEniCS Form Compiler X Documentation',
-     [author], 1)
+    (master_doc, "fenicsformcompilerx", "FEniCS Form Compiler X Documentation", [author], 1)
 ]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'FEniCSFormCompilerX', 'FEniCS Form Compiler X Documentation',
-     author, 'FEniCSFormCompilerX', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "FEniCSFormCompilerX",
+        "FEniCS Form Compiler X Documentation",
+        author,
+        "FEniCSFormCompilerX",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
-autodoc_default_options = {'members': True, 'show-inheritance': True, 'imported-members': True, 'undoc-members': True}
+autodoc_default_options = {
+    "members": True,
+    "show-inheritance": True,
+    "imported-members": True,
+    "undoc-members": True,
+}
 autosummary_generate = True
 autoclass_content = "both"
 
 
-autodoc_default_flags = ['members', 'show-inheritance']
+autodoc_default_flags = ["members", "show-inheritance"]
 napoleon_numpy_docstring = True
 napoleon_google_docstring = True
```

### Comparing `fenics-ffcx-0.7.0/doc/source/index.rst` & `fenics_ffcx-0.8.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/fenics_ffcx.egg-info/SOURCES.txt` & `fenics_ffcx-0.8.0/fenics_ffcx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 COPYING.LESSER
 ChangeLog.rst
 INSTALL
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 cmake/CMakeLists.txt
 cmake/ufcx.pc.in
 cmake/ufcxConfig.cmake.in
 demo/BiharmonicHHJ.py
 demo/BiharmonicRegge.py
 demo/CellGeometry.py
 demo/ComplexPoisson.py
 demo/Components.py
 demo/Conditional.py
 demo/ExpressionInterpolation.py
 demo/FacetIntegrals.py
 demo/FacetRestrictionAD.py
 demo/HyperElasticity.py
+demo/MassAction.py
 demo/MassDG0.py
 demo/MassHcurl_2D_1.py
 demo/MassHdiv_2D_1.py
 demo/MathFunctions.py
 demo/MetaData.py
 demo/Mini.py
 demo/MixedCoefficient.py
@@ -45,15 +45,14 @@
 doc/Makefile
 doc/source/conf.py
 doc/source/index.rst
 fenics_ffcx.egg-info/PKG-INFO
 fenics_ffcx.egg-info/SOURCES.txt
 fenics_ffcx.egg-info/dependency_links.txt
 fenics_ffcx.egg-info/entry_points.txt
-fenics_ffcx.egg-info/not-zip-safe
 fenics_ffcx.egg-info/requires.txt
 fenics_ffcx.egg-info/top_level.txt
 ffcx/__init__.py
 ffcx/__main__.py
 ffcx/analysis.py
 ffcx/compiler.py
 ffcx/element_interface.py
@@ -64,19 +63,19 @@
 ffcx/options.py
 ffcx/codegeneration/__init__.py
 ffcx/codegeneration/access.py
 ffcx/codegeneration/backend.py
 ffcx/codegeneration/codegeneration.py
 ffcx/codegeneration/definitions.py
 ffcx/codegeneration/expression_generator.py
-ffcx/codegeneration/flop_count.py
 ffcx/codegeneration/geometry.py
 ffcx/codegeneration/integral_generator.py
 ffcx/codegeneration/jit.py
 ffcx/codegeneration/lnodes.py
+ffcx/codegeneration/optimizer.py
 ffcx/codegeneration/symbols.py
 ffcx/codegeneration/ufcx.h
 ffcx/codegeneration/utils.py
 ffcx/codegeneration/C/__init__.py
 ffcx/codegeneration/C/basix_custom_element_template.py
 ffcx/codegeneration/C/c_implementation.py
 ffcx/codegeneration/C/dofmap.py
@@ -87,14 +86,15 @@
 ffcx/codegeneration/C/file_template.py
 ffcx/codegeneration/C/finite_element.py
 ffcx/codegeneration/C/finite_element_template.py
 ffcx/codegeneration/C/form.py
 ffcx/codegeneration/C/form_template.py
 ffcx/codegeneration/C/integrals.py
 ffcx/codegeneration/C/integrals_template.py
+ffcx/codegeneration/C/quadrature_rule_template.py
 ffcx/ir/__init__.py
 ffcx/ir/elementtables.py
 ffcx/ir/integral.py
 ffcx/ir/representation.py
 ffcx/ir/representationutils.py
 ffcx/ir/analysis/__init__.py
 ffcx/ir/analysis/factorization.py
@@ -106,11 +106,13 @@
 ffcx/ir/analysis/visualise.py
 test/Poisson.py
 test/conftest.py
 test/test_add_mode.py
 test/test_blocked_elements.py
 test/test_cache.py
 test/test_cmdline.py
-test/test_elements.py
 test/test_jit_expression.py
 test/test_jit_forms.py
-test/test_lnodes.py
+test/test_lnodes.py
+test/test_signatures.py
+test/test_submesh.py
+test/test_tensor_product.py
```

### Comparing `fenics-ffcx-0.7.0/ffcx/analysis.py` & `fenics_ffcx-0.8.0/ffcx/analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,138 +7,157 @@
 """Compiler stage 1: Analysis.
 
 This module implements the analysis/preprocessing of variational forms,
 including automatic selection of elements, degrees and form
 representation type.
 """
 
+from __future__ import annotations
+
 import logging
 import typing
-from warnings import warn
 
+import basix.ufl
 import numpy as np
 import numpy.typing as npt
-
-import basix.ufl
 import ufl
-from ffcx.element_interface import convert_element
 
 logger = logging.getLogger("ffcx")
 
 
 class UFLData(typing.NamedTuple):
-    form_data: typing.Tuple[ufl.algorithms.formdata.FormData, ...]  # Tuple of ufl form data
-    unique_elements: typing.List[basix.ufl._ElementBase]  # List of unique elements
+    """UFL data."""
+
+    # Tuple of ufl form data
+    form_data: tuple[ufl.algorithms.formdata.FormData, ...]
+    # List of unique elements
+    unique_elements: list[basix.ufl._ElementBase]
     # Lookup table from each unique element to its index in `unique_elements`
-    element_numbers: typing.Dict[basix.ufl._ElementBase, int]
-    unique_coordinate_elements: typing.List[basix.ufl._ElementBase]  # List of unique coordinate elements
+    element_numbers: dict[basix.ufl._ElementBase, int]
+    # List of unique coordinate elements
+    unique_coordinate_elements: list[basix.ufl._ElementBase]
     # List of ufl Expressions as tuples (expression, points, original_expression)
-    expressions: typing.List[typing.Tuple[ufl.core.expr.Expr, npt.NDArray[np.float64], ufl.core.expr.Expr]]
+    expressions: list[tuple[ufl.core.expr.Expr, npt.NDArray[np.float64], ufl.core.expr.Expr]]
 
 
-def analyze_ufl_objects(ufl_objects: typing.List, options: typing.Dict) -> UFLData:
+def analyze_ufl_objects(
+    ufl_objects: list[
+        ufl.form.Form
+        | ufl.AbstractFiniteElement
+        | ufl.Mesh
+        | tuple[ufl.core.expr.Expr, npt.NDArray[np.floating]]
+    ],
+    scalar_type: npt.DTypeLike,
+) -> UFLData:
     """Analyze ufl object(s).
 
-    Options
-    ----------
-    ufl_objects
-    options
-      FFCx options. These options take priority over all other set options.
-
-    Returns a data structure holding
-    -------
-    form_datas
-        Form_data objects
-    unique_elements
-        Unique elements across all forms and expressions
-    element_numbers
-        Mapping to unique numbers for all elements
-    unique_coordinate_elements
-        Unique coordinate elements across all forms and expressions
-    expressions
-        List of all expressions after post-processing, with its
-        evaluation points and the original expression
+    Args:
+        ufl_objects: UFL objects
+        scalar_type: Scalar type that should be used for the analysis
 
+    Returns:
+        A data structure holding:
+            form_datas: Form_data objects
+            unique_elements: Unique elements across all forms and expressions
+            element_numbers: Mapping to unique numbers for all elements
+            unique_coordinate_elements: Unique coordinate elements across all forms and expressions
+            expressions: List of all expressions after post-processing, with its evaluation points
+                         and the original expression
     """
     logger.info(79 * "*")
     logger.info("Compiler stage 1: Analyzing UFL objects")
     logger.info(79 * "*")
 
-    elements = []
-    coordinate_elements = []
+    elements: list[ufl.AbstractFiniteElement] = []
+    coordinate_elements: list[ufl.AbstractFiniteElement] = []
 
     # Group objects by types
-    forms = []
-    expressions = []
-    processed_expressions = []
+    forms: list[ufl.form.Form] = []
+    expressions: list[tuple[ufl.core.expr.Expr, npt.NDArray[np.floating]]] = []
+    processed_expressions: list[
+        tuple[ufl.core.expr.Expr, npt.NDArray[np.floating], ufl.core.expr.Expr]
+    ] = []
 
     for ufl_object in ufl_objects:
         if isinstance(ufl_object, ufl.form.Form):
             forms.append(ufl_object)
-        elif isinstance(ufl_object, ufl.FiniteElementBase):
-            elements.append(convert_element(ufl_object))
+        elif isinstance(ufl_object, ufl.AbstractFiniteElement):
+            elements.append(ufl_object)
         elif isinstance(ufl_object, ufl.Mesh):
-            coordinate_elements.append(convert_element(ufl_object.ufl_coordinate_element()))
+            coordinate_elements.append(ufl_object.ufl_coordinate_element())
         elif isinstance(ufl_object[0], ufl.core.expr.Expr):
             original_expression = ufl_object[0]
             points = np.asarray(ufl_object[1])
             expressions.append((original_expression, points))
         else:
             raise TypeError("UFL objects not recognised.")
 
-    form_data = tuple(_analyze_form(form, options) for form in forms)
+    form_data = tuple(_analyze_form(form, scalar_type) for form in forms)
     for data in form_data:
-        elements += [convert_element(e) for e in data.unique_sub_elements]
-        coordinate_elements += [convert_element(e) for e in data.coordinate_elements]
+        elements += data.unique_sub_elements
+        coordinate_elements += data.coordinate_elements
 
     for original_expression, points in expressions:
-        elements += [convert_element(e) for e in ufl.algorithms.extract_elements(original_expression)]
-        processed_expression = _analyze_expression(original_expression, options)
+        elements += ufl.algorithms.extract_elements(original_expression)
+        processed_expression = _analyze_expression(original_expression, scalar_type)
         processed_expressions += [(processed_expression, points, original_expression)]
 
     elements += ufl.algorithms.analysis.extract_sub_elements(elements)
 
     # Sort elements so sub-elements come before mixed elements
     unique_elements = ufl.algorithms.sort_elements(set(elements))
     unique_coordinate_element_list = sorted(set(coordinate_elements), key=lambda x: repr(x))
 
     for e in unique_elements:
         assert isinstance(e, basix.ufl._ElementBase)
 
     # Compute dict (map) from element to index
     element_numbers = {element: i for i, element in enumerate(unique_elements)}
 
-    return UFLData(form_data=form_data, unique_elements=unique_elements, element_numbers=element_numbers,
-                   unique_coordinate_elements=unique_coordinate_element_list, expressions=processed_expressions)
+    return UFLData(
+        form_data=form_data,
+        unique_elements=unique_elements,
+        element_numbers=element_numbers,
+        unique_coordinate_elements=unique_coordinate_element_list,
+        expressions=processed_expressions,
+    )
 
 
-def _analyze_expression(expression: ufl.core.expr.Expr, options: typing.Dict):
+def _analyze_expression(
+    expression: ufl.core.expr.Expr, scalar_type: npt.DTypeLike
+) -> ufl.core.expr.Expr:
     """Analyzes and preprocesses expressions."""
-    preserve_geometry_types = (ufl.classes.Jacobian, )
+    preserve_geometry_types = (ufl.classes.Jacobian,)
     expression = ufl.algorithms.apply_algebra_lowering.apply_algebra_lowering(expression)
     expression = ufl.algorithms.apply_derivatives.apply_derivatives(expression)
     expression = ufl.algorithms.apply_function_pullbacks.apply_function_pullbacks(expression)
-    expression = ufl.algorithms.apply_geometry_lowering.apply_geometry_lowering(expression, preserve_geometry_types)
+    expression = ufl.algorithms.apply_geometry_lowering.apply_geometry_lowering(
+        expression, preserve_geometry_types
+    )
     expression = ufl.algorithms.apply_derivatives.apply_derivatives(expression)
-    expression = ufl.algorithms.apply_geometry_lowering.apply_geometry_lowering(expression, preserve_geometry_types)
+    expression = ufl.algorithms.apply_geometry_lowering.apply_geometry_lowering(
+        expression, preserve_geometry_types
+    )
     expression = ufl.algorithms.apply_derivatives.apply_derivatives(expression)
 
-    complex_mode = "_Complex" in options["scalar_type"]
-    if not complex_mode:
+    # Remove complex nodes if scalar type is real valued
+    if not np.issubdtype(scalar_type, np.complexfloating):
         expression = ufl.algorithms.remove_complex_nodes.remove_complex_nodes(expression)
 
     return expression
 
 
-def _analyze_form(form: ufl.form.Form, options: typing.Dict) -> ufl.algorithms.formdata.FormData:
+def _analyze_form(
+    form: ufl.form.Form, scalar_type: npt.DTypeLike
+) -> ufl.algorithms.formdata.FormData:
     """Analyzes UFL form and attaches metadata.
 
     Args:
         form: forms
-        options: options
+        scalar_type: Scalar type used for form. This is used to simplify real valued forms
 
     Returns:
         Form data computed by UFL with metadata attached
 
     Note:
         The main workload of this function is extraction of
         unique/default metadata from options, integral metadata or
@@ -146,88 +165,93 @@
 
     """
     if form.empty():
         raise RuntimeError(f"Form ({form}) seems to be zero: cannot compile it.")
     if _has_custom_integrals(form):
         raise RuntimeError(f"Form ({form}) contains unsupported custom integrals.")
 
-    # Set default spacing for coordinate elements to be equispaced
-    for n, i in enumerate(form._integrals):
-        element = i._ufl_domain._ufl_coordinate_element
-        if not isinstance(element, basix.ufl._ElementBase) and element.degree() > 2:
-            warn("UFL coordinate elements using elements not created via Basix may not work with DOLFINx")
+    # Check that coordinate element is based on basix.ufl._ElementBase
+    for i in form._integrals:
+        assert isinstance(i._ufl_domain._ufl_coordinate_element, basix.ufl._ElementBase)
 
     # Check for complex mode
-    complex_mode = "_Complex" in options["scalar_type"]
+    complex_mode = np.issubdtype(scalar_type, np.complexfloating)
 
     # Compute form metadata
     form_data = ufl.algorithms.compute_form_data(
         form,
         do_apply_function_pullbacks=True,
         do_apply_integral_scaling=True,
         do_apply_geometry_lowering=True,
         preserve_geometry_types=(ufl.classes.Jacobian,),
         do_apply_restrictions=True,
         do_append_everywhere_integrals=False,  # do not add dx integrals to dx(i) in UFL
-        complex_mode=complex_mode)
-
-    # If form contains a quadrature element, use the custom quadrature scheme
-    custom_q = None
-    for e in form_data.unique_elements:
-        e = convert_element(e)
-        if e.has_custom_quadrature:
-            if custom_q is None:
-                custom_q = e.custom_quadrature()
-            else:
-                assert np.allclose(e._points, custom_q[0])
-                assert np.allclose(e._weights, custom_q[1])
+        complex_mode=complex_mode,
+    )
 
     # Determine unique quadrature degree and quadrature scheme
     # per each integral data
     for id, integral_data in enumerate(form_data.integral_data):
         # Iterate through groups of integral data. There is one integral
         # data for all integrals with same domain, itype, subdomain_id
         # (but possibly different metadata).
         #
         # Quadrature degree and quadrature scheme must be the same for
         # all integrals in this integral data group, i.e. must be the
         # same for for the same (domain, itype, subdomain_id)
 
-        qd_default = -1
-        qr_default = "default"
-
         for i, integral in enumerate(integral_data.integrals):
             metadata = integral.metadata()
+            # If form contains a quadrature element, use the custom quadrature scheme
+            custom_q = None
+            for e in ufl.algorithms.extract_elements(integral):
+                if e.has_custom_quadrature:
+                    if custom_q is None:
+                        custom_q = e.custom_quadrature()
+                    else:
+                        p, w = e.custom_quadrature()
+                        assert np.allclose(p, custom_q[0])
+                        assert np.allclose(w, custom_q[1])
+
             if custom_q is None:
                 # Extract quadrature degree
-                qd_metadata = integral.metadata().get("quadrature_degree", qd_default)
-                pd_estimated = np.max(integral.metadata()["estimated_polynomial_degree"])
-                if qd_metadata != qd_default:
-                    qd = qd_metadata
-                else:
-                    qd = pd_estimated
+                qd = -1
+                if "quadrature_degree" in metadata.keys():
+                    qd = metadata["quadrature_degree"]
+
+                # Sending in a negative quadrature degree means that we want to be
+                # able to customize it at a later stage.
+                if qd < 0:
+                    qd = np.max(integral.metadata()["estimated_polynomial_degree"])
 
                 # Extract quadrature rule
-                qr = integral.metadata().get("quadrature_rule", qr_default)
+                qr = integral.metadata().get("quadrature_rule", "default")
 
                 logger.info(f"Integral {i}, integral group {id}:")
                 logger.info(f"--- quadrature rule: {qr}")
                 logger.info(f"--- quadrature degree: {qd}")
 
                 metadata.update({"quadrature_degree": qd, "quadrature_rule": qr})
             else:
-                metadata.update({"quadrature_points": custom_q[0], "quadrature_weights": custom_q[1],
-                                 "quadrature_rule": "custom"})
+                metadata.update(
+                    {
+                        "quadrature_points": custom_q[0],
+                        "quadrature_weights": custom_q[1],
+                        "quadrature_rule": "custom",
+                    }
+                )
 
             integral_data.integrals[i] = integral.reconstruct(metadata=metadata)
 
     return form_data
 
 
-def _has_custom_integrals(o: typing.Union[ufl.integral.Integral, ufl.classes.Form, list, tuple]) -> bool:
+def _has_custom_integrals(
+    o: ufl.integral.Integral | ufl.classes.Form | list | tuple,
+) -> bool:
     """Check for custom integrals."""
     if isinstance(o, ufl.integral.Integral):
         return o.integral_type() in ufl.custom_integral_types
     elif isinstance(o, ufl.classes.Form):
         return any(_has_custom_integrals(itg) for itg in o.integrals())
     elif isinstance(o, (list, tuple)):
         return any(_has_custom_integrals(itg) for itg in o)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/basix_custom_element_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/basix_custom_element_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2018.
+"""Code generation strings for a Basix custom element."""
 
 factory = """
 // Code for custom element {factory_name}
 
 {value_shape_init}
 {wcoeffs_init}
 {npts_init}
@@ -24,15 +25,15 @@
   .npts = {npts},
   .ndofs = {ndofs},
   .x = {x},
   .M = {M},
   .map_type = {map_type},
   .sobolev_space = {sobolev_space},
   .discontinuous = {discontinuous},
-  .highest_complete_degree = {highest_complete_degree},
+  .embedded_subdegree = {embedded_subdegree},
   .interpolation_nderivs = {interpolation_nderivs},
-  .highest_degree = {highest_degree},
+  .embedded_superdegree = {embedded_superdegree},
   .polyset_type = {polyset_type}
 }};
 
 // End of code for custom element {factory_name}
 """
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/c_implementation.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/c_implementation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Copyright (C) 2023 Chris Richardson
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""C implementation."""
 
 import warnings
+
+import numpy as np
+import numpy.typing as npt
+
 import ffcx.codegeneration.lnodes as L
-from ffcx.codegeneration.utils import scalar_to_value_type
+from ffcx.codegeneration.utils import dtype_to_c_type, dtype_to_scalar_dtype
 
 math_table = {
-    "double": {
+    "float64": {
         "sqrt": "sqrt",
         "abs": "fabs",
         "cos": "cos",
         "sin": "sin",
         "tan": "tan",
         "acos": "acos",
         "asin": "asin",
@@ -30,15 +35,15 @@
         "erf": "erf",
         "atan_2": "atan2",
         "min_value": "fmin",
         "max_value": "fmax",
         "bessel_y": "yn",
         "bessel_j": "jn",
     },
-    "float": {
+    "float32": {
         "sqrt": "sqrtf",
         "abs": "fabsf",
         "cos": "cosf",
         "sin": "sinf",
         "tan": "tanf",
         "acos": "acosf",
         "asin": "asinf",
@@ -55,15 +60,15 @@
         "erf": "erff",
         "atan_2": "atan2f",
         "min_value": "fminf",
         "max_value": "fmaxf",
         "bessel_y": "yn",
         "bessel_j": "jn",
     },
-    "long double": {
+    "longdouble": {
         "sqrt": "sqrtl",
         "abs": "fabsl",
         "cos": "cosl",
         "sin": "sinl",
         "tan": "tanl",
         "acos": "acosl",
         "asin": "asinl",
@@ -78,15 +83,15 @@
         "exp": "expl",
         "ln": "logl",
         "erf": "erfl",
         "atan_2": "atan2l",
         "min_value": "fminl",
         "max_value": "fmaxl",
     },
-    "double _Complex": {
+    "complex128": {
         "sqrt": "csqrt",
         "abs": "cabs",
         "cos": "ccos",
         "sin": "csin",
         "tan": "ctan",
         "acos": "cacos",
         "asin": "casin",
@@ -104,15 +109,15 @@
         "imag": "cimag",
         "conj": "conj",
         "max_value": "fmax",
         "min_value": "fmin",
         "bessel_y": "yn",
         "bessel_j": "jn",
     },
-    "float _Complex": {
+    "complex64": {
         "sqrt": "csqrtf",
         "abs": "cabsf",
         "cos": "ccosf",
         "sin": "csinf",
         "tan": "ctanf",
         "acos": "cacosf",
         "asin": "casinf",
@@ -133,137 +138,181 @@
         "min_value": "fminf",
         "bessel_y": "yn",
         "bessel_j": "jn",
     },
 }
 
 
-class CFormatter(object):
-    def __init__(self, scalar) -> None:
-        self.scalar_type = scalar
-        self.real_type = scalar_to_value_type(scalar)
+class CFormatter:
+    """C formatter."""
+
+    scalar_type: np.dtype
+    real_type: np.dtype
 
-    def _dtype_to_name(self, dtype):
+    def __init__(self, dtype: npt.DTypeLike) -> None:
+        """Initialise."""
+        self.scalar_type = np.dtype(dtype)
+        self.real_type = dtype_to_scalar_dtype(dtype)
+
+    def _dtype_to_name(self, dtype) -> str:
+        """Convert dtype to C name."""
         if dtype == L.DataType.SCALAR:
-            return self.scalar_type
+            return dtype_to_c_type(self.scalar_type)
         if dtype == L.DataType.REAL:
-            return self.real_type
+            return dtype_to_c_type(self.real_type)
         if dtype == L.DataType.INT:
             return "int"
+        if dtype == L.DataType.BOOL:
+            return "bool"
         raise ValueError(f"Invalid dtype: {dtype}")
 
     def _format_number(self, x):
+        """Format a number."""
         # Use 16sf for precision (good for float64 or less)
         if isinstance(x, complex):
             return f"({x.real:.16}+I*{x.imag:.16})"
         elif isinstance(x, float):
             return f"{x:.16}"
         return str(x)
 
     def _build_initializer_lists(self, values):
+        """Build initializer lists."""
         arr = "{"
         if len(values.shape) == 1:
             arr += ", ".join(self._format_number(v) for v in values)
         elif len(values.shape) > 1:
             arr += ",\n  ".join(self._build_initializer_lists(v) for v in values)
         arr += "}"
         return arr
 
     def format_statement_list(self, slist) -> str:
+        """Format a statement list."""
         return "".join(self.c_format(s) for s in slist.statements)
 
+    def format_section(self, section) -> str:
+        """Format a section."""
+        # add new line before section
+        comments = "// ------------------------ \n"
+        comments += "// Section: " + section.name + "\n"
+        comments += "// Inputs: " + ", ".join(w.name for w in section.input) + "\n"
+        comments += "// Outputs: " + ", ".join(w.name for w in section.output) + "\n"
+        declarations = "".join(self.c_format(s) for s in section.declarations)
+
+        body = ""
+        if len(section.statements) > 0:
+            declarations += "{\n  "
+            body = "".join(self.c_format(s) for s in section.statements)
+            body = body.replace("\n", "\n  ")
+            body = body[:-2] + "}\n"
+
+        body += "// ------------------------ \n"
+        return comments + declarations + body
+
     def format_comment(self, c) -> str:
+        """Format a comment."""
         return "// " + c.comment + "\n"
 
     def format_array_decl(self, arr) -> str:
+        """Format an array declaration."""
         dtype = arr.symbol.dtype
         typename = self._dtype_to_name(dtype)
 
         symbol = self.c_format(arr.symbol)
         dims = "".join([f"[{i}]" for i in arr.sizes])
         if arr.values is None:
             assert arr.const is False
             return f"{typename} {symbol}{dims};\n"
 
         vals = self._build_initializer_lists(arr.values)
         cstr = "static const " if arr.const else ""
         return f"{cstr}{typename} {symbol}{dims} = {vals};\n"
 
     def format_array_access(self, arr) -> str:
+        """Format an array access."""
         name = self.c_format(arr.array)
         indices = f"[{']['.join(self.c_format(i) for i in arr.indices)}]"
         return f"{name}{indices}"
 
     def format_variable_decl(self, v) -> str:
+        """Format a variable declaration."""
         val = self.c_format(v.value)
         symbol = self.c_format(v.symbol)
         typename = self._dtype_to_name(v.symbol.dtype)
         return f"{typename} {symbol} = {val};\n"
 
     def format_nary_op(self, oper) -> str:
+        """Format an n-ary operation."""
         # Format children
         args = [self.c_format(arg) for arg in oper.args]
 
         # Apply parentheses
         for i in range(len(args)):
             if oper.args[i].precedence >= oper.precedence:
                 args[i] = "(" + args[i] + ")"
 
         # Return combined string
         return f" {oper.op} ".join(args)
 
     def format_binary_op(self, oper) -> str:
+        """Format a binary operation."""
         # Format children
         lhs = self.c_format(oper.lhs)
         rhs = self.c_format(oper.rhs)
 
         # Apply parentheses
         if oper.lhs.precedence >= oper.precedence:
             lhs = f"({lhs})"
         if oper.rhs.precedence >= oper.precedence:
             rhs = f"({rhs})"
 
         # Return combined string
         return f"{lhs} {oper.op} {rhs}"
 
     def format_unary_op(self, oper) -> str:
+        """Format a unary operation."""
         arg = self.c_format(oper.arg)
         if oper.arg.precedence >= oper.precedence:
             return f"{oper.op}({arg})"
         return f"{oper.op}{arg}"
 
     def format_literal_float(self, val) -> str:
+        """Format a literal float."""
         value = self._format_number(val.value)
         return f"{value}"
 
     def format_literal_int(self, val) -> str:
+        """Format a literal int."""
         return f"{val.value}"
 
     def format_for_range(self, r) -> str:
+        """Format a for loop over a range."""
         begin = self.c_format(r.begin)
         end = self.c_format(r.end)
         index = self.c_format(r.index)
         output = f"for (int {index} = {begin}; {index} < {end}; ++{index})\n"
         output += "{\n"
         body = self.c_format(r.body)
         for line in body.split("\n"):
             if len(line) > 0:
                 output += f"  {line}\n"
         output += "}\n"
         return output
 
     def format_statement(self, s) -> str:
+        """Format a statement."""
         return self.c_format(s.expr)
 
     def format_assign(self, expr) -> str:
+        """Format an assignment."""
         rhs = self.c_format(expr.rhs)
         lhs = self.c_format(expr.lhs)
         return f"{lhs} {expr.op} {rhs};\n"
 
     def format_conditional(self, s) -> str:
+        """Format a conditional."""
         # Format children
         c = self.c_format(s.condition)
         t = self.c_format(s.true)
         f = self.c_format(s.false)
 
         # Apply parentheses
         if s.condition.precedence >= s.precedence:
@@ -273,36 +322,40 @@
         if s.false.precedence >= s.precedence:
             f = "(" + f + ")"
 
         # Return combined string
         return c + " ? " + t + " : " + f
 
     def format_symbol(self, s) -> str:
+        """Format a symbol."""
         return f"{s.name}"
 
     def format_multi_index(self, mi) -> str:
+        """Format a multi-index."""
         return self.c_format(mi.global_index)
 
     def format_math_function(self, c) -> str:
+        """Format a mathematical function."""
         # Get a table of functions for this type, if available
         arg_type = self.scalar_type
         if hasattr(c.args[0], "dtype"):
             if c.args[0].dtype == L.DataType.REAL:
                 arg_type = self.real_type
         else:
             warnings.warn(f"Syntax item without dtype {c.args[0]}")
 
-        dtype_math_table = math_table.get(arg_type, {})
+        dtype_math_table = math_table[arg_type.name]
 
         # Get a function from the table, if available, else just use bare name
         func = dtype_math_table.get(c.function, c.function)
         args = ", ".join(self.c_format(arg) for arg in c.args)
         return f"{func}({args})"
 
     c_impl = {
+        "Section": format_section,
         "StatementList": format_statement_list,
         "Comment": format_comment,
         "ArrayDecl": format_array_decl,
         "ArrayAccess": format_array_access,
         "MultiIndex": format_multi_index,
         "VariableDecl": format_variable_decl,
         "ForRange": format_for_range,
@@ -329,12 +382,13 @@
         "GE": format_binary_op,
         "LE": format_binary_op,
         "GT": format_binary_op,
         "LT": format_binary_op,
     }
 
     def c_format(self, s) -> str:
+        """Format as C."""
         name = s.__class__.__name__
         try:
             return self.c_impl[name](self, s)
         except KeyError:
             raise RuntimeError("Unknown statement: ", name)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/dofmap.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/dofmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Note: Most of the code in this file is a direct translation from the
 # old implementation in FFC
+"""Generate UFC code for a DOF map."""
 
 import logging
 
 import ffcx.codegeneration.C.dofmap_template as ufcx_dofmap
 
 logger = logging.getLogger("ffcx")
 
@@ -56,38 +57,38 @@
     d["entity_closure_dofs"] = f"entity_closure_dofs_{ir.name}"
     values = ", ".join(str(i) for i in flattened_entity_closure_dofs)
     sizes = len(flattened_entity_closure_dofs)
     d["entity_closure_dofs_init"] = f"int entity_closure_dofs_{ir.name}[{sizes}] = {{{values}}};"
     d["entity_closure_dof_offsets"] = f"entity_closure_dof_offsets_{ir.name}"
     values = ", ".join(str(i) for i in entity_closure_dof_offsets)
     sizes = len(entity_dof_offsets)
-    d["entity_closure_dof_offsets_init"] = f"int entity_closure_dof_offsets_{ir.name}[{sizes}] = {{{values}}};"
+    d["entity_closure_dof_offsets_init"] = (
+        f"int entity_closure_dof_offsets_{ir.name}[{sizes}] = {{{values}}};"
+    )
 
     d["block_size"] = ir.block_size
 
     if len(ir.sub_dofmaps) > 0:
         values = ", ".join(f"&{dofmap}" for dofmap in ir.sub_dofmaps)
         sizes = len(ir.sub_dofmaps)
-        d["sub_dofmaps_initialization"] = f"ufcx_dofmap* sub_dofmaps_{ir.name}[{sizes}] = {{{values}}};"
+        d["sub_dofmaps_initialization"] = (
+            f"ufcx_dofmap* sub_dofmaps_{ir.name}[{sizes}] = {{{values}}};"
+        )
         d["sub_dofmaps"] = f"sub_dofmaps_{ir.name}"
     else:
         d["sub_dofmaps_initialization"] = ""
         d["sub_dofmaps"] = "NULL"
 
     # Check that no keys are redundant or have been missed
     from string import Formatter
 
-    fields = [
-        fname for _, fname, _, _ in Formatter().parse(ufcx_dofmap.factory) if fname
-    ]
+    fields = [fname for _, fname, _, _ in Formatter().parse(ufcx_dofmap.factory) if fname]
     # Remove square brackets from any field names
     fields = [f.split("[")[0] for f in fields]
-    assert set(fields) == set(
-        d.keys()
-    ), "Mismatch between keys in template and in formatting dict."
+    assert set(fields) == set(d.keys()), "Mismatch between keys in template and in formatting dict."
 
     # Format implementation code
     implementation = ufcx_dofmap.factory.format_map(d)
 
     # Format declaration
     declaration = ufcx_dofmap.declaration.format(factory_name=ir.name)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/dofmap_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/dofmap_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2018.
+"""Code generation strings for a DOF map."""
 
 declaration = """
 extern ufcx_dofmap {factory_name};
 """
 
 factory = """
 // Code for dofmap {factory_name}
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/expressions.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # Copyright (C) 2019 Michal Habera
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Generate UFC code for an expression."""
 
 import logging
 
-from ffcx.codegeneration.C import expressions_template
-from ffcx.codegeneration.expression_generator import ExpressionGenerator
+import numpy as np
+
 from ffcx.codegeneration.backend import FFCXBackend
+from ffcx.codegeneration.C import expressions_template
 from ffcx.codegeneration.C.c_implementation import CFormatter
-from ffcx.codegeneration.utils import cdtype_to_numpy, scalar_to_value_type
+from ffcx.codegeneration.expression_generator import ExpressionGenerator
+from ffcx.codegeneration.utils import dtype_to_c_type, dtype_to_scalar_dtype
 
 logger = logging.getLogger("ffcx")
 
 
 def generator(ir, options):
     """Generate UFC code for an expression."""
     logger.info("Generating code for expression:")
     logger.info(f"--- points: {ir.points}")
     logger.info(f"--- name: {ir.name}")
 
     factory_name = ir.name
 
     # Format declaration
     declaration = expressions_template.declaration.format(
-        factory_name=factory_name, name_from_uflfile=ir.name_from_uflfile)
+        factory_name=factory_name, name_from_uflfile=ir.name_from_uflfile
+    )
 
     backend = FFCXBackend(ir, options)
     eg = ExpressionGenerator(ir, backend)
 
     d = {}
     d["name_from_uflfile"] = ir.name_from_uflfile
     d["factory_name"] = ir.name
@@ -39,16 +43,17 @@
     CF = CFormatter(options["scalar_type"])
     d["tabulate_expression"] = CF.c_format(parts)
 
     if len(ir.original_coefficient_positions) > 0:
         d["original_coefficient_positions"] = f"original_coefficient_positions_{ir.name}"
         values = ", ".join(str(i) for i in ir.original_coefficient_positions)
         sizes = len(ir.original_coefficient_positions)
-        d["original_coefficient_positions_init"] = \
+        d["original_coefficient_positions_init"] = (
             f"static int original_coefficient_positions_{ir.name}[{sizes}] = {{{values}}};"
+        )
     else:
         d["original_coefficient_positions"] = "NULL"
         d["original_coefficient_positions_init"] = ""
 
     values = ", ".join(str(p) for p in ir.points.flatten())
     sizes = ir.points.size
     d["points_init"] = f"static double points_{ir.name}[{sizes}] = {{{values}}};"
@@ -63,67 +68,97 @@
         d["value_shape_init"] = ""
         d["value_shape"] = "NULL"
 
     d["num_components"] = len(ir.expression_shape)
     d["num_coefficients"] = len(ir.coefficient_numbering)
     d["num_constants"] = len(ir.constant_names)
     d["num_points"] = ir.points.shape[0]
-    d["topological_dimension"] = ir.points.shape[1]
-    d["scalar_type"] = options["scalar_type"]
-    d["geom_type"] = scalar_to_value_type(options["scalar_type"])
-    d["np_scalar_type"] = cdtype_to_numpy(options["scalar_type"])
+    d["entity_dimension"] = ir.points.shape[1]
+    d["scalar_type"] = dtype_to_c_type(options["scalar_type"])
+    d["geom_type"] = dtype_to_c_type(dtype_to_scalar_dtype(options["scalar_type"]))
+    d["np_scalar_type"] = np.dtype(options["scalar_type"]).name
 
     d["rank"] = len(ir.tensor_shape)
 
     if len(ir.coefficient_names) > 0:
         values = ", ".join(f'"{name}"' for name in ir.coefficient_names)
         sizes = len(ir.coefficient_names)
-        d["coefficient_names_init"] = f"static const char* coefficient_names_{ir.name}[{sizes}] = {{{values}}};"
+        d["coefficient_names_init"] = (
+            f"static const char* coefficient_names_{ir.name}[{sizes}] = {{{values}}};"
+        )
         d["coefficient_names"] = f"coefficient_names_{ir.name}"
     else:
         d["coefficient_names_init"] = ""
         d["coefficient_names"] = "NULL"
 
     if len(ir.constant_names) > 0:
         values = ", ".join(f'"{name}"' for name in ir.constant_names)
         sizes = len(ir.constant_names)
-        d["constant_names_init"] = f"static const char* constant_names_{ir.name}[{sizes}] = {{{values}}};"
+        d["constant_names_init"] = (
+            f"static const char* constant_names_{ir.name}[{sizes}] = {{{values}}};"
+        )
         d["constant_names"] = f"constant_names_{ir.name}"
     else:
         d["constant_names_init"] = ""
         d["constant_names"] = "NULL"
 
     code = []
+    vs_code = []
 
     # FIXME: Should be handled differently, revise how
     # ufcx_function_space is generated (also for ufcx_form)
-    for (name, (element, dofmap, cmap_family, cmap_degree)) in ir.function_spaces.items():
+    for name, (
+        element,
+        dofmap,
+        cmap_family,
+        cmap_degree,
+        cmap_celltype,
+        cmap_variant,
+        value_shape,
+    ) in ir.function_spaces.items():
         code += [f"static ufcx_function_space function_space_{name}_{ir.name_from_uflfile} ="]
         code += ["{"]
         code += [f".finite_element = &{element},"]
         code += [f".dofmap = &{dofmap},"]
-        code += [f".geometry_family = \"{cmap_family}\","]
-        code += [f".geometry_degree = {cmap_degree}"]
+        code += [f'.geometry_family = "{cmap_family}",']
+        code += [f".geometry_degree = {cmap_degree},"]
+        code += [f".geometry_basix_cell = {int(cmap_celltype)},"]
+        code += [f".geometry_basix_variant = {int(cmap_variant)},"]
+        code += [f".value_rank = {len(value_shape)},"]
+        if len(value_shape) == 0:
+            code += [".value_shape = NULL"]
+        else:
+            vs_code += [
+                f"int value_shape_{name}_{ir.name_from_uflfile}[{len(value_shape)}] = {{",
+                "  " + ", ".join([f"{i}" for i in value_shape]),
+                "};",
+            ]
+            code += [f".value_shape = value_shape_{name}_{ir.name_from_uflfile}"]
         code += ["};"]
 
-    d["function_spaces_alloc"] = "\n".join(code)
+    d["function_spaces_alloc"] = "\n".join(vs_code) + "\n" + "\n".join(code)
     d["function_spaces"] = ""
 
     if len(ir.function_spaces) > 0:
         d["function_spaces"] = f"function_spaces_{ir.name}"
-        values = ", ".join(f"&function_space_{name}_{ir.name_from_uflfile}"
-                           for (name, _) in ir.function_spaces.items())
+        values = ", ".join(
+            f"&function_space_{name}_{ir.name_from_uflfile}"
+            for (name, _) in ir.function_spaces.items()
+        )
         sizes = len(ir.function_spaces)
-        d["function_spaces_init"] = f"ufcx_function_space* function_spaces_{ir.name}[{sizes}] = {{{values}}};"
+        d["function_spaces_init"] = (
+            f"ufcx_function_space* function_spaces_{ir.name}[{sizes}] = {{{values}}};"
+        )
     else:
         d["function_spaces"] = "NULL"
         d["function_spaces_init"] = ""
 
     # Check that no keys are redundant or have been missed
     from string import Formatter
+
     fields = [fname for _, fname, _, _ in Formatter().parse(expressions_template.factory) if fname]
     assert set(fields) == set(d.keys()), "Mismatch between keys in template and in formatting dict"
 
     # Format implementation code
     implementation = expressions_template.factory.format_map(d)
 
     return declaration, implementation
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/expressions_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/expressions_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2019 Michal Habera
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Code generation strings for an expression."""
 
 declaration = """
 extern ufcx_expression {factory_name};
 
 // Helper used to create expression using name which was given to the
 // expression in the UFL file.
 // This helper is called in user c++ code.
@@ -41,15 +42,15 @@
   .tabulate_tensor_{np_scalar_type} = tabulate_tensor_{factory_name},
   .num_coefficients = {num_coefficients},
   .num_constants = {num_constants},
   .original_coefficient_positions = {original_coefficient_positions},
   .coefficient_names = {coefficient_names},
   .constant_names = {constant_names},
   .num_points = {num_points},
-  .topological_dimension = {topological_dimension},
+  .entity_dimension = {entity_dimension},
   .points = {points},
   .value_shape = {value_shape},
   .num_components = {num_components},
   .rank = {rank},
   .function_spaces = {function_spaces}
 }};
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/file.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Note: Most of the code in this file is a direct translation from the
 # old implementation in FFC
+"""Generate a file."""
 
 import logging
 import pprint
 import textwrap
 
-from ffcx.codegeneration.C import file_template
+import numpy as np
+
 from ffcx import __version__ as FFCX_VERSION
 from ffcx.codegeneration import __version__ as UFC_VERSION
-
+from ffcx.codegeneration.C import file_template
 
 logger = logging.getLogger("ffcx")
 
 
 def generator(options):
     """Generate UFC code for file output."""
     logger.info("Generating code for file")
 
     # Attributes
     d = {"ffcx_version": FFCX_VERSION, "ufcx_version": UFC_VERSION}
     d["options"] = textwrap.indent(pprint.pformat(options), "//  ")
     extra_c_includes = []
-    if "_Complex" in options["scalar_type"]:
+    if np.issubdtype(options["scalar_type"], np.complexfloating):
         extra_c_includes += ["complex.h"]
-    d["extra_c_includes"] = "\n".join(
-        f"#include <{header}>" for header in extra_c_includes
-    )
+    d["extra_c_includes"] = "\n".join(f"#include <{header}>" for header in extra_c_includes)
 
     # Format declaration code
     code_pre = (
         file_template.declaration_pre.format_map(d),
         file_template.implementation_pre.format_map(d),
     )
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/file_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/file_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2018.
+"""Code generation strings for a file."""
 
 declaration_pre = """
 // This code conforms with the UFC specification version {ufcx_version}
 // and was automatically generated by FFCx version {ffcx_version}.
 //
 // This code was generated with the following options:
 //
@@ -38,8 +39,10 @@
 #include <stdlib.h>
 #include <string.h>
 #include <ufcx.h>
 {extra_c_includes}
 
 """
 
+libraries = ["m"]
+
 implementation_post = ""
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/finite_element.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/finite_element.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,50 +3,49 @@
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 # Note: Much of the code in this file is a direct translation
 # from the old implementation in FFC, although some improvements
 # have been made to the generated code.
+"""Generate UFC code for a finite element."""
 
 import logging
 
+import ufl
+
 import ffcx.codegeneration.C.basix_custom_element_template as ufcx_basix_custom_finite_element
 import ffcx.codegeneration.C.finite_element_template as ufcx_finite_element
-import ufl
+import ffcx.codegeneration.C.quadrature_rule_template as ufcx_quadrature_rule
 
 logger = logging.getLogger("ffcx")
 index_type = "int"
 
 
 def generator(ir, options):
     """Generate UFC code for a finite element."""
     logger.info("Generating code for finite element:")
-    logger.info(f"--- family: {ir.family}")
     logger.info(f"--- degree: {ir.degree}")
-    logger.info(f"--- value shape: {ir.value_shape}")
+    logger.info(f"--- value shape: {ir.reference_value_shape}")
     logger.info(f"--- name: {ir.name}")
 
     d = {}
     d["factory_name"] = ir.name
-    d["signature"] = f"\"{ir.signature}\""
-    d["geometric_dimension"] = ir.geometric_dimension
+    d["signature"] = f'"{ir.signature}"'
     d["topological_dimension"] = ir.topological_dimension
     d["cell_shape"] = ir.cell_shape
     d["element_type"] = ir.element_type
     d["space_dimension"] = ir.space_dimension
-    d["value_rank"] = len(ir.value_shape)
-    d["value_size"] = ufl.product(ir.value_shape)
     d["reference_value_rank"] = len(ir.reference_value_shape)
     d["reference_value_size"] = ufl.product(ir.reference_value_shape)
     d["degree"] = ir.degree
-    d["family"] = f"\"{ir.family}\""
     d["num_sub_elements"] = ir.num_sub_elements
     d["block_size"] = ir.block_size
     d["discontinuous"] = "true" if ir.discontinuous else "false"
+    d["symmetric"] = "true" if ir.symmetric else "false"
 
     if ir.lagrange_variant is None:
         d["lagrange_variant"] = -1
     else:
         d["lagrange_variant"] = int(ir.lagrange_variant)
 
     if ir.dpc_variant is None:
@@ -59,74 +58,83 @@
     else:
         d["basix_family"] = int(ir.basix_family)
     if ir.basix_cell is None:
         d["basix_cell"] = -1
     else:
         d["basix_cell"] = int(ir.basix_cell)
 
-    if len(ir.value_shape) > 0:
-        d["value_shape"] = f"value_shape_{ir.name}"
-        values = ", ".join(str(i) for i in ir.value_shape)
-        sizes = len(ir.value_shape)
-        d["value_shape_init"] = f"int value_shape_{ir.name}[{sizes}] = {{{values}}};"
-    else:
-        d["value_shape"] = "NULL"
-        d["value_shape_init"] = ""
-
     if len(ir.reference_value_shape) > 0:
         d["reference_value_shape"] = f"reference_value_shape_{ir.name}"
         values = ", ".join(str(i) for i in ir.reference_value_shape)
         sizes = len(ir.reference_value_shape)
-        d["reference_value_shape_init"] = f"int reference_value_shape_{ir.name}[{sizes}] = {{{values}}};"
+        d["reference_value_shape_init"] = (
+            f"int reference_value_shape_{ir.name}[{sizes}] = {{{values}}};"
+        )
     else:
         d["reference_value_shape"] = "NULL"
         d["reference_value_shape_init"] = ""
 
     if len(ir.sub_elements) > 0:
         d["sub_elements"] = f"sub_elements_{ir.name}"
         values = ", ".join(f"&{el}" for el in ir.sub_elements)
         sizes = len(ir.sub_elements)
-        d["sub_elements_init"] = f"ufcx_finite_element* sub_elements_{ir.name}[{sizes}] = {{{values}}};"
+        d["sub_elements_init"] = (
+            f"ufcx_finite_element* sub_elements_{ir.name}[{sizes}] = {{{values}}};"
+        )
     else:
         d["sub_elements"] = "NULL"
         d["sub_elements_init"] = ""
 
     if ir.custom_element is not None:
         d["custom_element"] = f"&custom_element_{ir.name}"
-        d["custom_element_init"] = generate_custom_element(f"custom_element_{ir.name}", ir.custom_element)
+        d["custom_element_init"] = generate_custom_element(
+            f"custom_element_{ir.name}", ir.custom_element
+        )
     else:
         d["custom_element"] = "NULL"
         d["custom_element_init"] = ""
 
+    if ir.custom_quadrature is not None:
+        d["custom_quadrature"] = f"&custom_quadrature_{ir.name}"
+        d["custom_quadrature_init"] = generate_custom_quadrature(
+            f"custom_quadrature_{ir.name}", ir.custom_quadrature
+        )
+    else:
+        d["custom_quadrature"] = "NULL"
+        d["custom_quadrature_init"] = ""
+
     # Check that no keys are redundant or have been missed
     from string import Formatter
+
     fieldnames = [
         fname for _, fname, _, _ in Formatter().parse(ufcx_finite_element.factory) if fname
     ]
     assert set(fieldnames) == set(
-        d.keys()), "Mismatch between keys in template and in formatting dict"
+        d.keys()
+    ), "Mismatch between keys in template and in formatting dict"
 
     # Format implementation code
     implementation = ufcx_finite_element.factory.format_map(d)
 
     # Format declaration
     declaration = ufcx_finite_element.declaration.format(factory_name=ir.name)
 
     return declaration, implementation
 
 
 def generate_custom_element(name, ir):
+    """Generate UFC code for a custom element."""
     d = {}
     d["factory_name"] = name
     d["cell_type"] = int(ir.cell_type)
     d["polyset_type"] = int(ir.polyset_type)
     d["map_type"] = int(ir.map_type)
     d["sobolev_space"] = int(ir.sobolev_space)
-    d["highest_complete_degree"] = ir.highest_complete_degree
-    d["highest_degree"] = ir.highest_degree
+    d["embedded_subdegree"] = ir.embedded_subdegree
+    d["embedded_superdegree"] = ir.embedded_superdegree
     d["discontinuous"] = "true" if ir.discontinuous else "false"
     d["interpolation_nderivs"] = ir.interpolation_nderivs
     d["value_shape_length"] = len(ir.value_shape)
     if len(ir.value_shape) > 0:
         d["value_shape"] = f"value_shape_{name}"
         values = ", ".join(str(i) for i in ir.value_shape)
         sizes = len(ir.value_shape)
@@ -171,17 +179,54 @@
     d["ndofs_init"] += "{" + ",".join([f" {i}" for i in ndofs]) + "};"
     d["M"] = f"M_{name}"
     d["M_init"] = f"double M_{name}[{len(M)}] = "
     d["M_init"] += "{" + ",".join([f" {i}" for i in M]) + "};"
 
     # Check that no keys are redundant or have been missed
     from string import Formatter
+
     fieldnames = [
-        fname for _, fname, _, _ in Formatter().parse(ufcx_basix_custom_finite_element.factory) if fname
+        fname
+        for _, fname, _, _ in Formatter().parse(ufcx_basix_custom_finite_element.factory)
+        if fname
     ]
     assert set(fieldnames) == set(
-        d.keys()), "Mismatch between keys in template and in formatting dict"
+        d.keys()
+    ), "Mismatch between keys in template and in formatting dict"
 
     # Format implementation code
     implementation = ufcx_basix_custom_finite_element.factory.format_map(d)
 
     return implementation
+
+
+def generate_custom_quadrature(name, ir):
+    """Generate UFC code for a custom quadrature rule."""
+    npts = ir.points.shape[0]
+    tdim = ir.points.shape[1]
+
+    d = {}
+    d["factory_name"] = name
+    d["cell_shape"] = ir.cell_shape
+    d["topological_dimension"] = tdim
+    d["npts"] = npts
+    d["points"] = f"points_{name}"
+    d["points_init"] = f"double points_{name}[{npts * tdim}] = "
+    d["points_init"] += "{" + ",".join([f" {i}" for p in ir.points for i in p]) + "};"
+    d["weights"] = f"weights_{name}"
+    d["weights_init"] = f"double weights_{name}[{npts}] = "
+    d["weights_init"] += "{" + ",".join([f" {i}" for i in ir.weights]) + "};"
+
+    # Check that no keys are redundant or have been missed
+    from string import Formatter
+
+    fieldnames = [
+        fname for _, fname, _, _ in Formatter().parse(ufcx_quadrature_rule.factory) if fname
+    ]
+    assert set(fieldnames) == set(
+        d.keys()
+    ), "Mismatch between keys in template and in formatting dict"
+
+    # Format implementation code
+    implementation = ufcx_quadrature_rule.factory.format_map(d)
+
+    return implementation
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/finite_element_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/finite_element_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2018.
+"""Code generation strings for a finite element."""
 
 declaration = """
 extern ufcx_finite_element {factory_name};
 """
 
 factory = """
 // Code for element {factory_name}
 
-{value_shape_init}
 {reference_value_shape_init}
 {sub_elements_init}
 {custom_element_init}
+{custom_quadrature_init}
 
 ufcx_finite_element {factory_name} =
 {{
   .signature = {signature},
   .cell_shape = {cell_shape},
   .element_type = {element_type},
   .topological_dimension = {topological_dimension},
-  .geometric_dimension = {geometric_dimension},
   .space_dimension = {space_dimension},
-  .value_rank = {value_rank},
-  .value_shape = {value_shape},
-  .value_size = {value_size},
   .reference_value_rank = {reference_value_rank},
   .reference_value_shape = {reference_value_shape},
   .reference_value_size = {reference_value_size},
   .degree = {degree},
+  .symmetric = {symmetric},
   .block_size = {block_size},
-  .family = {family},
   .basix_family = {basix_family},
   .basix_cell = {basix_cell},
   .discontinuous = {discontinuous},
   .lagrange_variant = {lagrange_variant},
   .dpc_variant = {dpc_variant},
   .num_sub_elements = {num_sub_elements},
   .sub_elements = {sub_elements},
-  .custom_element = {custom_element}
+  .custom_element = {custom_element},
+  .custom_quadrature = {custom_quadrature}
 }};
 
 // End of code for element {factory_name}
 """
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/form.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 #
 # Modified by Chris Richardson and Jørgen S. Dokken 2023
 #
 # Note: Most of the code in this file is a direct translation from the
 # old implementation in FFC
+"""Generate UFC code for a form."""
 
 import logging
 
-import numpy
+import numpy as np
 
 from ffcx.codegeneration.C import form_template
 
 logger = logging.getLogger("ffcx")
 
 
 def generator(ir, options):
@@ -32,45 +33,51 @@
     d["num_coefficients"] = ir.num_coefficients
     d["num_constants"] = ir.num_constants
 
     if len(ir.original_coefficient_position) > 0:
         values = ", ".join(str(i) for i in ir.original_coefficient_position)
         sizes = len(ir.original_coefficient_position)
 
-        d["original_coefficient_position_init"] = \
+        d["original_coefficient_position_init"] = (
             f"int original_coefficient_position_{ir.name}[{sizes}] = {{{values}}};"
+        )
         d["original_coefficient_position"] = f"original_coefficient_position_{ir.name}"
     else:
         d["original_coefficient_position_init"] = ""
         d["original_coefficient_position"] = "NULL"
 
-    cnames = ir.coefficient_names
-    assert ir.num_coefficients == len(cnames)
-    if len(cnames) == 0:
-        code = ["return NULL;"]
-    else:
-        values = ", ".join(f'"{name}"' for name in cnames)
-        code = [f"static const char* names[{len(cnames)}] = {{{values}}};",
-                "return names;"]
-    d["coefficient_name_map"] = "\n".join(code)
-
-    cstnames = ir.constant_names
-    if len(cstnames) == 0:
-        code = ["return NULL;"]
-    else:
-        values = ", ".join(f'"{name}"' for name in cstnames)
-        code = [f"static const char* names[{len(cstnames)}] = {{{values}}};",
-                "return names;"]
-    d["constant_name_map"] = "\n".join(code)
+    if len(ir.coefficient_names) > 0:
+        values = ", ".join(f'"{name}"' for name in ir.coefficient_names)
+        sizes = len(ir.coefficient_names)
+        d["coefficient_names_init"] = (
+            f"static const char* coefficient_names_{ir.name}[{sizes}] = {{{values}}};"
+        )
+        d["coefficient_names"] = f"coefficient_names_{ir.name}"
+    else:
+        d["coefficient_names_init"] = ""
+        d["coefficient_names"] = "NULL"
+
+    if len(ir.constant_names) > 0:
+        values = ", ".join(f'"{name}"' for name in ir.constant_names)
+        sizes = len(ir.constant_names)
+        d["constant_names_init"] = (
+            f"static const char* constant_names_{ir.name}[{sizes}] = {{{values}}};"
+        )
+        d["constant_names"] = f"constant_names_{ir.name}"
+    else:
+        d["constant_names_init"] = ""
+        d["constant_names"] = "NULL"
 
     if len(ir.finite_elements) > 0:
         d["finite_elements"] = f"finite_elements_{ir.name}"
         values = ", ".join(f"&{el}" for el in ir.finite_elements)
         sizes = len(ir.finite_elements)
-        d["finite_elements_init"] = f"ufcx_finite_element* finite_elements_{ir.name}[{sizes}] = {{{values}}};"
+        d["finite_elements_init"] = (
+            f"ufcx_finite_element* finite_elements_{ir.name}[{sizes}] = {{{values}}};"
+        )
     else:
         d["finite_elements"] = "NULL"
         d["finite_elements_init"] = ""
 
     if len(ir.dofmaps) > 0:
         d["dofmaps"] = f"dofmaps_{ir.name}"
         values = ", ".join(f"&{dofmap}" for dofmap in ir.dofmaps)
@@ -87,77 +94,90 @@
     for itg_type in ("cell", "exterior_facet", "interior_facet"):
         unsorted_integrals = []
         unsorted_ids = []
         for name, id in zip(ir.integral_names[itg_type], ir.subdomain_ids[itg_type]):
             unsorted_integrals += [f"&{name}"]
             unsorted_ids += [id]
 
-        id_sort = numpy.argsort(unsorted_ids)
+        id_sort = np.argsort(unsorted_ids)
         integrals += [unsorted_integrals[i] for i in id_sort]
         integral_ids += [unsorted_ids[i] for i in id_sort]
 
         integral_offsets.append(len(integrals))
 
     if len(integrals) > 0:
         sizes = len(integrals)
         values = ", ".join(integrals)
-        d["form_integrals_init"] = f"static ufcx_integral* form_integrals_{ir.name}[{sizes}] = {{{values}}};"
+        d["form_integrals_init"] = (
+            f"static ufcx_integral* form_integrals_{ir.name}[{sizes}] = {{{values}}};"
+        )
         d["form_integrals"] = f"form_integrals_{ir.name}"
         sizes = len(integral_ids)
         values = ", ".join(str(i) for i in integral_ids)
         d["form_integral_ids_init"] = f"int form_integral_ids_{ir.name}[{sizes}] = {{{values}}};"
         d["form_integral_ids"] = f"form_integral_ids_{ir.name}"
     else:
         d["form_integrals_init"] = ""
         d["form_integrals"] = "NULL"
         d["form_integral_ids_init"] = ""
         d["form_integral_ids"] = "NULL"
 
     sizes = len(integral_offsets)
     values = ", ".join(str(i) for i in integral_offsets)
-    d["form_integral_offsets_init"] = f"int form_integral_offsets_{ir.name}[{sizes}] = {{{values}}};"
+    d["form_integral_offsets_init"] = (
+        f"int form_integral_offsets_{ir.name}[{sizes}] = {{{values}}};"
+    )
 
+    vs_code = []
     code = []
 
     # FIXME: Should be handled differently, revise how
     # ufcx_function_space is generated
     for name, (
         element,
         dofmap,
         cmap_family,
         cmap_degree,
         cmap_celltype,
         cmap_variant,
+        value_shape,
     ) in ir.function_spaces.items():
         code += [f"static ufcx_function_space functionspace_{name} ="]
         code += ["{"]
         code += [f".finite_element = &{element},"]
         code += [f".dofmap = &{dofmap},"]
         code += [f'.geometry_family = "{cmap_family}",']
         code += [f".geometry_degree = {cmap_degree},"]
         code += [f".geometry_basix_cell = {int(cmap_celltype)},"]
-        code += [f".geometry_basix_variant = {int(cmap_variant)}"]
+        code += [f".geometry_basix_variant = {int(cmap_variant)},"]
+        code += [f".value_rank = {len(value_shape)},"]
+        if len(value_shape) == 0:
+            code += [".value_shape = NULL"]
+        else:
+            vs_code += [
+                f"int value_shape_{ir.name}_{name}[{len(value_shape)}] = {{",
+                "  " + ", ".join([f"{i}" for i in value_shape]),
+                "};",
+            ]
+            code += [f".value_shape = value_shape_{ir.name}_{name}"]
         code += ["};"]
 
     for name in ir.function_spaces.keys():
         code += [f'if (strcmp(function_name, "{name}") == 0) return &functionspace_{name};']
 
     code += ["return NULL;\n"]
 
     d["functionspace"] = "\n".join(code)
+    d["value_shape_init"] = "\n".join(vs_code)
 
     # Check that no keys are redundant or have been missed
     from string import Formatter
 
-    fields = [
-        fname for _, fname, _, _ in Formatter().parse(form_template.factory) if fname
-    ]
-    assert set(fields) == set(
-        d.keys()
-    ), "Mismatch between keys in template and in formatting dict"
+    fields = [fname for _, fname, _, _ in Formatter().parse(form_template.factory) if fname]
+    assert set(fields) == set(d.keys()), "Mismatch between keys in template and in formatting dict"
 
     # Format implementation code
     implementation = form_template.factory.format_map(d)
 
     # Format declaration
     declaration = form_template.declaration.format(
         factory_name=d["factory_name"], name_from_uflfile=d["name_from_uflfile"]
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/form_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/form_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2020.
+"""Code generation strings for a form."""
 
 declaration = """
 extern ufcx_form {factory_name};
 
 // Helper used to create form using name which was given to the
 // form in the UFL file.
 // This helper is called in user c++ code.
@@ -24,49 +25,41 @@
 {original_coefficient_position_init}
 {dofmaps_init}
 {finite_elements_init}
 {form_integral_offsets_init}
 {form_integrals_init}
 {form_integral_ids_init}
 
-// Return a list of the coefficient names.
-const char** coefficient_name_{factory_name}(void)
-{{
-{coefficient_name_map}
-}}
-
-// Return a list of the constant names.
-const char** constant_name_{factory_name}(void)
-{{
-{constant_name_map}
-}}
+{coefficient_names_init}
+{constant_names_init}
 
 ufcx_form {factory_name} =
 {{
 
   .signature = {signature},
   .rank = {rank},
   .num_coefficients = {num_coefficients},
   .num_constants = {num_constants},
   .original_coefficient_position = {original_coefficient_position},
 
-  .coefficient_name_map = coefficient_name_{factory_name},
-  .constant_name_map = constant_name_{factory_name},
+  .coefficient_name_map = {coefficient_names},
+  .constant_name_map = {constant_names},
 
   .finite_elements = {finite_elements},
   .dofmaps = {dofmaps},
 
   .form_integrals = {form_integrals},
   .form_integral_ids = {form_integral_ids},
   .form_integral_offsets = form_integral_offsets_{factory_name}
 }};
 
 // Alias name
 ufcx_form* {name_from_uflfile} = &{factory_name};
 
+{value_shape_init}
 ufcx_function_space* functionspace_{name_from_uflfile}(const char* function_name)
 {{
 {functionspace}
 }}
 
 // End of code for form {factory_name}
 """
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/integrals.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/integrals.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # Copyright (C) 2015-2021 Martin Sandve Alnæs, Michal Habera, Igor Baratta
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Generate UFC code for an integral."""
 
 import logging
 
-from ffcx.codegeneration.integral_generator import IntegralGenerator
-from ffcx.codegeneration.C import integrals_template as ufcx_integrals
+import numpy as np
+
 from ffcx.codegeneration.backend import FFCXBackend
+from ffcx.codegeneration.C import integrals_template as ufcx_integrals
 from ffcx.codegeneration.C.c_implementation import CFormatter
-from ffcx.codegeneration.utils import cdtype_to_numpy, scalar_to_value_type
+from ffcx.codegeneration.integral_generator import IntegralGenerator
+from ffcx.codegeneration.utils import dtype_to_c_type, dtype_to_scalar_dtype
+from ffcx.ir.representation import IntegralIR
 
 logger = logging.getLogger("ffcx")
 
 
-def generator(ir, options):
+def generator(ir: IntegralIR, options):
+    """Generate C code for an integral."""
     logger.info("Generating code for integral:")
     logger.info(f"--- type: {ir.integral_type}")
     logger.info(f"--- name: {ir.name}")
 
     """Generate code for an integral."""
     factory_name = ir.name
 
@@ -41,28 +46,40 @@
 
     # Generate generic FFCx code snippets and add specific parts
     code = {}
 
     if len(ir.enabled_coefficients) > 0:
         values = ", ".join("1" if i else "0" for i in ir.enabled_coefficients)
         sizes = len(ir.enabled_coefficients)
-        code["enabled_coefficients_init"] = f"bool enabled_coefficients_{ir.name}[{sizes}] = {{{values}}};"
+        code["enabled_coefficients_init"] = (
+            f"bool enabled_coefficients_{ir.name}[{sizes}] = {{{values}}};"
+        )
         code["enabled_coefficients"] = f"enabled_coefficients_{ir.name}"
     else:
         code["enabled_coefficients_init"] = ""
         code["enabled_coefficients"] = "NULL"
 
-    code["additional_includes_set"] = set()  # FIXME: Get this out of code[]
     code["tabulate_tensor"] = body
 
+    code["tabulate_tensor_float32"] = "NULL"
+    code["tabulate_tensor_float64"] = "NULL"
+    code["tabulate_tensor_complex64"] = "NULL"
+    code["tabulate_tensor_complex128"] = "NULL"
+    np_scalar_type = np.dtype(options["scalar_type"]).name
+    code[f"tabulate_tensor_{np_scalar_type}"] = f"tabulate_tensor_{factory_name}"
+
     implementation = ufcx_integrals.factory.format(
         factory_name=factory_name,
         enabled_coefficients=code["enabled_coefficients"],
         enabled_coefficients_init=code["enabled_coefficients_init"],
         tabulate_tensor=code["tabulate_tensor"],
         needs_facet_permutations="true" if ir.needs_facet_permutations else "false",
-        scalar_type=options["scalar_type"],
-        geom_type=scalar_to_value_type(options["scalar_type"]),
-        np_scalar_type=cdtype_to_numpy(options["scalar_type"]),
-        coordinate_element=f"&{ir.coordinate_element}")
+        scalar_type=dtype_to_c_type(options["scalar_type"]),
+        geom_type=dtype_to_c_type(dtype_to_scalar_dtype(options["scalar_type"])),
+        coordinate_element=f"&{ir.coordinate_element}",
+        tabulate_tensor_float32=code["tabulate_tensor_float32"],
+        tabulate_tensor_float64=code["tabulate_tensor_float64"],
+        tabulate_tensor_complex64=code["tabulate_tensor_complex64"],
+        tabulate_tensor_complex128=code["tabulate_tensor_complex128"],
+    )
 
     return declaration, implementation
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/C/integrals_template.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/C/integrals_template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Code generation format strings for UFC (Unified Form-assembly Code)
 # This code is released into the public domain.
 #
 # The FEniCS Project (http://www.fenicsproject.org/) 2018
+"""Code generation strings for an integral."""
 
 declaration = """
 extern ufcx_integral {factory_name};
 """
 
 factory = """
 // Code for integral {factory_name}
@@ -21,14 +22,17 @@
 }}
 
 {enabled_coefficients_init}
 
 ufcx_integral {factory_name} =
 {{
   .enabled_coefficients = {enabled_coefficients},
-  .tabulate_tensor_{np_scalar_type} = tabulate_tensor_{factory_name},
+  .tabulate_tensor_float32 = {tabulate_tensor_float32},
+  .tabulate_tensor_float64 = {tabulate_tensor_float64},
+  .tabulate_tensor_complex64 = {tabulate_tensor_complex64},
+  .tabulate_tensor_complex128 = {tabulate_tensor_complex128},
   .needs_facet_permutations = {needs_facet_permutations},
   .coordinate_element = {coordinate_element},
 }};
 
 // End of code for integral {factory_name}
 """
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/__init__.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+"""FFCx code generation."""
+
 import hashlib
 import os
 
 # Version of FFCx header files
 __author__ = "FEniCS Project"
 __license__ = "This code is released into the public domain"
 __version__ = "2018.2.0.dev0"
 
 # Get abspath on import, it can in some cases be a relative path w.r.t.
 # curdir on startup
 _include_path = os.path.dirname(os.path.abspath(__file__))
 
 
 def get_include_path():
-    """Return location of UFC header files."""
+    """Return location of UFCx header files."""
     return _include_path
 
 
 def _compute_signature():
-    # Compute signature of ufc header files
+    """Compute signature of UFCx header files."""
     h = hashlib.sha1()
     with open(os.path.join(get_include_path(), "ufcx.h")) as f:
         h.update(f.read().encode("utf-8"))
     return h.hexdigest()
 
 
 _signature = _compute_signature()
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/access.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/access.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,71 +3,90 @@
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """FFCx/UFC specific variable access."""
 
 import logging
 import warnings
+from typing import Optional
 
-import ufl
 import basix.ufl
-from ffcx.element_interface import convert_element
+import ufl
+
 import ffcx.codegeneration.lnodes as L
+from ffcx.ir.analysis.modified_terminals import ModifiedTerminal
+from ffcx.ir.elementtables import UniqueTableReferenceT
+from ffcx.ir.representationutils import QuadratureRule
 
 logger = logging.getLogger("ffcx")
 
 
-class FFCXBackendAccess(object):
-    """FFCx specific cpp formatter class."""
+class FFCXBackendAccess:
+    """FFCx specific formatter class."""
 
     def __init__(self, ir, symbols, options):
-
+        """Initialise."""
         # Store ir and options
         self.entitytype = ir.entitytype
         self.integral_type = ir.integral_type
         self.symbols = symbols
         self.options = options
 
         # Lookup table for handler to call when the "get" method (below) is
         # called, depending on the first argument type.
-        self.call_lookup = {ufl.coefficient.Coefficient: self.coefficient,
-                            ufl.constant.Constant: self.constant,
-                            ufl.geometry.Jacobian: self.jacobian,
-                            ufl.geometry.CellCoordinate: self.cell_coordinate,
-                            ufl.geometry.FacetCoordinate: self.facet_coordinate,
-                            ufl.geometry.CellVertices: self.cell_vertices,
-                            ufl.geometry.FacetEdgeVectors: self.facet_edge_vectors,
-                            ufl.geometry.CellEdgeVectors: self.cell_edge_vectors,
-                            ufl.geometry.CellFacetJacobian: self.cell_facet_jacobian,
-                            ufl.geometry.ReferenceCellVolume: self.reference_cell_volume,
-                            ufl.geometry.ReferenceFacetVolume: self.reference_facet_volume,
-                            ufl.geometry.ReferenceCellEdgeVectors: self.reference_cell_edge_vectors,
-                            ufl.geometry.ReferenceFacetEdgeVectors: self.reference_facet_edge_vectors,
-                            ufl.geometry.ReferenceNormal: self.reference_normal,
-                            ufl.geometry.CellOrientation: self._pass,
-                            ufl.geometry.FacetOrientation: self.facet_orientation,
-                            ufl.geometry.SpatialCoordinate: self.spatial_coordinate}
-
-    def get(self, e, mt, tabledata, num_points):
+        self.call_lookup = {
+            ufl.coefficient.Coefficient: self.coefficient,
+            ufl.constant.Constant: self.constant,
+            ufl.geometry.Jacobian: self.jacobian,
+            ufl.geometry.CellCoordinate: self.cell_coordinate,
+            ufl.geometry.FacetCoordinate: self.facet_coordinate,
+            ufl.geometry.CellVertices: self.cell_vertices,
+            ufl.geometry.FacetEdgeVectors: self.facet_edge_vectors,
+            ufl.geometry.CellEdgeVectors: self.cell_edge_vectors,
+            ufl.geometry.CellFacetJacobian: self.cell_facet_jacobian,
+            ufl.geometry.ReferenceCellVolume: self.reference_cell_volume,
+            ufl.geometry.ReferenceFacetVolume: self.reference_facet_volume,
+            ufl.geometry.ReferenceCellEdgeVectors: self.reference_cell_edge_vectors,
+            ufl.geometry.ReferenceFacetEdgeVectors: self.reference_facet_edge_vectors,
+            ufl.geometry.ReferenceNormal: self.reference_normal,
+            ufl.geometry.CellOrientation: self._pass,
+            ufl.geometry.FacetOrientation: self.facet_orientation,
+            ufl.geometry.SpatialCoordinate: self.spatial_coordinate,
+        }
+
+    def get(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+    ):
+        """Format a terminal."""
+        e = mt.terminal
         # Call appropriate handler, depending on the type of e
         handler = self.call_lookup.get(type(e), False)
 
         if not handler:
             # Look for parent class types instead
             for k in self.call_lookup.keys():
                 if isinstance(e, k):
                     handler = self.call_lookup[k]
                     break
 
         if handler:
-            return handler(e, mt, tabledata, num_points)
+            return handler(mt, tabledata, quadrature_rule)
         else:
             raise RuntimeError(f"Not handled: {type(e)}")
 
-    def coefficient(self, e, mt, tabledata, num_points):
+    def coefficient(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+    ):
+        """Access a coefficient."""
         ttype = tabledata.ttype
         assert ttype != "zeros"
 
         num_dofs = tabledata.values.shape[3]
         begin = tabledata.offset
         end = begin + tabledata.block_size * (num_dofs - 1) + 1
 
@@ -76,88 +95,100 @@
             # array at dof begin (if mt is restricted, begin contains
             # cell offset)
             return self.symbols.coefficient_dof_access(mt.terminal, begin)
         else:
             # Return symbol, see definitions for computation
             return self.symbols.coefficient_value(mt)
 
-    def constant(self, e, mt, tabledata, num_points):
-        """Access to a constant is handled trivially, directly through constants symbol."""
+    def constant(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: Optional[UniqueTableReferenceT],
+        quadrature_rule: Optional[QuadratureRule],
+    ):
+        """Access a constant."""
+        # Access to a constant is handled trivially, directly through constants symbol
         return self.symbols.constant_index_access(mt.terminal, mt.flat_component)
 
-    def spatial_coordinate(self, e, mt, tabledata, num_points):
+    def spatial_coordinate(
+        self, mt: ModifiedTerminal, tabledata: UniqueTableReferenceT, num_points: QuadratureRule
+    ):
+        """Access a spatial coordinate."""
         if mt.global_derivatives:
             raise RuntimeError("Not expecting global derivatives of SpatialCoordinate.")
         if mt.averaged is not None:
             raise RuntimeError("Not expecting average of SpatialCoordinates.")
 
         if self.integral_type in ufl.custom_integral_types:
             if mt.local_derivatives:
                 raise RuntimeError("FIXME: Jacobian in custom integrals is not implemented.")
 
             # Access predefined quadrature points table
             x = self.symbols.custom_points_table
             iq = self.symbols.quadrature_loop_index
-            gdim, = mt.terminal.ufl_shape
+            (gdim,) = mt.terminal.ufl_shape
             if gdim == 1:
                 index = iq
             else:
                 index = iq * gdim + mt.flat_component
             return x[index]
         elif self.integral_type == "expression":
             # Physical coordinates are computed by code generated in
             # definitions
             return self.symbols.x_component(mt)
         else:
             # Physical coordinates are computed by code generated in
             # definitions
             return self.symbols.x_component(mt)
 
-    def cell_coordinate(self, e, mt, tabledata, num_points):
+    def cell_coordinate(self, mt, tabledata, num_points):
+        """Access a cell coordinate."""
         if mt.global_derivatives:
             raise RuntimeError("Not expecting derivatives of CellCoordinate.")
         if mt.local_derivatives:
             raise RuntimeError("Not expecting derivatives of CellCoordinate.")
         if mt.averaged is not None:
             raise RuntimeError("Not expecting average of CellCoordinate.")
 
         if self.integral_type == "cell" and not mt.restriction:
             # Access predefined quadrature points table
             X = self.symbols.points_table(num_points)
-            tdim, = mt.terminal.ufl_shape
+            (tdim,) = mt.terminal.ufl_shape
             iq = self.symbols.quadrature_loop_index()
             if num_points == 1:
                 index = mt.flat_component
             elif tdim == 1:
                 index = iq
             else:
                 index = iq * tdim + mt.flat_component
             return X[index]
         else:
             # X should be computed from x or Xf symbolically instead of
             # getting here
             raise RuntimeError("Expecting reference cell coordinate to be symbolically rewritten.")
 
-    def facet_coordinate(self, e, mt, tabledata, num_points):
+    def facet_coordinate(self, mt, tabledata, num_points):
+        """Access a facet coordinate."""
         if mt.global_derivatives:
             raise RuntimeError("Not expecting derivatives of FacetCoordinate.")
         if mt.local_derivatives:
             raise RuntimeError("Not expecting derivatives of FacetCoordinate.")
         if mt.averaged is not None:
             raise RuntimeError("Not expecting average of FacetCoordinate.")
         if mt.restriction:
             raise RuntimeError("Not expecting restriction of FacetCoordinate.")
 
         if self.integral_type in ("interior_facet", "exterior_facet"):
-            tdim, = mt.terminal.ufl_shape
+            (tdim,) = mt.terminal.ufl_shape
             if tdim == 0:
                 raise RuntimeError("Vertices have no facet coordinates.")
             elif tdim == 1:
                 warnings.warn(
-                    "Vertex coordinate is always 0, should get rid of this in ufl geometry lowering."
+                    "Vertex coordinate is always 0, should get rid of this in UFL "
+                    "geometry lowering."
                 )
                 return L.LiteralFloat(0.0)
             Xf = self.points_table(num_points)
             iq = self.symbols.quadrature_loop_index()
             assert 0 <= mt.flat_component < (tdim - 1)
             if num_points == 1:
                 index = mt.flat_component
@@ -167,187 +198,253 @@
                 index = iq * (tdim - 1) + mt.flat_component
             return Xf[index]
         else:
             # Xf should be computed from X or x symbolically instead of
             # getting here
             raise RuntimeError("Expecting reference facet coordinate to be symbolically rewritten.")
 
-    def jacobian(self, e, mt, tabledata, num_points):
+    def jacobian(self, mt, tabledata, num_points):
+        """Access a jacobian."""
         if mt.averaged is not None:
             raise RuntimeError("Not expecting average of Jacobian.")
         return self.symbols.J_component(mt)
 
-    def reference_cell_volume(self, e, mt, tabledata, access):
+    def reference_cell_volume(self, mt, tabledata, access):
+        """Access a reference cell volume."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("interval", "triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             return L.Symbol(f"{cellname}_reference_cell_volume", dtype=L.DataType.REAL)
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def reference_facet_volume(self, e, mt, tabledata, access):
+    def reference_facet_volume(self, mt, tabledata, access):
+        """Access a reference facet volume."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("interval", "triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             return L.Symbol(f"{cellname}_reference_facet_volume", dtype=L.DataType.REAL)
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def reference_normal(self, e, mt, tabledata, access):
+    def reference_normal(self, mt, tabledata, access):
+        """Access a reference normal."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("interval", "triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             table = L.Symbol(f"{cellname}_reference_facet_normals", dtype=L.DataType.REAL)
             facet = self.symbols.entity("facet", mt.restriction)
             return table[facet][mt.component[0]]
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def cell_facet_jacobian(self, e, mt, tabledata, num_points):
+    def cell_facet_jacobian(self, mt, tabledata, num_points):
+        """Access a cell facet jacobian."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             table = L.Symbol(f"{cellname}_reference_facet_jacobian", dtype=L.DataType.REAL)
             facet = self.symbols.entity("facet", mt.restriction)
             return table[facet][mt.component[0]][mt.component[1]]
         elif cellname == "interval":
             raise RuntimeError("The reference facet jacobian doesn't make sense for interval cell.")
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def reference_cell_edge_vectors(self, e, mt, tabledata, num_points):
+    def reference_cell_edge_vectors(self, mt, tabledata, num_points):
+        """Access a reference cell edge vector."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             table = L.Symbol(f"{cellname}_reference_edge_vectors", dtype=L.DataType.REAL)
             return table[mt.component[0]][mt.component[1]]
         elif cellname == "interval":
-            raise RuntimeError("The reference cell edge vectors doesn't make sense for interval cell.")
+            raise RuntimeError(
+                "The reference cell edge vectors doesn't make sense for interval cell."
+            )
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def reference_facet_edge_vectors(self, e, mt, tabledata, num_points):
+    def reference_facet_edge_vectors(self, mt, tabledata, num_points):
+        """Access a reference facet edge vector."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname in ("tetrahedron", "hexahedron"):
             table = L.Symbol(f"{cellname}_reference_edge_vectors", dtype=L.DataType.REAL)
             facet = self.symbols.entity("facet", mt.restriction)
             return table[facet][mt.component[0]][mt.component[1]]
         elif cellname in ("interval", "triangle", "quadrilateral"):
             raise RuntimeError(
-                "The reference cell facet edge vectors doesn't make sense for interval or triangle cell."
+                "The reference cell facet edge vectors doesn't make sense for interval "
+                "or triangle cell."
             )
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
-    def facet_orientation(self, e, mt, tabledata, num_points):
+    def facet_orientation(self, mt, tabledata, num_points):
+        """Access a facet orientation."""
         cellname = ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
         if cellname not in ("interval", "triangle", "tetrahedron"):
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
         table = L.Symbol(f"{cellname}_facet_orientations", dtype=L.DataType.INT)
         facet = self.symbols.entity("facet", mt.restriction)
         return table[facet]
 
-    def cell_vertices(self, e, mt, tabledata, num_points):
+    def cell_vertices(self, mt, tabledata, num_points):
+        """Access a cell vertex."""
         # Get properties of domain
         domain = ufl.domain.extract_unique_domain(mt.terminal)
         gdim = domain.geometric_dimension()
-        coordinate_element = convert_element(domain.ufl_coordinate_element())
+        coordinate_element = domain.ufl_coordinate_element()
 
         # Get dimension and dofmap of scalar element
         assert isinstance(coordinate_element, basix.ufl._BlockedElement)
-        assert coordinate_element.value_shape() == (gdim, )
-        ufl_scalar_element, = set(coordinate_element.sub_elements())
-        scalar_element = convert_element(ufl_scalar_element)
-        assert scalar_element.value_size == 1 and scalar_element.block_size == 1
+        assert coordinate_element.reference_value_shape == (gdim,)
+        (ufl_scalar_element,) = set(coordinate_element.sub_elements)
+        scalar_element = ufl_scalar_element
+        assert scalar_element.reference_value_size == 1 and scalar_element.block_size == 1
 
         vertex_scalar_dofs = scalar_element.entity_dofs[0]
         num_scalar_dofs = scalar_element.dim
 
         # Get dof and component
-        dof, = vertex_scalar_dofs[mt.component[0]]
+        (dof,) = vertex_scalar_dofs[mt.component[0]]
         component = mt.component[1]
 
         expr = self.symbols.domain_dof_access(dof, component, gdim, num_scalar_dofs, mt.restriction)
         return expr
 
-    def cell_edge_vectors(self, e, mt, tabledata, num_points):
+    def cell_edge_vectors(self, mt, tabledata, num_points):
+        """Access a cell edge vector."""
         # Get properties of domain
         domain = ufl.domain.extract_unique_domain(mt.terminal)
         cellname = domain.ufl_cell().cellname()
         gdim = domain.geometric_dimension()
-        coordinate_element = convert_element(domain.ufl_coordinate_element())
+        coordinate_element = domain.ufl_coordinate_element()
 
         if cellname in ("triangle", "tetrahedron", "quadrilateral", "hexahedron"):
             pass
         elif cellname == "interval":
-            raise RuntimeError("The physical cell edge vectors doesn't make sense for interval cell.")
+            raise RuntimeError(
+                "The physical cell edge vectors doesn't make sense for interval cell."
+            )
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
         # Get dimension and dofmap of scalar element
         assert isinstance(coordinate_element, basix.ufl._BlockedElement)
-        assert coordinate_element.value_shape() == (gdim, )
-        ufl_scalar_element, = set(coordinate_element.sub_elements())
-        scalar_element = convert_element(ufl_scalar_element)
-        assert scalar_element.value_size == 1 and scalar_element.block_size == 1
+        assert coordinate_element.reference_value_shape == (gdim,)
+        (ufl_scalar_element,) = set(coordinate_element.sub_elements)
+        scalar_element = ufl_scalar_element
+        assert scalar_element.reference_value_size == 1 and scalar_element.block_size == 1
 
         vertex_scalar_dofs = scalar_element.entity_dofs[0]
         num_scalar_dofs = scalar_element.dim
 
         # Get edge vertices
         edge = mt.component[0]
         vertex0, vertex1 = scalar_element.reference_topology[1][edge]
 
         # Get dofs and component
-        dof0, = vertex_scalar_dofs[vertex0]
-        dof1, = vertex_scalar_dofs[vertex1]
+        (dof0,) = vertex_scalar_dofs[vertex0]
+        (dof1,) = vertex_scalar_dofs[vertex1]
         component = mt.component[1]
 
         return self.symbols.domain_dof_access(
             dof0, component, gdim, num_scalar_dofs, mt.restriction
-        ) - self.symbols.domain_dof_access(
-            dof1, component, gdim, num_scalar_dofs, mt.restriction
-        )
-
-    def facet_edge_vectors(self, e, mt, tabledata, num_points):
+        ) - self.symbols.domain_dof_access(dof1, component, gdim, num_scalar_dofs, mt.restriction)
 
+    def facet_edge_vectors(self, mt, tabledata, num_points):
+        """Access a facet edge vector."""
         # Get properties of domain
         domain = ufl.domain.extract_unique_domain(mt.terminal)
         cellname = domain.ufl_cell().cellname()
         gdim = domain.geometric_dimension()
-        coordinate_element = convert_element(domain.ufl_coordinate_element())
+        coordinate_element = domain.ufl_coordinate_element()
 
         if cellname in ("tetrahedron", "hexahedron"):
             pass
         elif cellname in ("interval", "triangle", "quadrilateral"):
             raise RuntimeError(
-                f"The physical facet edge vectors doesn't make sense for {cellname} cell.")
+                f"The physical facet edge vectors doesn't make sense for {cellname} cell."
+            )
         else:
             raise RuntimeError(f"Unhandled cell types {cellname}.")
 
         # Get dimension and dofmap of scalar element
         assert isinstance(coordinate_element, basix.ufl._BlockedElement)
-        assert coordinate_element.value_shape() == (gdim, )
-        ufl_scalar_element, = set(coordinate_element.sub_elements())
-        scalar_element = convert_element(ufl_scalar_element)
-        assert scalar_element.value_size == 1 and scalar_element.block_size == 1
+        assert coordinate_element.reference_value_shape == (gdim,)
+        (ufl_scalar_element,) = set(coordinate_element.sub_elements)
+        scalar_element = ufl_scalar_element
+        assert scalar_element.reference_value_size == 1 and scalar_element.block_size == 1
 
-        scalar_element = convert_element(ufl_scalar_element)
+        scalar_element = ufl_scalar_element
         num_scalar_dofs = scalar_element.dim
 
         # Get edge vertices
         facet = self.symbols.entity("facet", mt.restriction)
         facet_edge = mt.component[0]
         facet_edge_vertices = L.Symbol(f"{cellname}_facet_edge_vertices", dtype=L.DataType.INT)
         vertex0 = facet_edge_vertices[facet][facet_edge][0]
         vertex1 = facet_edge_vertices[facet][facet_edge][1]
 
         # Get dofs and component
         component = mt.component[1]
-        assert coordinate_element.degree() == 1, "Assuming degree 1 element"
+        assert coordinate_element.embedded_superdegree == 1, "Assuming degree 1 element"
         dof0 = vertex0
         dof1 = vertex1
-        expr = (
-            self.symbols.domain_dof_access(dof0, component, gdim, num_scalar_dofs, mt.restriction)
-            - self.symbols.domain_dof_access(dof1, component, gdim, num_scalar_dofs, mt.restriction))
+        expr = self.symbols.domain_dof_access(
+            dof0, component, gdim, num_scalar_dofs, mt.restriction
+        ) - self.symbols.domain_dof_access(dof1, component, gdim, num_scalar_dofs, mt.restriction)
 
         return expr
 
     def _pass(self, *args, **kwargs):
         """Return one."""
         return 1
+
+    def table_access(
+        self,
+        tabledata: UniqueTableReferenceT,
+        entitytype: str,
+        restriction: str,
+        quadrature_index: L.MultiIndex,
+        dof_index: L.MultiIndex,
+    ):
+        """Access element table for given entity, quadrature point, and dof index.
+
+        Args:
+            tabledata: Table data object
+            entitytype: Entity type ("cell", "facet", "vertex")
+            restriction: Restriction ("+", "-")
+            quadrature_index: Quadrature index
+            dof_index: Dof index
+        """
+        entity = self.symbols.entity(entitytype, restriction)
+        iq_global_index = quadrature_index.global_index
+        ic_global_index = dof_index.global_index
+        qp = 0  # quadrature permutation
+
+        symbols = []
+        if tabledata.is_uniform:
+            entity = L.LiteralInt(0)
+
+        if tabledata.is_piecewise:
+            iq_global_index = L.LiteralInt(0)
+
+        # FIXME: Hopefully tabledata is not permuted when applying sum
+        # factorization
+        if tabledata.is_permuted:
+            qp = self.symbols.quadrature_permutation[0]
+            if restriction == "-":
+                qp = self.symbols.quadrature_permutation[1]
+
+        if dof_index.dim == 1 and quadrature_index.dim == 1:
+            symbols += [L.Symbol(tabledata.name, dtype=L.DataType.REAL)]
+            return self.symbols.element_tables[tabledata.name][qp][entity][iq_global_index][
+                ic_global_index
+            ], symbols
+        else:
+            FE = []
+            for i in range(dof_index.dim):
+                factor = tabledata.tensor_factors[i]
+                iq_i = quadrature_index.local_index(i)
+                ic_i = dof_index.local_index(i)
+                table = self.symbols.element_tables[factor.name][qp][entity][iq_i][ic_i]
+                symbols += [L.Symbol(factor.name, dtype=L.DataType.REAL)]
+                FE.append(table)
+            return L.Product(FE), symbols
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/backend.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 """Collection of FFCx specific pieces for the code generation phase."""
 
 from ffcx.codegeneration.access import FFCXBackendAccess
 from ffcx.codegeneration.definitions import FFCXBackendDefinitions
 from ffcx.codegeneration.symbols import FFCXBackendSymbols
 
 
-class FFCXBackend(object):
+class FFCXBackend:
     """Class collecting all aspects of the FFCx backend."""
 
     def __init__(self, ir, options):
-
+        """Initialise."""
         coefficient_numbering = ir.coefficient_numbering
         coefficient_offsets = ir.coefficient_offsets
 
         original_constant_offsets = ir.original_constant_offsets
 
-        self.symbols = FFCXBackendSymbols(coefficient_numbering,
-                                          coefficient_offsets, original_constant_offsets)
-        self.definitions = FFCXBackendDefinitions(ir, self.symbols, options)
+        self.symbols = FFCXBackendSymbols(
+            coefficient_numbering, coefficient_offsets, original_constant_offsets
+        )
         self.access = FFCXBackendAccess(ir, self.symbols, options)
+        self.definitions = FFCXBackendDefinitions(ir, self.access, options)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/codegeneration.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/codegeneration.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,57 +4,69 @@
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Compiler stage 4: Code generation.
 
 This module implements the generation of C code for the body of each
 UFC function from an intermediate representation (IR).
-
 """
 
+from __future__ import annotations
+
 import logging
 import typing
 
+import numpy.typing as npt
+
 from ffcx.codegeneration.C.dofmap import generator as dofmap_generator
 from ffcx.codegeneration.C.expressions import generator as expression_generator
-from ffcx.codegeneration.C.finite_element import \
-    generator as finite_element_generator
+from ffcx.codegeneration.C.file import generator as file_generator
+from ffcx.codegeneration.C.finite_element import generator as finite_element_generator
 from ffcx.codegeneration.C.form import generator as form_generator
 from ffcx.codegeneration.C.integrals import generator as integral_generator
-from ffcx.codegeneration.C.file import generator as file_generator
+from ffcx.ir.representation import DataIR
 
 logger = logging.getLogger("ffcx")
 
 
 class CodeBlocks(typing.NamedTuple):
-    """
-    Storage of code blocks of the form (declaration, implementation).
+    """Storage of code blocks of the form (declaration, implementation).
 
     Blocks for elements, dofmaps, integrals, forms and expressions,
     and start and end of file output
     """
 
-    file_pre: typing.List[typing.Tuple[str, str]]
-    elements: typing.List[typing.Tuple[str, str]]
-    dofmaps: typing.List[typing.Tuple[str, str]]
-    integrals: typing.List[typing.Tuple[str, str]]
-    forms: typing.List[typing.Tuple[str, str]]
-    expressions: typing.List[typing.Tuple[str, str]]
-    file_post: typing.List[typing.Tuple[str, str]]
+    file_pre: list[tuple[str, str]]
+    elements: list[tuple[str, str]]
+    dofmaps: list[tuple[str, str]]
+    integrals: list[tuple[str, str]]
+    forms: list[tuple[str, str]]
+    expressions: list[tuple[str, str]]
+    file_post: list[tuple[str, str]]
 
 
-def generate_code(ir, options) -> CodeBlocks:
+def generate_code(ir: DataIR, options: dict[str, int | float | npt.DTypeLike]) -> CodeBlocks:
     """Generate code blocks from intermediate representation."""
     logger.info(79 * "*")
     logger.info("Compiler stage 3: Generating code")
     logger.info(79 * "*")
 
     # Generate code for finite_elements
-    code_finite_elements = [finite_element_generator(element_ir, options) for element_ir in ir.elements]
+    code_finite_elements = [
+        finite_element_generator(element_ir, options) for element_ir in ir.elements
+    ]
     code_dofmaps = [dofmap_generator(dofmap_ir, options) for dofmap_ir in ir.dofmaps]
     code_integrals = [integral_generator(integral_ir, options) for integral_ir in ir.integrals]
     code_forms = [form_generator(form_ir, options) for form_ir in ir.forms]
-    code_expressions = [expression_generator(expression_ir, options) for expression_ir in ir.expressions]
+    code_expressions = [
+        expression_generator(expression_ir, options) for expression_ir in ir.expressions
+    ]
     code_file_pre, code_file_post = file_generator(options)
-    return CodeBlocks(file_pre=[code_file_pre], elements=code_finite_elements, dofmaps=code_dofmaps,
-                      integrals=code_integrals, forms=code_forms, expressions=code_expressions,
-                      file_post=[code_file_post])
+    return CodeBlocks(
+        file_pre=[code_file_pre],
+        elements=code_finite_elements,
+        dofmaps=code_dofmaps,
+        integrals=code_integrals,
+        forms=code_forms,
+        expressions=code_expressions,
+        file_post=[code_file_post],
+    )
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/definitions.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/definitions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,232 @@
-# Copyright (C) 2011-2017 Martin Sandve Alnæs
+# Copyright (C) 2011-2023 Martin Sandve Alnæs, Igor A. Baratta
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """FFCx/UFC specific variable definitions."""
 
 import logging
+from typing import Union
 
 import ufl
-from ffcx.element_interface import convert_element
+
 import ffcx.codegeneration.lnodes as L
+from ffcx.ir.analysis.modified_terminals import ModifiedTerminal
+from ffcx.ir.elementtables import UniqueTableReferenceT
+from ffcx.ir.representationutils import QuadratureRule
 
 logger = logging.getLogger("ffcx")
 
 
-class FFCXBackendDefinitions(object):
+def create_quadrature_index(quadrature_rule, quadrature_index_symbol):
+    """Create a multi index for the quadrature loop."""
+    ranges = [0]
+    name = quadrature_index_symbol.name
+    indices = [L.Symbol(name, dtype=L.DataType.INT)]
+    if quadrature_rule:
+        ranges = [quadrature_rule.weights.size]
+        if quadrature_rule.has_tensor_factors:
+            dim = len(quadrature_rule.tensor_factors)
+            ranges = [factor[1].size for factor in quadrature_rule.tensor_factors]
+            indices = [L.Symbol(name + f"{i}", dtype=L.DataType.INT) for i in range(dim)]
+
+    return L.MultiIndex(indices, ranges)
+
+
+def create_dof_index(tabledata, dof_index_symbol):
+    """Create a multi index for the coefficient dofs."""
+    name = dof_index_symbol.name
+    if tabledata.has_tensor_factorisation:
+        dim = len(tabledata.tensor_factors)
+        ranges = [factor.values.shape[-1] for factor in tabledata.tensor_factors]
+        indices = [L.Symbol(f"{name}{i}", dtype=L.DataType.INT) for i in range(dim)]
+    else:
+        ranges = [tabledata.values.shape[-1]]
+        indices = [L.Symbol(name, dtype=L.DataType.INT)]
+
+    return L.MultiIndex(indices, ranges)
+
+
+class FFCXBackendDefinitions:
     """FFCx specific code definitions."""
 
-    def __init__(self, ir, symbols, options):
+    def __init__(self, ir, access, options):
+        """Initialise."""
         # Store ir and options
         self.integral_type = ir.integral_type
         self.entitytype = ir.entitytype
-        self.symbols = symbols
+        self.access = access
+        self.symbols = access.symbols
         self.options = options
 
         self.ir = ir
 
-        # Lookup table for handler to call when the "get" method (below) is
         # called, depending on the first argument type.
-        self.call_lookup = {ufl.coefficient.Coefficient: self.coefficient,
-                            ufl.constant.Constant: self.constant,
-                            ufl.geometry.Jacobian: self.jacobian,
-                            ufl.geometry.CellVertices: self._expect_physical_coords,
-                            ufl.geometry.FacetEdgeVectors: self._expect_physical_coords,
-                            ufl.geometry.CellEdgeVectors: self._expect_physical_coords,
-                            ufl.geometry.CellFacetJacobian: self._expect_table,
-                            ufl.geometry.ReferenceCellVolume: self._expect_table,
-                            ufl.geometry.ReferenceFacetVolume: self._expect_table,
-                            ufl.geometry.ReferenceCellEdgeVectors: self._expect_table,
-                            ufl.geometry.ReferenceFacetEdgeVectors: self._expect_table,
-                            ufl.geometry.ReferenceNormal: self._expect_table,
-                            ufl.geometry.CellOrientation: self._pass,
-                            ufl.geometry.FacetOrientation: self._expect_table,
-                            ufl.geometry.SpatialCoordinate: self.spatial_coordinate}
-
-    def get(self, t, mt, tabledata, quadrature_rule, access):
-        # Call appropriate handler, depending on the type of t
-        ttype = type(t)
-        handler = self.call_lookup.get(ttype, False)
-
-        if not handler:
-            # Look for parent class types instead
-            for k in self.call_lookup.keys():
-                if isinstance(t, k):
-                    handler = self.call_lookup[k]
-                    break
+        self.handler_lookup = {
+            ufl.coefficient.Coefficient: self.coefficient,
+            ufl.geometry.Jacobian: self._define_coordinate_dofs_lincomb,
+            ufl.geometry.SpatialCoordinate: self.spatial_coordinate,
+            ufl.constant.Constant: self.pass_through,
+            ufl.geometry.CellVertices: self.pass_through,
+            ufl.geometry.FacetEdgeVectors: self.pass_through,
+            ufl.geometry.CellEdgeVectors: self.pass_through,
+            ufl.geometry.CellFacetJacobian: self.pass_through,
+            ufl.geometry.ReferenceCellVolume: self.pass_through,
+            ufl.geometry.ReferenceFacetVolume: self.pass_through,
+            ufl.geometry.ReferenceCellEdgeVectors: self.pass_through,
+            ufl.geometry.ReferenceFacetEdgeVectors: self.pass_through,
+            ufl.geometry.ReferenceNormal: self.pass_through,
+            ufl.geometry.CellOrientation: self.pass_through,
+            ufl.geometry.FacetOrientation: self.pass_through,
+        }
+
+    def get(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
+        """Return definition code for a terminal."""
+        # Call appropriate handler, depending on the type of terminal
+        terminal = mt.terminal
+        ttype = type(terminal)
+
+        # Look for parent class of ttype or direct handler
+        while ttype not in self.handler_lookup and ttype.__bases__:
+            ttype = ttype.__bases__[0]
+
+        # Get the handler from the lookup, or None if not found
+        handler = self.handler_lookup.get(ttype)
+
+        if handler is None:
+            raise NotImplementedError(f"No handler for terminal type: {ttype}")
+
+        # Call the handler
+        return handler(mt, tabledata, quadrature_rule, access)
+
+    def coefficient(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
+        """Return definition code for coefficients."""
+        # For applying tensor product to coefficients, we need to know if the coefficient
+        # has a tensor factorisation and if the quadrature rule has a tensor factorisation.
+        # If both are true, we can apply the tensor product to the coefficient.
 
-        if handler:
-            return handler(t, mt, tabledata, quadrature_rule, access)
-        else:
-            raise RuntimeError("Not handled: %s", ttype)
+        iq_symbol = self.symbols.quadrature_loop_index
+        ic_symbol = self.symbols.coefficient_dof_sum_index
 
-    def coefficient(self, t, mt, tabledata, quadrature_rule, access):
-        """Return definition code for coefficients."""
+        iq = create_quadrature_index(quadrature_rule, iq_symbol)
+        ic = create_dof_index(tabledata, ic_symbol)
+
+        # Get properties of tables
         ttype = tabledata.ttype
         num_dofs = tabledata.values.shape[3]
         bs = tabledata.block_size
         begin = tabledata.offset
         end = begin + bs * (num_dofs - 1) + 1
 
         if ttype == "zeros":
             logging.debug("Not expecting zero coefficients to get this far.")
-            return [], []
+            return []
 
         # For a constant coefficient we reference the dofs directly, so no definition needed
         if ttype == "ones" and end - begin == 1:
-            return [], []
+            return []
 
         assert begin < end
 
         # Get access to element table
-        FE = self.symbols.element_table(tabledata, self.entitytype, mt.restriction)
-        ic = self.symbols.coefficient_dof_sum_index
-
-        code = []
-        pre_code = []
-
-        if bs > 1 and not tabledata.is_piecewise:
-            # For bs > 1, the coefficient access has a stride of bs. e.g.: XYZXYZXYZ
-            # When memory access patterns are non-sequential, the number of cache misses increases.
-            # In turn, it results in noticeably reduced performance.
-            # In this case, we create temp arrays outside the quadrature to store the coefficients and
-            # have a sequential access pattern.
-            dof_access, dof_access_map = self.symbols.coefficient_dof_access_blocked(mt.terminal, ic, bs, begin)
-
-            # If a map is necessary from stride 1 to bs, the code must be added before the quadrature loop.
-            if dof_access_map:
-                pre_code += [L.ArrayDecl(dof_access.array, sizes=num_dofs)]
-                pre_body = [L.Assign(dof_access, dof_access_map)]
-                pre_code += [L.ForRange(ic, 0, num_dofs, pre_body)]
-        else:
-            dof_access = self.symbols.coefficient_dof_access(mt.terminal, ic * bs + begin)
-
-        body = [L.AssignAdd(access, dof_access * FE[ic])]
-        code += [L.VariableDecl(access, 0.0)]
-        code += [L.ForRange(ic, 0, num_dofs, body)]
-
-        return pre_code, code
-
-    def constant(self, t, mt, tabledata, quadrature_rule, access):
-        # Constants are not defined within the kernel.
-        # No definition is needed because access to them is directly
-        # via symbol c[], i.e. as passed into the kernel.
-        return [], []
-
-    def _define_coordinate_dofs_lincomb(self, e, mt, tabledata, quadrature_rule, access):
+        FE, tables = self.access.table_access(tabledata, self.entitytype, mt.restriction, iq, ic)
+        dof_access: L.ArrayAccess = self.symbols.coefficient_dof_access(
+            mt.terminal, (ic.global_index) * bs + begin
+        )
+
+        declaration: list[L.Declaration] = [L.VariableDecl(access, 0.0)]
+        body = [L.AssignAdd(access, dof_access * FE)]
+        code = [L.create_nested_for_loops([ic], body)]
+
+        name = type(mt.terminal).__name__
+        input = [dof_access.array, *tables]
+        output = [access]
+        annotations = [L.Annotation.fuse]
+
+        # assert input and output are Symbol objects
+        assert all(isinstance(i, L.Symbol) for i in input)
+        assert all(isinstance(o, L.Symbol) for o in output)
+
+        return L.Section(name, code, declaration, input, output, annotations)
+
+    def _define_coordinate_dofs_lincomb(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
         """Define x or J as a linear combination of coordinate dofs with given table data."""
         # Get properties of domain
         domain = ufl.domain.extract_unique_domain(mt.terminal)
         coordinate_element = domain.ufl_coordinate_element()
-        num_scalar_dofs = convert_element(coordinate_element).sub_element.dim
+        num_scalar_dofs = coordinate_element._sub_element.dim
 
         num_dofs = tabledata.values.shape[3]
         begin = tabledata.offset
 
         assert num_scalar_dofs == num_dofs
 
         # Find table name
         ttype = tabledata.ttype
 
         assert ttype != "zeros"
         assert ttype != "ones"
 
         # Get access to element table
-        FE = self.symbols.element_table(tabledata, self.entitytype, mt.restriction)
-        ic = self.symbols.coefficient_dof_sum_index
-        dof_access = self.symbols.domain_dof_access(ic, begin, 3, num_scalar_dofs, mt.restriction)
+        ic_symbol = self.symbols.coefficient_dof_sum_index
+        iq_symbol = self.symbols.quadrature_loop_index
+        ic = create_dof_index(tabledata, ic_symbol)
+        iq = create_quadrature_index(quadrature_rule, iq_symbol)
+        FE, tables = self.access.table_access(tabledata, self.entitytype, mt.restriction, iq, ic)
+
+        dof_access = L.Symbol("coordinate_dofs", dtype=L.DataType.REAL)
+
+        # coordinate dofs is always 3d
+        dim = 3
+        offset = 0
+        if mt.restriction == "-":
+            offset = num_scalar_dofs * dim
 
         code = []
-        body = [L.AssignAdd(access, dof_access * FE[ic])]
-        code += [L.VariableDecl(access, 0.0)]
-        code += [L.ForRange(ic, 0, num_scalar_dofs, body)]
-
-        return [], code
-
-    def spatial_coordinate(self, e, mt, tabledata, quadrature_rule, access):
+        declaration = [L.VariableDecl(access, 0.0)]
+        body = [L.AssignAdd(access, dof_access[ic.global_index * dim + begin + offset] * FE)]
+        code = [L.create_nested_for_loops([ic], body)]
+
+        name = type(mt.terminal).__name__
+        output = [access]
+        input = [dof_access, *tables]
+        annotations = [L.Annotation.fuse]
+
+        # assert input and output are Symbol objects
+        assert all(isinstance(i, L.Symbol) for i in input)
+        assert all(isinstance(o, L.Symbol) for o in output)
+
+        return L.Section(name, code, declaration, input, output, annotations)
+
+    def spatial_coordinate(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
         """Return definition code for the physical spatial coordinates.
 
         If physical coordinates are given:
           No definition needed.
 
         If reference coordinates are given:
           x = sum_k xdof_k xphi_k(X)
@@ -158,27 +236,28 @@
         """
         if self.integral_type in ufl.custom_integral_types:
             # FIXME: Jacobian may need adjustment for custom_integral_types
             if mt.local_derivatives:
                 logging.exception("FIXME: Jacobian in custom integrals is not implemented.")
             return []
         else:
-            return self._define_coordinate_dofs_lincomb(e, mt, tabledata, quadrature_rule, access)
+            return self._define_coordinate_dofs_lincomb(mt, tabledata, quadrature_rule, access)
 
-    def jacobian(self, e, mt, tabledata, quadrature_rule, access):
+    def jacobian(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
         """Return definition code for the Jacobian of x(X)."""
-        return self._define_coordinate_dofs_lincomb(e, mt, tabledata, quadrature_rule, access)
+        return self._define_coordinate_dofs_lincomb(mt, tabledata, quadrature_rule, access)
 
-    def _expect_table(self, e, mt, tabledata, quadrature_rule, access):
-        """Return quantities referring to constant tables defined in the generated code."""
-        # TODO: Inject const static table here instead?
-        return [], []
-
-    def _expect_physical_coords(self, e, mt, tabledata, quadrature_rule, access):
-        """Return quantities referring to coordinate_dofs."""
-        # TODO: Generate more efficient inline code for Max/MinCell/FacetEdgeLength
-        #       and CellDiameter here rather than lowering these quantities?
-        return [], []
-
-    def _pass(self, *args, **kwargs):
-        """Return nothing."""
-        return [], []
+    def pass_through(
+        self,
+        mt: ModifiedTerminal,
+        tabledata: UniqueTableReferenceT,
+        quadrature_rule: QuadratureRule,
+        access: L.Symbol,
+    ) -> Union[L.Section, list]:
+        """Return definition code for pass through terminals."""
+        return []
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/expression_generator.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/expression_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 # Copyright (C) 2019 Michal Habera
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Expression generator."""
 
 import collections
 import logging
 from itertools import product
-from typing import Any, DefaultDict, Dict, Set
+from typing import Any
 
 import ufl
+
+import ffcx.codegeneration.lnodes as L
 from ffcx.codegeneration import geometry
 from ffcx.codegeneration.backend import FFCXBackend
-import ffcx.codegeneration.lnodes as L
 from ffcx.codegeneration.lnodes import LNode
 from ffcx.ir.representation import ExpressionIR
 
 logger = logging.getLogger("ffcx")
 
 
 class ExpressionGenerator:
-    def __init__(self, ir: ExpressionIR, backend: FFCXBackend):
+    """Expression generator."""
 
+    def __init__(self, ir: ExpressionIR, backend: FFCXBackend):
+        """Initialise."""
         if len(list(ir.integrand.keys())) != 1:
             raise RuntimeError("Only one set of points allowed for expression evaluation")
 
         self.ir = ir
         self.backend = backend
-        self.scope: Dict[Any, LNode] = {}
-        self._ufl_names: Set[Any] = set()
-        self.symbol_counters: DefaultDict[Any, int] = collections.defaultdict(int)
-        self.shared_symbols: Dict[Any, Any] = {}
+        self.scope: dict[Any, LNode] = {}
+        self._ufl_names: set[Any] = set()
+        self.symbol_counters: collections.defaultdict[Any, int] = collections.defaultdict(int)
+        self.shared_symbols: dict[Any, Any] = {}
         self.quadrature_rule = list(self.ir.integrand.keys())[0]
 
     def generate(self):
+        """Generate."""
         parts = []
         parts += self.generate_element_tables()
+
         # Generate the tables of geometry data that are needed
         parts += self.generate_geometry_tables()
         parts += self.generate_piecewise_partition()
 
         all_preparts = []
         all_quadparts = []
 
@@ -54,24 +60,31 @@
         return L.StatementList(parts)
 
     def generate_geometry_tables(self):
         """Generate static tables of geometry data."""
         # Currently we only support circumradius
         ufl_geometry = {
             ufl.geometry.ReferenceCellVolume: "reference_cell_volume",
+            ufl.geometry.ReferenceNormal: "reference_facet_normals",
         }
-        cells: Dict[Any, Set[Any]] = {t: set() for t in ufl_geometry.keys()}
 
+        cells: dict[Any, set[Any]] = {t: set() for t in ufl_geometry.keys()}  # type: ignore
         for integrand in self.ir.integrand.values():
             for attr in integrand["factorization"].nodes.values():
                 mt = attr.get("mt")
                 if mt is not None:
                     t = type(mt.terminal)
+                    if self.ir.entitytype == "cell" and issubclass(
+                        t, ufl.geometry.GeometricFacetQuantity
+                    ):
+                        raise RuntimeError(f"Expressions for cells do not support {t}.")
                     if t in ufl_geometry:
-                        cells[t].add(ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname())
+                        cells[t].add(
+                            ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
+                        )
 
         parts = []
         for i, cell_list in cells.items():
             for c in cell_list:
                 parts.append(geometry.write_table(ufl_geometry[i], c))
 
         return parts
@@ -87,61 +100,67 @@
             table = tables[name]
             symbol = L.Symbol(name, dtype=L.DataType.REAL)
             self.backend.symbols.element_tables[name] = symbol
             decl = L.ArrayDecl(symbol, sizes=table.shape, values=table, const=True)
             parts += [decl]
 
         # Add leading comment if there are any tables
-        parts = L.commented_code_list(parts, [
-            "Precomputed values of basis functions",
-            "FE* dimensions: [entities][points][dofs]",
-        ])
+        parts = L.commented_code_list(
+            parts,
+            [
+                "Precomputed values of basis functions",
+                "FE* dimensions: [entities][points][dofs]",
+            ],
+        )
         return parts
 
     def generate_quadrature_loop(self):
         """Generate quadrature loop for this quadrature rule.
 
         In the context of expressions quadrature loop is not accumulated.
-
         """
         # Generate varying partition
         body = self.generate_varying_partition()
         body = L.commented_code_list(
-            body, f"Points loop body setup quadrature loop {self.quadrature_rule.id()}")
+            body, f"Points loop body setup quadrature loop {self.quadrature_rule.id()}"
+        )
 
         # Generate dofblock parts, some of this
         # will be placed before or after quadloop
-        preparts, quadparts = \
-            self.generate_dofblock_partition()
+        preparts, quadparts = self.generate_dofblock_partition()
         body += quadparts
 
         # Wrap body in loop or scope
         if not body:
             # Could happen for integral with everything zero and optimized away
             quadparts = []
         else:
             iq = self.backend.symbols.quadrature_loop_index
             num_points = self.quadrature_rule.points.shape[0]
             quadparts = [L.ForRange(iq, 0, num_points, body=body)]
-
         return preparts, quadparts
 
     def generate_varying_partition(self):
         """Generate factors of blocks which are not cellwise constant."""
         # Get annotated graph of factorisation
         F = self.ir.integrand[self.quadrature_rule]["factorization"]
 
         arraysymbol = L.Symbol(f"sv_{self.quadrature_rule.id()}", dtype=L.DataType.SCALAR)
         parts = self.generate_partition(arraysymbol, F, "varying")
         parts = L.commented_code_list(
-            parts, f"Unstructured varying computations for quadrature rule {self.quadrature_rule.id()}")
+            parts,
+            f"Unstructured varying computations for quadrature rule {self.quadrature_rule.id()}",
+        )
         return parts
 
     def generate_piecewise_partition(self):
-        """Generate factors of blocks which are constant (i.e. do not depend on quadrature points)."""
+        """Generate factors of blocks which are constant.
+
+        I.e. do not depend on quadrature points).
+        """
         # Get annotated graph of factorisation
         F = self.ir.integrand[self.quadrature_rule]["factorization"]
 
         arraysymbol = L.Symbol("sp", dtype=L.DataType.SCALAR)
         parts = self.generate_partition(arraysymbol, F, "piecewise")
         parts = L.commented_code_list(parts, "Unstructured piecewise computations")
         return parts
@@ -149,23 +168,23 @@
     def generate_dofblock_partition(self):
         """Generate assignments of blocks multiplied with their factors into final tensor A."""
         block_contributions = self.ir.integrand[self.quadrature_rule]["block_contributions"]
 
         preparts = []
         quadparts = []
 
-        blocks = [(blockmap, blockdata)
-                  for blockmap, contributions in sorted(block_contributions.items())
-                  for blockdata in contributions]
+        blocks = [
+            (blockmap, blockdata)
+            for blockmap, contributions in sorted(block_contributions.items())
+            for blockdata in contributions
+        ]
 
         for blockmap, blockdata in blocks:
-
             # Define code for block depending on mode
-            block_preparts, block_quadparts = \
-                self.generate_block_parts(blockmap, blockdata)
+            block_preparts, block_quadparts = self.generate_block_parts(blockmap, blockdata)
 
             # Add definitions
             preparts.extend(block_preparts)
 
             # Add computations
             quadparts.extend(block_quadparts)
 
@@ -194,37 +213,37 @@
         num_points = self.quadrature_rule.points.shape[0]
         A_shape = [num_points, components] + self.ir.tensor_shape
         A = self.backend.symbols.element_tensor
         iq = self.backend.symbols.quadrature_loop_index
 
         # Check if DOFs in dofrange are equally spaced.
         expand_loop = False
-        for i, bm in enumerate(blockmap):
+        for bm in blockmap:
             for a, b in zip(bm[1:-1], bm[2:]):
                 if b - a != bm[1] - bm[0]:
                     expand_loop = True
                     break
             else:
                 continue
             break
 
         if expand_loop:
             # If DOFs in dofrange are not equally spaced, then expand out the for loop
-            for A_indices, B_indices in zip(product(*blockmap),
-                                            product(*[range(len(b)) for b in blockmap])):
+            for A_indices, B_indices in zip(
+                product(*blockmap), product(*[range(len(b)) for b in blockmap])
+            ):
                 B_indices = tuple([iq] + list(B_indices))
                 A_indices = tuple([iq] + A_indices)
                 for fi_ci in blockdata.factor_indices_comp_indices:
                     f = self.get_var(F.nodes[fi_ci[0]]["expression"])
                     arg_factors = self.get_arg_factors(blockdata, block_rank, B_indices)
                     Brhs = L.float_product([f] + arg_factors)
                     multi_index = L.MultiIndex([A_indices[0], fi_ci[1]] + A_indices[1:], A_shape)
                     quadparts.append(L.AssignAdd(A[multi_index], Brhs))
         else:
-
             # Prepend dimensions of dofmap block with free index
             # for quadrature points and expression components
             B_indices = tuple([iq] + list(arg_indices))
 
             # Fetch code to access modified arguments
             # An access to FE table data
             arg_factors = self.get_arg_factors(blockdata, block_rank, B_indices)
@@ -251,30 +270,26 @@
                 f = self.get_var(F.nodes[fi_ci[0]]["expression"])
                 Brhs = L.float_product([f] + arg_factors)
                 indices = [A_indices[0], fi_ci[1]] + list(A_indices[1:])
                 multi_index = L.MultiIndex(indices, A_shape)
                 body.append(L.AssignAdd(A[multi_index], Brhs))
 
             for i in reversed(range(block_rank)):
-                body = L.ForRange(
-                    B_indices[i + 1], 0, blockdims[i], body=body)
+                body = L.ForRange(B_indices[i + 1], 0, blockdims[i], body=body)
             quadparts += [body]
 
         return preparts, quadparts
 
     def get_arg_factors(self, blockdata, block_rank, indices):
         """Get argument factors (i.e. blocks).
 
-        Options
-        ----------
-        blockdata
-        block_rank
-        indices
-            Indices used to index element tables
-
+        Args:
+            blockdata: block data
+            block_rank: block rank
+            indices: Indices used to index element tables
         """
         arg_factors = []
         for i in range(block_rank):
             mad = blockdata.ma_data[i]
             td = mad.tabledata
             mt = self.ir.integrand[self.quadrature_rule]["modified_arguments"][mad.ma_index]
 
@@ -292,103 +307,68 @@
     def new_temp_symbol(self, basename):
         """Create a new code symbol named basename + running counter."""
         name = "%s%d" % (basename, self.symbol_counters[basename])
         self.symbol_counters[basename] += 1
         return L.Symbol(name, dtype=L.DataType.SCALAR)
 
     def get_var(self, v):
+        """Get a variable."""
         if v._ufl_is_literal_:
             return L.ufl_to_lnodes(v)
         f = self.scope.get(v)
         return f
 
     def generate_partition(self, symbol, F, mode):
         """Generate computations of factors of blocks."""
         definitions = []
-        pre_definitions = dict()
         intermediates = []
 
-        use_symbol_array = True
-
-        for i, attr in F.nodes.items():
-            if attr['status'] != mode:
+        for _, attr in F.nodes.items():
+            if attr["status"] != mode:
                 continue
-            v = attr['expression']
-            mt = attr.get('mt')
+            v = attr["expression"]
+            mt = attr.get("mt")
 
             if v._ufl_is_literal_:
                 vaccess = L.ufl_to_lnodes(v)
             elif mt is not None:
                 # All finite element based terminals have table data, as well
                 # as some, but not all, of the symbolic geometric terminals
-                tabledata = attr.get('tr')
+                tabledata = attr.get("tr")
 
                 # Backend specific modified terminal translation
-                vaccess = self.backend.access.get(mt.terminal, mt, tabledata, 0)
+                vaccess = self.backend.access.get(mt, tabledata, 0)
+                vdef = self.backend.definitions.get(mt, tabledata, 0, vaccess)
 
-                predef, vdef = self.backend.definitions.get(mt.terminal, mt, tabledata, 0, vaccess)
-                if predef:
-                    pre_definitions[str(predef[0].symbol.name)] = predef
+                if vdef:
+                    assert isinstance(vdef, L.Section)
+                    vdef = vdef.declarations + vdef.statements
 
                 # Store definitions of terminals in list
                 assert isinstance(vdef, list)
                 definitions.extend(vdef)
             else:
                 # Get previously visited operands
                 vops = [self.get_var(op) for op in v.ufl_operands]
 
-                # get parent operand
-                pid = F.in_edges[i][0] if F.in_edges[i] else -1
-                if pid and pid > i:
-                    parent_exp = F.nodes.get(pid)['expression']
-                else:
-                    parent_exp = None
-
                 # Mapping UFL operator to target language
                 self._ufl_names.add(v._ufl_handler_name_)
                 vexpr = L.ufl_to_lnodes(v, *vops)
 
-                # Create a new intermediate for each subexpression
-                # except boolean conditions and its childs
-                if isinstance(parent_exp, ufl.classes.Condition):
-                    # Skip intermediates for 'x' and 'y' in x<y
-                    # Avoid the creation of complex valued intermediates
-                    vaccess = vexpr
-                elif isinstance(v, ufl.classes.Condition):
-                    # Inline the conditions x < y, condition values
-                    # This removes the need to handle boolean intermediate variables.
-                    # With tensor-valued conditionals it may not be optimal but we
-                    # let the compiler take responsibility for optimizing those cases.
-                    vaccess = vexpr
-                elif any(op._ufl_is_literal_ for op in v.ufl_operands):
-                    # Skip intermediates for e.g. -2.0*x,
-                    # resulting in lines like z = y + -2.0*x
-                    vaccess = vexpr
-                else:
-                    # Record assignment of vexpr to intermediate variable
-                    j = len(intermediates)
-                    if use_symbol_array:
-                        vaccess = symbol[j]
-                        intermediates.append(L.Assign(vaccess, vexpr))
-                    else:
-                        scalar_type = self.backend.access.options["scalar_type"]
-                        vaccess = L.Symbol("%s_%d" % (symbol.name, j), dtype=L.DataType.SCALAR)
-                        intermediates.append(L.VariableDecl(f"const {scalar_type}", vaccess, vexpr))
+                is_cond = isinstance(v, ufl.classes.Condition)
+                dtype = L.DataType.BOOL if is_cond else L.DataType.SCALAR
+
+                j = len(intermediates)
+                vaccess = L.Symbol(f"{symbol.name}_{j}", dtype=dtype)
+                intermediates.append(L.VariableDecl(vaccess, vexpr))
 
             # Store access node for future reference
             self.scope[v] = vaccess
 
         # Join terminal computation, array of intermediate expressions,
         # and intermediate computations
         parts = []
 
-        for _, definition in pre_definitions.items():
-            parts += definition
-
-        if definitions:
-            parts += definitions
+        parts += definitions
+        parts += intermediates
 
-        if intermediates:
-            if use_symbol_array:
-                parts += [L.ArrayDecl(symbol, sizes=len(intermediates))]
-            parts += intermediates
         return parts
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/geometry.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/geometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright (C) 2021 Matthew Scroggs
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Geometry."""
 
+import basix
 import numpy as np
+
 import ffcx.codegeneration.lnodes as L
-import basix
 
 
 def write_table(tablename, cellname):
+    """Write a table."""
     if tablename == "facet_edge_vertices":
         return facet_edge_vertices(tablename, cellname)
     if tablename == "reference_facet_jacobian":
         return reference_facet_jacobian(tablename, cellname)
     if tablename == "reference_cell_volume":
         return reference_cell_volume(tablename, cellname)
     if tablename == "reference_facet_volume":
@@ -26,14 +29,15 @@
         return reference_facet_normals(tablename, cellname)
     if tablename == "facet_orientation":
         return facet_orientation(tablename, cellname)
     raise ValueError(f"Unknown geometry table name: {tablename}")
 
 
 def facet_edge_vertices(tablename, cellname):
+    """Write facet edge vertices."""
     celltype = getattr(basix.CellType, cellname)
     topology = basix.topology(celltype)
     triangle_edges = basix.topology(basix.CellType.triangle)[1]
     quadrilateral_edges = basix.topology(basix.CellType.quadrilateral)[1]
 
     if len(topology) != 4:
         raise ValueError("Can only get facet edges for 3D cells.")
@@ -49,76 +53,85 @@
 
     out = np.array(edge_vertices, dtype=int)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.INT)
     return L.ArrayDecl(symbol, values=out, const=True)
 
 
 def reference_facet_jacobian(tablename, cellname):
+    """Write a reference facet jacobian."""
     celltype = getattr(basix.CellType, cellname)
     out = basix.cell.facet_jacobians(celltype)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.ArrayDecl(symbol, values=out, const=True)
 
 
 def reference_cell_volume(tablename, cellname):
+    """Write a reference cell volume."""
     celltype = getattr(basix.CellType, cellname)
     out = basix.cell.volume(celltype)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.VariableDecl(symbol, out)
 
 
 def reference_facet_volume(tablename, cellname):
+    """Write a reference facet volume."""
     celltype = getattr(basix.CellType, cellname)
     volumes = basix.cell.facet_reference_volumes(celltype)
     for i in volumes[1:]:
         if not np.isclose(i, volumes[0]):
             raise ValueError("Reference facet volume not supported for this cell type.")
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.VariableDecl(symbol, volumes[0])
 
 
 def reference_edge_vectors(tablename, cellname):
+    """Write reference edge vectors."""
     celltype = getattr(basix.CellType, cellname)
     topology = basix.topology(celltype)
     geometry = basix.geometry(celltype)
     edge_vectors = [geometry[j] - geometry[i] for i, j in topology[1]]
     out = np.array(edge_vectors)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.ArrayDecl(symbol, values=out, const=True)
 
 
 def facet_reference_edge_vectors(tablename, cellname):
+    """Write facet reference edge vectors."""
     celltype = getattr(basix.CellType, cellname)
     topology = basix.topology(celltype)
     geometry = basix.geometry(celltype)
     triangle_edges = basix.topology(basix.CellType.triangle)[1]
     quadrilateral_edges = basix.topology(basix.CellType.quadrilateral)[1]
 
     if len(topology) != 4:
         raise ValueError("Can only get facet edges for 3D cells.")
 
     edge_vectors = []
     for facet in topology[-2]:
         if len(facet) == 3:
             edge_vectors += [geometry[facet[j]] - geometry[facet[i]] for i, j in triangle_edges]
         elif len(facet) == 4:
-            edge_vectors += [geometry[facet[j]] - geometry[facet[i]] for i, j in quadrilateral_edges]
+            edge_vectors += [
+                geometry[facet[j]] - geometry[facet[i]] for i, j in quadrilateral_edges
+            ]
         else:
             raise ValueError("Only triangular and quadrilateral faces supported.")
 
     out = np.array(edge_vectors)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.ArrayDecl(symbol, values=out, const=True)
 
 
 def reference_facet_normals(tablename, cellname):
+    """Write reference facet normals."""
     celltype = getattr(basix.CellType, cellname)
     out = basix.cell.facet_outward_normals(celltype)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.ArrayDecl(symbol, values=out, const=True)
 
 
 def facet_orientation(tablename, cellname):
+    """Write facet orientations."""
     celltype = getattr(basix.CellType, cellname)
     out = basix.cell.facet_orientations(celltype)
     symbol = L.Symbol(f"{cellname}_{tablename}", dtype=L.DataType.REAL)
     return L.ArrayDecl(symbol, values=out, const=True)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/integral_generator.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/integral_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-# Copyright (C) 2015-2023 Martin Sandve Alnæs, Michal Habera, Igor Baratta, Chris Richardson
+# Copyright (C) 2015-2024 Martin Sandve Alnæs, Michal Habera, Igor Baratta, Chris Richardson
+#
+# Modified by Jørgen S. Dokken, 2024
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Integral generator."""
 
 import collections
 import logging
-from typing import Any, Dict, List, Set, Tuple
+from numbers import Integral
+from typing import Any
 
 import ufl
+
+import ffcx.codegeneration.lnodes as L
 from ffcx.codegeneration import geometry
+from ffcx.codegeneration.definitions import create_dof_index, create_quadrature_index
+from ffcx.codegeneration.optimizer import optimize
 from ffcx.ir.elementtables import piecewise_ttypes
 from ffcx.ir.integral import BlockDataT
-import ffcx.codegeneration.lnodes as L
-from ffcx.codegeneration.lnodes import LNode, BinOp
 from ffcx.ir.representationutils import QuadratureRule
 
 logger = logging.getLogger("ffcx")
 
 
-class IntegralGenerator(object):
+def extract_dtype(v, vops: list[Any]):
+    """Extract dtype from ufl expression v and its operands."""
+    dtypes = []
+    for op in vops:
+        if hasattr(op, "dtype"):
+            dtypes.append(op.dtype)
+        elif hasattr(op, "symbol"):
+            dtypes.append(op.symbol.dtype)
+        elif isinstance(op, Integral):
+            dtypes.append(L.DataType.INT)
+        else:
+            raise RuntimeError(f"Not expecting this type of operand {type(op)}")
+    is_cond = isinstance(v, ufl.classes.Condition)
+    return L.DataType.BOOL if is_cond else L.merge_dtypes(dtypes)
+
+
+class IntegralGenerator:
+    """Integral generator."""
+
     def __init__(self, ir, backend):
+        """Initialise."""
         # Store ir
         self.ir = ir
 
         # Backend specific plugin with attributes
         # - symbols: for translating ufl operators to target language
         # - definitions: for defining backend specific variables
         # - access: for accessing backend specific variables
@@ -34,15 +59,15 @@
         # end for selecting necessary includes
         self._ufl_names = set()
 
         # Initialize lookup tables for variable scopes
         self.init_scopes()
 
         # Cache
-        self.shared_symbols = {}
+        self.temp_symbols = {}
 
         # Set of counters used for assigning names to intermediate
         # variables
         self.symbol_counters = collections.defaultdict(int)
 
     def init_scopes(self):
         """Initialize variable scope dicts."""
@@ -52,17 +77,18 @@
 
     def set_var(self, quadrature_rule, v, vaccess):
         """Set a new variable in variable scope dicts.
 
         Scope is determined by quadrature_rule which identifies the
         quadrature loop scope or None if outside quadrature loops.
 
-        v is the ufl expression and vaccess is the LNodes
-        expression to access the value in the code.
-
+        Args:
+            quadrature_rule: Quadrature rule
+            v: the ufl expression
+            vaccess: the LNodes expression to access the value in the code
         """
         self.scopes[quadrature_rule][v] = vaccess
 
     def get_var(self, quadrature_rule, v):
         """Lookup ufl expression v in variable scope dicts.
 
         Scope is determined by quadrature rule which identifies the
@@ -71,32 +97,37 @@
         If v is not found in quadrature loop scope, the piecewise
         scope (None) is checked.
 
         Returns the LNodes expression to access the value in the code.
         """
         if v._ufl_is_literal_:
             return L.ufl_to_lnodes(v)
+
+        # quadrature loop scope
         f = self.scopes[quadrature_rule].get(v)
+
+        # piecewise scope
         if f is None:
             f = self.scopes[None].get(v)
         return f
 
     def new_temp_symbol(self, basename):
         """Create a new code symbol named basename + running counter."""
         name = "%s%d" % (basename, self.symbol_counters[basename])
         self.symbol_counters[basename] += 1
         return L.Symbol(name, dtype=L.DataType.SCALAR)
 
     def get_temp_symbol(self, tempname, key):
+        """Get a temporary symbol."""
         key = (tempname,) + key
-        s = self.shared_symbols.get(key)
+        s = self.temp_symbols.get(key)
         defined = s is not None
         if not defined:
             s = self.new_temp_symbol(tempname)
-            self.shared_symbols[key] = s
+            self.temp_symbols[key] = s
         return s, defined
 
     def generate(self):
         """Generate entire tabulate_tensor body.
 
         Assumes that the code returned from here will be wrapped in a
         context that matches a suitable version of the UFC
@@ -122,28 +153,21 @@
         # quadloops, to define the quadloops, and to go after the
         # quadloops
         all_preparts = []
         all_quadparts = []
 
         # Pre-definitions are collected across all quadrature loops to
         # improve re-use and avoid name clashes
-        all_predefinitions = dict()
         for rule in self.ir.integrand.keys():
             # Generate code to compute piecewise constant scalar factors
             all_preparts += self.generate_piecewise_partition(rule)
 
             # Generate code to integrate reusable blocks of final
             # element tensor
-            pre_definitions, preparts, quadparts = self.generate_quadrature_loop(rule)
-            all_preparts += preparts
-            all_quadparts += quadparts
-            all_predefinitions.update(pre_definitions)
-
-        parts += L.commented_code_list(self.fuse_loops(all_predefinitions),
-                                       "Pre-definitions of modified terminals to enable unit-stride access")
+            all_quadparts += self.generate_quadrature_loop(rule)
 
         # Collect parts before, during, and after quadrature loops
         parts += all_preparts
         parts += all_quadparts
 
         return L.StatementList(parts)
 
@@ -173,35 +197,40 @@
             ufl.geometry.FacetEdgeVectors: "facet_edge_vertices",
             ufl.geometry.CellFacetJacobian: "reference_facet_jacobian",
             ufl.geometry.ReferenceCellVolume: "reference_cell_volume",
             ufl.geometry.ReferenceFacetVolume: "reference_facet_volume",
             ufl.geometry.ReferenceCellEdgeVectors: "reference_edge_vectors",
             ufl.geometry.ReferenceFacetEdgeVectors: "facet_reference_edge_vectors",
             ufl.geometry.ReferenceNormal: "reference_facet_normals",
-            ufl.geometry.FacetOrientation: "facet_orientation"
+            ufl.geometry.FacetOrientation: "facet_orientation",
         }
-        cells: Dict[Any, Set[Any]] = {t: set() for t in ufl_geometry.keys()}
+        cells: dict[Any, set[Any]] = {t: set() for t in ufl_geometry.keys()}  # type: ignore
 
         for integrand in self.ir.integrand.values():
             for attr in integrand["factorization"].nodes.values():
                 mt = attr.get("mt")
                 if mt is not None:
                     t = type(mt.terminal)
                     if t in ufl_geometry:
-                        cells[t].add(ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname())
+                        cells[t].add(
+                            ufl.domain.extract_unique_domain(mt.terminal).ufl_cell().cellname()
+                        )
 
         parts = []
         for i, cell_list in cells.items():
             for c in cell_list:
                 parts.append(geometry.write_table(ufl_geometry[i], c))
 
         return parts
 
     def generate_element_tables(self):
-        """Generate static tables with precomputed element basisfunction values in quadrature points."""
+        """Generate static tables.
+
+        With precomputed element basis function values in quadrature points.
+        """
         parts = []
         tables = self.ir.unique_tables
         table_types = self.ir.unique_table_types
         if self.ir.integral_type in ufl.custom_integral_types:
             # Define only piecewise tables
             table_names = [name for name in sorted(tables) if table_types[name] in piecewise_ttypes]
         else:
@@ -209,17 +238,21 @@
             table_names = sorted(tables)
 
         for name in table_names:
             table = tables[name]
             parts += self.declare_table(name, table)
 
         # Add leading comment if there are any tables
-        parts = L.commented_code_list(parts, [
-            "Precomputed values of basis functions and precomputations",
-            "FE* dimensions: [permutation][entities][points][dofs]"])
+        parts = L.commented_code_list(
+            parts,
+            [
+                "Precomputed values of basis functions and precomputations",
+                "FE* dimensions: [permutation][entities][points][dofs]",
+            ],
+        )
         return parts
 
     def declare_table(self, name, table):
         """Declare a table.
 
         If the dof dimensions of the table have dof rotations, apply
         these rotations.
@@ -228,157 +261,114 @@
         table_symbol = L.Symbol(name, dtype=L.DataType.REAL)
         self.backend.symbols.element_tables[name] = table_symbol
         return [L.ArrayDecl(table_symbol, values=table, const=True)]
 
     def generate_quadrature_loop(self, quadrature_rule: QuadratureRule):
         """Generate quadrature loop with for this quadrature_rule."""
         # Generate varying partition
-        pre_definitions, body = self.generate_varying_partition(quadrature_rule)
+        definitions, intermediates_0 = self.generate_varying_partition(quadrature_rule)
 
-        body = L.commented_code_list(body, f"Quadrature loop body setup for quadrature rule {quadrature_rule.id()}")
+        # Generate dofblock parts, some of this will be placed before or after quadloop
+        tensor_comp, intermediates_fw = self.generate_dofblock_partition(quadrature_rule)
+        assert all([isinstance(tc, L.Section) for tc in tensor_comp])
+
+        # Check if we only have Section objects
+        inputs = []
+        for definition in definitions:
+            assert isinstance(definition, L.Section)
+            inputs += definition.output
+
+        # Create intermediates section
+        output = []
+        declarations = []
+        for fw in intermediates_fw:
+            assert isinstance(fw, L.VariableDecl)
+            output += [fw.symbol]
+            declarations += [L.VariableDecl(fw.symbol, 0)]
+            intermediates_0 += [L.Assign(fw.symbol, fw.value)]
+        intermediates = [L.Section("Intermediates", intermediates_0, declarations, inputs, output)]
 
-        # Generate dofblock parts, some of this will be placed before or
-        # after quadloop
-        preparts, quadparts = self.generate_dofblock_partition(quadrature_rule)
-        body += quadparts
-
-        # Wrap body in loop or scope
-        if not body:
-            # Could happen for integral with everything zero and
-            # optimized away
-            quadparts = []
-        else:
-            num_points = quadrature_rule.points.shape[0]
-            iq = self.backend.symbols.quadrature_loop_index
-            quadparts = [L.ForRange(iq, 0, num_points, body=body)]
+        iq_symbol = self.backend.symbols.quadrature_loop_index
+        iq = create_quadrature_index(quadrature_rule, iq_symbol)
 
-        return pre_definitions, preparts, quadparts
+        code = definitions + intermediates + tensor_comp
+        code = optimize(code, quadrature_rule)
+
+        return [L.create_nested_for_loops([iq], code)]
 
     def generate_piecewise_partition(self, quadrature_rule):
+        """Generate a piecewise partition."""
         # Get annotated graph of factorisation
         F = self.ir.integrand[quadrature_rule]["factorization"]
-
         arraysymbol = L.Symbol(f"sp_{quadrature_rule.id()}", dtype=L.DataType.SCALAR)
-        pre_definitions, parts = self.generate_partition(arraysymbol, F, "piecewise", None)
-        assert len(pre_definitions) == 0, "Quadrature independent code should have not pre-definitions"
-        parts = L.commented_code_list(
-            parts, f"Quadrature loop independent computations for quadrature rule {quadrature_rule.id()}")
-
-        return parts
+        return self.generate_partition(arraysymbol, F, "piecewise", None)
 
     def generate_varying_partition(self, quadrature_rule):
-
+        """Generate a varying partition."""
         # Get annotated graph of factorisation
         F = self.ir.integrand[quadrature_rule]["factorization"]
-
         arraysymbol = L.Symbol(f"sv_{quadrature_rule.id()}", dtype=L.DataType.SCALAR)
-        pre_definitions, parts = self.generate_partition(arraysymbol, F, "varying", quadrature_rule)
-        parts = L.commented_code_list(parts, f"Varying computations for quadrature rule {quadrature_rule.id()}")
-
-        return pre_definitions, parts
+        return self.generate_partition(arraysymbol, F, "varying", quadrature_rule)
 
     def generate_partition(self, symbol, F, mode, quadrature_rule):
-
-        definitions = dict()
-        pre_definitions = dict()
+        """Generate a partition."""
+        definitions = []
         intermediates = []
 
-        use_symbol_array = True
-
         for i, attr in F.nodes.items():
-            if attr['status'] != mode:
+            if attr["status"] != mode:
                 continue
-            v = attr['expression']
-            mt = attr.get('mt')
+            v = attr["expression"]
 
-            # Generate code only if the expression is not already in
-            # cache
+            # Generate code only if the expression is not already in cache
             if not self.get_var(quadrature_rule, v):
                 if v._ufl_is_literal_:
                     vaccess = L.ufl_to_lnodes(v)
-                elif mt is not None:
-                    # All finite element based terminals have table
-                    # data, as well as some, but not all, of the
-                    # symbolic geometric terminals
-                    tabledata = attr.get('tr')
+                elif mt := attr.get("mt"):
+                    tabledata = attr.get("tr")
 
                     # Backend specific modified terminal translation
-                    vaccess = self.backend.access.get(mt.terminal, mt, tabledata, quadrature_rule)
-                    predef, vdef = self.backend.definitions.get(mt.terminal, mt, tabledata, quadrature_rule, vaccess)
-                    if predef:
-                        access = predef[0].symbol.name
-                        pre_definitions[str(access)] = predef
-
-                    # Store definitions of terminals in list
-                    assert isinstance(vdef, list)
-                    definitions[str(vaccess)] = vdef
+                    vaccess = self.backend.access.get(mt, tabledata, quadrature_rule)
+                    vdef = self.backend.definitions.get(mt, tabledata, quadrature_rule, vaccess)
+
+                    if vdef:
+                        assert isinstance(vdef, L.Section)
+                    # Only add if definition is unique.
+                    # This can happen when using sub-meshes
+                    if vdef not in definitions:
+                        definitions += [vdef]
                 else:
                     # Get previously visited operands
                     vops = [self.get_var(quadrature_rule, op) for op in v.ufl_operands]
-
-                    # get parent operand
-                    pid = F.in_edges[i][0] if F.in_edges[i] else -1
-                    if pid and pid > i:
-                        parent_exp = F.nodes.get(pid)['expression']
-                    else:
-                        parent_exp = None
+                    dtype = extract_dtype(v, vops)
 
                     # Mapping UFL operator to target language
                     self._ufl_names.add(v._ufl_handler_name_)
                     vexpr = L.ufl_to_lnodes(v, *vops)
 
-                    # Create a new intermediate for each subexpression
-                    # except boolean conditions and its childs
-                    if isinstance(parent_exp, ufl.classes.Condition):
-                        # Skip intermediates for 'x' and 'y' in x<y
-                        # Avoid the creation of complex valued intermediates
-                        vaccess = vexpr
-                    elif isinstance(v, ufl.classes.Condition):
-                        # Inline the conditions x < y, condition values
-                        # This removes the need to handle boolean
-                        # intermediate variables. With tensor-valued
-                        # conditionals it may not be optimal but we let
-                        # the compiler take responsibility for
-                        # optimizing those cases.
-                        vaccess = vexpr
-                    elif any(op._ufl_is_literal_ for op in v.ufl_operands):
-                        # Skip intermediates for e.g. -2.0*x,
-                        # resulting in lines like z = y + -2.0*x
-                        vaccess = vexpr
-                    else:
-                        # Record assignment of vexpr to intermediate variable
-                        j = len(intermediates)
-                        if use_symbol_array:
-                            vaccess = symbol[j]
-                            intermediates.append(L.Assign(vaccess, vexpr))
-                        else:
-                            vaccess = L.Symbol("%s_%d" % (symbol.name, j))
-                            intermediates.append(L.VariableDecl(vaccess, vexpr))
+                    j = len(intermediates)
+                    vaccess = L.Symbol(f"{symbol.name}_{j}", dtype=dtype)
+                    intermediates.append(L.VariableDecl(vaccess, vexpr))
 
                 # Store access node for future reference
                 self.set_var(quadrature_rule, v, vaccess)
 
-        # Join terminal computation, array of intermediate expressions,
-        # and intermediate computations
-        parts = []
-        parts += self.fuse_loops(definitions)
-
-        if intermediates:
-            if use_symbol_array:
-                parts += [L.ArrayDecl(symbol, sizes=len(intermediates))]
-            parts += intermediates
-        return pre_definitions, parts
+        # Optimize definitions
+        definitions = optimize(definitions, quadrature_rule)
+        return definitions, intermediates
 
     def generate_dofblock_partition(self, quadrature_rule: QuadratureRule):
+        """Generate a dofblock partition."""
         block_contributions = self.ir.integrand[quadrature_rule]["block_contributions"]
-        preparts = []
         quadparts = []
-        blocks = [(blockmap, blockdata)
-                  for blockmap, contributions in sorted(block_contributions.items())
-                  for blockdata in contributions]
+        blocks = [
+            (blockmap, blockdata)
+            for blockmap, contributions in sorted(block_contributions.items())
+            for blockdata in contributions
+        ]
 
         block_groups = collections.defaultdict(list)
 
         # Group loops by blockmap, in Vector elements each component has
         # a different blockmap
         for blockmap, blockdata in blocks:
             scalar_blockmap = []
@@ -386,221 +376,188 @@
             for i, b in enumerate(blockmap):
                 bs = blockdata.ma_data[i].tabledata.block_size
                 offset = blockdata.ma_data[i].tabledata.offset
                 b = tuple([(idx - offset) // bs for idx in b])
                 scalar_blockmap.append(b)
             block_groups[tuple(scalar_blockmap)].append(blockdata)
 
+        intermediates = []
         for blockmap in block_groups:
-            block_preparts, block_quadparts = self.generate_block_parts(
-                quadrature_rule, blockmap, block_groups[blockmap])
-
-            # Add definitions
-            preparts.extend(block_preparts)
+            block_quadparts, intermediate = self.generate_block_parts(
+                quadrature_rule, blockmap, block_groups[blockmap]
+            )
+            intermediates += intermediate
 
             # Add computations
             quadparts.extend(block_quadparts)
 
-        return preparts, quadparts
+        return quadparts, intermediates
 
     def get_arg_factors(self, blockdata, block_rank, quadrature_rule, iq, indices):
+        """Get arg factors."""
         arg_factors = []
+        tables = []
         for i in range(block_rank):
             mad = blockdata.ma_data[i]
             td = mad.tabledata
             scope = self.ir.integrand[quadrature_rule]["modified_arguments"]
             mt = scope[mad.ma_index]
+            arg_tables = []
 
             # Translate modified terminal to code
             # TODO: Move element table access out of backend?
             #       Not using self.backend.access.argument() here
             #       now because it assumes too much about indices.
 
-            table = self.backend.symbols.element_table(td, self.ir.entitytype, mt.restriction)
-
             assert td.ttype != "zeros"
 
             if td.ttype == "ones":
                 arg_factor = 1
             else:
                 # Assuming B sparsity follows element table sparsity
-                arg_factor = table[indices[i]]
+                arg_factor, arg_tables = self.backend.access.table_access(
+                    td, self.ir.entitytype, mt.restriction, iq, indices[i]
+                )
+
+            tables += arg_tables
             arg_factors.append(arg_factor)
-        return arg_factors
 
-    def generate_block_parts(self, quadrature_rule: QuadratureRule, blockmap: Tuple, blocklist: List[BlockDataT]):
+        return arg_factors, tables
+
+    def generate_block_parts(
+        self, quadrature_rule: QuadratureRule, blockmap: tuple, blocklist: list[BlockDataT]
+    ):
         """Generate and return code parts for a given block.
 
         Returns parts occurring before, inside, and after the quadrature
         loop identified by the quadrature rule.
 
         Should be called with quadrature_rule=None for
         quadloop-independent blocks.
         """
         # The parts to return
-        preparts: List[LNode] = []
-        quadparts: List[LNode] = []
+        quadparts: list[L.LNode] = []
+        intermediates: list[L.LNode] = []
+        tables = []
+        vars = []
 
         # RHS expressions grouped by LHS "dofmap"
         rhs_expressions = collections.defaultdict(list)
 
         block_rank = len(blockmap)
-        blockdims = tuple(len(dofmap) for dofmap in blockmap)
-
-        iq = self.backend.symbols.quadrature_loop_index
-
-        # Override dof index with quadrature loop index for arguments
-        # with quadrature element, to index B like B[iq*num_dofs + iq]
-        arg_indices = tuple(self.backend.symbols.argument_loop_index(i) for i in range(block_rank))
-        B_indices = []
-        for i in range(block_rank):
-            B_indices.append(arg_indices[i])
-        B_indices = list(B_indices)
+        iq_symbol = self.backend.symbols.quadrature_loop_index
+        iq = create_quadrature_index(quadrature_rule, iq_symbol)
 
         for blockdata in blocklist:
+            B_indices = []
+            for i in range(block_rank):
+                table_ref = blockdata.ma_data[i].tabledata
+                symbol = self.backend.symbols.argument_loop_index(i)
+                index = create_dof_index(table_ref, symbol)
+                B_indices.append(index)
+
             ttypes = blockdata.ttypes
             if "zeros" in ttypes:
-                raise RuntimeError("Not expecting zero arguments to be left in dofblock generation.")
+                raise RuntimeError(
+                    "Not expecting zero arguments to be left in dofblock generation."
+                )
 
             if len(blockdata.factor_indices_comp_indices) > 1:
                 raise RuntimeError("Code generation for non-scalar integrals unsupported")
 
             # We have scalar integrand here, take just the factor index
             factor_index = blockdata.factor_indices_comp_indices[0][0]
 
             # Get factor expression
             F = self.ir.integrand[quadrature_rule]["factorization"]
 
-            v = F.nodes[factor_index]['expression']
+            v = F.nodes[factor_index]["expression"]
             f = self.get_var(quadrature_rule, v)
 
             # Quadrature weight was removed in representation, add it back now
             if self.ir.integral_type in ufl.custom_integral_types:
                 weights = self.backend.symbols.custom_weights_table
-                weight = weights[iq]
+                weight = weights[iq.global_index]
             else:
                 weights = self.backend.symbols.weights_table(quadrature_rule)
-                weight = weights[iq]
+                weight = weights[iq.global_index]
 
             # Define fw = f * weight
             fw_rhs = L.float_product([f, weight])
             if not isinstance(fw_rhs, L.Product):
                 fw = fw_rhs
             else:
                 # Define and cache scalar temp variable
                 key = (quadrature_rule, factor_index, blockdata.all_factors_piecewise)
                 fw, defined = self.get_temp_symbol("fw", key)
                 if not defined:
-                    quadparts.append(L.VariableDecl(fw, fw_rhs))
+                    input = [f, weight]
+                    # filter only L.Symbol in input
+                    input = [i for i in input if isinstance(i, L.Symbol)]
+                    output = [fw]
+
+                    # assert input and output are Symbol objects
+                    assert all(isinstance(i, L.Symbol) for i in input)
+                    assert all(isinstance(o, L.Symbol) for o in output)
 
+                    intermediates += [L.VariableDecl(fw, fw_rhs)]
+
+            var = fw if isinstance(fw, L.Symbol) else fw.array
+            vars += [var]
             assert not blockdata.transposed, "Not handled yet"
 
             # Fetch code to access modified arguments
-            arg_factors = self.get_arg_factors(blockdata, block_rank, quadrature_rule, iq, B_indices)
+            arg_factors, table = self.get_arg_factors(
+                blockdata, block_rank, quadrature_rule, iq, B_indices
+            )
+            tables += table
 
+            # Define B_rhs = fw * arg_factors
             B_rhs = L.float_product([fw] + arg_factors)
 
             A_indices = []
             for i in range(block_rank):
-                offset = blockdata.ma_data[i].tabledata.offset
-                index = arg_indices[i]
+                index = B_indices[i]
+                tabledata = blockdata.ma_data[i].tabledata
+                offset = tabledata.offset
                 if len(blockmap[i]) == 1:
-                    A_indices.append(index + offset)
+                    A_indices.append(index.global_index + offset)
                 else:
                     block_size = blockdata.ma_data[i].tabledata.block_size
-                    A_indices.append(block_size * index + offset)
+                    A_indices.append(block_size * index.global_index + offset)
             rhs_expressions[tuple(A_indices)].append(B_rhs)
 
         # List of statements to keep in the inner loop
         keep = collections.defaultdict(list)
-        # List of temporary array declarations
-        pre_loop: List[LNode] = []
-        # List of loop invariant expressions to hoist
-        hoist: List[BinOp] = []
 
         for indices in rhs_expressions:
-            hoist_rhs = collections.defaultdict(list)
-
-            # Hoist loop invariant code and group array access (each
-            # table should only be read one time in the inner loop)
-            if block_rank == 2:
-                ind = B_indices[-1]
-                for rhs in rhs_expressions[indices]:
-                    if len(rhs.args) <= 2:
-                        keep[indices].append(rhs)
-                    else:
-                        varying = next((x for x in rhs.args if hasattr(x, 'indices') and (ind in x.indices)), None)
-                        if varying:
-                            invariant = [x for x in rhs.args if x is not varying]
-                            hoist_rhs[varying].append(invariant)
-                        else:
-                            keep[indices].append(rhs)
-
-                # Perform algebraic manipulations to reduce number of
-                # floating point operations (factorize expressions by
-                # grouping)
-                for statement in hoist_rhs:
-                    sum = L.Sum([L.float_product(rhs) for rhs in hoist_rhs[statement]])
-
-                    lhs = None
-                    for h in hoist:
-                        if h.rhs == sum:
-                            lhs = h.lhs
-                            break
-                    if lhs:
-                        keep[indices].append(L.float_product([statement, lhs]))
-                    else:
-                        t = self.new_temp_symbol("t")
-                        pre_loop.append(L.ArrayDecl(t, sizes=blockdims[0]))
-                        keep[indices].append(L.float_product([statement, t[B_indices[0]]]))
-                        hoist.append(L.Assign(t[B_indices[i - 1]], sum))
-            else:
-                keep[indices] = rhs_expressions[indices]
-
-        hoist_code: List[LNode] = [L.ForRange(B_indices[0], 0, blockdims[0], body=hoist)] if hoist else []
+            keep[indices] = rhs_expressions[indices]
 
-        body: List[LNode] = []
+        body: list[L.LNode] = []
 
         A = self.backend.symbols.element_tensor
         A_shape = self.ir.tensor_shape
         for indices in keep:
             multi_index = L.MultiIndex(list(indices), A_shape)
-            body.append(L.AssignAdd(A[multi_index], L.Sum(keep[indices])))
-
-        for i in reversed(range(block_rank)):
-            body = [L.ForRange(B_indices[i], 0, blockdims[i], body=body)]
+            for expression in keep[indices]:
+                body.append(L.AssignAdd(A[multi_index], expression))
 
-        quadparts += pre_loop
-        quadparts += hoist_code
-        quadparts += body
+        # reverse B_indices
+        B_indices = B_indices[::-1]
+        body = [L.create_nested_for_loops(B_indices, body)]
+        input = [*vars, *tables]
+        output = [A]
 
-        return preparts, quadparts
+        # Make sure we don't have repeated symbols in input
+        input = list(set(input))
 
-    def fuse_loops(self, definitions):
-        """Merge a sequence of loops with the same iteration space into a single loop.
+        # assert input and output are Symbol objects
+        assert all(isinstance(i, L.Symbol) for i in input)
+        assert all(isinstance(o, L.Symbol) for o in output)
 
-        Loop fusion improves data locality, cache reuse and decreases
-        the loop control overhead.
+        annotations = []
+        if len(B_indices) > 1:
+            annotations.append(L.Annotation.licm)
 
-        NOTE: Loop fusion might increase the pressure on register
-        allocation. Ideally, we should define a cost function to
-        determine how many loops should fuse at a time.
-
-        """
-        loops = collections.defaultdict(list)
-        pre_loop = []
-        for access, definition in definitions.items():
-            for d in definition:
-                if isinstance(d, L.ForRange):
-                    loops[(d.index, d.begin, d.end)] += [d.body]
-                else:
-                    pre_loop += [d]
-        fused = []
+        quadparts += [L.Section("Tensor Computation", body, [], input, output, annotations)]
 
-        for info, body in loops.items():
-            index, begin, end = info
-            fused += [L.ForRange(index, begin, end, body)]
-
-        code = []
-        code += pre_loop
-        code += fused
-        return code
+        return quadparts, intermediates
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/lnodes.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/lnodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 # Copyright (C) 2013-2023 Martin Sandve Alnæs, Chris Richardson
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""LNodes.
+
+LNodes is intended as a minimal generic language description.
+Formatting is done later, depending on the target language.
+
+Supported:
+ Floating point (and complex) and integer variables and multidimensional arrays
+ Range loops
+ Simple arithmetic, +-*/
+ Math operations
+ Logic conditions
+ Comments
+Not supported:
+ Pointers
+ Function Calls
+ Flow control (if, switch, while)
+ Booleans
+ Strings
+"""
 
 import numbers
-import ufl
-import numpy as np
+from collections.abc import Sequence
 from enum import Enum
+from typing import Optional
+
+import numpy as np
+import ufl
 
 
 class PRECEDENCE:
     """An enum-like class for operator precedence levels."""
 
     HIGHEST = 0
     LITERAL = 0
@@ -36,53 +58,40 @@
     AND = 11
     OR = 12
     CONDITIONAL = 13
     ASSIGN = 13
     LOWEST = 15
 
 
-"""LNodes is intended as a minimal generic language description.
-Formatting is done later, depending on the target language.
-
-Supported:
- Floating point (and complex) and integer variables and multidimensional arrays
- Range loops
- Simple arithmetic, +-*/
- Math operations
- Logic conditions
- Comments
-Not supported:
- Pointers
- Function Calls
- Flow control (if, switch, while)
- Booleans
- Strings
-"""
-
-
 def is_zero_lexpr(lexpr):
+    """Check if an expression is zero."""
     return (isinstance(lexpr, LiteralFloat) and lexpr.value == 0.0) or (
         isinstance(lexpr, LiteralInt) and lexpr.value == 0
     )
 
 
 def is_one_lexpr(lexpr):
+    """Check if an expression is one."""
     return (isinstance(lexpr, LiteralFloat) and lexpr.value == 1.0) or (
         isinstance(lexpr, LiteralInt) and lexpr.value == 1
     )
 
 
 def is_negative_one_lexpr(lexpr):
+    """Check if an expression is negative one."""
     return (isinstance(lexpr, LiteralFloat) and lexpr.value == -1.0) or (
         isinstance(lexpr, LiteralInt) and lexpr.value == -1
     )
 
 
 def float_product(factors):
-    """Build product of float factors, simplifying ones and zeros and returning 1.0 if empty sequence."""
+    """Build product of float factors.
+
+    Simplify ones and zeros and returning 1.0 if empty sequence.
+    """
     factors = [f for f in factors if not is_one_lexpr(f)]
     if len(factors) == 0:
         return LiteralFloat(1.0)
     elif len(factors) == 1:
         return factors[0]
     else:
         for f in factors:
@@ -97,103 +106,114 @@
     These can be REAL (same type as geometry),
     SCALAR (same type as tensor), or INT (for entity indices etc.)
     """
 
     REAL = 0
     SCALAR = 1
     INT = 2
-    NONE = 3
+    BOOL = 3
+    NONE = 4
 
 
-def merge_dtypes(dtype0, dtype1):
-    # Promote dtype to SCALAR or REAL if either argument matches
-    if DataType.NONE in (dtype0, dtype1):
-        raise ValueError(f"Invalid DataType in LNodes {dtype0, dtype1}")
-    if DataType.SCALAR in (dtype0, dtype1):
+def merge_dtypes(dtypes: list[DataType]):
+    """Promote dtype to SCALAR or REAL if either argument matches."""
+    if DataType.NONE in dtypes:
+        raise ValueError(f"Invalid DataType in LNodes {dtypes}")
+    if DataType.SCALAR in dtypes:
         return DataType.SCALAR
-    elif DataType.REAL in (dtype0, dtype1):
+    elif DataType.REAL in dtypes:
         return DataType.REAL
-    elif (dtype0 == DataType.INT and dtype1 == DataType.INT):
+    elif DataType.INT in dtypes:
         return DataType.INT
+    elif DataType.BOOL in dtypes:
+        return DataType.BOOL
     else:
-        raise ValueError(f"Can't get dtype for binary operation with {dtype0, dtype1}")
+        raise ValueError(f"Can't get dtype for operation with {dtypes}")
 
 
-class LNode(object):
+class LNode:
     """Base class for all AST nodes."""
 
     def __eq__(self, other):
-        name = self.__class__.__name__
-        raise NotImplementedError("Missing implementation of __eq__ in " + name)
+        """Check for equality."""
+        return NotImplemented
 
     def __ne__(self, other):
-        return not self.__eq__(other)
+        """Check for inequality."""
+        return NotImplemented
 
 
 class LExpr(LNode):
     """Base class for all expressions.
 
     All subtypes should define a 'precedence' class attribute.
     """
 
     dtype = DataType.NONE
 
     def __getitem__(self, indices):
+        """Get an item."""
         return ArrayAccess(self, indices)
 
     def __neg__(self):
+        """Negate."""
         if isinstance(self, LiteralFloat):
             return LiteralFloat(-self.value)
         if isinstance(self, LiteralInt):
             return LiteralInt(-self.value)
         return Neg(self)
 
     def __add__(self, other):
+        """Add."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return other
         if is_zero_lexpr(other):
             return self
         if isinstance(other, Neg):
             return Sub(self, other.arg)
         return Add(self, other)
 
     def __radd__(self, other):
+        """Add."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return other
         if is_zero_lexpr(other):
             return self
         if isinstance(self, Neg):
             return Sub(other, self.arg)
         return Add(other, self)
 
     def __sub__(self, other):
+        """Subtract."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return -other
         if is_zero_lexpr(other):
             return self
         if isinstance(other, Neg):
             return Add(self, other.arg)
         if isinstance(self, LiteralInt) and isinstance(other, LiteralInt):
             return LiteralInt(self.value - other.value)
         return Sub(self, other)
 
     def __rsub__(self, other):
+        """Subtract."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return other
         if is_zero_lexpr(other):
             return -self
         if isinstance(self, Neg):
             return Add(other, self.arg)
         return Sub(other, self)
 
     def __mul__(self, other):
+        """Multiply."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return self
         if is_zero_lexpr(other):
             return other
         if is_one_lexpr(self):
             return other
@@ -204,14 +224,15 @@
         if is_negative_one_lexpr(self):
             return Neg(other)
         if isinstance(self, LiteralInt) and isinstance(other, LiteralInt):
             return LiteralInt(self.value * other.value)
         return Mul(self, other)
 
     def __rmul__(self, other):
+        """Multiply."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             return self
         if is_zero_lexpr(other):
             return other
         if is_one_lexpr(self):
             return other
@@ -220,22 +241,24 @@
         if is_negative_one_lexpr(other):
             return Neg(self)
         if is_negative_one_lexpr(self):
             return Neg(other)
         return Mul(other, self)
 
     def __div__(self, other):
+        """Divide."""
         other = as_lexpr(other)
         if is_zero_lexpr(other):
             raise ValueError("Division by zero!")
         if is_zero_lexpr(self):
             return self
         return Div(self, other)
 
     def __rdiv__(self, other):
+        """Divide."""
         other = as_lexpr(other)
         if is_zero_lexpr(self):
             raise ValueError("Division by zero!")
         if is_zero_lexpr(other):
             return other
         return Div(other, self)
 
@@ -254,271 +277,339 @@
 
 class LExprTerminal(LExpr):
     """Base class for all  expression terminals."""
 
     sideeffect = False
 
 
-# LExprTerminal types
-
-
 class LiteralFloat(LExprTerminal):
     """A floating point literal value."""
 
     precedence = PRECEDENCE.LITERAL
 
     def __init__(self, value):
+        """Initialise."""
         assert isinstance(value, (float, complex))
         self.value = value
         if isinstance(value, complex):
             self.dtype = DataType.SCALAR
         else:
             self.dtype = DataType.REAL
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, LiteralFloat) and self.value == other.value
 
     def __float__(self):
+        """Convert to float."""
         return float(self.value)
 
     def __repr__(self):
+        """Representation."""
         return str(self.value)
 
 
 class LiteralInt(LExprTerminal):
     """An integer literal value."""
 
     precedence = PRECEDENCE.LITERAL
 
     def __init__(self, value):
+        """Initialise."""
         assert isinstance(value, (int, np.number))
         self.value = value
         self.dtype = DataType.INT
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, LiteralInt) and self.value == other.value
 
     def __hash__(self):
+        """Hash."""
         return hash(self.value)
 
     def __repr__(self):
+        """Representation."""
         return str(self.value)
 
 
 class Symbol(LExprTerminal):
     """A named symbol."""
 
     precedence = PRECEDENCE.SYMBOL
 
     def __init__(self, name: str, dtype):
+        """Initialise."""
         assert isinstance(name, str)
         assert name.replace("_", "").isalnum()
         self.name = name
         self.dtype = dtype
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, Symbol) and self.name == other.name
 
     def __hash__(self):
+        """Hash."""
         return hash(self.name)
 
     def __repr__(self):
+        """Representation."""
         return self.name
 
 
 class MultiIndex(LExpr):
     """A multi-index for accessing tensors flattened in memory."""
 
+    precedence = PRECEDENCE.SYMBOL
+
     def __init__(self, symbols: list, sizes: list):
+        """Initialise."""
         self.dtype = DataType.INT
         self.sizes = sizes
         self.symbols = [as_lexpr(sym) for sym in symbols]
         for sym in self.symbols:
             assert sym.dtype == DataType.INT
 
         dim = len(sizes)
         if dim == 0:
             self.global_index: LExpr = LiteralInt(0)
         else:
             stride = [np.prod(sizes[i:]) for i in range(dim)] + [LiteralInt(1)]
             self.global_index = Sum(n * sym for n, sym in zip(stride[1:], symbols))
 
+    @property
+    def dim(self):
+        """Dimension of the multi-index."""
+        return len(self.sizes)
+
     def size(self):
+        """Size of the multi-index."""
         return np.prod(self.sizes)
 
     def local_index(self, idx):
+        """Get the local index."""
         assert idx < len(self.symbols)
         return self.symbols[idx]
 
     def intersection(self, other):
+        """Get the intersection."""
         symbols = []
         sizes = []
-        for (sym, size) in zip(self.symbols, self.sizes):
+        for sym, size in zip(self.symbols, self.sizes):
             if sym in other.symbols:
                 i = other.symbols.index(sym)
                 assert other.sizes[i] == size
                 symbols.append(sym)
                 sizes.append(size)
         return MultiIndex(symbols, sizes)
 
     def union(self, other):
-        # NB result may depend on order a.union(b) != b.union(a)
+        """Get the union.
+
+        Note:
+            Result may depend on order a.union(b) != b.union(a)
+        """
         symbols = self.symbols.copy()
         sizes = self.sizes.copy()
-        for (sym, size) in zip(other.symbols, other.sizes):
+        for sym, size in zip(other.symbols, other.sizes):
             if sym in symbols:
                 i = symbols.index(sym)
                 assert sizes[i] == size
             else:
                 symbols.append(sym)
                 sizes.append(size)
         return MultiIndex(symbols, sizes)
 
     def difference(self, other):
+        """Get the difference."""
         symbols = []
         sizes = []
-        for (idx, size) in zip(self.symbols, self.sizes):
+        for idx, size in zip(self.symbols, self.sizes):
             if idx not in other.symbols:
                 symbols.append(idx)
                 sizes.append(size)
         return MultiIndex(symbols, sizes)
 
     def __hash__(self):
-        return hash(self.global_idx)
+        """Hash."""
+        return hash(self.global_index.__repr__)
 
 
 class PrefixUnaryOp(LExprOperator):
     """Base class for unary operators."""
 
     def __init__(self, arg):
+        """Initialise."""
         self.arg = as_lexpr(arg)
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, type(self)) and self.arg == other.arg
 
 
 class BinOp(LExprOperator):
+    """A binary operator."""
+
     def __init__(self, lhs, rhs):
+        """Initialise."""
         self.lhs = as_lexpr(lhs)
         self.rhs = as_lexpr(rhs)
 
     def __eq__(self, other):
-        return (
-            isinstance(other, type(self))
-            and self.lhs == other.lhs
-            and self.rhs == other.rhs
-        )
+        """Check equality."""
+        return isinstance(other, type(self)) and self.lhs == other.lhs and self.rhs == other.rhs
 
     def __hash__(self):
+        """Hash."""
         return hash(self.lhs) + hash(self.rhs)
 
     def __repr__(self):
+        """Representation."""
         return f"({self.lhs} {self.op} {self.rhs})"
 
 
 class ArithmeticBinOp(BinOp):
+    """An artithmetic binary operator."""
+
     def __init__(self, lhs, rhs):
+        """Initialise."""
         self.lhs = as_lexpr(lhs)
         self.rhs = as_lexpr(rhs)
-        self.dtype = merge_dtypes(self.lhs.dtype, self.rhs.dtype)
+        self.dtype = merge_dtypes([self.lhs.dtype, self.rhs.dtype])
 
 
 class NaryOp(LExprOperator):
     """Base class for special n-ary operators."""
 
     op = ""
 
     def __init__(self, args):
+        """Initialise."""
         self.args = [as_lexpr(arg) for arg in args]
+        self.dtype = self.args[0].dtype
+        for arg in self.args:
+            self.dtype = merge_dtypes([self.dtype, arg.dtype])
 
     def __eq__(self, other):
+        """Check equality."""
         return (
             isinstance(other, type(self))
             and len(self.args) == len(other.args)
             and all(a == b for a, b in zip(self.args, other.args))
         )
 
     def __repr__(self) -> str:
+        """Representation."""
         return f"{self.op} ".join(f"{i} " for i in self.args)
 
+    def __hash__(self):
+        """Hash."""
+        return hash(tuple(self.args))
+
 
 class Neg(PrefixUnaryOp):
+    """Negation operator."""
+
     precedence = PRECEDENCE.NEG
     op = "-"
 
     def __init__(self, arg):
+        """Initialise."""
         self.arg = as_lexpr(arg)
         self.dtype = self.arg.dtype
 
 
 class Not(PrefixUnaryOp):
+    """Not operator."""
+
     precedence = PRECEDENCE.NOT
     op = "!"
 
 
-# Binary operators
-# Arithmetic operators preserve the dtype of their operands
-# The other operations (logical) do not need a dtype
-
 class Add(ArithmeticBinOp):
+    """Add operator."""
+
     precedence = PRECEDENCE.ADD
     op = "+"
 
 
 class Sub(ArithmeticBinOp):
+    """Subtract operator."""
+
     precedence = PRECEDENCE.SUB
     op = "-"
 
 
 class Mul(ArithmeticBinOp):
+    """Multiply operator."""
+
     precedence = PRECEDENCE.MUL
     op = "*"
 
 
 class Div(ArithmeticBinOp):
+    """Division operator."""
+
     precedence = PRECEDENCE.DIV
     op = "/"
 
 
 class EQ(BinOp):
+    """Equality operator."""
+
     precedence = PRECEDENCE.EQ
     op = "=="
 
 
 class NE(BinOp):
+    """Inequality operator."""
+
     precedence = PRECEDENCE.NE
     op = "!="
 
 
 class LT(BinOp):
+    """Less than operator."""
+
     precedence = PRECEDENCE.LT
     op = "<"
 
 
 class GT(BinOp):
+    """Greater than operator."""
+
     precedence = PRECEDENCE.GT
     op = ">"
 
 
 class LE(BinOp):
+    """Less than or equal to operator."""
+
     precedence = PRECEDENCE.LE
     op = "<="
 
 
 class GE(BinOp):
+    """Greater than or equal to operator."""
+
     precedence = PRECEDENCE.GE
     op = ">="
 
 
 class And(BinOp):
+    """And operator."""
+
     precedence = PRECEDENCE.AND
     op = "&&"
 
 
 class Or(BinOp):
+    """Or operator."""
+
     precedence = PRECEDENCE.OR
     op = "||"
 
 
 class Sum(NaryOp):
     """Sum of any number of operands."""
 
@@ -535,19 +626,21 @@
 
 class MathFunction(LExprOperator):
     """A Math Function, with any arguments."""
 
     precedence = PRECEDENCE.HIGHEST
 
     def __init__(self, func, args):
+        """Initialise."""
         self.function = func
         self.args = [as_lexpr(arg) for arg in args]
         self.dtype = self.args[0].dtype
 
     def __eq__(self, other):
+        """Check equality."""
         return (
             isinstance(other, type(self))
             and self.function == other.function
             and len(self.args) == len(other.args)
             and all(a == b for a, b in zip(self.args, other.args))
         )
 
@@ -555,51 +648,65 @@
 class AssignOp(BinOp):
     """Base class for assignment operators."""
 
     precedence = PRECEDENCE.ASSIGN
     sideeffect = True
 
     def __init__(self, lhs, rhs):
+        """Initialise."""
         assert isinstance(lhs, LNode)
         BinOp.__init__(self, lhs, rhs)
 
 
 class Assign(AssignOp):
+    """Assign operator."""
+
     op = "="
 
 
 class AssignAdd(AssignOp):
+    """Assign add operator."""
+
     op = "+="
 
 
 class AssignSub(AssignOp):
+    """Assign subtract operator."""
+
     op = "-="
 
 
 class AssignMul(AssignOp):
+    """Assign multiply operator."""
+
     op = "*="
 
 
 class AssignDiv(AssignOp):
+    """Assign division operator."""
+
     op = "/="
 
 
 class ArrayAccess(LExprOperator):
+    """Array access."""
+
     precedence = PRECEDENCE.SUBSCRIPT
 
     def __init__(self, array, indices):
+        """Initialise."""
         # Typecheck array argument
         if isinstance(array, Symbol):
             self.array = array
             self.dtype = array.dtype
         elif isinstance(array, ArrayDecl):
             self.array = array.symbol
             self.dtype = array.symbol.dtype
         else:
-            raise ValueError("Unexpected array type %s." % (type(array).__name__,))
+            raise ValueError(f"Unexpected array type {type(array).__name__}")
 
         # Allow expressions or literals as indices
         if not isinstance(indices, (list, tuple)):
             indices = (indices,)
         self.indices = tuple(as_lexpr(i) for i in indices)
 
         # Early error checking for negative array dimensions
@@ -622,37 +729,44 @@
         if isinstance(indices, list):
             indices = tuple(indices)
         elif not isinstance(indices, tuple):
             indices = (indices,)
         return ArrayAccess(self.array, self.indices + indices)
 
     def __eq__(self, other):
+        """Check equality."""
         return (
             isinstance(other, type(self))
             and self.array == other.array
             and self.indices == other.indices
         )
 
     def __hash__(self):
+        """Hash."""
         return hash(self.array)
 
     def __repr__(self):
+        """Representation."""
         return str(self.array) + "[" + ", ".join(str(i) for i in self.indices) + "]"
 
 
 class Conditional(LExprOperator):
+    """Conditional."""
+
     precedence = PRECEDENCE.CONDITIONAL
 
     def __init__(self, condition, true, false):
+        """Initialise."""
         self.condition = as_lexpr(condition)
         self.true = as_lexpr(true)
         self.false = as_lexpr(false)
-        self.dtype = merge_dtypes(self.true.dtype, self.false.dtype)
+        self.dtype = merge_dtypes([self.true.dtype, self.false.dtype])
 
     def __eq__(self, other):
+        """Check equality."""
         return (
             isinstance(other, type(self))
             and self.condition == other.condition
             and self.true == other.true
             and self.false == other.false
         )
 
@@ -666,28 +780,32 @@
     if isinstance(node, LExpr):
         return node
     elif isinstance(node, numbers.Integral):
         return LiteralInt(node)
     elif isinstance(node, numbers.Real):
         return LiteralFloat(node)
     else:
-        raise RuntimeError("Unexpected LExpr type %s:\n%s" % (type(node), str(node)))
+        raise RuntimeError(f"Unexpected LExpr type {type(node)}:\n{node}")
 
 
 class Statement(LNode):
     """Make an expression into a statement."""
 
-    is_scoped = False
-
     def __init__(self, expr):
+        """Initialise."""
         self.expr = as_lexpr(expr)
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, type(self)) and self.expr == other.expr
 
+    def __hash__(self) -> int:
+        """Hash."""
+        return hash(self.expr)
+
 
 def as_statement(node):
     """Perform type checking on node and wrap in a suitable statement type if necessary."""
     if isinstance(node, StatementList) and len(node.statements) == 1:
         # Cleans up the expression tree a bit
         return node.statements[0]
     elif isinstance(node, Statement):
@@ -695,54 +813,119 @@
         return node
     elif isinstance(node, LExprOperator):
         if node.sideeffect:
             # Special case for using assignment expressions as statements
             return Statement(node)
         else:
             raise RuntimeError(
-                "Trying to create a statement of lexprOperator type %s:\n%s"
-                % (type(node), str(node))
+                f"Trying to create a statement of lexprOperator type {type(node)}:\n{node}"
             )
+
     elif isinstance(node, list):
         # Convenience case for list of statements
         if len(node) == 1:
             # Cleans up the expression tree a bit
             return as_statement(node[0])
         else:
             return StatementList(node)
+    elif isinstance(node, Section):
+        return node
     else:
-        raise RuntimeError(
-            "Unexpected Statement type %s:\n%s" % (type(node), str(node))
+        raise RuntimeError(f"Unexpected Statement type {type(node)}:\n{node}")
+
+
+class Annotation(Enum):
+    """Annotation."""
+
+    fuse = 1  # fuse loops in section
+    unroll = 2  # unroll loop in section
+    licm = 3  # loop invariant code motion
+    factorize = 4  # apply sum factorization
+
+
+class Declaration(Statement):
+    """Base class for all declarations."""
+
+    def __init__(self, symbol):
+        """Initialise."""
+        self.symbol = symbol
+
+    def __eq__(self, other):
+        """Check equality."""
+        return isinstance(other, type(self)) and self.symbol == other.symbol
+
+
+def is_declaration(node) -> bool:
+    """Check if a node is a declaration."""
+    return isinstance(node, VariableDecl) or isinstance(node, ArrayDecl)
+
+
+class Section(LNode):
+    """A section of code with a name and a list of statements."""
+
+    def __init__(
+        self,
+        name: str,
+        statements: list[LNode],
+        declarations: Sequence[Declaration],
+        input: Optional[list[Symbol]] = None,
+        output: Optional[list[Symbol]] = None,
+        annotations: Optional[list[Annotation]] = None,
+    ):
+        """Initialise."""
+        self.name = name
+        self.statements = [as_statement(st) for st in statements]
+        self.annotations = annotations or []
+        self.input = input or []
+        self.declarations = declarations or []
+        self.output = output or []
+
+        for decl in self.declarations:
+            assert is_declaration(decl)
+            if decl.symbol not in self.output:
+                self.output.append(decl.symbol)
+
+    def __eq__(self, other):
+        """Check equality."""
+        attributes = ("name", "input", "output", "annotations", "statements")
+        return isinstance(other, type(self)) and all(
+            getattr(self, name) == getattr(other, name) for name in attributes
         )
 
 
 class StatementList(LNode):
-    """A simple sequence of statements. No new scopes are introduced."""
+    """A simple sequence of statements."""
 
     def __init__(self, statements):
+        """Initialise."""
         self.statements = [as_statement(st) for st in statements]
 
-    @property
-    def is_scoped(self):
-        return all(st.is_scoped for st in self.statements)
-
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, type(self)) and self.statements == other.statements
 
+    def __hash__(self) -> int:
+        """Hash."""
+        return hash(tuple(self.statements))
+
+    def __repr__(self):
+        """Representation."""
+        return f"StatementList({self.statements})"
+
 
 class Comment(Statement):
     """Line comment(s) used for annotating the generated code with human readable remarks."""
 
-    is_scoped = True
-
     def __init__(self, comment):
+        """Initialise."""
         assert isinstance(comment, str)
         self.comment = comment
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, type(self)) and self.comment == other.comment
 
 
 def commented_code_list(code, comments):
     """Add comment to code list if the list is not empty."""
     if isinstance(code, LNode):
         code = [code]
@@ -754,52 +937,50 @@
         code = comments + code
     return code
 
 
 # Type and variable declarations
 
 
-class VariableDecl(Statement):
+class VariableDecl(Declaration):
     """Declare a variable, optionally define initial value."""
 
-    is_scoped = False
-
     def __init__(self, symbol, value=None):
-
+        """Initialise."""
         assert isinstance(symbol, Symbol)
         assert symbol.dtype is not None
         self.symbol = symbol
 
         if value is not None:
             value = as_lexpr(value)
         self.value = value
 
     def __eq__(self, other):
+        """Check equality."""
         return (
             isinstance(other, type(self))
             and self.typename == other.typename
             and self.symbol == other.symbol
             and self.value == other.value
         )
 
 
-class ArrayDecl(Statement):
+class ArrayDecl(Declaration):
     """A declaration or definition of an array.
 
     Note that just setting values=0 is sufficient to initialize the
     entire array to zero.
 
     Otherwise use nested lists of lists to represent multidimensional
     array values to initialize to.
 
     """
 
-    is_scoped = False
-
     def __init__(self, symbol, sizes=None, values=None, const=False):
+        """Initialise."""
         assert isinstance(symbol, Symbol)
         self.symbol = symbol
         assert symbol.dtype
 
         if sizes is None:
             assert values is not None
             sizes = values.shape
@@ -813,51 +994,76 @@
         # NB! No type checking, assuming nested lists of literal values. Not applying as_lexpr.
         if isinstance(values, (list, tuple)):
             self.values = np.asarray(values)
         else:
             self.values = values
 
         self.const = const
+        self.dtype = symbol.dtype
 
     def __eq__(self, other):
-        attributes = ("typename", "symbol", "sizes", "values")
+        """Check equality."""
+        attributes = ("dtype", "symbol", "sizes", "values")
         return isinstance(other, type(self)) and all(
             getattr(self, name) == getattr(self, name) for name in attributes
         )
 
+    def __hash__(self) -> int:
+        """Hash."""
+        return hash(self.symbol)
+
 
 def is_simple_inner_loop(code):
+    """Check if code is a simple inner loop."""
     if isinstance(code, ForRange) and is_simple_inner_loop(code.body):
         return True
     if isinstance(code, Statement) and isinstance(code.expr, AssignOp):
         return True
     return False
 
 
+def depth(code) -> int:
+    """Get depth of code."""
+    if isinstance(code, ForRange):
+        return 1 + depth(code.body)
+    if isinstance(code, StatementList):
+        return max([depth(c) for c in code.statements])
+    return 0
+
+
 class ForRange(Statement):
     """Slightly higher-level for loop assuming incrementing an index over a range."""
 
-    is_scoped = True
-
     def __init__(self, index, begin, end, body):
-        assert isinstance(index, Symbol)
+        """Initialise."""
+        assert isinstance(index, Symbol) or isinstance(index, MultiIndex)
         self.index = index
         self.begin = as_lexpr(begin)
         self.end = as_lexpr(end)
         assert isinstance(body, list)
         self.body = StatementList(body)
 
+    def as_tuple(self):
+        """Convert to a tuple."""
+        return (self.index, self.begin, self.end, self.body)
+
     def __eq__(self, other):
+        """Check equality."""
         attributes = ("index", "begin", "end", "body")
         return isinstance(other, type(self)) and all(
             getattr(self, name) == getattr(self, name) for name in attributes
         )
 
+    def __hash__(self) -> int:
+        """Hash."""
+        return hash(self.as_tuple())
+
 
 def _math_function(op, *args):
+    """Get a math function."""
     name = op._ufl_handler_name_
     dtype = args[0].dtype
     if name in ("conj", "real") and dtype == DataType.REAL:
         assert len(args) == 1
         return args[0]
     if name == "imag" and dtype == DataType.REAL:
         assert len(args) == 1
@@ -904,17 +1110,32 @@
     ufl.mathfunctions.Acos: _math_function,
     ufl.mathfunctions.Asin: _math_function,
     ufl.mathfunctions.Atan: _math_function,
     ufl.mathfunctions.Erf: _math_function,
     ufl.mathfunctions.Atan2: _math_function,
     ufl.mathfunctions.MathFunction: _math_function,
     ufl.mathfunctions.BesselJ: _math_function,
-    ufl.mathfunctions.BesselY: _math_function}
+    ufl.mathfunctions.BesselY: _math_function,
+}
 
 
 def ufl_to_lnodes(operator, *args):
-    # Call appropriate handler, depending on the type of operator
+    """Call appropriate handler, depending on the type of operator."""
     optype = type(operator)
     if optype in _ufl_call_lookup:
         return _ufl_call_lookup[optype](operator, *args)
     else:
         raise RuntimeError(f"Missing lookup for expr type {optype}.")
+
+
+def create_nested_for_loops(indices: list[MultiIndex], body):
+    """Create nested for loops over list of indices.
+
+    The depth of the nested for loops is equal to the sub-indices for all
+    MultiIndex combined.
+    """
+    ranges = [r for idx in indices for r in idx.sizes]
+    indices = [idx.local_index(i) for idx in indices for i in range(len(idx.sizes))]
+    depth = len(ranges)
+    for i in reversed(range(depth)):
+        body = ForRange(indices[i], 0, ranges[i], body=[body])
+    return body
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/symbols.py` & `fenics_ffcx-0.8.0/ffcx/codegeneration/symbols.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# Copyright (C) 2011-2017 Martin Sandve Alnæs
+# Copyright (C) 2011-2023 Martin Sandve Alnæs, Igor A. Baratta
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """FFCx/UFC specific symbol naming."""
 
 import logging
+
 import ufl
+
 import ffcx.codegeneration.lnodes as L
 
 logger = logging.getLogger("ffcx")
 
 
-# TODO: Get restriction postfix from somewhere central
 def ufcx_restriction_postfix(restriction):
+    """Get restriction postfix."""
+    # TODO: Get restriction postfix from somewhere central
     if restriction == "+":
         res = "_0"
     elif restriction == "-":
         res = "_1"
     else:
         res = ""
     return res
@@ -54,19 +57,19 @@
     if mt.component:
         comp = f"_c{mt.flat_component}"
         access += comp
 
     return access
 
 
-class FFCXBackendSymbols(object):
+class FFCXBackendSymbols:
     """FFCx specific symbol definitions. Provides non-ufl symbols."""
 
-    def __init__(self, coefficient_numbering, coefficient_offsets,
-                 original_constant_offsets):
+    def __init__(self, coefficient_numbering, coefficient_offsets, original_constant_offsets):
+        """Initialise."""
         self.coefficient_numbering = coefficient_numbering
         self.coefficient_offsets = coefficient_offsets
 
         self.original_constant_offsets = original_constant_offsets
 
         # Keep tabs on tables, so the symbols can be reused
         self.quadrature_weight_tables = {}
@@ -105,24 +108,25 @@
                 return self.entity_local_index[0]
         elif entitytype == "vertex":
             return self.entity_local_index[0]
         else:
             logging.exception(f"Unknown entitytype {entitytype}")
 
     def argument_loop_index(self, iarg):
-        """Loop index for argument #iarg."""
+        """Loop index for argument iarg."""
         indices = ["i", "j", "k", "l"]
         return L.Symbol(indices[iarg], dtype=L.DataType.INT)
 
     def weights_table(self, quadrature_rule):
         """Table of quadrature weights."""
         key = f"weights_{quadrature_rule.id()}"
         if key not in self.quadrature_weight_tables:
-            self.quadrature_weight_tables[key] = L.Symbol(f"weights_{quadrature_rule.id()}",
-                                                          dtype=L.DataType.REAL)
+            self.quadrature_weight_tables[key] = L.Symbol(
+                f"weights_{quadrature_rule.id()}", dtype=L.DataType.REAL
+            )
         return self.quadrature_weight_tables[key]
 
     def points_table(self, quadrature_rule):
         """Table of quadrature points (points on the reference integration entity)."""
         return L.Symbol(f"points_{quadrature_rule.id()}", dtype=L.DataType.REAL)
 
     def x_component(self, mt):
@@ -131,52 +135,52 @@
 
     def J_component(self, mt):
         """Jacobian component."""
         # FIXME: Add domain number!
         return L.Symbol(format_mt_name("J", mt), dtype=L.DataType.REAL)
 
     def domain_dof_access(self, dof, component, gdim, num_scalar_dofs, restriction):
+        """Domain DOF access."""
         # FIXME: Add domain number or offset!
         offset = 0
         if restriction == "-":
             offset = num_scalar_dofs * 3
         return self.coordinate_dofs[3 * dof + component + offset]
 
-    def domain_dofs_access(self, gdim, num_scalar_dofs, restriction):
-        # FIXME: Add domain number or offset!
-        return [
-            self.domain_dof_access(dof, component, gdim, num_scalar_dofs, restriction)
-            for dof in range(num_scalar_dofs) for component in range(gdim)
-        ]
-
     def coefficient_dof_access(self, coefficient, dof_index):
+        """Coefficient DOF access."""
         offset = self.coefficient_offsets[coefficient]
         w = self.coefficients
         return w[offset + dof_index]
 
-    def coefficient_dof_access_blocked(self, coefficient: ufl.Coefficient, index,
-                                       block_size, dof_offset):
+    def coefficient_dof_access_blocked(
+        self, coefficient: ufl.Coefficient, index, block_size, dof_offset
+    ):
+        """Blocked coefficient DOF access."""
         coeff_offset = self.coefficient_offsets[coefficient]
         w = self.coefficients
         _w = L.Symbol(f"_w_{coeff_offset}_{dof_offset}", dtype=L.DataType.SCALAR)
         unit_stride_access = _w[index]
         original_access = w[coeff_offset + index * block_size + dof_offset]
         return unit_stride_access, original_access
 
     def coefficient_value(self, mt):
         """Symbol for variable holding value or derivative component of coefficient."""
         c = self.coefficient_numbering[mt.terminal]
-        return L.Symbol(format_mt_name("w%d" % (c, ), mt), dtype=L.DataType.SCALAR)
+        return L.Symbol(format_mt_name("w%d" % (c,), mt), dtype=L.DataType.SCALAR)
 
     def constant_index_access(self, constant, index):
+        """Constant index access."""
         offset = self.original_constant_offsets[constant]
         c = self.constants
         return c[offset + index]
 
+    # TODO: Remove this, use table_access instead
     def element_table(self, tabledata, entitytype, restriction):
+        """Get an element table."""
         entity = self.entity(entitytype, restriction)
 
         if tabledata.is_uniform:
             entity = 0
         else:
             entity = self.entity(entitytype, restriction)
 
@@ -190,10 +194,9 @@
             if restriction == "-":
                 qp = self.quadrature_permutation[1]
         else:
             qp = 0
 
         # Return direct access to element table, reusing symbol if possible
         if tabledata.name not in self.element_tables:
-            self.element_tables[tabledata.name] = L.Symbol(tabledata.name,
-                                                           dtype=L.DataType.REAL)
+            self.element_tables[tabledata.name] = L.Symbol(tabledata.name, dtype=L.DataType.REAL)
         return self.element_tables[tabledata.name][qp][entity][iq]
```

### Comparing `fenics-ffcx-0.7.0/ffcx/codegeneration/ufcx.h` & `fenics_ffcx-0.8.0/ffcx/codegeneration/ufcx.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 /// This is UFCx
-/// This code is released into the public domain.
+/// This software is released under the terms of the unlicense (see the file
+/// UNLICENSE).
 ///
 /// The FEniCS Project (http://www.fenicsproject.org/) 2006-2021.
 ///
 /// UFCx defines the interface between code generated by FFCx and the
 /// DOLFINx C++ library. Changes here must be reflected both in the FFCx
 /// code generation and in the DOLFINx library calls.
 
 #pragma once
 
 #define UFCX_VERSION_MAJOR 0
-#define UFCX_VERSION_MINOR 7
+#define UFCX_VERSION_MINOR 8
 #define UFCX_VERSION_MAINTENANCE 0
 #define UFCX_VERSION_RELEASE 1
 
 #if UFCX_VERSION_RELEASE
 #define UFCX_VERSION                                                            \
   UFCX_VERSION_MAJOR "." UFCX_VERSION_MINOR "." UFCX_VERSION_MAINTENANCE
 #else
@@ -67,14 +68,15 @@
     ufcx_basix_custom_element = 3,
     ufcx_real_element = 4,
   } ufcx_element_type;
 
   /// Forward declarations
   typedef struct ufcx_finite_element ufcx_finite_element;
   typedef struct ufcx_basix_custom_finite_element ufcx_basix_custom_finite_element;
+  typedef struct ufcx_quadrature_rule ufcx_quadrature_rule;
   typedef struct ufcx_dofmap ufcx_dofmap;
   typedef struct ufcx_function_space ufcx_function_space;
 
   // </HEADER_DECL>
 
   typedef struct ufcx_finite_element
   {
@@ -86,48 +88,36 @@
 
     /// Element type
     ufcx_element_type element_type;
 
     /// Topological dimension of the cell
     int topological_dimension;
 
-    /// Geometric dimension of the cell
-    int geometric_dimension;
-
     /// Dimension of the finite element function space
     int space_dimension;
 
-    /// Rank of the value space
-    int value_rank;
-
-    /// Dimension of the value space for axis i
-    int* value_shape;
-
-    /// Number of components of the value space
-    int value_size;
-
     /// Rank of the reference value space
     int reference_value_rank;
 
     /// Dimension of the reference value space for axis i
     int* reference_value_shape;
 
     /// Number of components of the reference value space
     int reference_value_size;
 
     /// Maximum polynomial degree of the finite element function space
     int degree;
 
+    /// Is the value a symmetric 2-tensor
+    bool symmetric;
+
     /// Block size for a VectorElement. For a TensorElement, this is the
     /// product of the tensor's dimensions
     int block_size;
 
-    /// Family of the finite element function space
-    const char* family;
-
     /// Basix identifier of the family of the finite element function space
     int basix_family;
 
     /// Basix identifier of the cell shape
     int basix_cell;
 
     /// Indicates whether or not this is the discontinuous version of the element
@@ -144,14 +134,17 @@
 
     /// Get a finite element for sub element i (for a mixed
     /// element).
     ufcx_finite_element** sub_elements;
 
     /// Pointer to data to recreate the element if it is a custom Basix element
     ufcx_basix_custom_finite_element* custom_element;
+
+    /// Pointer to data to recreate the custom quadrature rule if the element has one
+    ufcx_quadrature_rule* custom_quadrature;
   } ufcx_finite_element;
 
   typedef struct ufcx_basix_custom_finite_element
   {
     /// Basix identifier of the cell shape
     int cell_type;
 
@@ -189,29 +182,46 @@
     /// The Sobolev space for the element
     int sobolev_space;
 
     /// Indicates whether or not this is the discontinuous version of the element
     bool discontinuous;
 
     /// The highest degree full polynomial space contained in this element
-    int highest_complete_degree;
+    int embedded_subdegree;
 
     /// The number of derivatives needed when interpolating
     int interpolation_nderivs;
 
     /// The highest degree of a polynomial in the element
-    int highest_degree;
+    int embedded_superdegree;
 
     /// The polyset type of the element
     int polyset_type;
   } ufcx_basix_custom_finite_element;
 
-  typedef struct ufcx_dofmap
+  typedef struct ufcx_quadrature_rule
   {
+    /// Cell shape
+    ufcx_shape cell_shape;
+
+    /// The number of points
+    int npts;
 
+    /// The topological dimension of the cell
+    int topological_dimension;
+
+    /// The quadraute points
+    double* points;
+
+    /// The quadraute weights
+    double* weights;
+  } ufcx_quadrature_rule;
+
+  typedef struct ufcx_dofmap
+  {
     /// String identifying the dofmap
     const char* signature;
 
     /// Number of dofs with global support (i.e. global constants)
     int num_global_support_dofs;
 
     /// Dimension of the local finite element function space for a cell
@@ -229,26 +239,14 @@
 
     /// Flattened list of closure dofs associated with each entity
     int *entity_closure_dofs;
 
     /// Offset for closure dofs of each entity in entity_closure_dofs
     int *entity_closure_dof_offsets;
 
-    /// Number of dofs associated with each cell entity of dimension d
-    int *num_entity_dofs;
-
-    /// Tabulate the local-to-local mapping of dofs on entity (d, i)
-    void (*tabulate_entity_dofs)(int* restrict dofs, int d, int i);
-
-    /// Number of dofs associated with the closure of each cell entity of dimension d
-    int *num_entity_closure_dofs;
-
-    /// Tabulate the local-to-local mapping of dofs on the closure of entity (d, i)
-    void (*tabulate_entity_closure_dofs)(int* restrict dofs, int d, int i);
-
     /// Number of sub dofmaps (for a mixed element)
     int num_sub_dofmaps;
 
     /// Get a dofmap for sub dofmap i (for a mixed element)
     ufcx_dofmap** sub_dofmaps;
 
   } ufcx_dofmap;
@@ -298,24 +296,14 @@
   typedef void(ufcx_tabulate_tensor_float64)(
       double* restrict A, const double* restrict w,
       const double* restrict c, const double* restrict coordinate_dofs,
       const int* restrict entity_local_index,
       const uint8_t* restrict quadrature_permutation);
 
   /// Tabulate integral into tensor A with compiled
-  /// quadrature rule and extended double precision
-  ///
-  /// @see ufcx_tabulate_tensor_single
-  typedef void(ufcx_tabulate_tensor_longdouble)(
-      long double* restrict A, const long double* restrict w,
-      const long double* restrict c, const long double* restrict coordinate_dofs,
-      const int* restrict entity_local_index,
-      const uint8_t* restrict quadrature_permutation);
-
-  /// Tabulate integral into tensor A with compiled
   /// quadrature rule and complex single precision
   ///
   /// @see ufcx_tabulate_tensor_single
   typedef void(ufcx_tabulate_tensor_complex64)(
       float _Complex* restrict A, const float _Complex* restrict w,
       const float _Complex* restrict c, const float* restrict coordinate_dofs,
       const int* restrict entity_local_index,
@@ -332,15 +320,14 @@
       const uint8_t* restrict quadrature_permutation);
 
   typedef struct ufcx_integral
   {
     const bool* enabled_coefficients;
     ufcx_tabulate_tensor_float32* tabulate_tensor_float32;
     ufcx_tabulate_tensor_float64* tabulate_tensor_float64;
-    ufcx_tabulate_tensor_longdouble* tabulate_tensor_longdouble;
     ufcx_tabulate_tensor_complex64* tabulate_tensor_complex64;
     ufcx_tabulate_tensor_complex128* tabulate_tensor_complex128;
     bool needs_facet_permutations;
 
     /// Get the coordinate element associated with the geometry of the mesh.
     ufcx_finite_element* coordinate_element;
   } ufcx_integral;
@@ -352,15 +339,14 @@
     /// @param[out] A
     ///         Dimensions: A[num_points][num_components][num_argument_dofs]
     ///
     /// @see ufcx_tabulate_tensor
     ///
     ufcx_tabulate_tensor_float32* tabulate_tensor_float32;
     ufcx_tabulate_tensor_float64* tabulate_tensor_float64;
-    ufcx_tabulate_tensor_longdouble* tabulate_tensor_longdouble;
     ufcx_tabulate_tensor_complex64* tabulate_tensor_complex64;
     ufcx_tabulate_tensor_complex128* tabulate_tensor_complex128;
 
     /// Number of coefficients
     int num_coefficients;
 
     /// Number of constants
@@ -374,20 +360,19 @@
 
     /// List of names of constants
     const char** constant_names;
 
     /// Number of evaluation points
     int num_points;
 
-    /// Dimension of evaluation point, i.e. topological dimension of
-    /// reference cell
-    int topological_dimension;
+    /// Dimension of evaluation point
+    int entity_dimension;
 
     /// Coordinates of evaluations points. Dimensions:
-    /// points[num_points][topological_dimension]
+    /// points[num_points][entity_dimension]
     const double* points;
 
     /// Shape of expression. Dimension: value_shape[num_components]
     const int* value_shape;
 
     /// Number of components of return_shape
     int num_components;
@@ -431,19 +416,19 @@
 
     /// Number of constants
     int num_constants;
 
     /// Original coefficient position for each coefficient
     int* original_coefficient_position;
 
-    /// Return list of names of coefficients
-    const char** (*coefficient_name_map)(void);
+    /// List of names of coefficients
+    const char** coefficient_name_map;
 
-    /// Return list of names of constants
-    const char** (*constant_name_map)(void);
+    /// List of names of constants
+    const char** constant_name_map;
 
     /// Get a finite element for the i-th argument function, where 0 <=
     /// i < r + n.
     ///
     /// @param i Argument number if 0 <= i < r Coefficient number j = i
     /// - r if r + j <= i < r + n
     ufcx_finite_element** finite_elements;
@@ -480,13 +465,19 @@
     int geometry_degree;
 
     /// The Basix cell of the finite element for the geometry map
     int geometry_basix_cell;
 
     /// The Basix variant of the finite element for the geometry map
     int geometry_basix_variant;
+
+    /// Rank of the value space
+    int value_rank;
+
+    /// Shape of the value space
+    int* value_shape;
   } ufcx_function_space;
 
 #ifdef __cplusplus
 #undef restrict
 }
 #endif
```

### Comparing `fenics-ffcx-0.7.0/ffcx/compiler.py` & `fenics_ffcx-0.8.0/ffcx/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,57 +59,68 @@
 
    This stage examines the generated C++ code and formats it according
    to the UFC format, generating as output one or more .h/.c files
    conforming to the UFC format.
 
 """
 
+from __future__ import annotations
+
 import logging
 import typing
 from time import time
 
+import numpy.typing as npt
+
 from ffcx.analysis import analyze_ufl_objects
 from ffcx.codegeneration.codegeneration import generate_code
 from ffcx.formatting import format_code
 from ffcx.ir.representation import compute_ir
 
 logger = logging.getLogger("ffcx")
 
 
 def _print_timing(stage: int, timing: float):
     logger.info(f"Compiler stage {stage} finished in {timing:.4f} seconds.")
 
 
-def compile_ufl_objects(ufl_objects: typing.List[typing.Any],
-                        object_names: typing.Dict = {},
-                        prefix: typing.Optional[str] = None,
-                        options: typing.Dict = {},
-                        visualise: bool = False):
+def compile_ufl_objects(
+    ufl_objects: list[typing.Any],
+    options: dict[str, int | float | npt.DTypeLike],
+    object_names: dict[int, str] | None = None,
+    prefix: str | None = None,
+    visualise: bool = False,
+) -> tuple[str, str]:
     """Generate UFC code for a given UFL objects.
 
-    Options
-    ----------
-    @param ufl_objects:
-        Objects to be compiled. Accepts elements, forms, integrals or coordinate mappings.
-
+    Args:
+        ufl_objects: Objects to be compiled. Accepts elements, forms,
+          integrals or coordinate mappings.
+        object_names: Map from object Python id to object name
+        prefix: Prefix
+        options: Options
+        visualise: Toggle visualisation
     """
+    _object_names = object_names if object_names is not None else {}
+    _prefix = prefix if prefix is not None else ""
+
     # Stage 1: analysis
     cpu_time = time()
-    analysis = analyze_ufl_objects(ufl_objects, options)
+    analysis = analyze_ufl_objects(ufl_objects, options["scalar_type"])  # type: ignore
     _print_timing(1, time() - cpu_time)
 
     # Stage 2: intermediate representation
     cpu_time = time()
-    ir = compute_ir(analysis, object_names, prefix, options, visualise)
+    ir = compute_ir(analysis, _object_names, _prefix, options, visualise)
     _print_timing(2, time() - cpu_time)
 
     # Stage 3: code generation
     cpu_time = time()
     code = generate_code(ir, options)
     _print_timing(3, time() - cpu_time)
 
     # Stage 4: format code
     cpu_time = time()
-    code_h, code_c = format_code(code, options)
+    code_h, code_c = format_code(code)
     _print_timing(4, time() - cpu_time)
 
     return code_h, code_c
```

### Comparing `fenics-ffcx-0.7.0/ffcx/formatting.py` & `fenics_ffcx-0.8.0/ffcx/formatting.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 dictionary of generated C++ code for the body of each UFC function.
 
 It relies on templates for UFC code available as part of the module
 ufcx_utils.
 
 """
 
+from __future__ import annotations
+
 import logging
 import os
 
+from ffcx.codegeneration.codegeneration import CodeBlocks
+
 logger = logging.getLogger("ffcx")
 
 
-def format_code(code, options: dict):
+def format_code(code: CodeBlocks) -> tuple[str, str]:
     """Format given code in UFC format. Returns two strings with header and source file contents."""
     logger.info(79 * "*")
     logger.info("Compiler stage 5: Formatting code")
     logger.info(79 * "*")
 
     code_c = ""
     code_h = ""
@@ -31,14 +35,15 @@
         code_h += "".join([c[0] for c in parts_code])
         code_c += "".join([c[1] for c in parts_code])
 
     return code_h, code_c
 
 
 def write_code(code_h, code_c, prefix, output_dir):
+    """Write code to files."""
     _write_file(code_h, prefix, ".h", output_dir)
     _write_file(code_c, prefix, ".c", output_dir)
 
 
 def _write_file(output, prefix, postfix, output_dir):
     """Write generated code to file."""
     filename = os.path.join(output_dir, prefix + postfix)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/factorization.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/factorization.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,38 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Algorithms for factorizing argument dependent monomials."""
 
 import logging
 from functools import singledispatch
 
-from ffcx.ir.analysis.graph import ExpressionGraph
-from ffcx.ir.analysis.modified_terminals import (analyse_modified_terminal,
-                                                 strip_modified_terminal)
 from ufl import as_ufl, conditional
-from ufl.classes import (Argument, Conditional, Conj, Division, Product, Sum,
-                         Zero)
+from ufl.classes import Argument, Conditional, Conj, Division, Product, Sum, Zero
+
+from ffcx.ir.analysis.graph import ExpressionGraph
+from ffcx.ir.analysis.modified_terminals import analyse_modified_terminal, strip_modified_terminal
 
 logger = logging.getLogger("ffcx")
 
 
 def build_argument_indices(S):
     """Build ordered list of indices to modified arguments."""
     arg_indices = []
     for i, v in S.nodes.items():
-        arg = strip_modified_terminal(v['expression'])
+        arg = strip_modified_terminal(v["expression"])
         if isinstance(arg, Argument):
             arg_indices.append(i)
 
     # Make a canonical ordering of vertex indices for modified arguments
     def arg_ordering_key(i):
         """Return a key for sorting argument vertex indices.
 
         Key is based on the properties of the modified terminal.
         """
-        mt = analyse_modified_terminal(S.nodes[i]['expression'])
+        mt = analyse_modified_terminal(S.nodes[i]["expression"])
         return mt.argument_ordering_key()
 
     ordered_arg_indices = sorted(arg_indices, key=arg_ordering_key)
     return ordered_arg_indices
 
 
 def graph_insert(F, expr):
@@ -51,25 +50,28 @@
 
 # Reuse these empty objects where appropriate to save memory
 noargs = {}  # type: ignore
 
 
 @singledispatch
 def handler(v, fac, sf, F):
+    """Handler."""
     # Error checking
     if any(fac):
         raise RuntimeError(
-            "Assuming that a {0} cannot be applied to arguments. If this is wrong please report a bug.".
-            format(type(v)))
+            f"Assuming that a {type(v)} cannot be applied to arguments. "
+            "If this is wrong please report a bug."
+        )
     # Record non-argument subexpression
     raise RuntimeError("No arguments")
 
 
 @handler.register(Sum)
 def handle_sum(v, fac, sf, F):
+    """Handle a sum."""
     if len(fac) != 2:
         raise RuntimeError("Assuming binary sum here. This can be fixed if needed.")
 
     fac0 = fac[0]
     fac1 = fac[1]
     argkeys = set(fac0) | set(fac1)
 
@@ -84,101 +86,104 @@
             fi0 = fac0.get(argkey)
             fi1 = fac1.get(argkey)
             if fi0 is None:
                 fisum = fi1
             elif fi1 is None:
                 fisum = fi0
             else:
-                f0 = F.nodes[fi0]['expression']
-                f1 = F.nodes[fi1]['expression']
+                f0 = F.nodes[fi0]["expression"]
+                f1 = F.nodes[fi1]["expression"]
                 fisum = graph_insert(F, f0 + f1)
             factors[argkey] = fisum
 
     else:  # non-arg + non-arg
         raise RuntimeError("No arguments")
 
     return factors
 
 
 @handler.register(Product)
 def handle_product(v, fac, sf, F):
+    """Handle a product."""
     if len(fac) != 2:
         raise RuntimeError("Assuming binary product here. This can be fixed if needed.")
     fac0 = fac[0]
     fac1 = fac[1]
 
     if not fac0 and not fac1:  # non-arg * non-arg
         raise RuntimeError("No arguments")
 
     elif not fac0:  # non-arg * arg
         # Record products of non-arg operand with each factor of arg-dependent operand
         f0 = sf[0]
         factors = {}
         for k1 in sorted(fac1):
-            f1 = F.nodes[fac1[k1]]['expression']
+            f1 = F.nodes[fac1[k1]]["expression"]
             factors[k1] = graph_insert(F, f0 * f1)
 
     elif not fac1:  # arg * non-arg
         # Record products of non-arg operand with each factor of arg-dependent operand
         f1 = sf[1]
         factors = {}
         for k0 in sorted(fac0):
-            f0 = F.nodes[fac0[k0]]['expression']
+            f0 = F.nodes[fac0[k0]]["expression"]
             factors[k0] = graph_insert(F, f1 * f0)
 
     else:  # arg * arg
         # Record products of each factor of arg-dependent operand
         factors = {}
         for k0 in sorted(fac0):
-            f0 = F.nodes[fac0[k0]]['expression']
+            f0 = F.nodes[fac0[k0]]["expression"]
             for k1 in sorted(fac1):
-                f1 = F.nodes[fac1[k1]]['expression']
+                f1 = F.nodes[fac1[k1]]["expression"]
                 argkey = tuple(sorted(k0 + k1))  # sort key for canonical representation
                 factors[argkey] = graph_insert(F, f0 * f1)
 
     return factors
 
 
 @handler.register(Conj)
 def handle_conj(v, fac, sf, F):
-
+    """Handle a conjugation."""
     fac = fac[0]
     if fac:
         factors = {}
         for k in fac:
-            f0 = F.nodes[fac[k]]['expression']
+            f0 = F.nodes[fac[k]]["expression"]
             factors[k] = graph_insert(F, Conj(f0))
     else:
         raise RuntimeError("No arguments")
 
     return factors
 
 
 @handler.register(Division)
 def handle_division(v, fac, sf, F):
+    """Handle a division."""
     fac0 = fac[0]
     fac1 = fac[1]
     assert not fac1, "Cannot divide by arguments."
 
     if fac0:  # arg / non-arg
         # Record products of non-arg operand with each factor of arg-dependent operand
         f1 = sf[1]
         factors = {}
         for k0 in sorted(fac0):
-            f0 = F.nodes[fac0[k0]]['expression']
+            f0 = F.nodes[fac0[k0]]["expression"]
             factors[k0] = graph_insert(F, f0 / f1)
 
     else:  # non-arg / non-arg
         raise RuntimeError("No arguments")
 
     return factors
 
 
 @handler.register(Conditional)
 def handle_conditional(v, fac, sf, F):
+    """Handle a conditional."""
     fac0 = fac[0]
     fac1 = fac[1]
     fac2 = fac[2]
     assert not fac0, "Cannot have argument in condition."
 
     if not (fac1 or fac2):  # non-arg ? non-arg : non-arg
         raise RuntimeError("No arguments")
@@ -192,61 +197,51 @@
         assert fac2 or isinstance(f2, Zero)
         assert () not in fac1
         assert () not in fac2
 
         z = as_ufl(0.0)
 
         # In general, can decompose like this:
-        #    conditional(c, sum_i fi*ui, sum_j fj*uj) -> sum_i conditional(c, fi, 0)*ui + sum_j conditional(c, 0, fj)*uj
+        #    conditional(c, sum_i fi*ui, sum_j fj*uj) -> sum_i conditional(c, fi, 0)*ui
+        #    + sum_j conditional(c, 0, fj)*uj
         mas = sorted(set(fac1.keys()) | set(fac2.keys()))
         factors = {}
         for k in mas:
             fi1 = fac1.get(k)
             fi2 = fac2.get(k)
-            f1 = z if fi1 is None else F.nodes[fi1]['expression']
-            f2 = z if fi2 is None else F.nodes[fi2]['expression']
+            f1 = z if fi1 is None else F.nodes[fi1]["expression"]
+            f2 = z if fi2 is None else F.nodes[fi2]["expression"]
             factors[k] = graph_insert(F, conditional(f0, f1, f2))
 
     return factors
 
 
 def compute_argument_factorization(S, rank):
-    """Factorizes a scalar expression graph w.r.t. scalar Argument components.
-
-    The result is a triplet (AV, FV, IM):
-
-      - The scalar argument component subgraph:
-
-          AV[ai] = v
-
-        with the property
-
-          SV[arg_indices] == AV[:]
-
-      - An expression graph vertex list with all non-argument factors:
-
-          FV[fi] = f
-
-        with the property that none of the expressions depend on Arguments.
-
-      - A dict representation of the final integrand of rank r:
-
-          IM = { (ai1_1, ..., ai1_r): fi1, (ai2_1, ..., ai2_r): fi2, }
-
-        This mapping represents the factorization of SV[-1] w.r.t. Arguments s.t.:
-
-          SV[-1] := sum(FV[fik] * product(AV[ai] for ai in aik) for aik, fik in IM.items())
-
-        where := means equivalence in the mathematical sense,
-        of course in a different technical representation.
+    """Factorize a scalar expression graph w.r.t. scalar Argument components.
 
+    Returns:
+        a triplet (AV, FV, IM), where:
+        - The scalar argument component subgraph:
+            AV[ai] = v
+          with the property
+            SV[arg_indices] == AV[:]
+
+        - An expression graph vertex list with all non-argument factors:
+            FV[fi] = f
+          with the property that none of the expressions depend on Arguments.
+        - A dict representation of the final integrand of rank r:
+            IM = { (ai1_1, ..., ai1_r): fi1, (ai2_1, ..., ai2_r): fi2, }
+          This mapping represents the factorization of SV[-1] w.r.t. Arguments s.t.:
+            SV[-1] := sum(FV[fik] * product(AV[ai] for ai in aik) for aik, fik in IM.items())
+          where := means equivalence in the mathematical sense,
+          of course in a different technical representation.
     """
     # Extract argument component subgraph
     arg_indices = build_argument_indices(S)
-    AV = [S.nodes[i]['expression'] for i in arg_indices]
+    AV = [S.nodes[i]["expression"] for i in arg_indices]
 
     # Data structure for building non-argument factors
     F = ExpressionGraph()
     # Attach a quick lookup dict for expression to index
     F.e2i = {}
 
     # Insert arguments as first entries in factorisation graph
@@ -266,62 +261,62 @@
     #   argkey is a tuple with indices into SV for each of the argument components SV[si] depends on
     # SV_factors[si] = { argkey1: fi1, argkey2: fi2, ... } # if SV[si]
     # is a linear combination of multiple argkey configurations
 
     # Factorize each subexpression in order:
     for si, attr in S.nodes.items():
         deps = S.out_edges[si]
-        v = attr['expression']
+        v = attr["expression"]
 
         if si in arg_indices:
             assert len(deps) == 0
             # v is a modified Argument
-            factors = {(si, ): one_index}
+            factors = {(si,): one_index}
         else:
-            fac = [S.nodes[d]['factors'] for d in deps]
+            fac = [S.nodes[d]["factors"] for d in deps]
             if not any(fac):
                 # Entirely scalar (i.e. no arg factors)
                 # Just add unchanged to F
                 graph_insert(F, v)
                 factors = noargs
             else:
                 # Get scalar factors for dependencies
                 # which do not have arg factors
                 sf = []
                 for i, d in enumerate(deps):
                     if fac[i]:
                         sf.append(None)
                     else:
-                        sf.append(S.nodes[d]['expression'])
+                        sf.append(S.nodes[d]["expression"])
                 # Use appropriate handler to deal with Sum, Product, etc.
                 factors = handler(v, fac, sf, F)
 
-        attr['factors'] = factors
+        attr["factors"] = factors
 
     assert len(F.nodes) == len(F.e2i)
 
     # Prepare a mapping from component of expression to factors
     factors = {}
-    S_targets = [i for i, v in S.nodes.items() if v.get('target', False)]
+    S_targets = [i for i, v in S.nodes.items() if v.get("target", False)]
 
     for S_target in S_targets:
         # Get the factorizations of the target values
-        if S.nodes[S_target]['factors'] == {}:
+        if S.nodes[S_target]["factors"] == {}:
             if rank == 0:
                 # Functionals and expressions: store as no args * factor
                 for comp in S.nodes[S_target]["component"]:
-                    factors[comp] = {(): F.e2i[S.nodes[S_target]['expression']]}
+                    factors[comp] = {(): F.e2i[S.nodes[S_target]["expression"]]}
             else:
                 # Zero form of arity 1 or higher: make factors empty
                 pass
         else:
             # Forms of arity 1 or higher:
             # Map argkeys from indices into SV to indices into AV,
             # and resort keys for canonical representation
-            for argkey, fi in S.nodes[S_target]['factors'].items():
+            for argkey, fi in S.nodes[S_target]["factors"].items():
                 ai_fi = {tuple(sorted(arg_indices.index(si) for si in argkey)): fi}
                 for comp in S.nodes[S_target]["component"]:
                     if factors.get(comp):
                         factors[comp].update(ai_fi)
                     else:
                         factors[comp] = ai_fi
 
@@ -332,13 +327,13 @@
             F.nodes[fi]["target"].append(argkey)
 
             F.nodes[fi]["component"] = F.nodes[fi].get("component", [])
             F.nodes[fi]["component"].append(comp)
 
     # Compute dependencies in FV
     for i, v in F.nodes.items():
-        expr = v['expression']
+        expr = v["expression"]
         if not expr._ufl_is_terminal_ and not expr._ufl_is_terminal_modifier_:
             for o in expr.ufl_operands:
                 F.add_edge(i, F.e2i[o])
 
     return F
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/graph.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Linearized data structure for the computational graph."""
 
 import logging
 
 import numpy as np
-
 import ufl
+
 from ffcx.ir.analysis.modified_terminals import is_modified_terminal
 from ffcx.ir.analysis.reconstruct import reconstruct
 from ffcx.ir.analysis.valuenumbering import ValueNumberer
 
 logger = logging.getLogger("ffcx")
 
 
-class ExpressionGraph(object):
+class ExpressionGraph:
     """A directed multi-edge graph.
 
     ExpressionGraph allows multiple edges between the same nodes,
     and respects the insertion order of nodes and edges.
     """
 
     def __init__(self):
-
+        """Initialise."""
         # Data structures for directed multi-edge graph
         self.nodes = {}
         self.out_edges = {}
         self.in_edges = {}
 
     def number_of_nodes(self):
+        """Get number of nodes."""
         return len(self.nodes)
 
     def add_node(self, key, **kwargs):
         """Add a node with optional properties."""
         self.nodes[key] = kwargs
         self.out_edges[key] = []
         self.in_edges[key] = []
@@ -46,31 +47,32 @@
             raise KeyError("Adding edge to unknown node")
 
         self.out_edges[node1] += [node2]
         self.in_edges[node2] += [node1]
 
 
 def build_graph_vertices(expressions, skip_terminal_modifiers=False):
+    """Build graph vertices."""
     # Count unique expression nodes
     G = ExpressionGraph()
     G.e2i = _count_nodes_with_unique_post_traversal(expressions, skip_terminal_modifiers)
 
     # Invert the map to get index->expression
     GV = sorted(G.e2i, key=G.e2i.get)
 
     # Add nodes to 'new' graph structure
     for i, v in enumerate(GV):
         G.add_node(i, expression=v)
 
     for comp, expr in enumerate(expressions):
         # Get vertex index representing input expression root
         V_target = G.e2i[expr]
-        G.nodes[V_target]['target'] = True
-        G.nodes[V_target]['component'] = G.nodes[V_target].get("component", [])
-        G.nodes[V_target]['component'].append(comp)
+        G.nodes[V_target]["target"] = True
+        G.nodes[V_target]["component"] = G.nodes[V_target].get("component", [])
+        G.nodes[V_target]["component"].append(comp)
 
     return G
 
 
 def build_scalar_graph(expression):
     """Build list representation of expression graph covering the given expressions."""
     # Populate with vertices
@@ -82,15 +84,15 @@
     # Build new list representation of graph where all
     # vertices of V represent single scalar operations
     G = build_graph_vertices(scalar_expressions, skip_terminal_modifiers=True)
 
     # Compute graph edges
     V_deps = []
     for i, v in G.nodes.items():
-        expr = v['expression']
+        expr = v["expression"]
         if expr._ufl_is_terminal_ or expr._ufl_is_terminal_modifier_:
             V_deps.append(())
         else:
             V_deps.append([G.e2i[o] for o in expr.ufl_operands])
 
     for i, edges in enumerate(V_deps):
         for j in edges:
@@ -126,15 +128,15 @@
     total_unique_symbols = value_numberer.symbol_count
 
     # Array to store the scalar subexpression in for each symbol
     W = np.empty(total_unique_symbols, dtype=object)
 
     # Iterate over each graph node in order
     for i, v in G.nodes.items():
-        expr = v['expression']
+        expr = v["expression"]
         # Find symbols of v components
         vs = V_symbols[i]
 
         # Skip if there's nothing new here (should be the case for indexing types)
         # New symbols are not given to indexing types, so W[symbol] already equals
         # an expression, since it was assigned to the symbol in a previous loop
         # cycle
@@ -148,15 +150,17 @@
                 # actually need all of these later, but that will be
                 # optimized away.
                 # Note: symmetries will be dealt with in the value numbering.
                 ws = [expr[c] for c in ufl.permutation.compute_indices(sh)]
             else:
                 # Store single modified terminal expression component
                 if len(vs) != 1:
-                    raise RuntimeError("Expecting single symbol for scalar valued modified terminal.")
+                    raise RuntimeError(
+                        "Expecting single symbol for scalar valued modified terminal."
+                    )
                 ws = [expr]
             # FIXME: Replace ws[:] with 0's if its table is empty
             # Possible redesign: loop over modified terminals only first,
             # then build tables for them, set W[s] = 0.0 for modified terminals with zero table,
             # then loop over non-(modified terminal)s to reconstruct expression.
         else:
             # Find symbols of operands
@@ -186,30 +190,35 @@
         # Store each new scalar subexpression in W at the index of its symbol
         handled = set()
         for s, w in zip(vs, ws):
             if W[s] is None:
                 W[s] = w
                 handled.add(s)
             else:
-                assert s in handled  # Result of symmetry! - but I think this never gets reached anyway (CNR)
+                assert (
+                    s in handled
+                )  # Result of symmetry! - but I think this never gets reached anyway (CNR)
 
     # Find symbols of final v from input graph
     vs = V_symbols[-1]
     scalar_expressions = W[vs]
     return scalar_expressions
 
 
 def _count_nodes_with_unique_post_traversal(expressions, skip_terminal_modifiers=False):
     """Yield o for each node o in expr, child before parent.
 
     Never visits a node twice.
     """
 
     def getops(e):
-        """Get a modifiable list of operands of e, optionally treating modified terminals as a unit."""
+        """Get a modifiable list of operands of e.
+
+        Optionally treating modified terminals as a unit.
+        """
         # TODO: Maybe use e._ufl_is_terminal_modifier_
         if e._ufl_is_terminal_ or (skip_terminal_modifiers and is_modified_terminal(e)):
             return []
         else:
             return list(e.ufl_operands)
 
     e2i = {}
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/indexing.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/indexing.py`

 * *Files identical despite different names*

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/modified_terminals.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/modified_terminals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 # Copyright (C) 2011-2017 Martin Sandve Alnæs
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Modified terminals."""
 
 import logging
+import typing
 
-from ufl.classes import (Argument, CellAvg, FacetAvg, FixedIndex, FormArgument,
-                         Grad, Indexed, Jacobian, ReferenceGrad,
-                         ReferenceValue, Restricted, SpatialCoordinate)
+from ufl.classes import (
+    Argument,
+    CellAvg,
+    FacetAvg,
+    FixedIndex,
+    FormArgument,
+    Grad,
+    Indexed,
+    Jacobian,
+    ReferenceGrad,
+    ReferenceValue,
+    Restricted,
+    SpatialCoordinate,
+)
 from ufl.permutation import build_component_numbering
 
-from ...element_interface import convert_element
-
 logger = logging.getLogger("ffcx")
 
 
-class ModifiedTerminal(object):
-    """A modified terminal expression is an object of a Terminal subtype.
-
-    It is wrapped in terminal modifier types.
-
-    The variables of this class are:
-
-        expr - The original UFL expression
-        terminal           - the underlying Terminal object
-
-        global_derivatives - tuple of ints, each meaning derivative in that global direction
-        local_derivatives  - tuple of ints, each meaning derivative in that local direction
-        reference_value    - bool, whether this is represented in reference frame
-        averaged           - None, 'facet' or 'cell'
-        restriction        - None, '+' or '-'
-
-        component          - tuple of ints, the global component of the Terminal
-        flat_component     - single int, flattened local component of the Terminal, considering symmetry
+class ModifiedTerminal:
+    """A modified terminal."""
 
-
-        Possibly other component model:
-        - global_component
-        - reference_component
-        - flat_component
-    """
-
-    def __init__(self, expr, terminal, reference_value, base_shape, base_symmetry, component,
-                 flat_component, global_derivatives, local_derivatives, averaged, restriction):
+    def __init__(
+        self,
+        expr,
+        terminal,
+        reference_value: bool,
+        base_shape,
+        base_symmetry,
+        component: tuple[int, ...],
+        flat_component: int,
+        global_derivatives: tuple[int, ...],
+        local_derivatives: tuple[int, ...],
+        averaged: typing.Union[None, str],
+        restriction: typing.Union[None, str],
+    ):
+        """Initialise.
+
+        Args:
+            expr: The original UFL expression
+            terminal: the underlying Terminal object
+            reference_value: whether this is represented in reference frame
+            base_shape: base shape
+            base_symmetry: base symmetry
+            component: the global component of the Terminal
+            flat_component: flattened local component of the Terminal, considering symmetry
+            global_derivatives: each entry is a derivative in that global direction
+            local_derivatives: each entry is a derivative in that local direction
+            averaged: Entity to average over (None, 'facet' or 'cell')
+            restriction: The restriction (None, '+' or '-')
+        """
         # The original expression
         self.expr = expr
 
         # The underlying terminal expression
         self.terminal = terminal
 
         # Are we seeing the terminal in physical or reference frame
@@ -110,33 +125,31 @@
         gd = self.global_derivatives
         ld = self.local_derivatives
         a = self.averaged
         r = self.restriction
         return (n, p, rv, fc, gd, ld, a, r)
 
     def __hash__(self):
+        """Hash."""
         return hash(self.as_tuple())
 
     def __eq__(self, other):
+        """Check equality."""
         return isinstance(other, ModifiedTerminal) and self.as_tuple() == other.as_tuple()
 
-    # def __lt__(self, other):
-    #    error("Shouldn't use this?")
-    #    # FIXME: Terminal is not sortable, so the as_tuple contents
-    #    # must be changed for this to work properly
-    #    return self.as_tuple() < other.as_tuple()
-
     def __str__(self):
+        """Format as string."""
         return (
             f"terminal:           {self.terminal}\n"
             f"global_derivatives: {self.global_derivatives}\n"
             f"local_derivatives:  {self.local_derivatives}\n"
             f"averaged:           {self.averaged}\n"
             f"component:          {self.component}\n"
-            f"restriction:        {self.restriction}")
+            f"restriction:        {self.restriction}"
+        )
 
 
 def is_modified_terminal(v):
     """Check if v is a terminal or a terminal wrapped in terminal modifier types."""
     while not v._ufl_is_terminal_:
         if v._ufl_is_terminal_modifier_:
             v = v.ufl_operands[0]
@@ -188,60 +201,60 @@
             if not all(isinstance(j, FixedIndex) for j in i):
                 raise RuntimeError("Expected only fixed indices.")
 
         elif isinstance(t, ReferenceValue):
             if reference_value is not None:
                 raise RuntimeError("Got twice pulled back terminal!")
 
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
             reference_value = True
 
         elif isinstance(t, ReferenceGrad):
             if not component:  # covers None or ()
                 raise RuntimeError("Got local gradient of terminal without prior indexing.")
 
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
             local_derivatives.append(component[-1])
             component = component[:-1]
 
         elif isinstance(t, Grad):
             if not component:  # covers None or ()
                 raise RuntimeError("Got local gradient of terminal without prior indexing.")
 
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
             global_derivatives.append(component[-1])
             component = component[:-1]
 
         elif isinstance(t, Restricted):
             if restriction is not None:
                 raise RuntimeError("Got twice restricted terminal!")
 
             restriction = t._side
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
 
         elif isinstance(t, CellAvg):
             if averaged is not None:
                 raise RuntimeError("Got twice averaged terminal!")
 
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
             averaged = "cell"
 
         elif isinstance(t, FacetAvg):
             if averaged is not None:
                 raise RuntimeError("Got twice averaged terminal!")
 
-            t, = t.ufl_operands
+            (t,) = t.ufl_operands
             averaged = "facet"
 
         elif t._ufl_terminal_modifiers_:
-            raise RuntimeError("Missing handler for terminal modifier type {}, object is {}.".format(
-                type(t), repr(t)))
-
+            raise RuntimeError(
+                f"Missing handler for terminal modifier type {type(t)}, object is {t!r}."
+            )
         else:
-            raise RuntimeError("Unexpected type %s object %s." % (type(t), repr(t)))
+            raise RuntimeError(f"Unexpected type {type(t)} object {t}.")
 
     # Make canonical representation of derivatives
     global_derivatives = tuple(sorted(global_derivatives))
     local_derivatives = tuple(sorted(local_derivatives))
 
     # Make reference_value true or false
     reference_value = reference_value or False
@@ -260,34 +273,44 @@
         component = ()
     else:
         component = tuple(component)
 
     # Get the shape of the core terminal or its reference value, this is
     # the shape that component refers to
     if isinstance(t, FormArgument):
-        element = convert_element(t.ufl_function_space().ufl_element())
+        element = t.ufl_function_space().ufl_element()
         if reference_value:
             # Ignoring symmetry, assuming already applied in conversion
             # to reference frame
             base_symmetry = {}
-            base_shape = element.reference_value_shape()
+            base_shape = element.reference_value_shape
         else:
             base_symmetry = element.symmetry()
             base_shape = t.ufl_shape
     else:
         base_symmetry = {}
         base_shape = t.ufl_shape
 
     # Assert that component is within the shape of the (reference)
     # terminal
     if len(component) != len(base_shape):
         raise RuntimeError("Length of component does not match rank of (reference) terminal.")
     if not all(c >= 0 and c < d for c, d in zip(component, base_shape)):
-        raise RuntimeError("Component indices %s are outside value shape %s" % (component, base_shape))
+        raise RuntimeError("Component indices {component} are outside value shape {base_shape}.")
 
     # Flatten component
     vi2si, _ = build_component_numbering(base_shape, base_symmetry)
     flat_component = vi2si[component]
 
-    return ModifiedTerminal(expr, t, reference_value, base_shape, base_symmetry, component,
-                            flat_component, global_derivatives, local_derivatives, averaged,
-                            restriction)
+    return ModifiedTerminal(
+        expr,
+        t,
+        reference_value,
+        base_shape,
+        base_symmetry,
+        component,
+        flat_component,
+        global_derivatives,
+        local_derivatives,
+        averaged,
+        restriction,
+    )
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/reconstruct.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/reconstruct.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,84 @@
 # Copyright (C) 2011-2017 Martin Sandve Alnæs and Chris Richardson
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Reconstruct."""
 
 import ufl
 
 
 def handle_scalar_nary(o, ops):
+    """Handle a scalary nary operator."""
     if o.ufl_shape != ():
         raise RuntimeError("Expecting scalar.")
     sops = [op[0] for op in ops]
     return [o._ufl_expr_reconstruct_(*sops)]
 
 
 def handle_condition(o, ops):
+    """Handle a condition."""
     # A condition is always scalar, so len(op) == 1
     sops = [op[0] for op in ops]
     return [o._ufl_expr_reconstruct_(*sops)]
 
 
 def handle_conditional(o, ops):
+    """Handle a conditional."""
     # A condition can be non scalar
     symbols = []
     n = len(ops[1])
     if len(ops[0]) != 1:
         raise RuntimeError("Condition should be scalar.")
     if n != len(ops[2]):
         raise RuntimeError("Conditional branches should have same shape.")
     for i in range(len(ops[1])):
         sops = (ops[0][0], ops[1][i], ops[2][i])
         symbols.append(o._ufl_expr_reconstruct_(*sops))
     return symbols
 
 
 def handle_elementwise_unary(o, ops):
+    """Handle a elementwise unary operator."""
     if len(ops) > 1:
         raise RuntimeError("Expecting unary operator.")
     return [o._ufl_expr_reconstruct_(op) for op in ops[0]]
 
 
 def handle_division(o, ops):
+    """Handle a division."""
     if len(ops) != 2:
         raise RuntimeError("Expecting two operands.")
     if len(ops[1]) != 1:
         raise RuntimeError("Expecting scalar divisor.")
-    b, = ops[1]
+    (b,) = ops[1]
     return [o._ufl_expr_reconstruct_(a, b) for a in ops[0]]
 
 
 def handle_sum(o, ops):
+    """Handle a sum."""
     if len(ops) != 2:
         raise RuntimeError("Expecting two operands.")
     if len(ops[0]) != len(ops[1]):
         raise RuntimeError("Expecting scalar divisor.")
     return [o._ufl_expr_reconstruct_(a, b) for a, b in zip(ops[0], ops[1])]
 
 
 def handle_product(o, ops):
+    """Handle a product."""
     if len(ops) != 2:
         raise RuntimeError("Expecting two operands.")
 
     # Get the simple cases out of the way
     if len(ops[0]) == 1:  # True scalar * something
-        a, = ops[0]
+        (a,) = ops[0]
         return [ufl.classes.Product(a, b) for b in ops[1]]
     elif len(ops[1]) == 1:  # Something * true scalar
-        b, = ops[1]
+        (b,) = ops[1]
         return [ufl.classes.Product(a, b) for a in ops[0]]
 
     # Neither of operands are true scalars, this is the tricky part
     o0, o1 = o.ufl_operands
 
     # Get shapes and index shapes
     fi = o.ufl_free_indices
@@ -87,34 +95,39 @@
     # Compute which component of o0 is used in component (comp,ind) of o
     # Compute strides within free index spaces
     ist0 = ufl.utils.indexflattening.shape_to_strides(fid0)
     ist1 = ufl.utils.indexflattening.shape_to_strides(fid1)
     # Map o0 and o1 indices to o indices
     indmap0 = [fi.index(i) for i in fi0]
     indmap1 = [fi.index(i) for i in fi1]
-    indks = [(ufl.utils.indexflattening.flatten_multiindex([ind[i] for i in indmap0], ist0),
-              ufl.utils.indexflattening.flatten_multiindex([ind[i] for i in indmap1], ist1))
-             for ind in indices]
+    indks = [
+        (
+            ufl.utils.indexflattening.flatten_multiindex([ind[i] for i in indmap0], ist0),
+            ufl.utils.indexflattening.flatten_multiindex([ind[i] for i in indmap1], ist1),
+        )
+        for ind in indices
+    ]
 
     # Build products for scalar components
     results = [ufl.classes.Product(ops[0][k0], ops[1][k1]) for k0, k1 in indks]
     return results
 
 
 def handle_index_sum(o, ops):
+    """Handle an index sum."""
     summand, mi = o.ufl_operands
     ic = mi[0].count()
     fi = summand.ufl_free_indices
     fid = summand.ufl_index_dimensions
     ipos = fi.index(ic)
     d = fid[ipos]
 
     # Compute "macro-dimensions" before and after i in the total shape of a
     predim = ufl.product(summand.ufl_shape) * ufl.product(fid[:ipos])
-    postdim = ufl.product(fid[ipos + 1:])
+    postdim = ufl.product(fid[ipos + 1 :])
 
     # Map each flattened total component of summand to
     # flattened total component of indexsum o by removing
     # axis corresponding to summation index ii.
     ss = ops[0]  # Scalar subexpressions of summand
     if len(ss) != predim * postdim * d:
         raise RuntimeError("Mismatching number of subexpressions.")
@@ -127,38 +140,42 @@
 
     # For each scalar output component, sum over collected subcomponents
     # TODO: Need to split this into binary additions to work with future CRSArray format,
     #       i.e. emitting more expressions than there are symbols for this node.
     results = [sum(sop) for sop in sops]
     return results
 
+
 # TODO: To implement compound tensor operators such as dot and inner,
 # we need to identify which index to do the contractions over,
 # and build expressions such as sum(a*b for a,b in zip(aops, bops))
 
 
-_reconstruct_call_lookup = {ufl.classes.MathFunction: handle_scalar_nary,
-                            ufl.classes.Abs: handle_scalar_nary,
-                            ufl.classes.MinValue: handle_scalar_nary,
-                            ufl.classes.MaxValue: handle_scalar_nary,
-                            ufl.classes.Real: handle_elementwise_unary,
-                            ufl.classes.Imag: handle_elementwise_unary,
-                            ufl.classes.Power: handle_scalar_nary,
-                            ufl.classes.BesselFunction: handle_scalar_nary,
-                            ufl.classes.Atan2: handle_scalar_nary,
-                            ufl.classes.Product: handle_product,
-                            ufl.classes.Division: handle_division,
-                            ufl.classes.Sum: handle_sum,
-                            ufl.classes.IndexSum: handle_index_sum,
-                            ufl.classes.Conj: handle_elementwise_unary,
-                            ufl.classes.Conditional: handle_conditional,
-                            ufl.classes.Condition: handle_condition}
+_reconstruct_call_lookup = {
+    ufl.classes.MathFunction: handle_scalar_nary,
+    ufl.classes.Abs: handle_scalar_nary,
+    ufl.classes.MinValue: handle_scalar_nary,
+    ufl.classes.MaxValue: handle_scalar_nary,
+    ufl.classes.Real: handle_elementwise_unary,
+    ufl.classes.Imag: handle_elementwise_unary,
+    ufl.classes.Power: handle_scalar_nary,
+    ufl.classes.BesselFunction: handle_scalar_nary,
+    ufl.classes.Atan2: handle_scalar_nary,
+    ufl.classes.Product: handle_product,
+    ufl.classes.Division: handle_division,
+    ufl.classes.Sum: handle_sum,
+    ufl.classes.IndexSum: handle_index_sum,
+    ufl.classes.Conj: handle_elementwise_unary,
+    ufl.classes.Conditional: handle_conditional,
+    ufl.classes.Condition: handle_condition,
+}
 
 
 def reconstruct(o, *args):
+    """Reconstruct."""
     # First look for exact match
     f = _reconstruct_call_lookup.get(type(o), False)
     if f:
         return f(o, *args)
     else:
         # Look for parent class types instead
         for k in _reconstruct_call_lookup.keys():
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/valuenumbering.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/valuenumbering.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,46 +4,53 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Algorithms for value numbering within computational graphs."""
 
 import logging
 
 import ufl
-from ffcx.ir.analysis.indexing import (map_component_tensor_arg_components,
-                                       map_indexed_arg_components)
+from ufl.pullback import SymmetricPullback
+
+from ffcx.ir.analysis.indexing import (
+    map_component_tensor_arg_components,
+    map_indexed_arg_components,
+)
 from ffcx.ir.analysis.modified_terminals import analyse_modified_terminal
 
 logger = logging.getLogger("ffcx")
 
 
-class ValueNumberer(object):
+class ValueNumberer:
     """Maps scalar components to unique values.
 
     An algorithm to map the scalar components of an expression node to unique value numbers,
     with fallthrough for types that can be mapped to the value numbers
     of their operands.
     """
 
     def __init__(self, G):
+        """Initialise."""
         self.symbol_count = 0
         self.G = G
         self.V_symbols = []
-        self.call_lookup = {ufl.classes.Expr: self.expr,
-                            ufl.classes.Argument: self.form_argument,
-                            ufl.classes.Coefficient: self.form_argument,
-                            ufl.classes.Grad: self._modified_terminal,
-                            ufl.classes.ReferenceGrad: self._modified_terminal,
-                            ufl.classes.FacetAvg: self._modified_terminal,
-                            ufl.classes.CellAvg: self._modified_terminal,
-                            ufl.classes.Restricted: self._modified_terminal,
-                            ufl.classes.ReferenceValue: self._modified_terminal,
-                            ufl.classes.Indexed: self.indexed,
-                            ufl.classes.ComponentTensor: self.component_tensor,
-                            ufl.classes.ListTensor: self.list_tensor,
-                            ufl.classes.Variable: self.variable}
+        self.call_lookup = {
+            ufl.classes.Expr: self.expr,
+            ufl.classes.Argument: self.form_argument,
+            ufl.classes.Coefficient: self.form_argument,
+            ufl.classes.Grad: self._modified_terminal,
+            ufl.classes.ReferenceGrad: self._modified_terminal,
+            ufl.classes.FacetAvg: self._modified_terminal,
+            ufl.classes.CellAvg: self._modified_terminal,
+            ufl.classes.Restricted: self._modified_terminal,
+            ufl.classes.ReferenceValue: self._modified_terminal,
+            ufl.classes.Indexed: self.indexed,
+            ufl.classes.ComponentTensor: self.component_tensor,
+            ufl.classes.ListTensor: self.list_tensor,
+            ufl.classes.Variable: self.variable,
+        }
 
     def new_symbols(self, n):
         """Generate new symbols with a running counter."""
         begin = self.symbol_count
         end = begin + n
         self.symbol_count = end
         return list(range(begin, end))
@@ -51,20 +58,22 @@
     def new_symbol(self):
         """Generate new symbol with a running counter."""
         begin = self.symbol_count
         self.symbol_count += 1
         return begin
 
     def get_node_symbols(self, expr):
-        idx = [i for i, v in self.G.nodes.items() if v['expression'] == expr][0]
+        """Get node symbols."""
+        idx = [i for i, v in self.G.nodes.items() if v["expression"] == expr][0]
         return self.V_symbols[idx]
 
     def compute_symbols(self):
+        """Compute symbols."""
         for i, v in self.G.nodes.items():
-            expr = v['expression']
+            expr = v["expression"]
             symbol = None
             # First look for exact type match
             f = self.call_lookup.get(type(expr), False)
             if f:
                 symbol = f(expr)
             else:
                 # Look for parent class types instead
@@ -84,23 +93,23 @@
     def expr(self, v):
         """Create new symbols for expressions that represent new values."""
         n = ufl.product(v.ufl_shape + v.ufl_index_dimensions)
         return self.new_symbols(n)
 
     def form_argument(self, v):
         """Create new symbols for expressions that represent new values."""
-        symmetry = v.ufl_function_space().ufl_element().symmetry()
+        e = v.ufl_function_space().ufl_element()
 
-        if symmetry:
+        if isinstance(e.pullback, SymmetricPullback):
             # Build symbols with symmetric components skipped
             symbols = []
             mapped_symbols = {}
             for c in ufl.permutation.compute_indices(v.ufl_shape):
                 # Build mapped component mc with symmetries from element considered
-                mc = symmetry.get(c, c)
+                mc = min(i for i, j in e.pullback._symmetry.items() if j == e.pullback._symmetry[c])
 
                 # Get existing symbol or create new and store with mapped component mc as key
                 s = mapped_symbols.get(mc)
                 if s is None:
                     s = self.new_symbol()
                     mapped_symbols[mc] = s
                 symbols.append(s)
@@ -113,50 +122,52 @@
     # Handle modified terminals with element symmetries and second derivative symmetries!
     # terminals are implemented separately, or maybe they don't need to be?
 
     def _modified_terminal(self, v):
         """Handle modified terminal.
 
         Modifiers:
-        ---------
-        terminal           - the underlying Terminal object
-        global_derivatives - tuple of ints, each meaning derivative in that global direction
-        local_derivatives  - tuple of ints, each meaning derivative in that local direction
-        reference_value    - bool, whether this is represented in reference frame
-        averaged           - None, 'facet' or 'cell'
-        restriction        - None, '+' or '-'
-        component          - tuple of ints, the global component of the Terminal
-        flat_component     - single int, flattened local component of the Terminal, considering symmetry
-
+            terminal: the underlying Terminal object
+            global_derivatives: tuple of ints, each meaning derivative
+                in that global direction
+            local_derivatives: tuple of ints, each meaning derivative in
+                that local direction
+            reference_value: bool, whether this is represented in
+                reference frame
+            averaged: None, 'facet' or 'cell'
+            restriction: None, '+' or '-'
+            component: tuple of ints, the global component of the Terminal
+                flat_component: single int, flattened local component of the
+            Terminal, considering symmetry
         """
         # (1) mt.terminal.ufl_shape defines a core indexing space UNLESS mt.reference_value,
         #     in which case the reference value shape of the element must be used.
         # (2) mt.terminal.ufl_element().symmetry() defines core symmetries
         # (3) averaging and restrictions define distinct symbols, no additional symmetries
         # (4) two or more grad/reference_grad defines distinct symbols with additional symmetries
 
         # v is not necessary scalar here, indexing in (0,...,0) picks the first scalar component
         # to analyse, which should be sufficient to get the base shape and derivatives
         if v.ufl_shape:
-            mt = analyse_modified_terminal(v[(0, ) * len(v.ufl_shape)])
+            mt = analyse_modified_terminal(v[(0,) * len(v.ufl_shape)])
         else:
             mt = analyse_modified_terminal(v)
 
         # Get derivatives
         num_ld = len(mt.local_derivatives)
         num_gd = len(mt.global_derivatives)
         assert not (num_ld and num_gd)
         if num_ld:
             domain = ufl.domain.extract_unique_domain(mt.terminal)
             tdim = domain.topological_dimension()
-            d_components = ufl.permutation.compute_indices((tdim, ) * num_ld)
+            d_components = ufl.permutation.compute_indices((tdim,) * num_ld)
         elif num_gd:
             domain = ufl.domain.extract_unique_domiain(mt.terminal)
             gdim = domain.geometric_dimension()
-            d_components = ufl.permutation.compute_indices((gdim, ) * num_gd)
+            d_components = ufl.permutation.compute_indices((gdim,) * num_gd)
         else:
             d_components = [()]
 
         # Get base shape without the derivative axes
         base_components = ufl.permutation.compute_indices(mt.base_shape)
 
         # Build symbols with symmetric components and derivatives skipped
@@ -180,40 +191,45 @@
 
         # Consistency check before returning symbols
         assert not v.ufl_free_indices
         if ufl.product(v.ufl_shape) != len(symbols):
             raise RuntimeError("Internal error in value numbering.")
         return symbols
 
-    # indexed is implemented as a fall-through operation
     def indexed(self, Aii):
+        """Return indexed value.
+
+        This is implemented as a fall-through operation.
+        """
         # Reuse symbols of arg A for Aii
         A = Aii.ufl_operands[0]
 
         # Get symbols of argument A
         A_symbols = self.get_node_symbols(A)
 
         # Map A_symbols to Aii_symbols
         d = map_indexed_arg_components(Aii)
         symbols = [A_symbols[k] for k in d]
         return symbols
 
     def component_tensor(self, A):
+        """Component tensor."""
         # Reuse symbols of arg Aii for A
         Aii = A.ufl_operands[0]
 
         # Get symbols of argument Aii
         Aii_symbols = self.get_node_symbols(Aii)
 
         # Map A_symbols to Aii_symbols
         d = map_component_tensor_arg_components(A)
         symbols = [Aii_symbols[k] for k in d]
         return symbols
 
     def list_tensor(self, v):
+        """List tensor."""
         symbols = []
         for row in v.ufl_operands:
             symbols.extend(self.get_node_symbols(row))
         return symbols
 
     def variable(self, v):
         """Direct reuse of all symbols."""
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/analysis/visualise.py` & `fenics_ffcx-0.8.0/ffcx/ir/analysis/visualise.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 # Copyright (C) 2018 Chris Richardson
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Utility to draw graphs."""
 
+from ufl.classes import (
+    Argument,
+    Division,
+    FloatValue,
+    Indexed,
+    IntValue,
+    Product,
+    ReferenceValue,
+    Sum,
+)
 
 from ffcx.ir.analysis.modified_terminals import strip_modified_terminal
-from ufl.classes import (Argument, Division, FloatValue, Indexed, IntValue,
-                         Product, ReferenceValue, Sum)
 
 
 def visualise_graph(Gx, filename):
-
+    """Visualise a graph."""
     try:
         import pygraphviz as pgv
     except ImportError:
         raise RuntimeError("Install pygraphviz")
 
     if Gx.number_of_nodes() > 400:
         print("Skipping visualisation")
         return
 
     G = pgv.AGraph(strict=False, directed=True)
     for nd, v in Gx.nodes.items():
-        ex = v['expression']
+        ex = v["expression"]
         label = ex.__class__.__name__
         if isinstance(ex, Sum):
-            label = '+'
+            label = "+"
         elif isinstance(ex, Product):
-            label = '*'
+            label = "*"
         elif isinstance(ex, Division):
-            label = '/'
+            label = "/"
         elif isinstance(ex, (IntValue, FloatValue)):
             label = ex.value()
         elif isinstance(ex, (Indexed, ReferenceValue)):
             label = str(ex)
-        G.add_node(nd, label='[%d] %s' % (nd, label))
+        G.add_node(nd, label="[%d] %s" % (nd, label))
 
         arg = strip_modified_terminal(ex)
         if isinstance(arg, Argument):
-            G.get_node(nd).attr['shape'] = 'box'
+            G.get_node(nd).attr["shape"] = "box"
 
-        stat = v.get('status')
-        if stat == 'piecewise':
-            G.get_node(nd).attr['color'] = 'blue'
-            G.get_node(nd).attr['penwidth'] = 5
-        elif stat == 'varying':
-            G.get_node(nd).attr['color'] = 'red'
-            G.get_node(nd).attr['penwidth'] = 5
-        elif stat == 'inactive':
-            G.get_node(nd).attr['color'] = 'dimgray'
-            G.get_node(nd).attr['penwidth'] = 5
+        stat = v.get("status")
+        if stat == "piecewise":
+            G.get_node(nd).attr["color"] = "blue"
+            G.get_node(nd).attr["penwidth"] = 5
+        elif stat == "varying":
+            G.get_node(nd).attr["color"] = "red"
+            G.get_node(nd).attr["penwidth"] = 5
+        elif stat == "inactive":
+            G.get_node(nd).attr["color"] = "dimgray"
+            G.get_node(nd).attr["penwidth"] = 5
 
-        t = v.get('target')
+        t = v.get("target")
         if t:
-            G.get_node(nd).attr['label'] += ':' + str(t)
-            G.get_node(nd).attr['shape'] = 'hexagon'
+            G.get_node(nd).attr["label"] += ":" + str(t)
+            G.get_node(nd).attr["shape"] = "hexagon"
 
-        c = v.get('component')
+        c = v.get("component")
         if c:
-            G.get_node(nd).attr['label'] += f", comp={c}"
+            G.get_node(nd).attr["label"] += f", comp={c}"
 
     for nd, eds in Gx.out_edges.items():
         for ed in eds:
             G.add_edge(nd, ed)
 
-    G.layout(prog='dot')
+    G.layout(prog="dot")
     G.draw(filename)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/elementtables.py` & `fenics_ffcx-0.8.0/ffcx/ir/elementtables.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,91 +4,104 @@
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Tools for precomputed tables of terminal values."""
 
 import logging
 import typing
 
+import basix.ufl
 import numpy as np
 import numpy.typing as npt
-
 import ufl
-from ffcx.element_interface import (QuadratureElement, basix_index,
-                                    convert_element)
-from ffcx.ir.representationutils import (create_quadrature_points_and_weights,
-                                         integral_type_to_entity_dim,
-                                         map_integral_points)
+
+from ffcx.element_interface import basix_index
+from ffcx.ir.representationutils import (
+    create_quadrature_points_and_weights,
+    integral_type_to_entity_dim,
+    map_integral_points,
+)
 
 logger = logging.getLogger("ffcx")
 
 # Using same defaults as np.allclose
 default_rtol = 1e-6
 default_atol = 1e-9
 
 piecewise_ttypes = ("piecewise", "fixed", "ones", "zeros")
 uniform_ttypes = ("fixed", "ones", "zeros", "uniform")
 
 
 class ModifiedTerminalElement(typing.NamedTuple):
-    element: ufl.FiniteElementBase
+    """Modified terminal element."""
+
+    element: basix.ufl._ElementBase
     averaged: str
-    local_derivatives: typing.Tuple[int, ...]
+    local_derivatives: tuple[int, ...]
     fc: int
 
 
 class UniqueTableReferenceT(typing.NamedTuple):
+    """Unique table reference."""
+
     name: str
     values: npt.NDArray[np.float64]
     offset: int
     block_size: int
     ttype: str
     is_piecewise: bool
     is_uniform: bool
     is_permuted: bool
+    has_tensor_factorisation: bool
+    tensor_factors: list[typing.Any]
+    tensor_permutation: np.typing.NDArray[np.int32]
 
 
 def equal_tables(a, b, rtol=default_rtol, atol=default_atol):
+    """Check if two tables are equal."""
     a = np.asarray(a)
     b = np.asarray(b)
     if a.shape != b.shape:
         return False
     else:
         return np.allclose(a, b, rtol=rtol, atol=atol)
 
 
-def clamp_table_small_numbers(table,
-                              rtol=default_rtol,
-                              atol=default_atol,
-                              numbers=(-1.0, 0.0, 1.0)):
+def clamp_table_small_numbers(
+    table, rtol=default_rtol, atol=default_atol, numbers=(-1.0, 0.0, 1.0)
+):
     """Clamp almost 0,1,-1 values to integers. Returns new table."""
     # Get shape of table and number of columns, defined as the last axis
     table = np.asarray(table)
     for n in numbers:
         table[np.where(np.isclose(table, n, rtol=rtol, atol=atol))] = n
     return table
 
 
-def get_ffcx_table_values(points, cell, integral_type, element, avg, entitytype,
-                          derivative_counts, flat_component):
+def get_ffcx_table_values(
+    points, cell, integral_type, element, avg, entitytype, derivative_counts, flat_component
+):
     """Extract values from FFCx element table.
 
     Returns a 3D numpy array with axes
     (entity number, quadrature point number, dof number)
     """
-    element = convert_element(element)
     deriv_order = sum(derivative_counts)
 
     if integral_type in ufl.custom_integral_types:
         # Use quadrature points on cell for analysis in custom integral types
         integral_type = "cell"
         assert not avg
 
     if integral_type == "expression":
-        # FFCx tables for expression are generated as interior cell points
-        integral_type = "cell"
+        # FFCx tables for expression are generated as either interior cell points
+        # or points on a facet
+        if entitytype == "cell":
+            integral_type = "cell"
+        else:
+            integral_type = "exterior_facet"
 
     if avg in ("cell", "facet"):
         # Redefine points to compute average tables
 
         # Make sure this is not called with points, that doesn't make sense
         # assert points is None
 
@@ -99,21 +112,22 @@
         # Doesn't matter if it's exterior or interior facet integral,
         # just need a valid integral type to create quadrature rule
         if avg == "cell":
             integral_type = "cell"
         elif avg == "facet":
             integral_type = "exterior_facet"
 
-        if isinstance(element, QuadratureElement):
+        if isinstance(element, basix.ufl.QuadratureElement):
             points = element._points
             weights = element._weights
         else:
             # Make quadrature rule and get points and weights
             points, weights = create_quadrature_points_and_weights(
-                integral_type, cell, element.highest_degree(), "default", [element])
+                integral_type, cell, element.embedded_superdegree(), "default", [element]
+            )
 
     # Tabulate table of basis functions and derivatives in points for each entity
     tdim = cell.topological_dimension()
     entity_dim = integral_type_to_entity_dim(integral_type, tdim)
     num_entities = cell.num_sub_entities(entity_dim)
 
     # Extract arrays for the right scalar component
@@ -140,143 +154,146 @@
     assert len(component_tables) == num_entities
     num_points, num_dofs = component_tables[0].shape
     shape = (1, num_entities, num_points, num_dofs)
     res = np.zeros(shape)
     for entity in range(num_entities):
         res[:, entity, :, :] = component_tables[entity]
 
-    return {'array': res, 'offset': offset, 'stride': stride}
+    return {"array": res, "offset": offset, "stride": stride}
 
 
-def generate_psi_table_name(quadrature_rule, element_counter, averaged: str, entitytype, derivative_counts,
-                            flat_component):
+def generate_psi_table_name(
+    quadrature_rule, element_counter, averaged: str, entitytype, derivative_counts, flat_component
+):
     """Generate a name for the psi table.
 
     Format:
-    FE#_C#_D###[_AC|_AF|][_F|V][_Q#], where '#' will be an integer value.
-
-    FE  - is a simple counter to distinguish the various bases, it will be
+        FE#_C#_D###[_AC|_AF|][_F|V][_Q#], where '#' will be an integer value and:
+        - FE is a simple counter to distinguish the various bases, it will be
           assigned in an arbitrary fashion.
-
-    C   - is the component number if any (this does not yet take into account
+        - C is the component number if any (this does not yet take into account
           tensor valued functions)
-
-    D   - is the number of derivatives in each spatial direction if any.
+        - D is the number of derivatives in each spatial direction if any.
           If the element is defined in 3D, then D012 means d^3(*)/dydz^2.
-
-    AC  - marks that the element values are averaged over the cell
-
-    AF  - marks that the element values are averaged over the facet
-
-    F   - marks that the first array dimension enumerates facets on the cell
-
-    V   - marks that the first array dimension enumerates vertices on the cell
-
-    Q   - unique ID of quadrature rule, to distinguish between tables in a mixed quadrature rule setting
-
+        - AC marks that the element values are averaged over the cell
+        - AF marks that the element values are averaged over the facet
+        - F marks that the first array dimension enumerates facets on the cell
+        - V marks that the first array dimension enumerates vertices on the cell
+        - Q unique ID of quadrature rule, to distinguish between tables
+          in a mixed quadrature rule setting
     """
     name = "FE%d" % element_counter
     if flat_component is not None:
         name += "_C%d" % flat_component
     if any(derivative_counts):
         name += "_D" + "".join(str(d) for d in derivative_counts)
     name += {None: "", "cell": "_AC", "facet": "_AF"}[averaged]
     name += {"cell": "", "facet": "_F", "vertex": "_V"}[entitytype]
     name += f"_Q{quadrature_rule.id()}"
     return name
 
 
 def get_modified_terminal_element(mt) -> typing.Optional[ModifiedTerminalElement]:
+    """Get modified terminal element."""
     gd = mt.global_derivatives
     ld = mt.local_derivatives
     domain = ufl.domain.extract_unique_domain(mt.terminal)
     # Extract element from FormArguments and relevant GeometricQuantities
     if isinstance(mt.terminal, ufl.classes.FormArgument):
         if gd and mt.reference_value:
-            raise RuntimeError(
-                "Global derivatives of reference values not defined.")
+            raise RuntimeError("Global derivatives of reference values not defined.")
         elif ld and not mt.reference_value:
-            raise RuntimeError(
-                "Local derivatives of global values not defined.")
-        element = convert_element(mt.terminal.ufl_function_space().ufl_element())
+            raise RuntimeError("Local derivatives of global values not defined.")
+        element = mt.terminal.ufl_function_space().ufl_element()
         fc = mt.flat_component
     elif isinstance(mt.terminal, ufl.classes.SpatialCoordinate):
         if mt.reference_value:
             raise RuntimeError("Not expecting reference value of x.")
         if gd:
             raise RuntimeError("Not expecting global derivatives of x.")
-        element = convert_element(domain.ufl_coordinate_element())
+        element = domain.ufl_coordinate_element()
         if not ld:
             fc = mt.flat_component
         else:
             # Actually the Jacobian expressed as reference_grad(x)
             fc = mt.flat_component  # x-component
             assert len(mt.component) == 1
             assert mt.component[0] == mt.flat_component
     elif isinstance(mt.terminal, ufl.classes.Jacobian):
         if mt.reference_value:
             raise RuntimeError("Not expecting reference value of J.")
         if gd:
             raise RuntimeError("Not expecting global derivatives of J.")
-        element = convert_element(domain.ufl_coordinate_element())
+        element = domain.ufl_coordinate_element()
         assert len(mt.component) == 2
         # Translate component J[i,d] to x element context rgrad(x[i])[d]
         fc, d = mt.component  # x-component, derivative
-        ld = tuple(sorted((d, ) + ld))
+        ld = tuple(sorted((d,) + ld))
     else:
         return None
 
     assert (mt.averaged is None) or not (ld or gd)
     # Change derivatives format for table lookup
     tdim = domain.topological_dimension()
-    local_derivatives: typing.Tuple[int, ...] = tuple(ld.count(i) for i in range(tdim))
+    local_derivatives: tuple[int, ...] = tuple(ld.count(i) for i in range(tdim))
 
     return ModifiedTerminalElement(element, mt.averaged, local_derivatives, fc)
 
 
 def permute_quadrature_interval(points, reflections=0):
+    """Permute quadrature points for an interval."""
     output = points.copy()
     for p in output:
         assert len(p) < 2 or np.isclose(p[1], 0)
         assert len(p) < 3 or np.isclose(p[2], 0)
-    for i in range(reflections):
+    for _ in range(reflections):
         for n, p in enumerate(output):
             output[n] = [1 - p[0]]
     return output
 
 
 def permute_quadrature_triangle(points, reflections=0, rotations=0):
+    """Permute quadrature points for a triangle."""
     output = points.copy()
     for p in output:
         assert len(p) < 3 or np.isclose(p[2], 0)
-    for i in range(rotations):
+    for _ in range(rotations):
         for n, p in enumerate(output):
             output[n] = [p[1], 1 - p[0] - p[1]]
-    for i in range(reflections):
+    for _ in range(reflections):
         for n, p in enumerate(output):
             output[n] = [p[1], p[0]]
     return output
 
 
 def permute_quadrature_quadrilateral(points, reflections=0, rotations=0):
+    """Permute quadrature points for a quadrilateral."""
     output = points.copy()
     for p in output:
         assert len(p) < 3 or np.isclose(p[2], 0)
-    for i in range(rotations):
+    for _ in range(rotations):
         for n, p in enumerate(output):
             output[n] = [p[1], 1 - p[0]]
-    for i in range(reflections):
+    for _ in range(reflections):
         for n, p in enumerate(output):
             output[n] = [p[1], p[0]]
     return output
 
 
-def build_optimized_tables(quadrature_rule, cell, integral_type, entitytype,
-                           modified_terminals, existing_tables,
-                           rtol=default_rtol, atol=default_atol):
+def build_optimized_tables(
+    quadrature_rule,
+    cell,
+    integral_type,
+    entitytype,
+    modified_terminals,
+    existing_tables,
+    use_sum_factorization,
+    rtol=default_rtol,
+    atol=default_atol,
+):
     """Build the element tables needed for a list of modified terminals.
 
     Input:
       entitytype - str
       modified_terminals - ordered sequence of unique modified terminals
       FIXME: Document
 
@@ -290,83 +307,127 @@
         if res:
             analysis[mt] = res
 
     # Build element numbering using topological ordering so subelements
     # get priority
     all_elements = [res[0] for res in analysis.values()]
     unique_elements = ufl.algorithms.sort_elements(
-        ufl.algorithms.analysis.extract_sub_elements(all_elements))
+        set(ufl.algorithms.analysis.extract_sub_elements(all_elements))
+    )
     element_numbers = {element: i for i, element in enumerate(unique_elements)}
     mt_tables = {}
 
     _existing_tables = existing_tables.copy()
 
+    all_tensor_factors = []
+    tensor_n = 0
+
     for mt in modified_terminals:
         res = analysis.get(mt)
         if not res:
             continue
         element, avg, local_derivatives, flat_component = res
 
         # Generate table and store table name with modified terminal
 
         # Build name for this particular table
         element_number = element_numbers[element]
-        name = generate_psi_table_name(quadrature_rule, element_number, avg, entitytype,
-                                       local_derivatives, flat_component)
+        name = generate_psi_table_name(
+            quadrature_rule, element_number, avg, entitytype, local_derivatives, flat_component
+        )
 
         # FIXME - currently just recalculate the tables every time,
         # only reusing them if they match numerically.
         # It should be possible to reuse the cached tables by name, but
         # the dofmap offset may differ due to restriction.
 
         tdim = cell.topological_dimension()
-
         if integral_type == "interior_facet":
             if tdim == 1:
-                t = get_ffcx_table_values(quadrature_rule.points, cell,
-                                          integral_type, element, avg, entitytype,
-                                          local_derivatives, flat_component)
+                t = get_ffcx_table_values(
+                    quadrature_rule.points,
+                    cell,
+                    integral_type,
+                    element,
+                    avg,
+                    entitytype,
+                    local_derivatives,
+                    flat_component,
+                )
             elif tdim == 2:
                 new_table = []
                 for ref in range(2):
-                    new_table.append(get_ffcx_table_values(
-                        permute_quadrature_interval(quadrature_rule.points, ref), cell,
-                        integral_type, element, avg, entitytype, local_derivatives, flat_component))
+                    new_table.append(
+                        get_ffcx_table_values(
+                            permute_quadrature_interval(quadrature_rule.points, ref),
+                            cell,
+                            integral_type,
+                            element,
+                            avg,
+                            entitytype,
+                            local_derivatives,
+                            flat_component,
+                        )
+                    )
 
                 t = new_table[0]
-                t['array'] = np.vstack([td['array'] for td in new_table])
+                t["array"] = np.vstack([td["array"] for td in new_table])
             elif tdim == 3:
                 cell_type = cell.cellname()
                 if cell_type == "tetrahedron":
                     new_table = []
                     for rot in range(3):
                         for ref in range(2):
-                            new_table.append(get_ffcx_table_values(
-                                permute_quadrature_triangle(
-                                    quadrature_rule.points, ref, rot),
-                                cell, integral_type, element, avg, entitytype, local_derivatives,
-                                flat_component))
+                            new_table.append(
+                                get_ffcx_table_values(
+                                    permute_quadrature_triangle(quadrature_rule.points, ref, rot),
+                                    cell,
+                                    integral_type,
+                                    element,
+                                    avg,
+                                    entitytype,
+                                    local_derivatives,
+                                    flat_component,
+                                )
+                            )
                     t = new_table[0]
-                    t['array'] = np.vstack([td['array'] for td in new_table])
+                    t["array"] = np.vstack([td["array"] for td in new_table])
                 elif cell_type == "hexahedron":
                     new_table = []
                     for rot in range(4):
                         for ref in range(2):
-                            new_table.append(get_ffcx_table_values(
-                                permute_quadrature_quadrilateral(
-                                    quadrature_rule.points, ref, rot),
-                                cell, integral_type, element, avg, entitytype, local_derivatives, flat_component))
+                            new_table.append(
+                                get_ffcx_table_values(
+                                    permute_quadrature_quadrilateral(
+                                        quadrature_rule.points, ref, rot
+                                    ),
+                                    cell,
+                                    integral_type,
+                                    element,
+                                    avg,
+                                    entitytype,
+                                    local_derivatives,
+                                    flat_component,
+                                )
+                            )
                     t = new_table[0]
-                    t['array'] = np.vstack([td['array'] for td in new_table])
+                    t["array"] = np.vstack([td["array"] for td in new_table])
         else:
-            t = get_ffcx_table_values(quadrature_rule.points, cell,
-                                      integral_type, element, avg, entitytype,
-                                      local_derivatives, flat_component)
+            t = get_ffcx_table_values(
+                quadrature_rule.points,
+                cell,
+                integral_type,
+                element,
+                avg,
+                entitytype,
+                local_derivatives,
+                flat_component,
+            )
         # Clean up table
-        tbl = clamp_table_small_numbers(t['array'], rtol=rtol, atol=atol)
+        tbl = clamp_table_small_numbers(t["array"], rtol=rtol, atol=atol)
         tabletype = analyse_table_type(tbl)
 
         if tabletype in piecewise_ttypes:
             # Reduce table to dimension 1 along num_points axis in generated code
             tbl = tbl[:, :, :1, :]
         if tabletype in uniform_ttypes:
             # Reduce table to dimension 1 along num_entities axis in generated code
@@ -385,69 +446,131 @@
                 new_table = False
                 break
 
         if new_table:
             _existing_tables[name] = tbl
 
         cell_offset = 0
-        element = convert_element(element)
+
+        if use_sum_factorization and (not quadrature_rule.has_tensor_factors):
+            raise RuntimeError("Sum factorization not available for this quadrature rule.")
+
+        tensor_factors = None
+        tensor_perm = None
+        if (
+            use_sum_factorization
+            and element.has_tensor_product_factorisation
+            and len(element.get_tensor_product_representation()) == 1
+            and quadrature_rule.has_tensor_factors
+        ):
+            factors = element.get_tensor_product_representation()
+
+            tensor_factors = []
+            for i, j in enumerate(factors[0]):
+                pts = quadrature_rule.tensor_factors[i][0]
+                d = local_derivatives[i]
+                sub_tbl = j.tabulate(d, pts)[d]
+                sub_tbl = sub_tbl.reshape(1, 1, sub_tbl.shape[0], sub_tbl.shape[1])
+                for i in all_tensor_factors:
+                    if i.values.shape == sub_tbl.shape and np.allclose(i.values, sub_tbl):
+                        tensor_factors.append(i)
+                        break
+                else:
+                    ut = UniqueTableReferenceT(
+                        f"FE_TF{tensor_n}",
+                        sub_tbl,
+                        None,
+                        None,
+                        None,
+                        False,
+                        False,
+                        False,
+                        False,
+                        None,
+                        None,
+                    )
+                    all_tensor_factors.append(ut)
+                    tensor_factors.append(ut)
+                    mt_tables[ut.name] = ut
+                    tensor_n += 1
+
+            tensor_perm = factors[0][1]
 
         if mt.restriction == "-" and isinstance(mt.terminal, ufl.classes.FormArgument):
             # offset = 0 or number of element dofs, if restricted to "-"
             cell_offset = element.dim
 
-        offset = cell_offset + t['offset']
-        block_size = t['stride']
+        offset = cell_offset + t["offset"]
+        block_size = t["stride"]
 
         # tables is just np.arrays, mt_tables hold metadata too
         mt_tables[mt] = UniqueTableReferenceT(
-            name, tbl, offset, block_size, tabletype,
-            tabletype in piecewise_ttypes, tabletype in uniform_ttypes, is_permuted)
+            name,
+            tbl,
+            offset,
+            block_size,
+            tabletype,
+            tabletype in piecewise_ttypes,
+            tabletype in uniform_ttypes,
+            is_permuted,
+            tensor_factors is not None,
+            tensor_factors,
+            tensor_perm,
+        )
 
     return mt_tables
 
 
 def is_zeros_table(table, rtol=default_rtol, atol=default_atol):
-    return (np.prod(table.shape) == 0
-            or np.allclose(table, np.zeros(table.shape), rtol=rtol, atol=atol))
+    """Check if table values are all zero."""
+    return np.prod(table.shape) == 0 or np.allclose(
+        table, np.zeros(table.shape), rtol=rtol, atol=atol
+    )
 
 
 def is_ones_table(table, rtol=default_rtol, atol=default_atol):
+    """Check if table values are all one."""
     return np.allclose(table, np.ones(table.shape), rtol=rtol, atol=atol)
 
 
 def is_quadrature_table(table, rtol=default_rtol, atol=default_atol):
+    """Check if table is a quadrature table."""
     _, num_entities, num_points, num_dofs = table.shape
     Id = np.eye(num_points)
-    return (num_points == num_dofs and all(
-        np.allclose(table[0, i, :, :], Id, rtol=rtol, atol=atol) for i in range(num_entities)))
+    return num_points == num_dofs and all(
+        np.allclose(table[0, i, :, :], Id, rtol=rtol, atol=atol) for i in range(num_entities)
+    )
 
 
 def is_permuted_table(table, rtol=default_rtol, atol=default_atol):
+    """Check if table is permuted."""
     return not all(
-        np.allclose(table[0, :, :, :],
-                    table[i, :, :, :], rtol=rtol, atol=atol)
-        for i in range(1, table.shape[0]))
+        np.allclose(table[0, :, :, :], table[i, :, :, :], rtol=rtol, atol=atol)
+        for i in range(1, table.shape[0])
+    )
 
 
 def is_piecewise_table(table, rtol=default_rtol, atol=default_atol):
+    """Check if table is piecewise."""
     return all(
-        np.allclose(table[0, :, 0, :],
-                    table[0, :, i, :], rtol=rtol, atol=atol)
-        for i in range(1, table.shape[2]))
+        np.allclose(table[0, :, 0, :], table[0, :, i, :], rtol=rtol, atol=atol)
+        for i in range(1, table.shape[2])
+    )
 
 
 def is_uniform_table(table, rtol=default_rtol, atol=default_atol):
+    """Check if table is uniform."""
     return all(
-        np.allclose(table[0, 0, :, :],
-                    table[0, i, :, :], rtol=rtol, atol=atol)
-        for i in range(1, table.shape[1]))
+        np.allclose(table[0, 0, :, :], table[0, i, :, :], rtol=rtol, atol=atol)
+        for i in range(1, table.shape[1])
+    )
 
 
 def analyse_table_type(table, rtol=default_rtol, atol=default_atol):
+    """Analyse table type."""
     if is_zeros_table(table, rtol=rtol, atol=atol):
         # Table is empty or all values are 0.0
         ttype = "zeros"
     elif is_ones_table(table, rtol=rtol, atol=atol):
         # All values are 1.0
         ttype = "ones"
     elif is_quadrature_table(table, rtol=rtol, atol=atol):
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/integral.py` & `fenics_ffcx-0.8.0/ffcx/ir/integral.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,63 +7,62 @@
 
 import collections
 import itertools
 import logging
 import typing
 
 import numpy as np
-
 import ufl
+from ufl.algorithms.balancing import balance_modifiers
+from ufl.checks import is_cellwise_constant
+from ufl.classes import QuadratureWeight
+
 from ffcx.ir.analysis.factorization import compute_argument_factorization
 from ffcx.ir.analysis.graph import build_scalar_graph
-from ffcx.ir.analysis.modified_terminals import (analyse_modified_terminal,
-                                                 is_modified_terminal)
+from ffcx.ir.analysis.modified_terminals import analyse_modified_terminal, is_modified_terminal
 from ffcx.ir.analysis.visualise import visualise_graph
 from ffcx.ir.elementtables import UniqueTableReferenceT, build_optimized_tables
-from ufl.algorithms.balancing import balance_modifiers
-from ufl.checks import is_cellwise_constant
-from ufl.classes import QuadratureWeight
 
 logger = logging.getLogger("ffcx")
 
 
 class ModifiedArgumentDataT(typing.NamedTuple):
+    """Modified argument data."""
+
     ma_index: int
     tabledata: UniqueTableReferenceT
 
 
 class BlockDataT(typing.NamedTuple):
-    ttypes: typing.Tuple[str, ...]  # list of table types for each block rank
-    factor_indices_comp_indices: typing.List[typing.Tuple[int, int]]  # list of tuples (factor index, component index)
+    """Block data."""
+
+    ttypes: tuple[str, ...]  # list of table types for each block rank
+    factor_indices_comp_indices: list[tuple[int, int]]  # list of (factor index, component index)
     all_factors_piecewise: bool  # True if all factors for this block are piecewise
-    unames: typing.Tuple[str, ...]  # list of unique FE table names for each block rank
-    restrictions: typing.Tuple[str, ...]  # restriction "+" | "-" | None for each block rank
+    unames: tuple[str, ...]  # list of unique FE table names for each block rank
+    restrictions: tuple[str, ...]  # restriction "+" | "-" | None for each block rank
     transposed: bool  # block is the transpose of another
     is_uniform: bool
-    ma_data: typing.Tuple[ModifiedArgumentDataT, ...]  # used in "full", "safe" and "partial"
+    ma_data: tuple[ModifiedArgumentDataT, ...]  # used in "full", "safe" and "partial"
     is_permuted: bool  # Do quad points on facets need to be permuted?
 
 
-def compute_integral_ir(cell, integral_type, entitytype, integrands, argument_shape,
-                        p, visualise):
+def compute_integral_ir(cell, integral_type, entitytype, integrands, argument_shape, p, visualise):
+    """Compute intermediate representation for an integral."""
     # The intermediate representation dict we're building and returning
     # here
     ir = {}
 
-    # Pass on options for consumption in code generation
-    ir["options"] = p
-
     # Shared unique tables for all quadrature loops
     ir["unique_tables"] = {}
     ir["unique_table_types"] = {}
 
     ir["integrand"] = {}
 
     for quadrature_rule, integrand in integrands.items():
-
         expression = integrand
 
         # Rebalance order of nested terminal modifiers
         expression = balance_modifiers(expression)
 
         # Remove QuadratureWeight terminals from expression and replace with 1.0
         expression = replace_quadratureweight(expression)
@@ -73,81 +72,87 @@
 
         # Build terminal_data from V here before factorization. Then we
         # can use it to derive table properties for all modified
         # terminals, and then use that to rebuild the scalar graph more
         # efficiently before argument factorization. We can build
         # terminal_data again after factorization if that's necessary.
 
-        initial_terminals = {i: analyse_modified_terminal(v['expression'])
-                             for i, v in S.nodes.items()
-                             if is_modified_terminal(v['expression'])}
+        initial_terminals = {
+            i: analyse_modified_terminal(v["expression"])
+            for i, v in S.nodes.items()
+            if is_modified_terminal(v["expression"])
+        }
 
         mt_table_reference = build_optimized_tables(
             quadrature_rule,
             cell,
             integral_type,
             entitytype,
             initial_terminals.values(),
             ir["unique_tables"],
+            use_sum_factorization=p["sum_factorization"],
             rtol=p["table_rtol"],
-            atol=p["table_atol"])
+            atol=p["table_atol"],
+        )
 
         # Fetch unique tables for this quadrature rule
         table_types = {v.name: v.ttype for v in mt_table_reference.values()}
         tables = {v.name: v.values for v in mt_table_reference.values()}
 
-        S_targets = [i for i, v in S.nodes.items() if v.get('target', False)]
+        S_targets = [i for i, v in S.nodes.items() if v.get("target", False)]
         num_components = np.int32(np.prod(expression.ufl_shape))
 
-        if 'zeros' in table_types.values():
+        if "zeros" in table_types.values():
             # If there are any 'zero' tables, replace symbolically and rebuild graph
             for i, mt in initial_terminals.items():
                 # Set modified terminals with zero tables to zero
                 tr = mt_table_reference.get(mt)
                 if tr is not None and tr.ttype == "zeros":
-                    S.nodes[i]['expression'] = ufl.as_ufl(0.0)
+                    S.nodes[i]["expression"] = ufl.as_ufl(0.0)
 
             # Propagate expression changes using dependency list
             for i, v in S.nodes.items():
-                deps = [S.nodes[j]['expression'] for j in S.out_edges[i]]
+                deps = [S.nodes[j]["expression"] for j in S.out_edges[i]]
                 if deps:
-                    v['expression'] = v['expression']._ufl_expr_reconstruct_(*deps)
+                    v["expression"] = v["expression"]._ufl_expr_reconstruct_(*deps)
 
             # Recreate expression with correct ufl_shape
-            expressions = [None, ] * num_components
+            expressions = [
+                None,
+            ] * num_components
             for target in S_targets:
                 for comp in S.nodes[target]["component"]:
                     assert expressions[comp] is None
                     expressions[comp] = S.nodes[target]["expression"]
             expression = ufl.as_tensor(np.reshape(expressions, expression.ufl_shape))
 
             # Rebuild scalar list-based graph representation
             S = build_scalar_graph(expression)
 
         # Output diagnostic graph as pdf
         if visualise:
-            visualise_graph(S, 'S.pdf')
+            visualise_graph(S, "S.pdf")
 
         # Compute factorization of arguments
         rank = len(argument_shape)
         F = compute_argument_factorization(S, rank)
 
         # Get the 'target' nodes that are factors of arguments, and insert in dict
-        FV_targets = [i for i, v in F.nodes.items() if v.get('target', False)]
+        FV_targets = [i for i, v in F.nodes.items() if v.get("target", False)]
         argument_factorization = {}
 
         for fi in FV_targets:
             # Number of blocks using this factor must agree with number of components
             # to which this factor contributes. I.e. there are more blocks iff there are more
             # components
-            assert len(F.nodes[fi]['target']) == len(F.nodes[fi]['component'])
+            assert len(F.nodes[fi]["target"]) == len(F.nodes[fi]["component"])
 
             k = 0
-            for w in F.nodes[fi]['target']:
-                comp = F.nodes[fi]['component'][k]
+            for w in F.nodes[fi]["target"]:
+                comp = F.nodes[fi]["component"][k]
                 argument_factorization[w] = argument_factorization.get(w, [])
 
                 # Store tuple of (factor index, component index)
                 argument_factorization[w].append((fi, comp))
                 k += 1
 
         # Get list of indices in F which are the arguments (should be at start)
@@ -155,35 +160,35 @@
         for w in argument_factorization:
             argkeys = argkeys | set(w)
         argkeys = list(argkeys)
 
         # Build set of modified_terminals for each mt factorized vertex in F
         # and attach tables, if appropriate
         for i, v in F.nodes.items():
-            expr = v['expression']
+            expr = v["expression"]
             if is_modified_terminal(expr):
                 mt = analyse_modified_terminal(expr)
-                F.nodes[i]['mt'] = mt
+                F.nodes[i]["mt"] = mt
                 tr = mt_table_reference.get(mt)
                 if tr is not None:
-                    F.nodes[i]['tr'] = tr
+                    F.nodes[i]["tr"] = tr
 
         # Attach 'status' to each node: 'inactive', 'piecewise' or 'varying'
         analyse_dependencies(F, mt_table_reference)
 
         # Output diagnostic graph as pdf
         if visualise:
-            visualise_graph(F, 'F.pdf')
+            visualise_graph(F, "F.pdf")
 
         # Loop over factorization terms
         block_contributions = collections.defaultdict(list)
         for ma_indices, fi_ci in sorted(argument_factorization.items()):
             # Get a bunch of information about this term
             assert rank == len(ma_indices)
-            trs = tuple(F.nodes[ai]['tr'] for ai in ma_indices)
+            trs = tuple(F.nodes[ai]["tr"] for ai in ma_indices)
 
             unames = tuple(tr.name for tr in trs)
             ttypes = tuple(tr.ttype for tr in trs)
             assert not any(tt == "zeros" for tt in ttypes)
 
             blockmap = []
             for tr in trs:
@@ -198,52 +203,66 @@
             # Collect relevant restrictions to identify blocks correctly
             # in interior facet integrals
             block_restrictions = []
             for i, ai in enumerate(ma_indices):
                 if trs[i].is_uniform:
                     r = None
                 else:
-                    r = F.nodes[ai]['mt'].restriction
+                    r = F.nodes[ai]["mt"].restriction
 
                 block_restrictions.append(r)
             block_restrictions = tuple(block_restrictions)
 
             # Check if each *each* factor corresponding to this argument is piecewise
-            all_factors_piecewise = all(F.nodes[ifi[0]]["status"] == 'piecewise' for ifi in fi_ci)
+            all_factors_piecewise = all(F.nodes[ifi[0]]["status"] == "piecewise" for ifi in fi_ci)
             block_is_permuted = False
             for name in unames:
                 if tables[name].shape[0] > 1:
                     block_is_permuted = True
             ma_data = []
             for i, ma in enumerate(ma_indices):
                 ma_data.append(ModifiedArgumentDataT(ma, trs[i]))
 
             block_is_transposed = False  # FIXME: Handle transposes for these block types
             block_unames = unames
-            blockdata = BlockDataT(ttypes, fi_ci,
-                                   all_factors_piecewise, block_unames,
-                                   block_restrictions, block_is_transposed,
-                                   block_is_uniform, tuple(ma_data), block_is_permuted)
+            blockdata = BlockDataT(
+                ttypes,
+                fi_ci,
+                all_factors_piecewise,
+                block_unames,
+                block_restrictions,
+                block_is_transposed,
+                block_is_uniform,
+                tuple(ma_data),
+                block_is_permuted,
+            )
 
             # Insert in expr_ir for this quadrature loop
             block_contributions[blockmap].append(blockdata)
 
         # Figure out which table names are referenced
         active_table_names = set()
         for i, v in F.nodes.items():
-            tr = v.get('tr')
-            if tr is not None and F.nodes[i]['status'] != 'inactive':
-                active_table_names.add(tr.name)
+            tr = v.get("tr")
+            if tr is not None and F.nodes[i]["status"] != "inactive":
+                if tr.has_tensor_factorisation:
+                    for t in tr.tensor_factors:
+                        active_table_names.add(t.name)
+                else:
+                    active_table_names.add(tr.name)
 
         # Figure out which table names are referenced in blocks
-        for blockmap, contributions in itertools.chain(
-                block_contributions.items()):
+        for blockmap, contributions in itertools.chain(block_contributions.items()):
             for blockdata in contributions:
                 for mad in blockdata.ma_data:
-                    active_table_names.add(mad.tabledata.name)
+                    if mad.tabledata.has_tensor_factorisation:
+                        for t in mad.tabledata.tensor_factors:
+                            active_table_names.add(t.name)
+                    else:
+                        active_table_names.add(mad.tabledata.name)
 
         active_tables = {}
         active_table_types = {}
 
         for name in active_table_names:
             # Drop tables not referenced from modified terminals
             if table_types[name] not in ("zeros", "ones"):
@@ -251,77 +270,81 @@
                 active_table_types[name] = table_types[name]
 
         # Add tables and types for this quadrature rule to global tables dict
         ir["unique_tables"].update(active_tables)
         ir["unique_table_types"].update(active_table_types)
         # Build IR dict for the given expressions
         # Store final ir for this num_points
-        ir["integrand"][quadrature_rule] = {"factorization": F,
-                                            "modified_arguments": [F.nodes[i]['mt'] for i in argkeys],
-                                            "block_contributions": block_contributions}
+        ir["integrand"][quadrature_rule] = {
+            "factorization": F,
+            "modified_arguments": [F.nodes[i]["mt"] for i in argkeys],
+            "block_contributions": block_contributions,
+        }
 
         restrictions = [i.restriction for i in initial_terminals.values()]
         ir["needs_facet_permutations"] = "+" in restrictions and "-" in restrictions
 
     return ir
 
 
 def analyse_dependencies(F, mt_unique_table_reference):
-    # Sets 'status' of all nodes to either: 'inactive', 'piecewise' or 'varying'
-    # Children of 'target' nodes are either 'piecewise' or 'varying'.
-    # All other nodes are 'inactive'.
-    # Varying nodes are identified by their tables ('tr'). All their parent
-    # nodes are also set to 'varying' - any remaining active nodes are 'piecewise'.
+    """Analyse dependencies.
 
+    Sets 'status' of all nodes to either: 'inactive', 'piecewise' or 'varying'
+    Children of 'target' nodes are either 'piecewise' or 'varying'.
+    All other nodes are 'inactive'.
+    Varying nodes are identified by their tables ('tr'). All their parent
+    nodes are also set to 'varying' - any remaining active nodes are 'piecewise'.
+    """
     # Set targets, and dependencies to 'active'
-    targets = [i for i, v in F.nodes.items() if v.get('target')]
-    for i, v in F.nodes.items():
-        v['status'] = 'inactive'
+    targets = [i for i, v in F.nodes.items() if v.get("target")]
+    for _, v in F.nodes.items():
+        v["status"] = "inactive"
 
     while targets:
         s = targets.pop()
-        F.nodes[s]['status'] = 'active'
+        F.nodes[s]["status"] = "active"
         for j in F.out_edges[s]:
-            if F.nodes[j]['status'] == 'inactive':
+            if F.nodes[j]["status"] == "inactive":
                 targets.append(j)
 
     # Build piecewise/varying markers for factorized_vertices
     varying_ttypes = ("varying", "quadrature", "uniform")
     varying_indices = []
     for i, v in F.nodes.items():
-        if v.get('mt') is None:
+        if v.get("mt") is None:
             continue
-        tr = v.get('tr')
+        tr = v.get("tr")
         if tr is not None:
             ttype = tr.ttype
             # Check if table computations have revealed values varying over points
             if ttype in varying_ttypes:
                 varying_indices.append(i)
             else:
                 if ttype not in ("fixed", "piecewise", "ones", "zeros"):
-                    raise RuntimeError("Invalid ttype %s" % (ttype, ))
+                    raise RuntimeError(f"Invalid ttype {ttype}.")
 
-        elif not is_cellwise_constant(v['expression']):
+        elif not is_cellwise_constant(v["expression"]):
             raise RuntimeError("Error " + str(tr))
             # Keeping this check to be on the safe side,
             # not sure which cases this will cover (if any)
             # varying_indices.append(i)
 
     # Set all parents of active varying nodes to 'varying'
     while varying_indices:
         s = varying_indices.pop()
-        if F.nodes[s]['status'] == 'active':
-            F.nodes[s]['status'] = 'varying'
+        if F.nodes[s]["status"] == "active":
+            F.nodes[s]["status"] = "varying"
             for j in F.in_edges[s]:
                 varying_indices.append(j)
 
     # Any remaining active nodes must be 'piecewise'
-    for i, v in F.nodes.items():
-        if v['status'] == 'active':
-            v['status'] = 'piecewise'
+    for _, v in F.nodes.items():
+        if v["status"] == "active":
+            v["status"] = "piecewise"
 
 
 def replace_quadratureweight(expression):
     """Remove any QuadratureWeight terminals and replace with 1.0."""
     r = []
     for node in ufl.corealg.traversal.unique_pre_traversal(expression):
         if is_modified_terminal(node) and isinstance(node, QuadratureWeight):
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/representation.py` & `fenics_ffcx-0.8.0/ffcx/ir/representation.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,388 +12,442 @@
 
 The representation should conform strictly to the naming and order of
 functions in UFC. Thus, for code generation of the function "foo", one
 should only need to use the data stored in the intermediate
 representation under the key "foo".
 """
 
+from __future__ import annotations
+
 import itertools
 import logging
 import typing
 import warnings
 
-import numpy as np
-import numpy.typing as npt
-
 import basix
 import basix.ufl
+import numpy as np
+import numpy.typing as npt
 import ufl
+from ufl.classes import Integral
+from ufl.sorting import sorted_expr_sum
+
 from ffcx import naming
 from ffcx.analysis import UFLData
-from ffcx.element_interface import convert_element
 from ffcx.ir.integral import compute_integral_ir
-from ffcx.ir.representationutils import (QuadratureRule,
-                                         create_quadrature_points_and_weights)
-from ufl.classes import Integral
-from ufl.sorting import sorted_expr_sum
+from ffcx.ir.representationutils import QuadratureRule, create_quadrature_points_and_weights
 
 logger = logging.getLogger("ffcx")
 
 
 class FormIR(typing.NamedTuple):
+    """Intermediate representation of a form."""
+
     id: int
     name: str
     signature: str
     rank: int
     num_coefficients: int
     num_constants: int
     name_from_uflfile: str
-    function_spaces: typing.Dict[str, typing.Tuple[str, str, str, int, basix.CellType, basix.LagrangeVariant]]
-    original_coefficient_position: typing.List[int]
-    coefficient_names: typing.List[str]
-    constant_names: typing.List[str]
-    finite_elements: typing.List[str]
-    dofmaps: typing.List[str]
-    integral_names: typing.Dict[str, typing.List[str]]
-    subdomain_ids: typing.Dict[str, typing.List[int]]
+    function_spaces: dict[
+        str, tuple[str, str, str, int, basix.CellType, basix.LagrangeVariant, tuple[int]]
+    ]
+    original_coefficient_position: list[int]
+    coefficient_names: list[str]
+    constant_names: list[str]
+    finite_elements: list[str]
+    dofmaps: list[str]
+    integral_names: dict[str, list[str]]
+    subdomain_ids: dict[str, list[int]]
 
 
 class CustomElementIR(typing.NamedTuple):
+    """Intermediate representation of a custom element."""
+
     cell_type: basix.CellType
-    value_shape: typing.Tuple[int, ...]
+    value_shape: tuple[int, ...]
     wcoeffs: npt.NDArray[np.float64]
-    x: typing.List[typing.List[npt.NDArray[np.float64]]]
-    M: typing.List[typing.List[npt.NDArray[np.float64]]]
+    x: list[list[npt.NDArray[np.float64]]]
+    M: list[list[npt.NDArray[np.float64]]]
     map_type: basix.MapType
     sobolev_space: basix.SobolevSpace
     interpolation_nderivs: int
     discontinuous: bool
-    highest_complete_degree: int
-    highest_degree: int
+    embedded_subdegree: int
+    embedded_superdegree: int
     polyset_type: basix.PolysetType
 
 
+class QuadratureIR(typing.NamedTuple):
+    """Intermediate representation of a quadrature rule."""
+
+    cell_shape: str
+    points: npt.NDArray[np.float64]
+    weights: npt.NDArray[np.float64]
+
+
 class ElementIR(typing.NamedTuple):
+    """Intermediate representation of an element."""
+
     id: int
     name: str
     signature: str
     cell_shape: str
     topological_dimension: int
-    geometric_dimension: int
     space_dimension: int
-    value_shape: typing.Tuple[int, ...]
-    reference_value_shape: typing.Tuple[int, ...]
+    reference_value_shape: tuple[int, ...]
     degree: int
-    family: str
+    symmetric: bool
     num_sub_elements: int
     block_size: int
-    sub_elements: typing.List[str]
+    sub_elements: list[str]
     element_type: str
-    entity_dofs: typing.List[typing.List[typing.List[int]]]
+    entity_dofs: list[list[list[int]]]
     lagrange_variant: basix.LagrangeVariant
     dpc_variant: basix.DPCVariant
     basix_family: basix.ElementFamily
     basix_cell: basix.CellType
     discontinuous: bool
     custom_element: CustomElementIR
+    custom_quadrature: QuadratureIR
 
 
 class DofMapIR(typing.NamedTuple):
+    """Intermediate representation of a DOF map."""
+
     id: int
     name: str
     signature: str
     num_global_support_dofs: int
     num_element_support_dofs: int
-    entity_dofs: typing.List[typing.List[typing.List[int]]]
-    num_entity_dofs: typing.List[typing.List[int]]
-    entity_closure_dofs: typing.List[typing.List[typing.List[int]]]
-    num_entity_closure_dofs: typing.List[typing.List[int]]
+    entity_dofs: list[list[list[int]]]
+    entity_closure_dofs: list[list[list[int]]]
+    num_entity_closure_dofs: list[list[int]]
     num_sub_dofmaps: int
-    sub_dofmaps: typing.List[str]
+    sub_dofmaps: list[str]
     block_size: int
 
 
 class IntegralIR(typing.NamedTuple):
+    """Intermediate representation of an integral."""
+
     integral_type: str
-    subdomain_id: typing.Union[str, typing.Tuple[int, ...], int]
     rank: int
-    geometric_dimension: int
-    topological_dimension: int
     entitytype: str
-    num_facets: int
-    num_vertices: int
-    enabled_coefficients: typing.List[bool]
-    element_dimensions: typing.Dict[ufl.FiniteElementBase, int]
-    element_ids: typing.Dict[ufl.FiniteElementBase, int]
-    tensor_shape: typing.List[int]
-    coefficient_numbering: typing.Dict[ufl.Coefficient, int]
-    coefficient_offsets: typing.Dict[ufl.Coefficient, int]
-    original_constant_offsets: typing.Dict[ufl.Constant, int]
-    options: dict
-    cell_shape: str
-    unique_tables: typing.Dict[str, npt.NDArray[np.float64]]
-    unique_table_types: typing.Dict[str, str]
-    integrand: typing.Dict[QuadratureRule, dict]
+    enabled_coefficients: list[bool]
+    tensor_shape: list[int]
+    coefficient_numbering: dict[ufl.Coefficient, int]
+    coefficient_offsets: dict[ufl.Coefficient, int]
+    original_constant_offsets: dict[ufl.Constant, int]
+    unique_tables: dict[str, npt.NDArray[np.float64]]
+    unique_table_types: dict[str, str]
+    integrand: dict[QuadratureRule, dict]
     name: str
     needs_facet_permutations: bool
     coordinate_element: str
 
 
 class ExpressionIR(typing.NamedTuple):
+    """Intermediate representation of an expression."""
+
     name: str
-    element_dimensions: typing.Dict[ufl.FiniteElementBase, int]
     options: dict
-    unique_tables: typing.Dict[str, npt.NDArray[np.float64]]
-    unique_table_types: typing.Dict[str, str]
-    integrand: typing.Dict[QuadratureRule, dict]
-    coefficient_numbering: typing.Dict[ufl.Coefficient, int]
-    coefficient_offsets: typing.Dict[ufl.Coefficient, int]
+    unique_tables: dict[str, npt.NDArray[np.float64]]
+    unique_table_types: dict[str, str]
+    integrand: dict[QuadratureRule, dict]
+    coefficient_numbering: dict[ufl.Coefficient, int]
+    coefficient_offsets: dict[ufl.Coefficient, int]
     integral_type: str
     entitytype: str
-    tensor_shape: typing.List[int]
-    expression_shape: typing.List[int]
-    original_constant_offsets: typing.Dict[ufl.Constant, int]
+    tensor_shape: list[int]
+    expression_shape: list[int]
+    original_constant_offsets: dict[ufl.Constant, int]
     points: npt.NDArray[np.float64]
-    coefficient_names: typing.List[str]
-    constant_names: typing.List[str]
+    coefficient_names: list[str]
+    constant_names: list[str]
     needs_facet_permutations: bool
-    function_spaces: typing.Dict[str, typing.Tuple[str, str, str, int, basix.CellType, basix.LagrangeVariant]]
+    function_spaces: dict[
+        str, tuple[str, str, str, int, basix.CellType, basix.LagrangeVariant, tuple[int]]
+    ]
     name_from_uflfile: str
-    original_coefficient_positions: typing.List[int]
+    original_coefficient_positions: list[int]
 
 
 class DataIR(typing.NamedTuple):
-    elements: typing.List[ElementIR]
-    dofmaps: typing.List[DofMapIR]
-    integrals: typing.List[IntegralIR]
-    forms: typing.List[FormIR]
-    expressions: typing.List[ExpressionIR]
-
+    """Intermediate representation of data."""
 
-def compute_ir(analysis: UFLData, object_names, prefix, options, visualise):
+    elements: list[ElementIR]
+    dofmaps: list[DofMapIR]
+    integrals: list[IntegralIR]
+    forms: list[FormIR]
+    expressions: list[ExpressionIR]
+
+
+def compute_ir(
+    analysis: UFLData,
+    object_names: dict[int, str],
+    prefix: str,
+    options: dict[str, npt.DTypeLike | int | float],
+    visualise: bool,
+) -> DataIR:
     """Compute intermediate representation."""
     logger.info(79 * "*")
     logger.info("Compiler stage 2: Computing intermediate representation of objects")
     logger.info(79 * "*")
 
     # Compute object names
     # NOTE: This is done here for performance reasons, because repeated calls
     # within each IR computation would be expensive due to UFL signature computations
-    finite_element_names = {e: naming.finite_element_name(e, prefix) for e in analysis.unique_elements}
+    finite_element_names = {
+        e: naming.finite_element_name(e, prefix) for e in analysis.unique_elements
+    }
     dofmap_names = {e: naming.dofmap_name(e, prefix) for e in analysis.unique_elements}
     integral_names = {}
     form_names = {}
     for fd_index, fd in enumerate(analysis.form_data):
         form_names[fd_index] = naming.form_name(fd.original_form, fd_index, prefix)
         for itg_index, itg_data in enumerate(fd.integral_data):
-            integral_names[(fd_index, itg_index)] = naming.integral_name(fd.original_form, itg_data.integral_type,
-                                                                         fd_index, itg_data.subdomain_id, prefix)
-
-    ir_elements = [_compute_element_ir(e, analysis.element_numbers, finite_element_names)
-                   for e in analysis.unique_elements]
+            integral_names[(fd_index, itg_index)] = naming.integral_name(
+                fd.original_form, itg_data.integral_type, fd_index, itg_data.subdomain_id, prefix
+            )
+
+    ir_elements = [
+        _compute_element_ir(e, analysis.element_numbers, finite_element_names)
+        for e in analysis.unique_elements
+    ]
 
-    ir_dofmaps = [_compute_dofmap_ir(e, analysis.element_numbers, dofmap_names)
-                  for e in analysis.unique_elements]
+    ir_dofmaps = [
+        _compute_dofmap_ir(e, analysis.element_numbers, dofmap_names)
+        for e in analysis.unique_elements
+    ]
 
-    irs = [_compute_integral_ir(fd, i, analysis.element_numbers, integral_names, finite_element_names,
-                                options, visualise)
-           for (i, fd) in enumerate(analysis.form_data)]
+    irs = [
+        _compute_integral_ir(
+            fd,
+            i,
+            analysis.element_numbers,
+            integral_names,
+            finite_element_names,
+            options,
+            visualise,
+        )
+        for (i, fd) in enumerate(analysis.form_data)
+    ]
     ir_integrals = list(itertools.chain(*irs))
 
-    ir_forms = [_compute_form_ir(fd, i, prefix, form_names, integral_names, analysis.element_numbers,
-                                 finite_element_names, dofmap_names, object_names)
-                for (i, fd) in enumerate(analysis.form_data)]
-
-    ir_expressions = [_compute_expression_ir(expr, i, prefix, analysis, options, visualise, object_names,
-                                             finite_element_names, dofmap_names)
-                      for i, expr in enumerate(analysis.expressions)]
-
-    return DataIR(elements=ir_elements, dofmaps=ir_dofmaps,
-                  integrals=ir_integrals, forms=ir_forms,
-                  expressions=ir_expressions)
+    ir_forms = [
+        _compute_form_ir(
+            fd,
+            i,
+            prefix,
+            form_names,
+            integral_names,
+            analysis.element_numbers,
+            finite_element_names,
+            dofmap_names,
+            object_names,
+        )
+        for (i, fd) in enumerate(analysis.form_data)
+    ]
+
+    ir_expressions = [
+        _compute_expression_ir(
+            expr,
+            i,
+            prefix,
+            analysis,
+            options,
+            visualise,
+            object_names,
+            finite_element_names,
+            dofmap_names,
+        )
+        for i, expr in enumerate(analysis.expressions)
+    ]
+
+    return DataIR(
+        elements=ir_elements,
+        dofmaps=ir_dofmaps,
+        integrals=ir_integrals,
+        forms=ir_forms,
+        expressions=ir_expressions,
+    )
 
 
 def _compute_element_ir(element, element_numbers, finite_element_names):
     """Compute intermediate representation of element."""
     logger.info(f"Computing IR for element {element}")
 
-    element = convert_element(element)
-
     # Create basix elements
-    cell = element.cell()
+    cell = element.cell
 
     # Store id
     ir = {"id": element_numbers[element]}
     ir["name"] = finite_element_names[element]
 
     # Compute data for each function
     ir["signature"] = repr(element)
     ir["cell_shape"] = element.cell_type.name
     ir["topological_dimension"] = cell.topological_dimension()
-    ir["geometric_dimension"] = cell.geometric_dimension()
     ir["space_dimension"] = element.dim + element.num_global_support_dofs
     ir["element_type"] = element.ufcx_element_type
     ir["lagrange_variant"] = element.lagrange_variant
     ir["dpc_variant"] = element.dpc_variant
     ir["basix_family"] = element.element_family
     ir["basix_cell"] = element.cell_type
     ir["discontinuous"] = element.discontinuous
-    ir["degree"] = element.degree()
-    ir["family"] = element.family_name
-    ir["value_shape"] = element.value_shape()
-    ir["reference_value_shape"] = element.reference_value_shape()
+    ir["degree"] = element.degree
+    ir["symmetric"] = isinstance(element, basix.ufl._BlockedElement) and isinstance(
+        element._pullback, ufl.pullback.SymmetricPullback
+    )
+    ir["reference_value_shape"] = element.reference_value_shape
 
-    ir["num_sub_elements"] = element.num_sub_elements()
-    ir["sub_elements"] = [finite_element_names[e] for e in element.sub_elements()]
+    ir["num_sub_elements"] = element.num_sub_elements
+    ir["sub_elements"] = [finite_element_names[e] for e in element.sub_elements]
 
     ir["block_size"] = element.block_size
     if element.block_size > 1:
-        element = element.sub_element
+        element = element._sub_element
 
     ir["entity_dofs"] = element.entity_dofs
 
     if element.is_custom_element:
-        ir["custom_element"] = _compute_custom_element_ir(element.element)
+        ir["custom_element"] = _compute_custom_element_ir(element._element)
     else:
         ir["custom_element"] = None
 
+    if element.has_custom_quadrature:
+        ir["custom_quadrature"] = _compute_custom_quadrature_ir(element)
+    else:
+        ir["custom_quadrature"] = None
+
     return ElementIR(**ir)
 
 
-def _compute_custom_element_ir(basix_element: basix.finite_element.FiniteElement):
+def _compute_custom_element_ir(
+    basix_element: basix.finite_element.FiniteElement,
+) -> CustomElementIR:
     """Compute intermediate representation of a custom Basix element."""
-    ir: typing.Dict[str, typing.Any] = {}
+    ir: dict[str, typing.Any] = {}
     ir["cell_type"] = basix_element.cell_type
     ir["value_shape"] = basix_element.value_shape
     ir["wcoeffs"] = basix_element.wcoeffs
     ir["x"] = basix_element.x
     ir["M"] = basix_element.M
     ir["map_type"] = basix_element.map_type
     ir["sobolev_space"] = basix_element.sobolev_space
     ir["discontinuous"] = basix_element.discontinuous
     ir["interpolation_nderivs"] = basix_element.interpolation_nderivs
-    ir["highest_complete_degree"] = basix_element.highest_complete_degree
-    ir["highest_degree"] = basix_element.highest_degree
+    ir["embedded_subdegree"] = basix_element.embedded_subdegree
+    ir["embedded_superdegree"] = basix_element.embedded_superdegree
     ir["polyset_type"] = basix_element.polyset_type
 
     return CustomElementIR(**ir)
 
 
+def _compute_custom_quadrature_ir(element: basix.ufl._ElementBase) -> QuadratureIR:
+    """Compute intermediate representation of a custom Basix element."""
+    ir: dict[str, typing.Any] = {}
+    ir["cell_shape"] = element.cell_type.name
+    ir["points"], ir["weights"] = element.custom_quadrature()
+
+    return QuadratureIR(**ir)
+
+
 def _compute_dofmap_ir(element, element_numbers, dofmap_names):
     """Compute intermediate representation of dofmap."""
     logger.info(f"Computing IR for dofmap of {element}")
 
-    # Create basix elements
-    element = convert_element(element)
-
     # Store id
     ir = {"id": element_numbers[element]}
     ir["name"] = dofmap_names[element]
 
     # Compute data for each function
     ir["signature"] = "FFCx dofmap for " + repr(element)
-    ir["sub_dofmaps"] = [dofmap_names[e] for e in element.sub_elements()]
-    ir["num_sub_dofmaps"] = element.num_sub_elements()
+    ir["sub_dofmaps"] = [dofmap_names[e] for e in element.sub_elements]
+    ir["num_sub_dofmaps"] = element.num_sub_elements
 
     ir["block_size"] = element.block_size
     if element.block_size > 1:
-        element = element.sub_element
+        element = element._sub_element
 
-    # Precompute repeatedly used items
-    for i in element.num_entity_dofs:
-        # FIXME: this assumes the same number of DOFs on each entity of the same dim: this
-        # assumption will not be true for prisms and pyramids
-        if max(i) != min(i):
-            raise RuntimeError("Elements with different numbers of DOFs on subentities of the same dimension"
-                               " are not yet supported in FFCx.")
-
-    # FIXME: This does not work for prisms and pyramids
-    num_dofs_per_entity = [i[0] for i in element.num_entity_dofs]
-    ir["num_entity_dofs"] = num_dofs_per_entity
     ir["entity_dofs"] = element.entity_dofs
+    ir["entity_closure_dofs"] = element.entity_closure_dofs
 
     num_dofs_per_entity_closure = [i[0] for i in element.num_entity_closure_dofs]
     ir["num_entity_closure_dofs"] = num_dofs_per_entity_closure
     ir["entity_closure_dofs"] = element.entity_closure_dofs
 
     ir["num_global_support_dofs"] = element.num_global_support_dofs
     ir["num_element_support_dofs"] = element.dim
 
     return DofMapIR(**ir)
 
 
-def _compute_integral_ir(form_data, form_index, element_numbers, integral_names,
-                         finite_element_names, options, visualise):
+def _compute_integral_ir(
+    form_data, form_index, element_numbers, integral_names, finite_element_names, options, visualise
+) -> list[IntegralIR]:
     """Compute intermediate representation for form integrals."""
     _entity_types = {
         "cell": "cell",
         "exterior_facet": "facet",
         "interior_facet": "facet",
         "vertex": "vertex",
-        "custom": "cell"
+        "custom": "cell",
     }
 
     # Iterate over groups of integrals
     irs = []
     for itg_data_index, itg_data in enumerate(form_data.integral_data):
-
         logger.info(f"Computing IR for integral in integral group {itg_data_index}")
 
         # Compute representation
         entitytype = _entity_types[itg_data.integral_type]
         cell = itg_data.domain.ufl_cell()
         cellname = cell.cellname()
         tdim = cell.topological_dimension()
         assert all(tdim == itg.ufl_domain().topological_dimension() for itg in itg_data.integrals)
 
         ir = {
             "integral_type": itg_data.integral_type,
-            "subdomain_id": itg_data.subdomain_id,
             "rank": form_data.rank,
-            "geometric_dimension": form_data.geometric_dimension,
-            "topological_dimension": tdim,
             "entitytype": entitytype,
-            "num_facets": cell.num_facets(),
-            "num_vertices": cell.num_vertices(),
             "enabled_coefficients": itg_data.enabled_coefficients,
-            "cell_shape": cellname,
-            "coordinate_element": finite_element_names[convert_element(itg_data.domain.ufl_coordinate_element())]
+            "coordinate_element": finite_element_names[itg_data.domain.ufl_coordinate_element()],
         }
 
         # Get element space dimensions
         unique_elements = element_numbers.keys()
-        ir["element_dimensions"] = {element: element.dim + element.num_global_support_dofs
-                                    for element in unique_elements}
-
-        ir["element_ids"] = {
-            element: i
-            for i, element in enumerate(unique_elements)
+        element_dimensions = {
+            element: element.dim + element.num_global_support_dofs for element in unique_elements
         }
 
         # Create dimensions of primary indices, needed to reset the argument
         # 'A' given to tabulate_tensor() by the assembler.
         argument_dimensions = [
-            ir["element_dimensions"][convert_element(element)] for element in form_data.argument_elements
+            element_dimensions[element] for element in form_data.argument_elements
         ]
 
         # Compute shape of element tensor
         if ir["integral_type"] == "interior_facet":
             ir["tensor_shape"] = [2 * dim for dim in argument_dimensions]
         else:
             ir["tensor_shape"] = argument_dimensions
 
         integral_type = itg_data.integral_type
         cell = itg_data.domain.ufl_cell()
 
         # Group integrands with the same quadrature rule
-        grouped_integrands = {}
+        grouped_integrands: dict[QuadratureRule, list[ufl.core.expr.Expr]] = {}
+        use_sum_factorization = options["sum_factorization"] and itg_data.integral_type == "cell"
         for integral in itg_data.integrals:
             md = integral.metadata() or {}
             scheme = md["quadrature_rule"]
-
+            tensor_factors = None
             if scheme == "custom":
                 points = md["quadrature_points"]
                 weights = md["quadrature_weights"]
             elif scheme == "vertex":
                 # FIXME: Could this come from basix?
 
                 # The vertex scheme, i.e., averaging the function value in the
@@ -406,57 +460,97 @@
 
                 degree = md["quadrature_degree"]
                 if integral_type != "cell":
                     facet_types = cell.facet_types()
                     assert len(facet_types) == 1
                     cellname = facet_types[0].cellname()
                 if degree > 1:
-                    warnings.warn("Explicitly selected vertex quadrature (degree 1), but requested degree is {}.".
-                                  format(degree))
+                    warnings.warn(
+                        "Explicitly selected vertex quadrature (degree 1), "
+                        f"but requested degree is {degree}."
+                    )
                 if cellname == "tetrahedron":
-                    points, weights = (np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0],
-                                                 [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]),
-                                       np.array([1.0 / 24.0, 1.0 / 24.0, 1.0 / 24.0, 1.0 / 24.0]))
+                    points, weights = (
+                        np.array(
+                            [[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
+                        ),
+                        np.array([1.0 / 24.0, 1.0 / 24.0, 1.0 / 24.0, 1.0 / 24.0]),
+                    )
                 elif cellname == "triangle":
-                    points, weights = (np.array([[0.0, 0.0], [1.0, 0.0], [0.0, 1.0]]),
-                                       np.array([1.0 / 6.0, 1.0 / 6.0, 1.0 / 6.0]))
+                    points, weights = (
+                        np.array([[0.0, 0.0], [1.0, 0.0], [0.0, 1.0]]),
+                        np.array([1.0 / 6.0, 1.0 / 6.0, 1.0 / 6.0]),
+                    )
                 elif cellname == "interval":
                     # Trapezoidal rule
                     points, weights = (np.array([[0.0], [1.0]]), np.array([1.0 / 2.0, 1.0 / 2.0]))
                 elif cellname == "quadrilateral":
-                    points, weights = (np.array([[0., 0], [1., 0.], [0., 1.], [1., 1]]),
-                                       np.array([1. / 4., 1. / 4., 1. / 4., 1. / 4.]))
+                    points, weights = (
+                        np.array([[0.0, 0], [1.0, 0.0], [0.0, 1.0], [1.0, 1]]),
+                        np.array([1.0 / 4.0, 1.0 / 4.0, 1.0 / 4.0, 1.0 / 4.0]),
+                    )
                 elif cellname == "hexahedron":
-                    points, weights = (np.array([[0., 0., 0.], [1., 0., 0.], [0., 1., 0.], [1., 1., 0.],
-                                                 [0., 0., 1.], [1., 0., 1.], [0., 1., 1.], [1., 1., 1.]]),
-                                       np.array([1. / 8., 1. / 8., 1. / 8., 1. / 8.,
-                                                 1. / 8., 1. / 8., 1. / 8., 1. / 8.]))
+                    points, weights = (
+                        np.array(
+                            [
+                                [0.0, 0.0, 0.0],
+                                [1.0, 0.0, 0.0],
+                                [0.0, 1.0, 0.0],
+                                [1.0, 1.0, 0.0],
+                                [0.0, 0.0, 1.0],
+                                [1.0, 0.0, 1.0],
+                                [0.0, 1.0, 1.0],
+                                [1.0, 1.0, 1.0],
+                            ]
+                        ),
+                        np.array(
+                            [
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                                1.0 / 8.0,
+                            ]
+                        ),
+                    )
                 else:
                     raise RuntimeError(f"Vertex scheme is not supported for cell: {cellname}")
             else:
                 degree = md["quadrature_degree"]
-                points, weights = create_quadrature_points_and_weights(
-                    integral_type, cell, degree, scheme, [convert_element(e) for e in form_data.argument_elements])
+                points, weights, tensor_factors = create_quadrature_points_and_weights(
+                    integral_type,
+                    cell,
+                    degree,
+                    scheme,
+                    form_data.argument_elements,
+                    use_sum_factorization,
+                )
 
             points = np.asarray(points)
             weights = np.asarray(weights)
-
-            rule = QuadratureRule(points, weights)
+            rule = QuadratureRule(points, weights, tensor_factors)
 
             if rule not in grouped_integrands:
                 grouped_integrands[rule] = []
-
             grouped_integrands[rule].append(integral.integrand())
-
-        sorted_integrals = {}
+        sorted_integrals: dict[QuadratureRule, Integral] = {}
         for rule, integrands in grouped_integrands.items():
             integrands_summed = sorted_expr_sum(integrands)
 
-            integral_new = Integral(integrands_summed, itg_data.integral_type, itg_data.domain,
-                                    itg_data.subdomain_id, {}, None)
+            integral_new = Integral(
+                integrands_summed,
+                itg_data.integral_type,
+                itg_data.domain,
+                itg_data.subdomain_id,
+                {},
+                None,
+            )
             sorted_integrals[rule] = integral_new
 
         # TODO: See if coefficient_numbering can be removed
         # Build coefficient numbering for UFC interface here, to avoid
         # renumbering in UFL and application of replace mapping
         coefficient_numbering = {}
         for i, f in enumerate(form_data.reduced_coefficients):
@@ -467,48 +561,65 @@
 
         index_to_coeff = sorted([(v, k) for k, v in coefficient_numbering.items()])
         offsets = {}
         width = 2 if integral_type in ("interior_facet") else 1
         _offset = 0
         for k, el in zip(index_to_coeff, form_data.coefficient_elements):
             offsets[k[1]] = _offset
-            _offset += width * ir["element_dimensions"][convert_element(el)]
+            _offset += width * element_dimensions[el]
 
         # Copy offsets also into IR
         ir["coefficient_offsets"] = offsets
 
         # Build offsets for Constants
         original_constant_offsets = {}
         _offset = 0
         for constant in form_data.original_form.constants():
             original_constant_offsets[constant] = _offset
             _offset += np.prod(constant.ufl_shape, dtype=int)
 
         ir["original_constant_offsets"] = original_constant_offsets
 
         # Create map from number of quadrature points -> integrand
-        integrands = {rule: integral.integrand() for rule, integral in sorted_integrals.items()}
+        integrand_map: dict[QuadratureRule, ufl.core.expr.Expr] = {
+            rule: integral.integrand() for rule, integral in sorted_integrals.items()
+        }
 
         # Build more specific intermediate representation
-        integral_ir = compute_integral_ir(itg_data.domain.ufl_cell(), itg_data.integral_type,
-                                          ir["entitytype"], integrands, ir["tensor_shape"],
-                                          options, visualise)
+        integral_ir = compute_integral_ir(
+            itg_data.domain.ufl_cell(),
+            itg_data.integral_type,
+            ir["entitytype"],
+            integrand_map,
+            ir["tensor_shape"],
+            options,
+            visualise,
+        )
 
         ir.update(integral_ir)
 
         # Fetch name
         ir["name"] = integral_names[(form_index, itg_data_index)]
 
         irs.append(IntegralIR(**ir))
 
     return irs
 
 
-def _compute_form_ir(form_data, form_id, prefix, form_names, integral_names, element_numbers, finite_element_names,
-                     dofmap_names, object_names) -> FormIR:
+def _compute_form_ir(
+    form_data,
+    form_id,
+    prefix,
+    form_names,
+    integral_names,
+    element_numbers,
+    finite_element_names,
+    dofmap_names,
+    object_names,
+) -> FormIR:
     """Compute intermediate representation of form."""
     logger.info(f"Computing IR for form {form_id}")
 
     # Store id
     ir = {"id": form_id}
 
     # Compute common data
@@ -516,46 +627,58 @@
 
     ir["signature"] = form_data.original_form.signature()
 
     ir["rank"] = len(form_data.original_form.arguments())
     ir["num_coefficients"] = len(form_data.reduced_coefficients)
     ir["num_constants"] = len(form_data.original_form.constants())
 
-    ir["coefficient_names"] = [object_names.get(id(obj), f"w{j}")
-                               for j, obj in enumerate(form_data.reduced_coefficients)]
+    ir["coefficient_names"] = [
+        object_names.get(id(obj), f"w{j}") for j, obj in enumerate(form_data.reduced_coefficients)
+    ]
 
-    ir["constant_names"] = [object_names.get(id(obj), f"c{j}")
-                            for j, obj in enumerate(form_data.original_form.constants())]
+    ir["constant_names"] = [
+        object_names.get(id(obj), f"c{j}")
+        for j, obj in enumerate(form_data.original_form.constants())
+    ]
 
     ir["original_coefficient_position"] = form_data.original_coefficient_positions
 
     ir["finite_elements"] = [
-        finite_element_names[convert_element(e)]
+        finite_element_names[e]
         for e in form_data.argument_elements + form_data.coefficient_elements
     ]
 
     ir["dofmaps"] = [
-        dofmap_names[convert_element(e)] for e in form_data.argument_elements + form_data.coefficient_elements
+        dofmap_names[e] for e in form_data.argument_elements + form_data.coefficient_elements
     ]
 
     fs = {}
     for function in form_data.original_form.arguments() + tuple(form_data.reduced_coefficients):
         name = object_names.get(id(function), str(function))
         if not str(name).isidentifier():
-            raise ValueError(f"Function name \"{name}\" must be a valid object identifier.")
-        el = convert_element(convert_element(function.ufl_function_space().ufl_element()))
-        cmap = function.ufl_function_space().ufl_domain().ufl_coordinate_element()
+            raise ValueError(f'Function name "{name}" must be a valid object identifier.')
+        el = function.ufl_function_space().ufl_element()
+        space = function.ufl_function_space()
+        domain = space.ufl_domain()
+        cmap = domain.ufl_coordinate_element()
         # Default point spacing for CoordinateElement is equispaced
         if not isinstance(cmap, basix.ufl._ElementBase) and cmap.variant() is None:
             cmap._sub_element._variant = "equispaced"
-        cmap = convert_element(cmap)
-        family = cmap.family()
-        degree = cmap.degree()
-        fs[name] = (finite_element_names[el], dofmap_names[el], family, degree,
-                    cmap.cell_type, cmap.lagrange_variant)
+        family = cmap.family_name
+        degree = cmap.degree
+        value_shape = space.value_shape
+        fs[name] = (
+            finite_element_names[el],
+            dofmap_names[el],
+            family,
+            degree,
+            cmap.cell_type,
+            cmap.lagrange_variant,
+            value_shape,
+        )
 
     form_name = object_names.get(id(form_data.original_form), form_id)
 
     ir["function_spaces"] = fs
     ir["name_from_uflfile"] = f"form_{prefix}_{form_name}"
 
     # Store names of integrals and subdomain_ids for this form, grouped
@@ -577,16 +700,25 @@
         ir["subdomain_ids"][integral_type] += subdomain_ids
         for _ in range(len(subdomain_ids)):
             ir["integral_names"][integral_type] += [integral_names[(form_id, itg_index)]]
 
     return FormIR(**ir)
 
 
-def _compute_expression_ir(expression, index, prefix, analysis, options, visualise, object_names,
-                           finite_element_names, dofmap_names):
+def _compute_expression_ir(
+    expression,
+    index,
+    prefix,
+    analysis,
+    options,
+    visualise,
+    object_names,
+    finite_element_names,
+    dofmap_names,
+):
     """Compute intermediate representation of expression."""
     logger.info(f"Computing IR for expression {index}")
 
     # Compute representation
     ir = {}
 
     original_expression = (expression[2], expression[1])
@@ -602,21 +734,23 @@
     except AttributeError:
         # This case corresponds to a spatially constant expression
         # without any dependencies
         cell = None
 
     # Prepare dimensions of all unique element in expression, including
     # elements for arguments, coefficients and coordinate mappings
-    ir["element_dimensions"] = {element: element.dim + element.num_global_support_dofs
-                                for element in analysis.unique_elements}
+    element_dimensions = {
+        element: element.dim + element.num_global_support_dofs
+        for element in analysis.unique_elements
+    }
 
     # Extract dimensions for elements of arguments only
     arguments = ufl.algorithms.extract_arguments(expression)
-    argument_elements = tuple(convert_element(f.ufl_function_space().ufl_element()) for f in arguments)
-    argument_dimensions = [ir["element_dimensions"][element] for element in argument_elements]
+    argument_elements = tuple(f.ufl_function_space().ufl_element() for f in arguments)
+    argument_dimensions = [element_dimensions[element] for element in argument_elements]
 
     tensor_shape = argument_dimensions
     ir["tensor_shape"] = tensor_shape
 
     ir["expression_shape"] = list(expression.ufl_shape)
 
     coefficients = ufl.algorithms.extract_coefficients(expression)
@@ -628,72 +762,102 @@
     ir["coefficient_numbering"] = coefficient_numbering
 
     original_coefficient_positions = []
     original_coefficients = ufl.algorithms.extract_coefficients(original_expression)
     for coeff in coefficients:
         original_coefficient_positions.append(original_coefficients.index(coeff))
 
-    ir["coefficient_names"] = [object_names.get(id(obj), f"w{j}")
-                               for j, obj in enumerate(coefficients)]
+    ir["coefficient_names"] = [
+        object_names.get(id(obj), f"w{j}") for j, obj in enumerate(coefficients)
+    ]
 
-    ir["constant_names"] = [object_names.get(id(obj), f"c{j}")
-                            for j, obj in enumerate(ufl.algorithms.analysis.extract_constants(expression))]
+    ir["constant_names"] = [
+        object_names.get(id(obj), f"c{j}")
+        for j, obj in enumerate(ufl.algorithms.analysis.extract_constants(expression))
+    ]
 
     fs = {}
     for function in tuple(original_coefficients) + tuple(arguments):
         name = object_names.get(id(function), str(function))
         if not str(name).isidentifier():
-            raise ValueError(f"Function name \"{name}\" must be a valid object identifier.")
-        el = convert_element(function.ufl_function_space().ufl_element())
-        cmap = convert_element(function.ufl_function_space().ufl_domain().ufl_coordinate_element())
-        family = cmap.family()
-        degree = cmap.degree()
-        fs[name] = (finite_element_names[el], dofmap_names[el], family, degree)
+            raise ValueError(f'Function name "{name}" must be a valid object identifier.')
+        el = function.ufl_function_space().ufl_element()
+        space = function.ufl_function_space()
+        domain = space.ufl_domain()
+        cmap = domain.ufl_coordinate_element()
+        family = cmap.family_name
+        degree = cmap.degree
+        value_shape = space.value_shape
+        fs[name] = (
+            finite_element_names[el],
+            dofmap_names[el],
+            family,
+            degree,
+            cmap.cell_type,
+            cmap.lagrange_variant,
+            value_shape,
+        )
 
     expression_name = object_names.get(id(original_expression), index)
 
     ir["function_spaces"] = fs
     ir["name_from_uflfile"] = f"expression_{prefix}_{expression_name}"
 
     if len(argument_elements) > 1:
         raise RuntimeError("Expression with more than one Argument not implemented.")
 
     ir["original_coefficient_positions"] = original_coefficient_positions
 
-    coefficient_elements = tuple(convert_element(f.ufl_element()) for f in coefficients)
+    coefficient_elements = tuple(f.ufl_element() for f in coefficients)
 
     offsets = {}
     _offset = 0
     for i, el in enumerate(coefficient_elements):
         offsets[coefficients[i]] = _offset
-        _offset += ir["element_dimensions"][convert_element(el)]
+        _offset += element_dimensions[el]
 
     # Copy offsets also into IR
     ir["coefficient_offsets"] = offsets
 
     ir["integral_type"] = "expression"
-    ir["entitytype"] = "cell"
+    if cell is not None:
+        if (tdim := cell.topological_dimension()) == (pdim := points.shape[1]):
+            ir["entitytype"] = "cell"
+        elif tdim - 1 == pdim:
+            ir["entitytype"] = "facet"
+        else:
+            raise ValueError(
+                f"Expression on domain with topological dimension {tdim}"
+                + f"with points of dimension {pdim} not supported."
+            )
+    else:
+        # For spatially invariant expressions, all expressions are evaluated in the cell
+        ir["entitytype"] = "cell"
 
     # Build offsets for Constants
     original_constant_offsets = {}
     _offset = 0
-    for constant in ufl.algorithms.analysis.extract_constants(expression):
+    for constant in ufl.algorithms.analysis.extract_constants(original_expression):
         original_constant_offsets[constant] = _offset
-        _offset += np.product(constant.ufl_shape, dtype=int)
+        _offset += np.prod(constant.ufl_shape, dtype=int)
 
     ir["original_constant_offsets"] = original_constant_offsets
 
     ir["points"] = points
 
     weights = np.array([1.0] * points.shape[0])
     rule = QuadratureRule(points, weights)
     integrands = {rule: expression}
 
     if cell is None:
-        assert len(ir["original_coefficient_positions"]) == 0 and len(ir["original_constant_offsets"]) == 0
-
-    expression_ir = compute_integral_ir(cell, ir["integral_type"], ir["entitytype"], integrands, tensor_shape,
-                                        options, visualise)
-
+        assert (
+            len(ir["original_coefficient_positions"]) == 0
+            and len(ir["original_constant_offsets"]) == 0
+        )
+
+    expression_ir = compute_integral_ir(
+        cell, ir["integral_type"], ir["entitytype"], integrands, tensor_shape, options, visualise
+    )
+    ir["options"] = options
     ir.update(expression_ir)
 
     return ExpressionIR(**ir)
```

### Comparing `fenics-ffcx-0.7.0/ffcx/ir/representationutils.py` & `fenics_ffcx-0.8.0/ffcx/ir/representationutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,69 +2,95 @@
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 """Utility functions for some code shared between representations."""
 
 import hashlib
+import itertools
 import logging
 
 import numpy as np
-
 import ufl
-from ffcx.element_interface import (create_quadrature, map_facet_points,
-                                    reference_cell_vertices)
+
+from ffcx.element_interface import create_quadrature, map_facet_points, reference_cell_vertices
 
 logger = logging.getLogger("ffcx")
 
 
 class QuadratureRule:
-    def __init__(self, points, weights):
+    """A quadrature rule."""
+
+    def __init__(self, points, weights, tensor_factors=None):
+        """Initialise."""
         self.points = np.ascontiguousarray(points)  # TODO: change basix to make this unnecessary
         self.weights = weights
+        self.tensor_factors = tensor_factors
+        self.has_tensor_factors = tensor_factors is not None
         self._hash = None
 
     def __hash__(self):
+        """Hash."""
         if self._hash is None:
             self.hash_obj = hashlib.sha1(self.points)
             self._hash = int(self.hash_obj.hexdigest(), 32)
         return self._hash
 
     def __eq__(self, other):
+        """Check equality."""
         return np.allclose(self.points, other.points) and np.allclose(self.weights, other.weights)
 
     def id(self):
         """Return unique deterministic identifier.
 
-        Note
-        ----
-        This identifier is used to provide unique names to tables and symbols
-        in generated code.
-
+        Note:
+            This identifier is used to provide unique names to tables and symbols
+            in generated code.
         """
         return self.hash_obj.hexdigest()[-3:]
 
 
-def create_quadrature_points_and_weights(integral_type, cell, degree, rule, elements):
+def create_quadrature_points_and_weights(
+    integral_type, cell, degree, rule, elements, use_tensor_product=False
+):
     """Create quadrature rule and return points and weights."""
+    pts = None
+    wts = None
+    tensor_factors = None
+
     if integral_type == "cell":
-        return create_quadrature(cell.cellname(), degree, rule, elements)
+        if cell.cellname() in ["quadrilateral", "hexahedron"] and use_tensor_product:
+            if cell.cellname() == "quadrilateral":
+                tensor_factors = [
+                    create_quadrature("interval", degree, rule, elements) for _ in range(2)
+                ]
+            elif cell.cellname() == "hexahedron":
+                tensor_factors = [
+                    create_quadrature("interval", degree, rule, elements) for _ in range(3)
+                ]
+            pts = np.array(
+                [tuple(i[0] for i in p) for p in itertools.product(*[f[0] for f in tensor_factors])]
+            )
+            wts = np.array([np.prod(p) for p in itertools.product(*[f[1] for f in tensor_factors])])
+        else:
+            pts, wts = create_quadrature(cell.cellname(), degree, rule, elements)
     elif integral_type in ufl.measure.facet_integral_types:
         facet_types = cell.facet_types()
         # Raise exception for cells with more than one facet type e.g. prisms
         if len(facet_types) > 1:
             raise Exception(f"Cell type {cell} not supported for integral type {integral_type}.")
-        return create_quadrature(facet_types[0].cellname(), degree, rule, elements)
+        pts, wts = create_quadrature(facet_types[0].cellname(), degree, rule, elements)
     elif integral_type in ufl.measure.point_integral_types:
-        return create_quadrature("vertex", degree, rule, elements)
+        pts, wts = create_quadrature("vertex", degree, rule, elements)
     elif integral_type == "expression":
-        return (None, None)
+        pass
+    else:
+        logging.exception(f"Unknown integral type: {integral_type}")
 
-    logging.exception(f"Unknown integral type: {integral_type}")
-    return (None, None)
+    return pts, wts, tensor_factors
 
 
 def integral_type_to_entity_dim(integral_type, tdim):
     """Given integral_type and domain tdim, return the tdim of the integration entity."""
     if integral_type == "cell":
         entity_dim = tdim
     elif integral_type in ufl.measure.facet_integral_types:
```

### Comparing `fenics-ffcx-0.7.0/ffcx/main.py` & `fenics_ffcx-0.8.0/ffcx/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,37 +12,45 @@
 import cProfile
 import logging
 import pathlib
 import re
 import string
 
 import ufl
+
 from ffcx import __version__ as FFCX_VERSION
 from ffcx import compiler, formatting
 from ffcx.options import FFCX_DEFAULT_OPTIONS, get_options
 
 logger = logging.getLogger("ffcx")
 
 parser = argparse.ArgumentParser(
-    description="FEniCS Form Compiler (FFCx, https://fenicsproject.org)")
-parser.add_argument(
-    "--version", action='version', version=f"%(prog)s (version {FFCX_VERSION})")
+    description="FEniCS Form Compiler (FFCx, https://fenicsproject.org)"
+)
+parser.add_argument("--version", action="version", version=f"%(prog)s (version {FFCX_VERSION})")
 parser.add_argument("-o", "--output-directory", type=str, default=".", help="output directory")
 parser.add_argument("--visualise", action="store_true", help="visualise the IR graph")
-parser.add_argument("-p", "--profile", action='store_true', help="enable profiling")
+parser.add_argument("-p", "--profile", action="store_true", help="enable profiling")
 
 # Add all options from FFCx option system
-for opt_name, (opt_val, opt_desc) in FFCX_DEFAULT_OPTIONS.items():
-    parser.add_argument(f"--{opt_name}",
-                        type=type(opt_val), help=f"{opt_desc} (default={opt_val})")
+for opt_name, (arg_type, opt_val, opt_desc, choices) in FFCX_DEFAULT_OPTIONS.items():
+    if isinstance(opt_val, bool):
+        parser.add_argument(
+            f"--{opt_name}", action="store_true", help=f"{opt_desc} (default={opt_val})"
+        )
+    else:
+        parser.add_argument(
+            f"--{opt_name}", type=arg_type, choices=choices, help=f"{opt_desc} (default={opt_val})"
+        )
 
-parser.add_argument("ufl_file", nargs='+', help="UFL file(s) to be compiled")
+parser.add_argument("ufl_file", nargs="+", help="UFL file(s) to be compiled")
 
 
 def main(args=None):
+    """Run ffcx on a UFL file."""
     xargs = parser.parse_args(args)
 
     # Parse all other options
     priority_options = {k: v for k, v in xargs.__dict__.items() if v is not None}
     options = get_options(priority_options)
 
     # Call parser and compiler for each file
@@ -61,16 +69,20 @@
             pr.enable()
 
         # Load UFL file
         ufd = ufl.algorithms.load_ufl_file(filename)
 
         # Generate code
         code_h, code_c = compiler.compile_ufl_objects(
-            ufd.forms + ufd.expressions + ufd.elements, ufd.object_names,
-            prefix=prefix, options=options, visualise=xargs.visualise)
+            ufd.forms + ufd.expressions + ufd.elements,
+            options=options,
+            object_names=ufd.object_names,
+            prefix=prefix,
+            visualise=xargs.visualise,
+        )
 
         # Write to file
         formatting.write_code(code_h, code_c, prefix, xargs.output_directory)
 
         # Turn off profiling and write status to file
         if xargs.profile:
             pr.disable()
```

### Comparing `fenics-ffcx-0.7.0/ffcx/naming.py` & `fenics_ffcx-0.8.0/ffcx/naming.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # Copyright (C) 2009-2020 Anders Logg and Michal Habera
 #
 # This file is part of FFCx.(https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Naming."""
+
+from __future__ import annotations
 
 import hashlib
-import typing
 
+import basix.ufl
 import numpy as np
 import numpy.typing as npt
-
-import ffcx
 import ufl
 
-from .element_interface import convert_element
+import ffcx
+import ffcx.codegeneration
 
 
-def compute_signature(ufl_objects: typing.List[
-    typing.Union[ufl.Form, ufl.FiniteElementBase,
-                 typing.Tuple[ufl.core.expr.Expr, npt.NDArray[np.float64]]]], tag: str) -> str:
+def compute_signature(
+    ufl_objects: list[
+        ufl.Form | basix.ufl._ElementBase | tuple[ufl.core.expr.Expr, npt.NDArray[np.float64]]
+    ],
+    tag: str,
+) -> str:
     """Compute the signature hash.
 
-    Based on the UFL type of the objects and an additional optional
-    'tag'.
-
+    Based on the UFL type of the objects and an additional optional 'tag'.
     """
     object_signature = ""
     for ufl_object in ufl_objects:
         # Get signature from ufl object
         if isinstance(ufl_object, ufl.Form):
             kind = "form"
             object_signature += ufl_object.signature()
-        elif isinstance(ufl_object, ufl.FiniteElementBase):
-            object_signature += repr(convert_element(ufl_object))
+        elif isinstance(ufl_object, ufl.AbstractFiniteElement):
+            object_signature += repr(ufl_object)
             kind = "element"
         elif isinstance(ufl_object, tuple) and isinstance(ufl_object[0], ufl.core.expr.Expr):
             expr = ufl_object[0]
             points = ufl_object[1]
 
             # FIXME Move this to UFL, cache the computation
             coeffs = ufl.algorithms.extract_coefficients(expr)
@@ -44,15 +47,15 @@
             args = ufl.algorithms.analysis.extract_arguments(expr)
 
             rn = dict()
             rn.update(dict((c, i) for i, c in enumerate(coeffs)))
             rn.update(dict((c, i) for i, c in enumerate(consts)))
             rn.update(dict((c, i) for i, c in enumerate(args)))
 
-            domains: typing.List[ufl.Mesh] = []
+            domains: list[ufl.Mesh] = []
             for coeff in coeffs:
                 domains.append(*coeff.ufl_domains())
             for arg in args:
                 domains.append(*arg.ufl_function_space().ufl_domains())
             for gc in ufl.algorithms.analysis.extract_type(expr, ufl.classes.GeometricQuantity):
                 domains.append(*gc.ufl_domains())
             for const in consts:
@@ -66,38 +69,57 @@
             object_signature += repr(points)
 
             kind = "expression"
         else:
             raise RuntimeError(f"Unknown ufl object type {ufl_object.__class__.__name__}")
 
     # Build combined signature
-    signatures = [object_signature, str(ffcx.__version__), ffcx.codegeneration.get_signature(), kind, tag]
+    signatures = [
+        object_signature,
+        str(ffcx.__version__),
+        ffcx.codegeneration.get_signature(),
+        kind,
+        tag,
+    ]
     string = ";".join(signatures)
-    return hashlib.sha1(string.encode('utf-8')).hexdigest()
+    return hashlib.sha1(string.encode("utf-8")).hexdigest()
 
 
-def integral_name(original_form, integral_type, form_id, subdomain_id, prefix):
+def integral_name(
+    original_form: ufl.form.Form,
+    integral_type: str,
+    form_id: int,
+    subdomain_id: tuple[int, ...] | tuple[str],
+    prefix: str,
+) -> str:
+    """Get integral name."""
     sig = compute_signature([original_form], str((prefix, integral_type, form_id, subdomain_id)))
     return f"integral_{sig}"
 
 
-def form_name(original_form, form_id, prefix):
+def form_name(original_form: ufl.form.Form, form_id: int, prefix: str) -> str:
+    """Get form name."""
     sig = compute_signature([original_form], str((prefix, form_id)))
     return f"form_{sig}"
 
 
-def finite_element_name(ufl_element, prefix):
-    assert isinstance(ufl_element, ufl.FiniteElementBase)
-    sig = compute_signature([convert_element(ufl_element)], prefix)
+def finite_element_name(ufl_element: basix.ufl._ElementBase, prefix: str) -> str:
+    """Get finite element name."""
+    assert isinstance(ufl_element, basix.ufl._ElementBase)
+    sig = compute_signature([ufl_element], prefix)
     return f"element_{sig}"
 
 
-def dofmap_name(ufl_element, prefix):
-    assert isinstance(ufl_element, ufl.FiniteElementBase)
-    sig = compute_signature([convert_element(ufl_element)], prefix)
+def dofmap_name(ufl_element: basix.ufl._ElementBase, prefix: str) -> str:
+    """Get DOF map name."""
+    assert isinstance(ufl_element, basix.ufl._ElementBase)
+    sig = compute_signature([ufl_element], prefix)
     return f"dofmap_{sig}"
 
 
-def expression_name(expression, prefix):
+def expression_name(
+    expression: tuple[ufl.core.expr.Expr, npt.NDArray[np.floating]], prefix: str
+) -> str:
+    """Get expression name."""
     assert isinstance(expression[0], ufl.core.expr.Expr)
     sig = compute_signature([expression], prefix)
     return f"expression_{sig}"
```

### Comparing `fenics-ffcx-0.7.0/ffcx/options.py` & `fenics_ffcx-0.8.0/ffcx/options.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 # Copyright (C) 2005-2020 Anders Logg, Michal Habera, Jack S. Hale
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
+"""Options."""
+
+from __future__ import annotations
 
 import functools
 import json
 import logging
 import os
 import os.path
 import pprint
 from pathlib import Path
-from typing import Any, Dict, Optional
+
+import numpy.typing as npt
 
 logger = logging.getLogger("ffcx")
 
 FFCX_DEFAULT_OPTIONS = {
-    "epsilon":
-        (1e-14, "Machine precision, used for dropping zero terms in tables"),
-    "scalar_type":
-        ("double", """Scalar type used in generated code. Any of real or complex C floating-point types, e.g.
-                      float, double, float _Complex, double _Complex, ..."""),
-    "table_rtol":
-        (1e-6, "Relative precision to use when comparing finite element table values for table reuse."),
-    "table_atol":
-        (1e-9, "Absolute precision to use when comparing finite element table values for reuse."),
-    "verbosity":
-        (30, "Logger verbosity. Follows standard logging library levels, i.e. INFO=20, DEBUG=10, etc.")
+    "epsilon": (float, 1e-14, "machine precision, used for dropping zero terms in tables.", None),
+    "scalar_type": (
+        str,
+        "float64",
+        "scalar type to use in generated code.",
+        ("float32", "float64", "complex64", "complex128"),
+    ),
+    "sum_factorization": (bool, False, "use sum factorization.", None),
+    "table_rtol": (
+        float,
+        1e-6,
+        "relative precision to use when comparing finite element table values for reuse.",
+        None,
+    ),
+    "table_atol": (
+        float,
+        1e-9,
+        "absolute precision to use when comparing finite element table values reuse.",
+        None,
+    ),
+    "verbosity": (
+        int,
+        30,
+        "logger verbosity, follows standard library levels, i.e. INFO=20, DEBUG=10, etc.",
+        None,
+    ),
 }
 
 
-@functools.lru_cache(maxsize=None)
-def _load_options():
+@functools.cache
+def _load_options() -> tuple[dict, dict]:
     """Load options from JSON files."""
-    user_config_file = os.getenv("XDG_CONFIG_HOME", default=Path.home().joinpath(".config")) \
-        / Path("ffcx", "ffcx_options.json")
+    user_config_file = os.getenv("XDG_CONFIG_HOME", default=Path.home().joinpath(".config")) / Path(
+        "ffcx", "ffcx_options.json"
+    )
     try:
         with open(user_config_file) as f:
             user_options = json.load(f)
     except FileNotFoundError:
         user_options = {}
 
     pwd_config_file = Path.cwd().joinpath("ffcx_options.json")
@@ -47,60 +67,57 @@
             pwd_options = json.load(f)
     except FileNotFoundError:
         pwd_options = {}
 
     return (user_options, pwd_options)
 
 
-def get_options(priority_options: Optional[dict] = None) -> dict:
+def get_options(
+    priority_options: dict[str, npt.DTypeLike | int | float] | None = None,
+) -> dict[str, int | float | npt.DTypeLike]:
     """Return (a copy of) the merged option values for FFCX.
 
-    Options
-    ----------
-      priority_options:
-        take priority over all other option values (see notes)
+    Args:
+        priority_options: take priority over all other option values (see notes)
 
-    Returns
-    -------
-      dict: merged option values
+    Returns:
+        merged option values
 
-    Notes
-    -----
-    This function sets the log level from the merged option values prior to
-    returning.
+    Note:
+        This function sets the log level from the merged option values prior to
+        returning.
 
-    The `ffcx_options.json` files are cached on the first call. Subsequent
-    calls to this function use this cache.
+        The `ffcx_options.json` files are cached on the first call. Subsequent
+        calls to this function use this cache.
 
-    Priority ordering of options from highest to lowest is:
+        Priority ordering of options from highest to lowest is:
 
-    -  **priority_options** (API and command line options)
-    -  **$PWD/ffcx_options.json** (local options)
-    -  **$XDG_CONFIG_HOME/ffcx/ffcx_options.json** (user options)
-    -  **FFCX_DEFAULT_OPTIONS** in `ffcx.options`
+        -  **priority_options** (API and command line options)
+        -  **$PWD/ffcx_options.json** (local options)
+        -  **$XDG_CONFIG_HOME/ffcx/ffcx_options.json** (user options)
+        -  **FFCX_DEFAULT_OPTIONS** in `ffcx.options`
 
-    `XDG_CONFIG_HOME` is `~/.config/` if the environment variable is not set.
+        `XDG_CONFIG_HOME` is `~/.config/` if the environment variable is not set.
 
-    Example `ffcx_options.json` file:
+        Example `ffcx_options.json` file:
 
-      { "epsilon": 1e-7 }
+          { "epsilon": 1e-7 }
 
     """
-    options: Dict[str, Any] = {}
+    options: dict[str, npt.DTypeLike | int | float] = {}
 
-    for opt, (value, _) in FFCX_DEFAULT_OPTIONS.items():
-        options[opt] = value
+    for opt, (_, value, _, _) in FFCX_DEFAULT_OPTIONS.items():
+        options[opt] = value  # type: ignore
 
     # NOTE: _load_options uses functools.lru_cache
     user_options, pwd_options = _load_options()
 
     options.update(user_options)
     options.update(pwd_options)
     if priority_options is not None:
         options.update(priority_options)
 
-    logger.setLevel(options["verbosity"])
-
+    logger.setLevel(int(options["verbosity"]))  # type: ignore
     logger.info("Final option values")
     logger.info(pprint.pformat(options))
 
     return options
```

### Comparing `fenics-ffcx-0.7.0/test/Poisson.py` & `fenics_ffcx-0.8.0/demo/MetaData.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2004-2007 Anders Logg
+# Copyright (C) 2009 Kristian B. Oelgaard
 #
 # This file is part of FFCx.
 #
 # FFCx is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,29 +10,45 @@
 # FFCx is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with FFCx. If not, see <http://www.gnu.org/licenses/>.
-#
-# The bilinear form a(u, v) and linear form L(v) for
-# Poisson's equation.
-#
-# Compile this form with FFCx: ffcx Poisson.ufl
-from ufl import (Coefficient, Constant, Mesh, TestFunction,
-                 TrialFunction, dx, grad, inner)
-import basix.ufl
+"""Metadata demo.
 
-mesh = Mesh(basix.ufl.element('P', "triangle", 2, shape=(2, )))
+Test form for metadata.
+"""
+
+import basix.ufl
+from ufl import (
+    Coefficient,
+    Constant,
+    FunctionSpace,
+    Mesh,
+    TestFunction,
+    TrialFunction,
+    dx,
+    grad,
+    inner,
+)
 
-e = basix.ufl.element("Lagrange", "triangle", 2)
+element = basix.ufl.element("Lagrange", "triangle", 1)
+vector_element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2,))
+domain = Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+space = FunctionSpace(domain, element)
+vector_space = FunctionSpace(domain, vector_element)
 
-u = TrialFunction(e)
-v = TestFunction(e)
-f = Coefficient(e)
+u = TrialFunction(space)
+v = TestFunction(space)
+c = Coefficient(vector_space)
+c2 = Constant(domain)
 
-kappa1 = Constant(mesh.ufl_cell(), shape=(2, 2))
-kappa2 = Constant(mesh.ufl_cell(), shape=(2, 2))
+# Terms on the same subdomain using different quadrature degree
+a = (
+    inner(grad(u), grad(v)) * dx(0, degree=8)
+    + inner(c, c) * inner(grad(u), grad(v)) * dx(1, degree=4)
+    + inner(c, c) * inner(grad(u), grad(v)) * dx(1, degree=2)
+    + inner(grad(u), grad(v)) * dx(1, degree=-1)
+)
 
-a = inner(kappa1, kappa2) * inner(grad(u), grad(v)) * dx
-L = f * v * dx
+L = inner(c2, v) * dx(0, metadata={"precision": 1})
```

### Comparing `fenics-ffcx-0.7.0/test/test_add_mode.py` & `fenics_ffcx-0.8.0/test/test_add_mode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # Copyright (C) 2019 Chris Richardson
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+import basix.ufl
 import numpy as np
 import pytest
+import ufl
 
 import ffcx.codegeneration.jit
-import basix.ufl
-import ufl
-from ffcx.codegeneration.utils import cdtype_to_numpy, scalar_to_value_type
+from ffcx.codegeneration.utils import dtype_to_c_type, dtype_to_scalar_dtype
 
 
-@pytest.mark.parametrize("mode",
-                         [
-                             "double",
-                             "float",
-                             "long double",
-                             "double _Complex",
-                             "float _Complex"
-                         ])
-def test_additive_facet_integral(mode, compile_args):
+@pytest.mark.parametrize(
+    "dtype",
+    [
+        "float32",
+        "float64",
+        "complex64",
+        "complex128",
+    ],
+)
+def test_additive_facet_integral(dtype, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(u, v) * ufl.ds
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     ffi = module.ffi
     form0 = compiled_forms[0]
 
@@ -41,51 +43,60 @@
     ex = module.lib.exterior_facet
     assert integral_offsets[ex + 1] - integral_offsets[ex] == 1
     integral_id = form0.form_integral_ids[integral_offsets[ex]]
     assert integral_id == -1
 
     default_integral = form0.form_integrals[integral_offsets[ex]]
 
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((3, 3), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np_type)
+    A = np.zeros((3, 3), dtype=dtype)
+    w = np.array([], dtype=dtype)
+    c = np.array([], dtype=dtype)
     facets = np.array([0], dtype=np.int32)
     perm = np.array([0], dtype=np.uint8)
 
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-    coords = np.array([0.0, 2.0, 0.0,
-                       np.sqrt(3.0), -1.0, 0.0,
-                       -np.sqrt(3.0), -1.0, 0.0], dtype=np_gtype)
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array(
+        [0.0, 2.0, 0.0, np.sqrt(3.0), -1.0, 0.0, -np.sqrt(3.0), -1.0, 0.0], dtype=xdtype
+    )
 
-    kernel = getattr(default_integral, f"tabulate_tensor_{np_type}")
+    kernel = getattr(default_integral, f"tabulate_tensor_{dtype}")
 
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
     for i in range(3):
         facets[0] = i
-        kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-               ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-               ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-               ffi.cast(f'{geom_type} *', coords.ctypes.data),
-               ffi.cast('int *', facets.ctypes.data),
-               ffi.cast('uint8_t *', perm.ctypes.data))
-
+        kernel(
+            ffi.cast(f"{c_type} *", A.ctypes.data),
+            ffi.cast(f"{c_type} *", w.ctypes.data),
+            ffi.cast(f"{c_type} *", c.ctypes.data),
+            ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+            ffi.cast("int *", facets.ctypes.data),
+            ffi.cast("uint8_t *", perm.ctypes.data),
+        )
         assert np.isclose(A.sum(), np.sqrt(12) * (i + 1))
 
 
-@pytest.mark.parametrize("mode", ["double", "float", "long double", "double _Complex", "float _Complex"])
-def test_additive_cell_integral(mode, compile_args):
+@pytest.mark.parametrize(
+    "dtype",
+    [
+        "float32",
+        "float64",
+        "complex64",
+        "complex128",
+    ],
+)
+def test_additive_cell_integral(dtype, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     ffi = module.ffi
     form0 = compiled_forms[0]
 
@@ -94,33 +105,40 @@
     num_integrals = offsets[cell + 1] - offsets[cell]
     assert num_integrals == 1
     integral_id = form0.form_integral_ids[offsets[cell]]
     assert integral_id == -1
 
     default_integral = form0.form_integrals[offsets[cell]]
 
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((3, 3), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-    coords = np.array([0.0, 2.0, 0.0,
-                       np.sqrt(3.0), -1.0, 0.0,
-                       -np.sqrt(3.0), -1.0, 0.0], dtype=np_gtype)
-
-    kernel = getattr(default_integral, f"tabulate_tensor_{np_type}")
-
-    kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    A = np.zeros((3, 3), dtype=dtype)
+    w = np.array([], dtype=dtype)
+    c = np.array([], dtype=dtype)
+
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array(
+        [0.0, 2.0, 0.0, np.sqrt(3.0), -1.0, 0.0, -np.sqrt(3.0), -1.0, 0.0], dtype=xdtype
+    )
+
+    kernel = getattr(default_integral, f"tabulate_tensor_{dtype}")
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel(
+        ffi.cast(f"{c_type} *", A.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     A0 = np.array(A)
     for i in range(3):
-        kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-               ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-               ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-               ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+        kernel(
+            ffi.cast(f"{c_type} *", A.ctypes.data),
+            ffi.cast(f"{c_type} *", w.ctypes.data),
+            ffi.cast(f"{c_type} *", c.ctypes.data),
+            ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+            ffi.NULL,
+            ffi.NULL,
+        )
 
         assert np.all(np.isclose(A, (i + 2) * A0))
```

### Comparing `fenics-ffcx-0.7.0/test/test_blocked_elements.py` & `fenics_ffcx-0.8.0/test/test_blocked_elements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # Copyright (C) 2020 Matthew Scroggs
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+import basix.ufl
 import numpy as np
 
 import ffcx
 import ffcx.codegeneration.jit
-import basix.ufl
-import ufl
 
 
 def test_finite_element(compile_args):
     ufl_element = basix.ufl.element("Lagrange", "triangle", 1)
     jit_compiled_elements, module, code = ffcx.codegeneration.jit.compile_elements(
-        [ufl_element], cffi_extra_compile_args=compile_args)
+        [ufl_element], cffi_extra_compile_args=compile_args
+    )
     ufcx_element, ufcx_dofmap = jit_compiled_elements[0]
 
     assert ufcx_element.topological_dimension == 2
-    assert ufcx_element.geometric_dimension == 2
     assert ufcx_element.space_dimension == 3
-    assert ufcx_element.value_rank == 0
-    assert ufcx_element.value_size == 1
     assert ufcx_element.reference_value_rank == 0
     assert ufcx_element.reference_value_size == 1
     assert ufcx_element.block_size == 1
     assert ufcx_element.num_sub_elements == 0
 
     assert ufcx_dofmap.block_size == 1
     assert ufcx_dofmap.num_global_support_dofs == 0
@@ -37,25 +34,22 @@
 
     for v in range(3):
         assert ufcx_dofmap.entity_dofs[v] == v
     assert ufcx_dofmap.num_sub_dofmaps == 0
 
 
 def test_vector_element(compile_args):
-    ufl_element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2, ))
+    ufl_element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2,))
     jit_compiled_elements, module, code = ffcx.codegeneration.jit.compile_elements(
-        [ufl_element], cffi_extra_compile_args=compile_args)
+        [ufl_element], cffi_extra_compile_args=compile_args
+    )
     ufcx_element, ufcx_dofmap = jit_compiled_elements[0]
 
     assert ufcx_element.topological_dimension == 2
-    assert ufcx_element.geometric_dimension == 2
     assert ufcx_element.space_dimension == 6
-    assert ufcx_element.value_rank == 1
-    assert ufcx_element.value_shape[0] == 2
-    assert ufcx_element.value_size == 2
     assert ufcx_element.reference_value_rank == 1
     assert ufcx_element.reference_value_shape[0] == 2
     assert ufcx_element.reference_value_size == 2
     assert ufcx_element.block_size == 2
     assert ufcx_element.num_sub_elements == 2
 
     assert ufcx_dofmap.block_size == 2
@@ -69,24 +63,20 @@
         assert ufcx_dofmap.entity_dofs[v] == v
     assert ufcx_dofmap.num_sub_dofmaps == 2
 
 
 def test_tensor_element(compile_args):
     ufl_element = basix.ufl.element("Lagrange", "triangle", 1, shape=(2, 2))
     jit_compiled_elements, module, code = ffcx.codegeneration.jit.compile_elements(
-        [ufl_element], cffi_extra_compile_args=compile_args)
+        [ufl_element], cffi_extra_compile_args=compile_args
+    )
     ufcx_element, ufcx_dofmap = jit_compiled_elements[0]
 
     assert ufcx_element.topological_dimension == 2
-    assert ufcx_element.geometric_dimension == 2
     assert ufcx_element.space_dimension == 12
-    assert ufcx_element.value_rank == 2
-    assert ufcx_element.value_shape[0] == 2
-    assert ufcx_element.value_shape[1] == 2
-    assert ufcx_element.value_size == 4
     assert ufcx_element.reference_value_rank == 2
     assert ufcx_element.reference_value_shape[0] == 2
     assert ufcx_element.reference_value_shape[1] == 2
     assert ufcx_element.reference_value_size == 4
     assert ufcx_element.block_size == 4
     assert ufcx_element.num_sub_elements == 4
 
@@ -99,25 +89,24 @@
 
     for v in range(3):
         assert ufcx_dofmap.entity_dofs[v] == v
     assert ufcx_dofmap.num_sub_dofmaps == 4
 
 
 def test_vector_quadrature_element(compile_args):
-    ufl_element = ufl.VectorElement(ufl.FiniteElement("Quadrature", "tetrahedron", degree=2, quad_scheme="default"))
+    ufl_element = basix.ufl.blocked_element(
+        basix.ufl.quadrature_element("tetrahedron", degree=2, scheme="default"), shape=(3,)
+    )
     jit_compiled_elements, module, code = ffcx.codegeneration.jit.compile_elements(
-        [ufl_element], cffi_extra_compile_args=compile_args)
+        [ufl_element], cffi_extra_compile_args=compile_args
+    )
     ufcx_element, ufcx_dofmap = jit_compiled_elements[0]
 
     assert ufcx_element.topological_dimension == 3
-    assert ufcx_element.geometric_dimension == 3
     assert ufcx_element.space_dimension == 12
-    assert ufcx_element.value_rank == 1
-    assert ufcx_element.value_shape[0] == 3
-    assert ufcx_element.value_size == 3
     assert ufcx_element.reference_value_rank == 1
     assert ufcx_element.reference_value_shape[0] == 3
     assert ufcx_element.reference_value_size == 3
     assert ufcx_element.block_size == 3
     assert ufcx_element.num_sub_elements == 3
 
     assert ufcx_dofmap.block_size == 3
```

### Comparing `fenics-ffcx-0.7.0/test/test_cache.py` & `fenics_ffcx-0.8.0/test/test_cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
 import sys
 
-import ffcx.codegeneration.jit
-import ufl
 import basix.ufl
+import ufl
+
+import ffcx.codegeneration.jit
 
 
 def test_cache_modes(compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx
     forms = [a]
 
     # Load form from /tmp
-    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(forms, cffi_extra_compile_args=compile_args)
+    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
+        forms, cffi_extra_compile_args=compile_args
+    )
     tmpname = module.__name__
     tmpfile = module.__file__
     print(tmpname, tmpfile)
     del sys.modules[tmpname]
 
     # Load form from cache
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, cache_dir="./compile-cache", cffi_extra_compile_args=compile_args)
+        forms, cache_dir="./compile-cache", cffi_extra_compile_args=compile_args
+    )
     newname = module.__name__
     newfile = module.__file__
     print(newname, newfile)
 
     assert newname == tmpname
     assert newfile != tmpfile
```

### Comparing `fenics-ffcx-0.7.0/test/test_jit_forms.py` & `fenics_ffcx-0.8.0/test/test_jit_forms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,56 @@
 # Copyright (C) 2018-2020 Garth N. Wells & Matthew Scroggs
 #
 # This file is part of FFCx. (https://www.fenicsproject.org)
 #
 # SPDX-License-Identifier:    LGPL-3.0-or-later
 
+import basix.ufl
 import numpy as np
 import pytest
 import sympy
+import ufl
 from sympy.abc import x, y, z
 
-import basix.ufl
 import ffcx.codegeneration.jit
-import ufl
-from ffcx.codegeneration.utils import cdtype_to_numpy, scalar_to_value_type
+from ffcx.codegeneration.utils import dtype_to_c_type, dtype_to_scalar_dtype
 
 
-@pytest.mark.parametrize("mode,expected_result", [
-    ("double", np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.float64)),
-    ("double _Complex",
-     np.array(
-         [[1.0 + 0j, -0.5 + 0j, -0.5 + 0j], [-0.5 + 0j, 0.5 + 0j, 0.0 + 0j],
-          [-0.5 + 0j, 0.0 + 0j, 0.5 + 0j]],
-         dtype=np.complex128)),
-])
-def test_laplace_bilinear_form_2d(mode, expected_result, compile_args):
+@pytest.mark.parametrize(
+    "dtype,expected_result",
+    [
+        (
+            "float64",
+            np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.float64),
+        ),
+        (
+            "complex128",
+            np.array(
+                [
+                    [1.0 + 0j, -0.5 + 0j, -0.5 + 0j],
+                    [-0.5 + 0j, 0.5 + 0j, 0.0 + 0j],
+                    [-0.5 + 0j, 0.0 + 0j, 0.5 + 0j],
+                ],
+                dtype=np.complex128,
+            ),
+        ),
+    ],
+)
+def test_laplace_bilinear_form_2d(dtype, expected_result, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     kappa = ufl.Constant(domain, shape=(2, 2))
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
 
     a = ufl.tr(kappa) * ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     ffi = module.ffi
     form0 = compiled_forms[0]
 
@@ -45,262 +58,286 @@
     cell = module.lib.cell
     assert offsets[cell + 1] - offsets[cell] == 1
     integral_id = form0.form_integral_ids[offsets[cell]]
     assert integral_id == -1
 
     default_integral = form0.form_integrals[offsets[cell]]
 
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((3, 3), dtype=np_type)
-    w = np.array([], dtype=np_type)
+    A = np.zeros((3, 3), dtype=dtype)
+    w = np.array([], dtype=dtype)
 
     kappa_value = np.array([[1.0, 2.0], [3.0, 4.0]])
-    c = np.array(kappa_value.flatten(), dtype=np_type)
+    c = np.array(kappa_value.flatten(), dtype=dtype)
 
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-
-    kernel = getattr(default_integral, f"tabulate_tensor_{np_type}")
-
-    kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel = getattr(default_integral, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type} *", A.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     assert np.allclose(A, np.trace(kappa_value) * expected_result)
 
 
-@pytest.mark.parametrize("mode,expected_result", [
-    ("float",
-     np.array(
-         [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
-          [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
-         dtype=np.float32)),
-    ("long double",
-     np.array(
-         [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
-          [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
-         dtype=np.longdouble)),
-    ("double",
-     np.array(
-         [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
-          [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
-         dtype=np.float64)),
-    ("double _Complex",
-     np.array(
-         [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
-          [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
-         dtype=np.complex128)),
-    ("float _Complex",
-     np.array(
-         [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
-          [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
-         dtype=np.complex64)),
-])
-def test_mass_bilinear_form_2d(mode, expected_result, compile_args):
+@pytest.mark.parametrize(
+    "dtype,expected_result",
+    [
+        (
+            "float32",
+            np.array(
+                [
+                    [1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0],
+                ],
+                dtype=np.float32,
+            ),
+        ),
+        # ("longdouble",
+        #  np.array(
+        #      [[1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0], [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
+        #       [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0]],
+        #      dtype=np.longdouble)),
+        (
+            "float64",
+            np.array(
+                [
+                    [1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0],
+                ],
+                dtype=np.float64,
+            ),
+        ),
+        (
+            "complex128",
+            np.array(
+                [
+                    [1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0],
+                ],
+                dtype=np.complex128,
+            ),
+        ),
+        (
+            "complex64",
+            np.array(
+                [
+                    [1.0 / 12.0, 1.0 / 24.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 12.0, 1.0 / 24.0],
+                    [1.0 / 24.0, 1.0 / 24.0, 1.0 / 12.0],
+                ],
+                dtype=np.complex64,
+            ),
+        ),
+    ],
+)
+def test_mass_bilinear_form_2d(dtype, expected_result, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(u, v) * ufl.dx
     L = ufl.conj(v) * ufl.dx
     forms = [a, L]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
-
-    for f, compiled_f in zip(forms, compiled_forms):
-        assert compiled_f.rank == len(f.arguments())
-
-    form0 = compiled_forms[0].form_integrals[0]
-    form1 = compiled_forms[1].form_integrals[0]
-
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((3, 3), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    ffi = module.ffi
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-
-    kernel0 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form0, f"tabulate_tensor_{np_type}"))
-    kernel0(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
-
-    b = np.zeros(3, dtype=np_type)
-    kernel1 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form1, f"tabulate_tensor_{np_type}"))
-    kernel1(ffi.cast('{type} *'.format(type=mode), b.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
-
-    assert np.allclose(A, expected_result)
-    assert np.allclose(b, 1.0 / 6.0)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
 
-@pytest.mark.parametrize("mode,expected_result", [
-    ("double", np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.float64)
-     - (1.0 / 24.0) * np.array([[2, 1, 1], [1, 2, 1], [1, 1, 2]], dtype=np.float64)),
-    ("double _Complex",
-     np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.complex128)
-     - (1.0j / 24.0) * np.array([[2, 1, 1], [1, 2, 1], [1, 1, 2]], dtype=np.complex128)),
-])
-def test_helmholtz_form_2d(mode, expected_result, compile_args):
+@pytest.mark.parametrize(
+    "dtype,expected_result",
+    [
+        (
+            "float64",
+            np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.float64)
+            - (1.0 / 24.0) * np.array([[2, 1, 1], [1, 2, 1], [1, 1, 2]], dtype=np.float64),
+        ),
+        (
+            "complex128",
+            np.array([[1.0, -0.5, -0.5], [-0.5, 0.5, 0.0], [-0.5, 0.0, 0.5]], dtype=np.complex128)
+            - (1.0j / 24.0) * np.array([[2, 1, 1], [1, 2, 1], [1, 1, 2]], dtype=np.complex128),
+        ),
+    ],
+)
+def test_helmholtz_form_2d(dtype, expected_result, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
-    if mode == "double":
-        k = 1.0
-    elif mode == "double _Complex":
+    if np.issubdtype(dtype, np.complexfloating):
         k = ufl.constantvalue.ComplexValue(1j)
+    elif np.issubdtype(dtype, np.floating):
+        k = 1.0
     else:
-        raise RuntimeError("Unknown mode type")
+        raise RuntimeError(
+            "Unknown mode type",
+        )
 
     a = (ufl.inner(ufl.grad(u), ufl.grad(v)) - ufl.inner(k * u, v)) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     form0 = compiled_forms[0].form_integrals[0]
 
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((3, 3), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    ffi = module.ffi
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-    kernel = getattr(form0, f"tabulate_tensor_{np_type}")
-
-    kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    A = np.zeros((3, 3), dtype=dtype)
+    w = np.array([], dtype=dtype)
+    c = np.array([], dtype=dtype)
 
-    assert np.allclose(A, expected_result)
+    ffi = module.ffi
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel = getattr(form0, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type} *", A.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
+
+    np.testing.assert_allclose(A, expected_result)
 
 
-@pytest.mark.parametrize("mode,expected_result", [
-    ("double", np.array([[0.5, -1 / 6, -1 / 6, -1 / 6],
-                         [-1 / 6, 1 / 6, 0.0, 0.0],
-                         [-1 / 6, 0.0, 1 / 6, 0.0],
-                         [-1 / 6, 0.0, 0.0, 1 / 6]], dtype=np.float64)),
-    ("double _Complex",
-     np.array(
-         [[0.5 + 0j, -1 / 6 + 0j, -1 / 6 + 0j, -1 / 6 + 0j],
-          [-1 / 6 + 0j, 1 / 6 + 0j, 0.0 + 0j, 0.0 + 0j],
-          [-1 / 6 + 0j, 0.0 + 0j, 1 / 6 + 0j, 0.0 + 0j],
-          [-1 / 6 + 0j, 0.0 + 0j, 0.0 + 0j, 1 / 6 + 0j]],
-         dtype=np.complex128)),
-])
-def test_laplace_bilinear_form_3d(mode, expected_result, compile_args):
+@pytest.mark.parametrize(
+    "dtype,expected_result",
+    [
+        (
+            "float64",
+            np.array(
+                [
+                    [0.5, -1 / 6, -1 / 6, -1 / 6],
+                    [-1 / 6, 1 / 6, 0.0, 0.0],
+                    [-1 / 6, 0.0, 1 / 6, 0.0],
+                    [-1 / 6, 0.0, 0.0, 1 / 6],
+                ],
+                dtype=np.float64,
+            ),
+        ),
+        (
+            "complex128",
+            np.array(
+                [
+                    [0.5 + 0j, -1 / 6 + 0j, -1 / 6 + 0j, -1 / 6 + 0j],
+                    [-1 / 6 + 0j, 1 / 6 + 0j, 0.0 + 0j, 0.0 + 0j],
+                    [-1 / 6 + 0j, 0.0 + 0j, 1 / 6 + 0j, 0.0 + 0j],
+                    [-1 / 6 + 0j, 0.0 + 0j, 0.0 + 0j, 1 / 6 + 0j],
+                ],
+                dtype=np.complex128,
+            ),
+        ),
+    ],
+)
+def test_laplace_bilinear_form_3d(dtype, expected_result, compile_args):
     element = basix.ufl.element("Lagrange", "tetrahedron", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     form0 = compiled_forms[0].form_integrals[0]
 
-    np_type = cdtype_to_numpy(mode)
-    A = np.zeros((4, 4), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    ffi = module.ffi
-    coords = np.array([0.0, 0.0, 0.0,
-                       1.0, 0.0, 0.0,
-                       0.0, 1.0, 0.0,
-                       0.0, 0.0, 1.0], dtype=np_gtype)
-
-    kernel = getattr(form0, f"tabulate_tensor_{np_type}")
-    kernel(ffi.cast('{type} *'.format(type=mode), A.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    A = np.zeros((4, 4), dtype=dtype)
+    w = np.array([], dtype=dtype)
+    c = np.array([], dtype=dtype)
+
+    ffi = module.ffi
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel = getattr(form0, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type} *", A.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     assert np.allclose(A, expected_result)
 
 
 def test_form_coefficient(compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TestFunction(space), ufl.TrialFunction(space)
     g = ufl.Coefficient(space)
     a = g * ufl.inner(u, v) * ufl.dx
     forms = [a]
-    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(forms, cffi_extra_compile_args=compile_args)
+    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
+        forms, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     form0 = compiled_forms[0].form_integrals[0]
     A = np.zeros((3, 3), dtype=np.float64)
     w = np.array([1.0, 1.0, 1.0], dtype=np.float64)
     c = np.array([], dtype=np.float64)
     perm = np.array([0], dtype=np.uint8)
 
     ffi = module.ffi
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np.float64)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=np.float64)
 
     kernel = getattr(form0, "tabulate_tensor_float64")
-    kernel(ffi.cast('double  *', A.ctypes.data),
-           ffi.cast('double  *', w.ctypes.data),
-           ffi.cast('double  *', c.ctypes.data),
-           ffi.cast('double  *', coords.ctypes.data), ffi.NULL,
-           ffi.cast('uint8_t *', perm.ctypes.data))
+    kernel(
+        ffi.cast("double  *", A.ctypes.data),
+        ffi.cast("double  *", w.ctypes.data),
+        ffi.cast("double  *", c.ctypes.data),
+        ffi.cast("double  *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.cast("uint8_t *", perm.ctypes.data),
+    )
 
     A_analytic = np.array([[2, 1, 1], [1, 2, 1], [1, 1, 2]], dtype=np.float64) / 24.0
-    A_diff = (A - A_analytic)
+    A_diff = A - A_analytic
     assert np.isclose(A_diff.max(), 0.0)
     assert np.isclose(A_diff.min(), 0.0)
 
 
 def test_subdomains(compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a0 = ufl.inner(u, v) * ufl.dx + ufl.inner(u, v) * ufl.dx(2)
     a1 = ufl.inner(u, v) * ufl.dx(2) + ufl.inner(u, v) * ufl.dx
     a2 = ufl.inner(u, v) * ufl.dx(2) + ufl.inner(u, v) * ufl.dx(1)
     a3 = ufl.inner(u, v) * ufl.ds(210) + ufl.inner(u, v) * ufl.ds(0)
     forms = [a0, a1, a2, a3]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': 'double'}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": "float64"}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     form0 = compiled_forms[0]
     offsets = form0.form_integral_offsets
     cell = module.lib.cell
@@ -321,583 +358,685 @@
     offsets = form3.form_integral_offsets
     assert offsets[cell + 1] - offsets[cell] == 0
     exf = module.lib.exterior_facet
     ids = [form3.form_integral_ids[j] for j in range(offsets[exf], offsets[exf + 1])]
     assert ids[0] == 0 and ids[1] == 210
 
 
-@pytest.mark.parametrize("mode", ["double", "double _Complex"])
-def test_interior_facet_integral(mode, compile_args):
+@pytest.mark.parametrize("dtype", ["float64", "complex128"])
+def test_interior_facet_integral(dtype, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a0 = ufl.inner(ufl.jump(ufl.grad(u)), ufl.jump(ufl.grad(v))) * ufl.dS
     forms = [a0]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     for f, compiled_f in zip(forms, compiled_forms):
         assert compiled_f.rank == len(f.arguments())
 
     ffi = module.ffi
 
     form0 = compiled_forms[0]
 
     ffi = module.ffi
-    np_type = cdtype_to_numpy(mode)
 
     integral0 = form0.form_integrals[0]
-    A = np.zeros((6, 6), dtype=np_type)
-    w = np.array([], dtype=np_type)
-    c = np.array([], dtype=np.float64)
+    A = np.zeros((6, 6), dtype=dtype)
+    w = np.array([], dtype=dtype)
+    c = np.array([], dtype=dtype)
 
     facets = np.array([0, 2], dtype=np.intc)
     perms = np.array([0, 1], dtype=np.uint8)
 
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array(
+        [
+            [0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+            [1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 1.0, 1.0, 0.0],
+        ],
+        dtype=xdtype,
+    )
 
-    coords = np.array([[0.0, 0.0, 0.0,
-                        1.0, 0.0, 0.0,
-                        0.0, 1.0, 0.0],
-                       [1.0, 0.0, 0.0,
-                       0.0, 1.0, 0.0,
-                       1.0, 1.0, 0.0]], dtype=np_gtype)
-
-    kernel = getattr(integral0, f"tabulate_tensor_{np_type}")
-    kernel(ffi.cast(f'{mode}  *', A.ctypes.data),
-           ffi.cast(f'{mode}  *', w.ctypes.data),
-           ffi.cast(f'{mode}  *', c.ctypes.data),
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.cast('int *', facets.ctypes.data),
-           ffi.cast('uint8_t *', perms.ctypes.data))
+    c_type = dtype_to_c_type(dtype)
+    c_xtype = dtype_to_c_type(xdtype)
+    kernel = getattr(integral0, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type}  *", A.ctypes.data),
+        ffi.cast(f"{c_type}  *", w.ctypes.data),
+        ffi.cast(f"{c_type}  *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.cast("int *", facets.ctypes.data),
+        ffi.cast("uint8_t *", perms.ctypes.data),
+    )
 
 
-@pytest.mark.parametrize("mode", ["double", "double _Complex"])
-def test_conditional(mode, compile_args):
+@pytest.mark.parametrize(
+    "dtype",
+    [
+        "float64",
+        "complex128",
+    ],
+)
+def test_conditional(dtype, compile_args):
     element = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     x = ufl.SpatialCoordinate(domain)
-    condition = ufl.Or(ufl.ge(ufl.real(x[0] + x[1]), 0.1),
-                       ufl.ge(ufl.real(x[1] + x[1]**2), 0.1))
+    condition = ufl.Or(ufl.ge(ufl.real(x[0] + x[1]), 0.1), ufl.ge(ufl.real(x[1] + x[1] ** 2), 0.1))
     c1 = ufl.conditional(condition, 2.0, 1.0)
     a = c1 * ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx
 
     x1x2 = ufl.real(x[0] + ufl.as_ufl(2) * x[1])
     c2 = ufl.conditional(ufl.ge(x1x2, 0), 6.0, 0.0)
     b = c2 * ufl.conj(v) * ufl.dx
 
     forms = [a, b]
 
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     form0 = compiled_forms[0].form_integrals[0]
     form1 = compiled_forms[1].form_integrals[0]
 
     ffi = module.ffi
-    np_type = cdtype_to_numpy(mode)
-
-    A1 = np.zeros((3, 3), dtype=np_type)
-    w1 = np.array([1.0, 1.0, 1.0], dtype=np_type)
-    c = np.array([], dtype=np.float64)
 
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-
-    kernel0 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form0, f"tabulate_tensor_{np_type}"))
-    kernel0(ffi.cast('{type} *'.format(type=mode), A1.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w1.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    A1 = np.zeros((3, 3), dtype=dtype)
+    w1 = np.array([1.0, 1.0, 1.0], dtype=dtype)
+    c = np.array([], dtype=dtype)
+
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel0 = ffi.cast(
+        f"ufcx_tabulate_tensor_{dtype} *", getattr(form0, f"tabulate_tensor_{dtype}")
+    )
+    kernel0(
+        ffi.cast(f"{c_type} *", A1.ctypes.data),
+        ffi.cast(f"{c_type} *", w1.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
-    expected_result = np.array([[2, -1, -1], [-1, 1, 0], [-1, 0, 1]], dtype=np_type)
+    expected_result = np.array([[2, -1, -1], [-1, 1, 0], [-1, 0, 1]], dtype=dtype)
     assert np.allclose(A1, expected_result)
 
-    A2 = np.zeros(3, dtype=np_type)
-    w2 = np.array([1.0, 1.0, 1.0], dtype=np_type)
+    A2 = np.zeros(3, dtype=dtype)
+    w2 = np.array([1.0, 1.0, 1.0], dtype=dtype)
 
-    kernel1 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form1, f"tabulate_tensor_{np_type}"))
-    kernel1(ffi.cast('{type} *'.format(type=mode), A2.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w2.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    kernel1 = ffi.cast(
+        f"ufcx_tabulate_tensor_{dtype} *", getattr(form1, f"tabulate_tensor_{dtype}")
+    )
+    kernel1(
+        ffi.cast(f"{c_type} *", A2.ctypes.data),
+        ffi.cast(f"{c_type} *", w2.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
-    expected_result = np.ones(3, dtype=np_type)
+    expected_result = np.ones(3, dtype=dtype)
     assert np.allclose(A2, expected_result)
 
 
 def test_custom_quadrature(compile_args):
-    ve = basix.ufl.element("P", "triangle", 1, shape=(2, ))
+    ve = basix.ufl.element("P", "triangle", 1, shape=(2,))
     mesh = ufl.Mesh(ve)
 
     e = basix.ufl.element("P", mesh.ufl_cell().cellname(), 2)
     V = ufl.FunctionSpace(mesh, e)
     u, v = ufl.TrialFunction(V), ufl.TestFunction(V)
 
     points = [[0.0, 0.0], [1.0, 0.0], [0.0, 1.0], [0.5, 0.5], [0.0, 0.5], [0.5, 0.0]]
     weights = [1 / 12] * 6
-    a = u * v * ufl.dx(metadata={"quadrature_rule": "custom",
-                                 "quadrature_points": points, "quadrature_weights": weights})
+    a = (
+        u
+        * v
+        * ufl.dx(
+            metadata={
+                "quadrature_rule": "custom",
+                "quadrature_points": points,
+                "quadrature_weights": weights,
+            }
+        )
+    )
 
     forms = [a]
-    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(forms, cffi_extra_compile_args=compile_args)
+    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
+        forms, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     form = compiled_forms[0]
     default_integral = form.form_integrals[0]
 
     A = np.zeros((6, 6), dtype=np.float64)
     w = np.array([], dtype=np.float64)
     c = np.array([], dtype=np.float64)
 
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np.float64)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=np.float64)
 
     kernel = getattr(default_integral, "tabulate_tensor_float64")
-    kernel(ffi.cast("double *", A.ctypes.data),
-           ffi.cast("double *", w.ctypes.data),
-           ffi.cast("double *", c.ctypes.data),
-           ffi.cast("double *", coords.ctypes.data), ffi.NULL, ffi.NULL)
+    kernel(
+        ffi.cast("double *", A.ctypes.data),
+        ffi.cast("double *", w.ctypes.data),
+        ffi.cast("double *", c.ctypes.data),
+        ffi.cast("double *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     # Check that A is diagonal
     assert np.count_nonzero(A - np.diag(np.diagonal(A))) == 0
 
 
 def test_curl_curl(compile_args):
     V = basix.ufl.element("N1curl", "triangle", 2)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, V)
     u, v = ufl.TrialFunction(space), ufl.TestFunction(space)
     a = ufl.inner(ufl.curl(u), ufl.curl(v)) * ufl.dx
 
     forms = [a]
-    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(forms, cffi_extra_compile_args=compile_args)
+    compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
+        forms, cffi_extra_compile_args=compile_args
+    )
 
 
-def lagrange_triangle_symbolic(order, corners=[(1, 0), (2, 0), (0, 1)], fun=lambda i: i):
+def lagrange_triangle_symbolic(order, corners=((1, 0), (2, 0), (0, 1)), fun=lambda i: i):
     from sympy import S
+
     poly_basis = [x**i * y**j for i in range(order + 1) for j in range(order + 1 - i)]
     # vertices
     eval_points = [S(c) for c in corners]
     # edges
     for e in [(1, 2), (0, 2), (0, 1)]:
         p0 = corners[e[0]]
         p1 = corners[e[1]]
         if order > 3:
             raise NotImplementedError
         elif order == 3:
-            eval_points += [tuple(S(a) + (b - a) * i for a, b in zip(p0, p1))
-                            for i in [(1 - 1 / sympy.sqrt(5)) / 2, (1 + 1 / sympy.sqrt(5)) / 2]]
+            eval_points += [
+                tuple(S(a) + (b - a) * i for a, b in zip(p0, p1))
+                for i in [(1 - 1 / sympy.sqrt(5)) / 2, (1 + 1 / sympy.sqrt(5)) / 2]
+            ]
         else:
-            eval_points += [tuple(S(a) + sympy.Rational((b - a) * i, order) for a, b in zip(p0, p1))
-                            for i in range(1, order)]
+            eval_points += [
+                tuple(S(a) + sympy.Rational((b - a) * i, order) for a, b in zip(p0, p1))
+                for i in range(1, order)
+            ]
     # face
     for f in [(0, 1, 2)]:
         p0 = corners[f[0]]
         p1 = corners[f[1]]
         p2 = corners[f[2]]
-        eval_points += [tuple(S(a) + sympy.Rational((b - a) * i, order)
-                        + sympy.Rational((c - a) * j, order) for a, b, c in zip(p0, p1, p2))
-                        for i in range(1, order) for j in range(1, order - i)]
+        eval_points += [
+            tuple(
+                S(a) + sympy.Rational((b - a) * i, order) + sympy.Rational((c - a) * j, order)
+                for a, b, c in zip(p0, p1, p2)
+            )
+            for i in range(1, order)
+            for j in range(1, order - i)
+        ]
 
     dual_mat = [[f.subs(x, p[0]).subs(y, p[1]) for p in eval_points] for f in poly_basis]
     dual_mat = sympy.Matrix(dual_mat)
     mat = dual_mat.inv()
     functions = [sum(i * j for i, j in zip(mat.row(k), poly_basis)) for k in range(mat.rows)]
     results = []
     for f in functions:
         integrand = fun(f)
         results.append(integrand.integrate((x, 1 - y, 2 - 2 * y), (y, 0, 1)))
     return results
 
 
-@pytest.mark.parametrize("mode", ["double"])
-@pytest.mark.parametrize("sym_fun,ufl_fun", [
-    (lambda i: i, lambda i: i),
-    (lambda i: i.diff(x), lambda i: ufl.grad(i)[0]),
-    (lambda i: i.diff(y), lambda i: ufl.grad(i)[1])])
+@pytest.mark.parametrize("dtype", ["float64"])
+@pytest.mark.parametrize(
+    "sym_fun,ufl_fun",
+    [
+        (lambda i: i, lambda i: i),
+        (lambda i: i.diff(x), lambda i: ufl.grad(i)[0]),
+        (lambda i: i.diff(y), lambda i: ufl.grad(i)[1]),
+    ],
+)
 @pytest.mark.parametrize("order", [1, 2, 3])
-def test_lagrange_triangle(compile_args, order, mode, sym_fun, ufl_fun):
+def test_lagrange_triangle(compile_args, order, dtype, sym_fun, ufl_fun):
     sym = lagrange_triangle_symbolic(order, fun=sym_fun)
     element = basix.ufl.element("Lagrange", "triangle", order)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, element)
     v = ufl.TestFunction(space)
 
     a = ufl_fun(v) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     form0 = compiled_forms[0]
 
     assert form0.form_integral_offsets[module.lib.cell + 1] == 1
     default_integral = form0.form_integrals[0]
 
-    np_type = cdtype_to_numpy(mode)
-    b = np.zeros((order + 2) * (order + 1) // 2, dtype=np_type)
-    w = np.array([], dtype=np_type)
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-    coords = np.array([[1.0, 0.0, 0.0],
-                       [2.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-    kernel = getattr(default_integral, f"tabulate_tensor_{np_type}")
-    kernel(ffi.cast('{type} *'.format(type=mode), b.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.NULL,
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    b = np.zeros((order + 2) * (order + 1) // 2, dtype=dtype)
+    w = np.array([], dtype=dtype)
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([[1.0, 0.0, 0.0], [2.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel = getattr(default_integral, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type} *", b.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.NULL,
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     # Check that the result is the same as for sympy
     assert np.allclose(b, [float(i) for i in sym])
 
 
-def lagrange_tetrahedron_symbolic(order, corners=[(1, 0, 0), (2, 0, 0), (0, 1, 0), (0, 0, 1)], fun=lambda i: i):
+def lagrange_tetrahedron_symbolic(
+    order, corners=((1, 0, 0), (2, 0, 0), (0, 1, 0), (0, 0, 1)), fun=lambda i: i
+):
     from sympy import S
+
     poly_basis = [
-        x**i * y**j * z**k for i in range(order + 1) for j in range(order + 1 - i)
-        for k in range(order + 1 - i - j)]
+        x**i * y**j * z**k
+        for i in range(order + 1)
+        for j in range(order + 1 - i)
+        for k in range(order + 1 - i - j)
+    ]
     # vertices
     eval_points = [S(c) for c in corners]
     # edges
     for e in [(2, 3), (1, 3), (1, 2), (0, 3), (0, 2), (0, 1)]:
         p0 = corners[e[0]]
         p1 = corners[e[1]]
         if order > 3:
             raise NotImplementedError
         elif order == 3:
-            eval_points += [tuple(S(a) + (b - a) * i for a, b in zip(p0, p1))
-                            for i in [(1 - 1 / sympy.sqrt(5)) / 2, (1 + 1 / sympy.sqrt(5)) / 2]]
+            eval_points += [
+                tuple(S(a) + (b - a) * i for a, b in zip(p0, p1))
+                for i in [(1 - 1 / sympy.sqrt(5)) / 2, (1 + 1 / sympy.sqrt(5)) / 2]
+            ]
         else:
-            eval_points += [tuple(S(a) + sympy.Rational((b - a) * i, order) for a, b in zip(p0, p1))
-                            for i in range(1, order)]
+            eval_points += [
+                tuple(S(a) + sympy.Rational((b - a) * i, order) for a, b in zip(p0, p1))
+                for i in range(1, order)
+            ]
     # face
     for f in [(1, 2, 3), (0, 2, 3), (0, 1, 3), (0, 1, 2)]:
         p0 = corners[f[0]]
         p1 = corners[f[1]]
         p2 = corners[f[2]]
-        eval_points += [tuple(S(a) + sympy.Rational((b - a) * i, order)
-                        + sympy.Rational((c - a) * j, order) for a, b, c in zip(p0, p1, p2))
-                        for i in range(1, order) for j in range(1, order - i)]
+        eval_points += [
+            tuple(
+                S(a) + sympy.Rational((b - a) * i, order) + sympy.Rational((c - a) * j, order)
+                for a, b, c in zip(p0, p1, p2)
+            )
+            for i in range(1, order)
+            for j in range(1, order - i)
+        ]
     # interior
     for v in [(0, 1, 2, 3)]:
         p0 = corners[v[0]]
         p1 = corners[v[1]]
         p2 = corners[v[2]]
         p3 = corners[v[3]]
-        eval_points += [tuple(S(a) + sympy.Rational((b - a) * i, order) + sympy.Rational((c - a) * j, order)
-                        + sympy.Rational((d - a) * k, order) for a, b, c, d in zip(p0, p1, p2, p3))
-                        for i in range(1, order) for j in range(1, order - i) for k in range(1, order - i - j)]
-
-    dual_mat = [[f.subs(x, p[0]).subs(y, p[1]).subs(z, p[2]) for p in eval_points] for f in poly_basis]
+        eval_points += [
+            tuple(
+                S(a)
+                + sympy.Rational((b - a) * i, order)
+                + sympy.Rational((c - a) * j, order)
+                + sympy.Rational((d - a) * k, order)
+                for a, b, c, d in zip(p0, p1, p2, p3)
+            )
+            for i in range(1, order)
+            for j in range(1, order - i)
+            for k in range(1, order - i - j)
+        ]
+
+    dual_mat = [
+        [f.subs(x, p[0]).subs(y, p[1]).subs(z, p[2]) for p in eval_points] for f in poly_basis
+    ]
     dual_mat = sympy.Matrix(dual_mat)
     mat = dual_mat.inv()
     functions = [sum(i * j for i, j in zip(mat.row(k), poly_basis)) for k in range(mat.rows)]
     results = []
     for f in functions:
         integrand = fun(f)
-        results.append(integrand.integrate((x, 1 - y - z, 2 - 2 * y - 2 * z), (y, 0, 1 - z), (z, 0, 1)))
+        results.append(
+            integrand.integrate((x, 1 - y - z, 2 - 2 * y - 2 * z), (y, 0, 1 - z), (z, 0, 1))
+        )
     return results
 
 
-@pytest.mark.parametrize("mode", ["double"])
-@pytest.mark.parametrize("sym_fun,ufl_fun", [
-    (lambda i: i, lambda i: i),
-    (lambda i: i.diff(x), lambda i: ufl.grad(i)[0]),
-    (lambda i: i.diff(y), lambda i: ufl.grad(i)[1])])
+@pytest.mark.parametrize("dtype", ["float64"])
+@pytest.mark.parametrize(
+    "sym_fun,ufl_fun",
+    [
+        (lambda i: i, lambda i: i),
+        (lambda i: i.diff(x), lambda i: ufl.grad(i)[0]),
+        (lambda i: i.diff(y), lambda i: ufl.grad(i)[1]),
+    ],
+)
 @pytest.mark.parametrize("order", [1, 2, 3])
-def test_lagrange_tetrahedron(compile_args, order, mode, sym_fun, ufl_fun):
+def test_lagrange_tetrahedron(compile_args, order, dtype, sym_fun, ufl_fun):
     sym = lagrange_tetrahedron_symbolic(order, fun=sym_fun)
     element = basix.ufl.element("Lagrange", "tetrahedron", order)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "tetrahedron", 1, shape=(3,)))
     space = ufl.FunctionSpace(domain, element)
     v = ufl.TestFunction(space)
 
     a = ufl_fun(v) * ufl.dx
     forms = [a]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     form0 = compiled_forms[0]
 
     assert form0.form_integral_offsets[module.lib.cell + 1] == 1
 
     default_integral = form0.form_integrals[0]
 
-    np_type = cdtype_to_numpy(mode)
-    b = np.zeros((order + 3) * (order + 2) * (order + 1) // 6, dtype=np_type)
-    w = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    coords = np.array([1.0, 0.0, 0.0,
-                       2.0, 0.0, 0.0,
-                       0.0, 1.0, 0.0,
-                       0.0, 0.0, 1.0], dtype=np_gtype)
-
-    kernel = getattr(default_integral, f"tabulate_tensor_{np_type}")
-    kernel(ffi.cast('{type} *'.format(type=mode), b.ctypes.data),
-           ffi.cast('{type} *'.format(type=mode), w.ctypes.data),
-           ffi.NULL,
-           ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    b = np.zeros((order + 3) * (order + 2) * (order + 1) // 6, dtype=dtype)
+    w = np.array([], dtype=dtype)
+
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([1.0, 0.0, 0.0, 2.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 1.0], dtype=xdtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel = getattr(default_integral, f"tabulate_tensor_{dtype}")
+    kernel(
+        ffi.cast(f"{c_type} *", b.ctypes.data),
+        ffi.cast(f"{c_type} *", w.ctypes.data),
+        ffi.NULL,
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     # Check that the result is the same as for sympy
     assert np.allclose(b, [float(i) for i in sym])
 
 
 def test_prism(compile_args):
     element = basix.ufl.element("Lagrange", "prism", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "prism", 1, shape=(3, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "prism", 1, shape=(3,)))
     space = ufl.FunctionSpace(domain, element)
     v = ufl.TestFunction(space)
-
     L = v * ufl.dx
     forms = [L]
     compiled_forms, module, _ = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': 'double'}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": "float64"}, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     form0 = compiled_forms[0]
     assert form0.form_integral_offsets[module.lib.cell + 1] == 1
 
     default_integral = form0.form_integrals[0]
     b = np.zeros(6, dtype=np.float64)
-    coords = np.array([1.0, 0.0, 0.0,
-                       0.0, 1.0, 0.0,
-                       0.0, 0.0, 0.0,
-                       1.0, 0.0, 1.0,
-                       0.0, 1.0, 1.0,
-                       0.0, 0.0, 1.0], dtype=np.float64)
-
+    coords = np.array(
+        [1.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 1.0, 0.0, 1.0, 1.0, 0.0, 0.0, 1.0],
+        dtype=np.float64,
+    )
     kernel = getattr(default_integral, "tabulate_tensor_float64")
-    kernel(ffi.cast('double *', b.ctypes.data),
-           ffi.NULL,
-           ffi.NULL,
-           ffi.cast('double *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    kernel(
+        ffi.cast("double *", b.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+        ffi.cast("double *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     assert np.isclose(sum(b), 0.5)
 
 
 def test_complex_operations(compile_args):
-    mode = "double _Complex"
+    dtype = "complex128"
     cell = "triangle"
-    c_element = basix.ufl.element("Lagrange", cell, 1, shape=(2, ))
+    c_element = basix.ufl.element("Lagrange", cell, 1, shape=(2,))
     mesh = ufl.Mesh(c_element)
-    element = basix.ufl.element("DG", cell, 0, shape=(2, ))
+    element = basix.ufl.element("DG", cell, 0, shape=(2,))
     V = ufl.FunctionSpace(mesh, element)
     u = ufl.Coefficient(V)
     J1 = ufl.real(u)[0] * ufl.imag(u)[1] * ufl.conj(u)[0] * ufl.dx
     J2 = ufl.real(u[0]) * ufl.imag(u[1]) * ufl.conj(u[0]) * ufl.dx
     forms = [J1, J2]
 
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, options={'scalar_type': mode}, cffi_extra_compile_args=compile_args)
+        forms, options={"scalar_type": dtype}, cffi_extra_compile_args=compile_args
+    )
 
     form0 = compiled_forms[0].form_integrals[0]
     form1 = compiled_forms[1].form_integrals[0]
 
     ffi = module.ffi
-    np_type = cdtype_to_numpy(mode)
-    w1 = np.array([3 + 5j, 8 - 7j], dtype=np_type)
-    c = np.array([], dtype=np_type)
-
-    geom_type = scalar_to_value_type(mode)
-    np_gtype = cdtype_to_numpy(geom_type)
-
-    coords = np.array([[0.0, 0.0, 0.0],
-                       [1.0, 0.0, 0.0],
-                       [0.0, 1.0, 0.0]], dtype=np_gtype)
-    J_1 = np.zeros((1), dtype=np_type)
-    kernel0 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form0, f"tabulate_tensor_{np_type}"))
-    kernel0(ffi.cast('{type} *'.format(type=mode), J_1.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w1.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    w1 = np.array([3 + 5j, 8 - 7j], dtype=dtype)
+    c = np.array([], dtype=dtype)
+
+    xdtype = dtype_to_scalar_dtype(dtype)
+    coords = np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]], dtype=xdtype)
+    J_1 = np.zeros((1), dtype=dtype)
+
+    c_type, c_xtype = dtype_to_c_type(dtype), dtype_to_c_type(xdtype)
+    kernel0 = ffi.cast(
+        f"ufcx_tabulate_tensor_{dtype} *", getattr(form0, f"tabulate_tensor_{dtype}")
+    )
+    kernel0(
+        ffi.cast(f"{c_type} *", J_1.ctypes.data),
+        ffi.cast(f"{c_type} *", w1.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
-    expected_result = np.array([0.5 * np.real(w1[0]) * np.imag(w1[1])
-                               * (np.real(w1[0]) - 1j * np.imag(w1[0]))], dtype=np_type)
+    expected_result = np.array(
+        [0.5 * np.real(w1[0]) * np.imag(w1[1]) * (np.real(w1[0]) - 1j * np.imag(w1[0]))],
+        dtype=dtype,
+    )
     assert np.allclose(J_1, expected_result)
 
-    J_2 = np.zeros((1), dtype=np_type)
+    J_2 = np.zeros((1), dtype=dtype)
 
-    kernel1 = ffi.cast(f"ufcx_tabulate_tensor_{np_type} *", getattr(form1, f"tabulate_tensor_{np_type}"))
-    kernel1(ffi.cast('{type} *'.format(type=mode), J_2.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), w1.ctypes.data),
-            ffi.cast('{type} *'.format(type=mode), c.ctypes.data),
-            ffi.cast(f'{geom_type} *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    kernel1 = ffi.cast(
+        f"ufcx_tabulate_tensor_{dtype} *", getattr(form1, f"tabulate_tensor_{dtype}")
+    )
+    kernel1(
+        ffi.cast(f"{c_type} *", J_2.ctypes.data),
+        ffi.cast(f"{c_type} *", w1.ctypes.data),
+        ffi.cast(f"{c_type} *", c.ctypes.data),
+        ffi.cast(f"{c_xtype} *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
 
     assert np.allclose(J_2, expected_result)
 
     assert np.allclose(J_1, J_2)
 
 
 def test_invalid_function_name(compile_args):
     # Monkey patch to force invalid name
     old_str = ufl.Coefficient.__str__
     ufl.Coefficient.__str__ = lambda self: "invalid function name"
 
     V = basix.ufl.element("Lagrange", "triangle", 1)
-    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2, )))
+    domain = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
     space = ufl.FunctionSpace(domain, V)
     u = ufl.Coefficient(space)
     a = ufl.inner(u, u) * ufl.dx
-
     forms = [a]
-
     try:
         compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-            forms, cffi_extra_compile_args=compile_args)
+            forms, cffi_extra_compile_args=compile_args
+        )
     except ValueError:
         pass
     except Exception:
         raise RuntimeError("Compilation should fail with ValueError.")
 
     # Revert monkey patch for other tests
     ufl.Coefficient.__str__ = old_str
 
 
 def test_interval_vertex_quadrature(compile_args):
-
-    c_el = basix.ufl.element("Lagrange", "interval", 1, shape=(1, ))
+    c_el = basix.ufl.element("Lagrange", "interval", 1, shape=(1,))
     mesh = ufl.Mesh(c_el)
 
     x = ufl.SpatialCoordinate(mesh)
-    dx = ufl.Measure(
-        "dx", metadata={"quadrature_rule": "vertex"})
+    dx = ufl.Measure("dx", metadata={"quadrature_rule": "vertex"})
     b = x[0] * dx
 
     forms = [b]
     compiled_forms, module, code = ffcx.codegeneration.jit.compile_forms(
-        forms, cffi_extra_compile_args=compile_args)
+        forms, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     form0 = compiled_forms[0]
     assert form0.form_integral_offsets[module.lib.cell + 1] == 1
 
     default_integral = form0.form_integrals[0]
     J = np.zeros(1, dtype=np.float64)
     a = np.pi
     b = np.exp(1)
-    coords = np.array([a, 0.0, 0.0,
-
-                       b, 0.0, 0.0], dtype=np.float64)
+    coords = np.array([a, 0.0, 0.0, b, 0.0, 0.0], dtype=np.float64)
 
     kernel = getattr(default_integral, "tabulate_tensor_float64")
-    kernel(ffi.cast('double *', J.ctypes.data),
-           ffi.NULL,
-           ffi.NULL,
-           ffi.cast('double *', coords.ctypes.data), ffi.NULL, ffi.NULL)
+    kernel(
+        ffi.cast("double *", J.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+        ffi.cast("double *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.NULL,
+    )
     assert np.isclose(J[0], (0.5 * a + 0.5 * b) * np.abs(b - a))
 
 
 def test_facet_vertex_quadrature(compile_args):
     """Test facet vertex quadrature"""
     c_el = basix.ufl.element("Lagrange", "quadrilateral", 1, shape=(2,))
     mesh = ufl.Mesh(c_el)
 
     x = ufl.SpatialCoordinate(mesh)
-    ds = ufl.Measure(
-        "ds", metadata={"quadrature_rule": "vertex"})
-    expr = (x[0] + ufl.cos(x[1]))
+    ds = ufl.Measure("ds", metadata={"quadrature_rule": "vertex"})
+    expr = x[0] + ufl.cos(x[1])
     b1 = expr * ds
     ds_c = ufl.Measure(
         "ds",
         metadata={
             "quadrature_rule": "custom",
             "quadrature_points": np.array([[0.0], [1.0]]),
             "quadrature_weights": np.array([1.0 / 2.0, 1.0 / 2.0]),
-        }
+        },
     )
     b2 = expr * ds_c
     forms = [b1, b2]
     compiled_forms, module, _ = ffcx.codegeneration.jit.compile_forms(
-        forms, cffi_extra_compile_args=compile_args)
+        forms, cffi_extra_compile_args=compile_args
+    )
 
     ffi = module.ffi
     assert len(compiled_forms) == 2
     solutions = []
     for form in compiled_forms:
         offsets = form.form_integral_offsets
         exf = module.lib.exterior_facet
         assert offsets[exf + 1] - offsets[exf] == 1
 
         default_integral = form.form_integrals[offsets[exf]]
         J = np.zeros(1, dtype=np.float64)
         a = np.pi
         b = np.exp(1)
-        coords = np.array([a, 0.1, 0.0,
-                           a + b, 0.0, 0.0,
-                           a, a, 0.,
-                           a + 2 * b, a, 0.], dtype=np.float64)
+        coords = np.array(
+            [a, 0.1, 0.0, a + b, 0.0, 0.0, a, a, 0.0, a + 2 * b, a, 0.0], dtype=np.float64
+        )
         # First facet is between vertex 0 and 1 in coords
         facets = np.array([0], dtype=np.intc)
 
         kernel = getattr(default_integral, "tabulate_tensor_float64")
-        kernel(ffi.cast('double *', J.ctypes.data),
-               ffi.NULL,
-               ffi.NULL,
-               ffi.cast('double *', coords.ctypes.data),
-               ffi.cast('int *', facets.ctypes.data),
-               ffi.NULL)
+        kernel(
+            ffi.cast("double *", J.ctypes.data),
+            ffi.NULL,
+            ffi.NULL,
+            ffi.cast("double *", coords.ctypes.data),
+            ffi.cast("int *", facets.ctypes.data),
+            ffi.NULL,
+        )
         solutions.append(J[0])
         # Test against exact result
-        assert np.isclose(J[0], (0.5 * (a + np.cos(0.1)) + 0.5 * (a + b + np.cos(0))) * np.sqrt(b**2 + 0.1**2))
+        assert np.isclose(
+            J[0], (0.5 * (a + np.cos(0.1)) + 0.5 * (a + b + np.cos(0))) * np.sqrt(b**2 + 0.1**2)
+        )
 
     # Compare custom quadrature with vertex quadrature
     assert np.isclose(solutions[0], solutions[1])
 
 
 def test_manifold_derivatives(compile_args):
     """Test higher order derivatives on manifolds"""
-    c_el = basix.ufl.element("Lagrange", "interval", 1, shape=(2,), gdim=2)
+    c_el = basix.ufl.element("Lagrange", "interval", 1, shape=(2,))
     mesh = ufl.Mesh(c_el)
 
     x = ufl.SpatialCoordinate(mesh)
     dx = ufl.Measure("dx", domain=mesh)
     order = 4
-    el = basix.ufl.element("Lagrange", "interval", order, gdim=2)
+    el = basix.ufl.element("Lagrange", "interval", order)
     V = ufl.FunctionSpace(mesh, el)
 
     u = ufl.Coefficient(V)
     d = 5.3
-    f_ex = d * order * (order - 1) * x[1]**(order - 2)
+    f_ex = d * order * (order - 1) * x[1] ** (order - 2)
     expr = u.dx(1).dx(1) - f_ex
     J = expr * expr * dx
 
     compiled_forms, module, _ = ffcx.codegeneration.jit.compile_forms(
-        [J], cffi_extra_compile_args=compile_args)
+        [J], cffi_extra_compile_args=compile_args
+    )
 
     default_integral = compiled_forms[0].form_integrals[0]
     scale = 2.5
     coords = np.array([0.0, 0.0, 0.0, 0.0, scale, 0.0], dtype=np.float64)
-    dof_coords = scale * el.element.points.reshape(-1)
+    dof_coords = scale * el._element.points.reshape(-1)
 
     w = np.array([d * d_c**order for d_c in dof_coords], dtype=np.float64)
     c = np.array([], dtype=np.float64)
     perm = np.array([0], dtype=np.uint8)
 
     ffi = module.ffi
     J = np.zeros(1, dtype=np.float64)
     kernel = getattr(default_integral, "tabulate_tensor_float64")
-    kernel(ffi.cast('double *', J.ctypes.data),
-           ffi.cast('double  *', w.ctypes.data),
-           ffi.cast('double  *', c.ctypes.data),
-           ffi.cast('double  *', coords.ctypes.data), ffi.NULL,
-           ffi.cast('uint8_t *', perm.ctypes.data))
+    kernel(
+        ffi.cast("double *", J.ctypes.data),
+        ffi.cast("double  *", w.ctypes.data),
+        ffi.cast("double  *", c.ctypes.data),
+        ffi.cast("double  *", coords.ctypes.data),
+        ffi.NULL,
+        ffi.cast("uint8_t *", perm.ctypes.data),
+    )
 
     assert np.isclose(J[0], 0.0)
 
 
 def test_integral_grouping(compile_args):
     """We group integrals with common integrands to avoid duplicated
     integration kernels. This means that `inner(u, v)*dx((1,2,3))  +
@@ -905,21 +1044,33 @@
     1. `inner(u,v)*dx(("everywhere", 1, 3))`
     2. `(inner(grad(u), grad(v)) + inner(u, v))*dx(2)`
     Each of the forms has one generated `tabulate_tensor_*` function,
     which is referred to multiple times in `integrals_` and
     `integral_ids_`
 
     """
-    mesh = ufl.Mesh(ufl.VectorElement("Lagrange", ufl.triangle, 1))
-    V = ufl.FunctionSpace(mesh, ufl.FiniteElement("Lagrange", ufl.triangle, 1))
+    mesh = ufl.Mesh(basix.ufl.element("Lagrange", "triangle", 1, shape=(2,)))
+    V = ufl.FunctionSpace(mesh, basix.ufl.element("Lagrange", "triangle", 1))
     u = ufl.TrialFunction(V)
     v = ufl.TestFunction(V)
-    a = ufl.inner(u, v) * ufl.dx((1, 2, 3)) + ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx(2) + ufl.inner(u, v) * ufl.dx
+    a = (
+        ufl.inner(u, v) * ufl.dx((1, 2, 3))
+        + ufl.inner(ufl.grad(u), ufl.grad(v)) * ufl.dx(2)
+        + ufl.inner(u, v) * ufl.dx
+    )
     compiled_forms, module, _ = ffcx.codegeneration.jit.compile_forms(
-        [a], cffi_extra_compile_args=compile_args)
+        [a], cffi_extra_compile_args=compile_args
+    )
     # NOTE: This assumes that the first integral type is cell integrals, see UFCx.h
     cell = module.lib.cell
-    num_integrals = compiled_forms[0].form_integral_offsets[cell + 1] - compiled_forms[0].form_integral_offsets[cell]
+    num_integrals = (
+        compiled_forms[0].form_integral_offsets[cell + 1]
+        - compiled_forms[0].form_integral_offsets[cell]
+    )
     assert num_integrals == 4
-    unique_integrals = set([compiled_forms[0].form_integrals[compiled_forms[0].form_integral_offsets[cell] + i]
-                            for i in range(num_integrals)])
+    unique_integrals = set(
+        [
+            compiled_forms[0].form_integrals[compiled_forms[0].form_integral_offsets[cell] + i]
+            for i in range(num_integrals)
+        ]
+    )
     assert len(unique_integrals) == 2
```

### Comparing `fenics-ffcx-0.7.0/test/test_lnodes.py` & `fenics_ffcx-0.8.0/test/test_lnodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,104 @@
+import importlib
 
-from ffcx.codegeneration import lnodes as L
-from ffcx.codegeneration.C.c_implementation import CFormatter
-from cffi import FFI
 import numpy as np
 import pytest
-import importlib
+from cffi import FFI
+
+from ffcx.codegeneration import lnodes as L
+from ffcx.codegeneration.C.c_implementation import CFormatter
+from ffcx.codegeneration.utils import dtype_to_c_type
 
 
-@pytest.mark.parametrize("scalar", ("float", "double", "int"))
-def test_gemm(scalar):
+@pytest.mark.parametrize("dtype", ("float32", "float64", "intc"))
+def test_gemm(dtype):
     # Test LNodes simple matrix-matrix multiply in C
     p, q, r = 5, 16, 12
 
     A = L.Symbol("A", dtype=L.DataType.SCALAR)
     B = L.Symbol("B", dtype=L.DataType.SCALAR)
     C = L.Symbol("C", dtype=L.DataType.SCALAR)
-    code = [L.Comment(f"Matrix multiply A{p,r} = B{p,q} * C{q,r}")]
+    code = [L.Comment(f"Matrix multiply A{p, r} = B{p, q} * C{q, r}")]
 
     i = L.Symbol("i", dtype=L.DataType.INT)
     j = L.Symbol("j", dtype=L.DataType.INT)
     k = L.Symbol("k", dtype=L.DataType.INT)
     m_ij = L.MultiIndex([i, j], [p, q])
     m_ik = L.MultiIndex([i, k], [p, r])
     m_jk = L.MultiIndex([j, k], [q, r])
 
     body = [L.AssignAdd(A[m_ik], B[m_ij] * C[m_jk])]
     body = [L.ForRange(i, 0, p, body=body)]
     body = [L.ForRange(j, 0, q, body=body)]
     code += [L.ForRange(k, 0, r, body=body)]
 
     # Format into C and compile with CFFI
-    Q = CFormatter(scalar=scalar)
-    decl = f"void gemm({scalar} *A, {scalar} *B, {scalar} *C)"
-    c_code = decl + "{\n" + \
-        Q.c_format(L.StatementList(code)) + "\n}\n"
+    Q = CFormatter(dtype=dtype)
+    c_scalar = dtype_to_c_type(dtype)
+    decl = f"void gemm({c_scalar} *A, {c_scalar} *B, {c_scalar} *C)"
+    c_code = decl + "{\n" + Q.c_format(L.StatementList(code)) + "\n}\n"
 
     ffibuilder = FFI()
     ffibuilder.cdef(decl + ";")
-    ffibuilder.set_source(f"_gemm_{scalar}", c_code)
+    ffibuilder.set_source(f"_gemm_{c_scalar}", c_code)
     ffibuilder.compile(verbose=True)
-    _gemm = importlib.import_module(f"_gemm_{scalar}")
+    _gemm = importlib.import_module(f"_gemm_{c_scalar}")
     gemm = _gemm.lib.gemm
     ffi = _gemm.ffi
 
-    c_to_np = {"double": np.float64, "float": np.float32, "int": np.int32}
-    np_scalar = c_to_np.get(scalar)
-    A = np.zeros((p, r), dtype=np_scalar)
-    B = np.ones((p, q), dtype=np_scalar)
-    C = np.ones((q, r), dtype=np_scalar)
-    pA = ffi.cast(f"{scalar} *", A.ctypes.data)
-    pB = ffi.cast(f"{scalar} *", B.ctypes.data)
-    pC = ffi.cast(f"{scalar} *", C.ctypes.data)
+    A = np.zeros((p, r), dtype=dtype)
+    B = np.ones((p, q), dtype=dtype)
+    C = np.ones((q, r), dtype=dtype)
+    pA = ffi.cast(f"{c_scalar} *", A.ctypes.data)
+    pB = ffi.cast(f"{c_scalar} *", B.ctypes.data)
+    pC = ffi.cast(f"{c_scalar} *", C.ctypes.data)
 
     gemm(pA, pB, pC)
     assert np.all(A == q)
 
 
-@pytest.mark.parametrize("scalar", ("float", "double", "int"))
-def test_gemv(scalar):
+@pytest.mark.parametrize("dtype", ("float32", "float64", "intc"))
+def test_gemv(dtype):
     # Test LNodes simple matvec multiply in C
     p, q = 5, 16
 
     y = L.Symbol("y", dtype=L.DataType.SCALAR)
     A = L.Symbol("A", dtype=L.DataType.SCALAR)
     x = L.Symbol("x", dtype=L.DataType.SCALAR)
-    code = [L.Comment(f"Matrix-vector multiply y({p}) = A{p,q} * x({q})")]
+    code = [L.Comment(f"Matrix-vector multiply y({p}) = A{p, q} * x({q})")]
 
     i = L.Symbol("i", dtype=L.DataType.INT)
     j = L.Symbol("j", dtype=L.DataType.INT)
     m_ij = L.MultiIndex([i, j], [p, q])
 
     body = [L.AssignAdd(y[i], A[m_ij] * x[j])]
     body = [L.ForRange(i, 0, p, body=body)]
     code += [L.ForRange(j, 0, q, body=body)]
 
     # Format into C and compile with CFFI
-    Q = CFormatter(scalar=scalar)
-    decl = f"void gemm({scalar} *y, {scalar} *A, {scalar} *x)"
-    c_code = decl + "{\n" + \
-        Q.c_format(L.StatementList(code)) + "\n}\n"
+    Q = CFormatter(dtype=dtype)
+    c_scalar = dtype_to_c_type(dtype)
+    decl = f"void gemm({c_scalar} *y, {c_scalar} *A, {c_scalar} *x)"
+    c_code = decl + "{\n" + Q.c_format(L.StatementList(code)) + "\n}\n"
 
     ffibuilder = FFI()
     ffibuilder.cdef(decl + ";")
-    ffibuilder.set_source(f"_gemv_{scalar}", c_code)
+    ffibuilder.set_source(f"_gemv_{c_scalar}", c_code)
     ffibuilder.compile(verbose=True)
-    _gemv = importlib.import_module(f"_gemv_{scalar}")
+    _gemv = importlib.import_module(f"_gemv_{c_scalar}")
     gemv = _gemv.lib.gemm
     ffi = _gemv.ffi
 
-    c_to_np = {"double": np.float64, "float": np.float32, "int": np.int32}
-    np_scalar = c_to_np.get(scalar)
-    y = np.arange(p, dtype=np_scalar)
-    x = np.arange(q, dtype=np_scalar)
+    y = np.arange(p, dtype=dtype)
+    x = np.arange(q, dtype=dtype)
     A = np.outer(y, x)
 
-    py = ffi.cast(f"{scalar} *", y.ctypes.data)
-    pA = ffi.cast(f"{scalar} *", A.ctypes.data)
-    px = ffi.cast(f"{scalar} *", x.ctypes.data)
+    py = ffi.cast(f"{c_scalar} *", y.ctypes.data)
+    pA = ffi.cast(f"{c_scalar} *", A.ctypes.data)
+    px = ffi.cast(f"{c_scalar} *", x.ctypes.data)
 
     # Compute expected result
     s2 = q * (q - 1) * (2 * q - 1) // 6 + 1
-    result = np.arange(p, dtype=np_scalar) * s2
+    result = np.arange(p, dtype=dtype) * s2
 
     gemv(py, pA, px)
     assert np.all(y == result)
```

