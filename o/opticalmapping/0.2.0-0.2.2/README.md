# Comparing `tmp/opticalmapping-0.2.0.tar.gz` & `tmp/opticalmapping-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opticalmapping-0.2.0.tar", last modified: Wed Feb 21 00:20:46 2024, max compression
+gzip compressed data, was "opticalmapping-0.2.2.tar", last modified: Mon May  6 21:12:08 2024, max compression
```

## Comparing `opticalmapping-0.2.0.tar` & `opticalmapping-0.2.2.tar`

### file list

```diff
@@ -1,249 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.650970 opticalmapping-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.602970 opticalmapping-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.606970 opticalmapping-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-21 00:20:46.650970 opticalmapping-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.610970 opticalmapping-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.610970 opticalmapping-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/_static/vscode-code-cells.png
--rw-r--r--   0 runner    (1001) docker     (127)  2376083 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/_static/vscode-plot-viewer.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.614970 opticalmapping-0.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.614970 opticalmapping-0.2.0/docs/chapters/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/chapters/bibliography.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/chapters/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/chapters/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/chapters/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/chapters/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/refs.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.614970 opticalmapping-0.2.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/activation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/apd.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/cv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/io.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/motion_compensation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/phase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/ratiometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22177 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/signal_extraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/smoothing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/docs/tutorials/strain.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.650970 opticalmapping-0.2.0/opticalmapping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/opticalmapping.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.618970 opticalmapping-0.2.0/optimap/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.618970 opticalmapping-0.2.0/optimap/_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/contrast_enhancement.h
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/filters.h
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/flow_filters.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.606970 opticalmapping-0.2.0/optimap/_cpp/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.634970 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaccessible.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaccumulator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    36156 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xadapt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24640 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xarray.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    49134 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xassign.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaxis_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11290 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaxis_slice_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    38555 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xblockwise_reducer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xblockwise_reducer_functors.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbroadcast.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbuffer_adaptor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42455 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbuilder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_array.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_assign.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcomplex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    41731 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcontainer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcsv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28975 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xdynamic_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xeval.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexception.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24760 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression_holder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    37637 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfixed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    39903 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    57648 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfunctor_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xgenerator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xhistogram.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26749 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xindex_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xinfo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26832 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xio.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    52665 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xiterable.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    35923 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xiterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xjson.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xlayout.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    38079 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmanipulation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24021 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmasked_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   120621 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmath.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmime.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmultiindex_iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnoalias.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31209 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnorm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27263 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnpy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoffset_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34576 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoperation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    48774 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27116 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    37733 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly_storage.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xpad.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xrandom.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    64806 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xreducer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23264 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xrepeat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34142 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xscalar.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24660 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xsemantic.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xset_operation.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16921 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xshape.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    49258 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xslice.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    48051 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xsort.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    59022 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstorage.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29524 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrided_view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34210 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrided_view_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31463 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrides.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_forward.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_simd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28368 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xutils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xvectorize.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    83925 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xview.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xview_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.634970 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19989 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyarray.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyarray_backstrides.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pycontainer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pynative_casters.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pystrides_adaptor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pytensor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyvectorize.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/xtensor_python_config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/xtensor_type_caster_base.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.642970 opticalmapping-0.2.0/optimap/_cpp/include/xtl/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xany.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xbase64.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   100835 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xbasic_fixed_string.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xclosure.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcompare.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47661 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcomplex.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18183 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcomplex_sequence.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    42230 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xdynamic_bitset.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xfunctional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhalf_float.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   197648 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhalf_float_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhash.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhierarchy_generator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xiterator_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xjson.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27810 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmasked_value.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmasked_value_meta.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmeta_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmultimethods.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    54666 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional_meta.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional_sequence.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xplatform.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xproxy_wrapper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xsequence.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xspan.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23074 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xspan_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xsystem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xtl_config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xtype_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvariant.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   102860 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvariant_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvisitor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/lib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/phase_filters.h
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/vec2.h
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/_cpp/vectors.h
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-21 00:20:46.000000 opticalmapping-0.2.0/optimap/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.642970 opticalmapping-0.2.0/optimap/activation/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/activation/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.642970 opticalmapping-0.2.0/optimap/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/draw_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/eraser_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/invert_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/redo_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/undo_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/visibility_off_symbol.png
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/assets/visibility_on_symbol.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.642970 opticalmapping-0.2.0/optimap/image/
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/_GHT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/image/_segmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.642970 opticalmapping-0.2.0/optimap/motion/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/motion/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/motion/_flowestimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/motion/_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/motion/_warping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.646970 opticalmapping-0.2.0/optimap/phase/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/phase/_singularities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.646970 opticalmapping-0.2.0/optimap/trace/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_detrend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_point_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/trace/_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.646970 opticalmapping-0.2.0/optimap/video/
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)    20518 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_importers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_player.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/optimap/video/_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 00:20:46.650970 opticalmapping-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 00:20:46.650970 opticalmapping-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_activationmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-02-21 00:20:33.000000 opticalmapping-0.2.0/tests/test_video_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.166470 opticalmapping-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.110470 opticalmapping-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.114470 opticalmapping-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-06 21:12:08.166470 opticalmapping-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.114470 opticalmapping-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.118470 opticalmapping-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   129548 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/_static/flow diagram tracking Lebert et al.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/_static/vscode-code-cells.png
+-rw-r--r--   0 runner    (1001) docker     (127)  2376083 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/_static/vscode-plot-viewer.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.118470 opticalmapping-0.2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.122470 opticalmapping-0.2.2/docs/chapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/chapters/bibliography.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/chapters/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/chapters/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/chapters/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/chapters/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/rename_example_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.122470 opticalmapping-0.2.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21505 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/01_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/activation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/apd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/cv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/example_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17824 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/io.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29171 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/motion_compensation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/phase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/ratiometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/signal_extraction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/smoothing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/docs/tutorials/strain.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.166470 opticalmapping-0.2.2/opticalmapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/opticalmapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/opticalmapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/opticalmapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:12:07.000000 opticalmapping-0.2.2/opticalmapping.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/opticalmapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/opticalmapping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.126470 opticalmapping-0.2.2/optimap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.126470 opticalmapping-0.2.2/optimap/_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6676 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/contrast_enhancement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/filters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/flow_filters.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.110470 opticalmapping-0.2.2/optimap/_cpp/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.142470 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaccessible.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaccumulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    36156 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xadapt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24640 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xarray.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    49134 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xassign.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaxis_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11290 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaxis_slice_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38555 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xblockwise_reducer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xblockwise_reducer_functors.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbroadcast.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbuffer_adaptor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42455 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbuilder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_array.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_assign.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcomplex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    41731 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcontainer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcsv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28975 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xdynamic_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xeval.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexception.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24760 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression_holder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37637 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfixed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39903 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    57648 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfunctor_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17080 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xgenerator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21613 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xhistogram.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26749 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xindex_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xinfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26832 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xio.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    52665 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xiterable.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35923 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xiterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xjson.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xlayout.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38079 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmanipulation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24021 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmasked_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   120621 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmath.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmime.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmultiindex_iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnoalias.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31209 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnorm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27263 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnpy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoffset_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34576 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoperation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    48774 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27116 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37733 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19544 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly_storage.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xpad.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xrandom.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    64806 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xreducer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23264 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xrepeat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34142 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xscalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24660 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xsemantic.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xset_operation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16921 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xshape.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    49258 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xslice.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    48051 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    59022 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstorage.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29524 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrided_view.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34210 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrided_view_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31463 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrides.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_forward.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_simd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28368 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xutils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xvectorize.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    83925 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xview.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xview_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.146470 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19989 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyarray.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyarray_backstrides.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16943 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pycontainer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pynative_casters.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pystrides_adaptor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pytensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyvectorize.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/xtensor_python_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/xtensor_type_caster_base.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.154470 opticalmapping-0.2.2/optimap/_cpp/include/xtl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xany.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xbase64.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   100835 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xbasic_fixed_string.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xclosure.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcompare.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47661 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcomplex.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18183 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcomplex_sequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42230 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xdynamic_bitset.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xfunctional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhalf_float.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   197648 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhalf_float_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhash.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhierarchy_generator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xiterator_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xjson.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27810 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmasked_value.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmasked_value_meta.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmeta_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmultimethods.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54666 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional_meta.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21055 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional_sequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xplatform.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xproxy_wrapper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xsequence.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xspan.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23074 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xspan_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xsystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xtl_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xtype_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvariant.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   102860 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvariant_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvisitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/phase_filters.h
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/vec2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/_cpp/vectors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 21:12:08.000000 opticalmapping-0.2.2/optimap/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.154470 opticalmapping-0.2.2/optimap/activation/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/activation/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.154470 opticalmapping-0.2.2/optimap/apd/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/apd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/apd/_apd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.154470 opticalmapping-0.2.2/optimap/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/draw_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/eraser_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/invert_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/redo_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/undo_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/visibility_off_symbol.png
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/assets/visibility_on_symbol.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.158470 opticalmapping-0.2.2/optimap/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/_GHT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13896 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/image/_segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.158470 opticalmapping-0.2.2/optimap/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/motion/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/motion/_flowestimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/motion/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/motion/_warping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.158470 opticalmapping-0.2.2/optimap/phase/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/phase/_singularities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.158470 opticalmapping-0.2.2/optimap/trace/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_detrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_point_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/trace/_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.162470 opticalmapping-0.2.2/optimap/video/
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21054 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_importers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/optimap/video/_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:12:08.166470 opticalmapping-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:12:08.162470 opticalmapping-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_activationmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-05-06 21:11:59.000000 opticalmapping-0.2.2/tests/test_video_io.py
```

### Comparing `opticalmapping-0.2.0/.github/workflows/main.yml` & `opticalmapping-0.2.2/.github/workflows/main.yml`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-12]
+        # macos-13 is an intel runner, macos-14 is apple silicon
+        os: [ubuntu-latest, windows-latest, macos-13, macos-14]
 
     steps:
-      - uses: actions/checkout@v4
+      - name: Checkout code
+        uses: actions/checkout@v4
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.5
+        uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_BUILD: "cp38-macosx* cp39-manylinux_x86_64 cp312-manylinux_x86_64 cp311-win_amd64" #  Speed up CI by only building a subset of wheels
+          CIBW_BUILD: "cp38-manylinux_x86_64 cp310-macosx* cp311-win_amd64 cp312-manylinux_x86_64" #  Speed up CI by only building a subset of wheels
 
-      - uses: actions/upload-artifact@v3
+      - name: Upload artifact
+        uses: actions/upload-artifact@v4
         with:
           path: ./wheelhouse/*.whl
+          name: wheels-${{ matrix.os }}-${{ strategy.job-index }}
```

### Comparing `opticalmapping-0.2.0/.github/workflows/publish.yml` & `opticalmapping-0.2.2/.github/workflows/publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -8,49 +8,57 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-12]
+        # macos-13 is an intel runner, macos-14 is apple silicon
+        os: [ubuntu-latest, windows-latest, macos-13, macos-14]
 
     steps:
-      - uses: actions/checkout@v4
+      - name: Checkout code
+        uses: actions/checkout@v4
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.16.5
+        uses: pypa/cibuildwheel@v2.17.0
 
-      - uses: actions/upload-artifact@v3
+      - name: Upload artifact
+        uses: actions/upload-artifact@v4
         with:
           path: ./wheelhouse/*.whl
+          name: wheels-${{ matrix.os }}-${{ strategy.job-index }}
 
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v4
+      - name: Checkout code
+        uses: actions/checkout@v4
 
       - name: Build sdist
         run: pipx run build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - name: Upload artifact
+        uses: actions/upload-artifact@v4
         with:
           path: dist/*.tar.gz
+          name: wheels-sdist
 
   upload_pypi:
     name: Upload to PyPI
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/opticalmapping
     permissions:
       id-token: write
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: artifact
+          pattern: wheels-*
           path: dist
+          merge-multiple: true
 
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `opticalmapping-0.2.0/.gitignore` & `opticalmapping-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/CONTRIBUTING.md` & `opticalmapping-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/LICENSE.md` & `opticalmapping-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/PKG-INFO` & `opticalmapping-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalmapping
-Version: 0.2.0
+Version: 0.2.2
 Summary: A toolbox for analyzing optical mapping and fluorescence imaging data.
 Home-page: https://github.com/cardiacvision/optimap
 Author: Jan Lebert
 Author-email: jan.lebert@ucsf.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,16 @@
 Requires-Dist: scikit-image
 Requires-Dist: scikit-video
 Requires-Dist: tqdm
 Requires-Dist: pooch
 Requires-Dist: seasonal
 Requires-Dist: static_ffmpeg
 Requires-Dist: mpl-pan-zoom
+Requires-Dist: monochrome-viewer
+Requires-Dist: Pillow>=10.0.1
 Provides-Extra: all
 Requires-Dist: opencv-contrib-python; extra == "all"
 Requires-Dist: PySide6; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
@@ -48,54 +50,60 @@
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-codeautolink; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst_nb>=1.0.0; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: jupyter-cache; extra == "docs"
+Requires-Dist: sphinx-remove-toctrees; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
 
 # optimap
 
 [![docs](https://readthedocs.org/projects/optimap/badge/?version=latest&style=)](https://optimap.readthedocs.org)
 [![tests](https://github.com/cardiacvision/optimap/actions/workflows/main.yml/badge.svg)](https://github.com/cardiacvision/optimap/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/opticalmapping.svg)](https://pypi.org/project/opticalmapping/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/opticalmapping.svg)](https://python.org)
 [![DOI](https://zenodo.org/badge/677528623.svg)](https://zenodo.org/badge/latestdoi/677528623)
 
 ### optimap: An open-source library for the processing of fluorescence video data
 
-`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more detailed information about optimap's usage and features.
+`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, conduction velocities, action potential durations, as well as measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more information about optimap's features.
 
 > ⚠️ optimap is currently in early development, expect breaking changes and bugs.
 
 ## Installation
 
-`optimap` is available for Mac OSX, Windows and Linux, see [Installing optimap](https://optimap.readthedocs.io/en/latest/chapters/getting_started/#installing-optimap) for more detailed information.
+`optimap` is available for macOS, Windows and Linux, see the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for more information.
 
-### Installing pre-built binaries (Mac OSX, Windows, Linux)
+### Installing pre-built binaries (macOS, Windows, Linux)
 
 Pre-built binaries can be installed using pip:
 
 ```bash
 pip install opticalmapping[all]
 ```
 
 The above command will install optimap and all recommended dependencies including OpenCV and PySide2. If you wish to install your own version of OpenCV (e.g. for CUDA support) or Qt implementation use:
 
 ```bash
 pip install opticalmapping
 ```
 
-## Getting Started
+To update optimap to the latest version run
 
-See [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for an introduction to optimap and installation instructions.
+```bash
+pip install --upgrade opticalmapping[all]
+```
 
 ## About optimap
 
-`optimap` is a script-based software, which means that you run Python-based analysis scripts rather than using a graphical user interface. We provide several example scripts which explain the usage of `optimap`, see [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/). The example scripts can also be downloaded directly by clicking on the right link in the green box at the top of each tutorial page. `optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). `optimap` was created for cardiovascular scientists in particular, but might also be useful for scientists in other fields, for instance, when performing calcium imaging or physiological research with moving cells or tissues. `optimap` is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, matplotlib and OpenCV.
+`optimap` is an interactive, script or notebook-based software library created for cardiovascular scientists in particular, but might also be useful for scientists in other fields. For instance, when performing calcium imaging or physiological research with moving cells or tissues. It is designed to be a flexible and customizable analysis workflow toolkit, which allows for a wide range of analyses and visualizations. See the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) for examples and more information about the usage of `optimap`. The tutorials can be downloaded by clicking on the link in the green box at the top of each tutorial page.
+
+`optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). It is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, Matplotlib and OpenCV.
 
 ## Links
 
 - [Documentation](https://optimap.readthedocs.io)
 - [Issue tracker](https://github.com/cardiacvision/optimap/issues)
 - [Source code](https://github.com/cardiacvision/optimap)
```

### Comparing `opticalmapping-0.2.0/README.md` & `opticalmapping-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,43 +4,47 @@
 [![tests](https://github.com/cardiacvision/optimap/actions/workflows/main.yml/badge.svg)](https://github.com/cardiacvision/optimap/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/opticalmapping.svg)](https://pypi.org/project/opticalmapping/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/opticalmapping.svg)](https://python.org)
 [![DOI](https://zenodo.org/badge/677528623.svg)](https://zenodo.org/badge/latestdoi/677528623)
 
 ### optimap: An open-source library for the processing of fluorescence video data
 
-`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more detailed information about optimap's usage and features.
+`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, conduction velocities, action potential durations, as well as measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more information about optimap's features.
 
 > ⚠️ optimap is currently in early development, expect breaking changes and bugs.
 
 ## Installation
 
-`optimap` is available for Mac OSX, Windows and Linux, see [Installing optimap](https://optimap.readthedocs.io/en/latest/chapters/getting_started/#installing-optimap) for more detailed information.
+`optimap` is available for macOS, Windows and Linux, see the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for more information.
 
-### Installing pre-built binaries (Mac OSX, Windows, Linux)
+### Installing pre-built binaries (macOS, Windows, Linux)
 
 Pre-built binaries can be installed using pip:
 
 ```bash
 pip install opticalmapping[all]
 ```
 
 The above command will install optimap and all recommended dependencies including OpenCV and PySide2. If you wish to install your own version of OpenCV (e.g. for CUDA support) or Qt implementation use:
 
 ```bash
 pip install opticalmapping
 ```
 
-## Getting Started
+To update optimap to the latest version run
 
-See [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for an introduction to optimap and installation instructions.
+```bash
+pip install --upgrade opticalmapping[all]
+```
 
 ## About optimap
 
-`optimap` is a script-based software, which means that you run Python-based analysis scripts rather than using a graphical user interface. We provide several example scripts which explain the usage of `optimap`, see [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/). The example scripts can also be downloaded directly by clicking on the right link in the green box at the top of each tutorial page. `optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). `optimap` was created for cardiovascular scientists in particular, but might also be useful for scientists in other fields, for instance, when performing calcium imaging or physiological research with moving cells or tissues. `optimap` is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, matplotlib and OpenCV.
+`optimap` is an interactive, script or notebook-based software library created for cardiovascular scientists in particular, but might also be useful for scientists in other fields. For instance, when performing calcium imaging or physiological research with moving cells or tissues. It is designed to be a flexible and customizable analysis workflow toolkit, which allows for a wide range of analyses and visualizations. See the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) for examples and more information about the usage of `optimap`. The tutorials can be downloaded by clicking on the link in the green box at the top of each tutorial page.
+
+`optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). It is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, Matplotlib and OpenCV.
 
 ## Links
 
 - [Documentation](https://optimap.readthedocs.io)
 - [Issue tracker](https://github.com/cardiacvision/optimap/issues)
 - [Source code](https://github.com/cardiacvision/optimap)
```

### Comparing `opticalmapping-0.2.0/docs/Makefile` & `opticalmapping-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/_static/vscode-code-cells.png` & `opticalmapping-0.2.2/docs/_static/vscode-code-cells.png`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/_static/vscode-plot-viewer.gif` & `opticalmapping-0.2.2/docs/_static/vscode-plot-viewer.gif`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/_templates/custom-module-template.rst` & `opticalmapping-0.2.2/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/chapters/getting_started.md` & `opticalmapping-0.2.2/docs/chapters/getting_started.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,61 +7,86 @@
 
 `optimap` requires Python 3.8 or later. To install [Python](https://en.wikipedia.org/wiki/Python_programming_language) we recommend installing the [Anaconda distribution](https://www.anaconda.com/download), which includes Python and many useful packages for scientific computing, or by installing [Python directly](https://code.visualstudio.com/docs/python/python-tutorial#_install-a-python-interpreter).
 
 ```{tip}
 optimap relies heavily on [NumPy](https://numpy.org) and [Matplotlib](https://matplotlib.org). We recommend the [Scientific Python Lectures](https://lectures.scientific-python.org) and the [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/) for an introduction to Python and these libraries.
 ```
 
-### Installing pre-built binaries (Mac OSX, Windows, Linux)
+#### Installing pre-built binaries (macOS, Windows, Linux)
 
 The easiest way to install optimap is using `pip` in the command line:
 
-```{code-block} bash
+```bash
 pip install opticalmapping[all]
 ```
 
 If this command fails, please try the following:
 
-```{code-block} bash
+```bash
 python -m pip install opticalmapping\[all\]
 ```
 
 ```{note}
 `pip install opticalmapping` will install the core functionality of optimap. However, the [OpenCV](https://opencv.org/) and dependencies are not installed by default which are required for the {mod}`optimap.motion` and {mod}`optimap.video` modules. To install these dependencies use `pip install opticalmapping[all]` or install OpenCV manually.
 
 If you do not have pip or Python installed you will first have to install these packages.
 
 To use GPU-accelerated motion tracking algorithms a CUDA-enabled version of OpenCV is required, which is currently not available on PyPI. See [](#opencv) for more information.
 ```
 
-To update optimap to the latest version run `pip install --upgrade opticalmapping[all]`. See [](#contributing) for instructions on how to install optimap from source.
+To update optimap to the latest version run
 
-# Overview
+```bash
+pip install --upgrade opticalmapping[all]`
+```
+
+#### Installing from source
+
+To install optimap from source, clone the GitHub repository and run `pip install .` in the root directory:
+
+```bash
+git clone https://github.com/cardiacvision/optimap.git
+cd optimap
+pip install .
+```
+
+See [](#contributing) for more details.
+
+# Overview of optimap
 
 optimap consists of the following modules:
 
 ```{eval-rst}
 .. autosummary::
    optimap.video
    optimap.image
    optimap.trace
    optimap.motion
    optimap.phase
    optimap.utils
 ```
 
-Some of the most important functions are imported into the top-level namespace:
+Some of the most important functions are also imported into the top-level namespace:
 
 ```{eval-rst}
 .. autosummary::
    optimap
 ```
 
 for convenience.
 
+See the tutorials listed below for an introduction to the main features of optimap and the API reference for a complete list of functions and classes.
+
+```{toctree}
+:maxdepth: 2
+:titlesonly:
+
+/tutorials/index.md
+```
+
 (vscode)=
 # Using optimap
 
 We highly recommend using [Visual Studio Code](https://code.visualstudio.com) for working with optimap. Visual Studio Code is a free and open-source editor with excellent support for Python and Jupyter notebooks.
 
 - Download and install [Visual Studio Code](https://code.visualstudio.com)
 - Install the Microsoft [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
@@ -90,16 +115,18 @@
 optimap is currently not designed to be used with Jupyter Notebook running on a remote server. The interactive plotting functions listed below might not work as expected.
 ```
 
 optimap uses [Matplotlib](https://matplotlib.org/) for plotting. The following functions require an interactive Matplotlib backend:
 
 ```{eval-rst}
 .. autosummary::
-   optimap.video.play
-   optimap.video.play2
+   optimap.video.show_video
+   optimap.video.show_videos
+   optimap.video.show_video_pair
+   optimap.video.show_video_overlay
    optimap.trace.select_positions
    optimap.trace.select_traces
    optimap.trace.compare_traces
    optimap.motion.play_displacements
    optimap.motion.play_displacements_points
 ```
```

### Comparing `opticalmapping-0.2.0/docs/chapters/installation.md` & `opticalmapping-0.2.2/docs/chapters/installation.md`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/chapters/misc.md` & `opticalmapping-0.2.2/docs/chapters/misc.md`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/conf.py` & `opticalmapping-0.2.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     "sphinx.ext.intersphinx",
     "sphinx_copybutton",
     "sphinx_codeautolink",
     'sphinxcontrib.bibtex',
     "sphinxcontrib.video",
     "sphinx.ext.viewcode",
     "myst_nb",
+    "sphinx_remove_toctrees",
+    "sphinx_design",
 ]
 myst_enable_extensions = [
     "dollarmath"
 ]
 
 # API settings
 autodoc_default_options = {
@@ -118,15 +120,15 @@
 intersphinx_mapping = {
     "ipywidgets": ("https://ipywidgets.readthedocs.io/en/stable", None),
     "matplotlib": ("https://matplotlib.org/stable", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "python": ("https://docs.python.org/3", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "skimage": ("https://scikit-image.org/docs/stable/", None),
-    # "monochrome": ("https://monochrome.readthedocs.io/en/latest/", None),  # TODO: fix
+    "monochrome": ("https://monochrome.readthedocs.io/stable/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -153,14 +155,18 @@
 # }
 html_theme_options = {
     "source_repository": "https://github.com/cardiacvision/optimap/",
     "source_branch": "main",
     "source_directory": "docs/",
 }
 
+remove_from_toctrees = [
+    "tutorials/converted/*",
+    "tutorials/index.md",
+]
 
 # based on pandas/doc/source/conf.py
 def linkcode_resolve(domain, info):
     """Determine the URL corresponding to Python object."""
     if domain != "py":
         return None
```

### Comparing `opticalmapping-0.2.0/docs/index.md` & `opticalmapping-0.2.2/docs/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 ```{toctree}
-:maxdepth: 2
+:maxdepth: 1
 :hidden:
 :caption: 🚀 Getting Started
 
 chapters/getting_started.md
 
 ```
 
 ```{toctree}
-:maxdepth: 2
+:maxdepth: 1
 :hidden:
 :caption: 🚀 Tutorials
 
-tutorials/basics.ipynb
-tutorials/signal_extraction.ipynb
-tutorials/mask.ipynb
-tutorials/motion_compensation.ipynb
-tutorials/activation.ipynb
-tutorials/cv.ipynb
-tutorials/ratiometry.ipynb
-tutorials/apd.ipynb
-tutorials/phase.ipynb
-tutorials/plotting.ipynb
-tutorials/smoothing.ipynb
-tutorials/io.ipynb
+tutorials/index.md
 ```
 
 ```{toctree}
-:maxdepth: 2
+:maxdepth: 1
 :hidden:
 :caption: Notes
 chapters/contributing
 chapters/misc
 chapters/bibliography
 ```
```

### Comparing `opticalmapping-0.2.0/docs/make.bat` & `opticalmapping-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/docs/refs.bib` & `opticalmapping-0.2.2/docs/refs.bib`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+@article{Bachtel2011,
+  title={A novel approach to dual excitation ratiometric optical mapping of cardiac action potentials with di-4-ANEPPS using pulsed LED excitation},
+  author={A. D. Bachtel and R. A. Gray and J. M. Rogers},
+  journal={IEEE Trans. Biomed. Eng.},
+  volume={58},
+  pages={2120-2126},
+  year={2011}
+}
+
 @article{Barron2020,
   author  = {Jonathan T. Barron},
   title   = {A Generalization of Otsu's Method and Minimum Error Thresholding},
   journal = {ECCV},
   year    = {2020}
 }
 
@@ -108,14 +117,23 @@
 pages = {1353-1370},
 keywords = {action potential duration, motion artifacts, motion tracking, optical mapping, ratiometry, ventricular fibrillation},
 doi = {https://doi.org/10.1113/JP283683},
 url = {https://physoc.onlinelibrary.wiley.com/doi/abs/10.1113/JP283683},
 year = {2023}
 }
 
+@article{Knisley2000,
+  doi       = {10.1152/ajpheart.2000.279.3.H1421},
+  year      = {2000},
+  volume    = {279},
+  author    = {Knisley, S. B. and Justice, R. K. and Kong, W. and Johnson, P. L.},
+  title     = {Ratiometry of transmembrane voltage-sensitive fluorescent dye emission in hearts},
+  journal   = {Am. J. Physiol.}
+}
+
 @article{Lebert2021,
   author  = {Lebert, Jan and Ravi, Namita and Fenton, Flavio H. and Christoph, Jan},
   title   = {Rotor Localization and Phase Mapping of Cardiac Excitation Waves Using Deep Neural Networks},
   journal = {Frontiers in Physiology},
   volume  = {12},
   year    = {2021},
   url     = {https://www.frontiersin.org/articles/10.3389/fphys.2021.782176},
@@ -154,14 +172,41 @@
   language  = {en},
   title     = {optimap: An open-source library for the processing of fluorescence video data},
   publisher = {Zenodo},
   year      = {2023},
   copyright = {MIT License}
 }
 
+@article{Rohde2005,
+  author={Rohde, G.K. and Dawant, B.M. and Shien-Fong Lin},
+  journal={IEEE Transactions on Biomedical Engineering}, 
+  title={Correction of motion artifact in cardiac optical mapping using image registration}, 
+  year={2005},
+  volume={52},
+  number={2},
+  pages={338-341},
+  keywords={Image registration;Analytical models;Anisotropic magnetoresistance;Extracellular;Equations;Conductivity;Slabs;Cardiac tissue;Biomedical optical imaging;Predictive models;Image registration;motion correction;mutual information;optical mapping},
+  doi={10.1109/TBME.2004.840464}
+}
+
+
+@article{Swift2021,
+  author = {Swift, Luther M. and Kay, Matthew W. and Ripplinger, Crystal M. and Posnack, Nikki Gillum},
+  title = {Stop the beat to see the rhythm: excitation-contraction uncoupling in cardiac research},
+  journal = {American Journal of Physiology-Heart and Circulatory Physiology},
+  volume = {321},
+  number = {6},
+  pages = {H1005-H1013},
+  year = {2021},
+  doi = {10.1152/ajpheart.00477.2021},
+  note ={PMID: 34623183},
+  URL = {https://doi.org/10.1152/ajpheart.00477.2021},
+  eprint = {https://doi.org/10.1152/ajpheart.00477.2021}
+}
+
 @inproceedings{Zach2007,
   title     = {A {{Duality Based Approach}} for {{Realtime TV-L1 Optical Flow}}},
   booktitle = {Pattern {{Recognition}}},
   author    = {Zach, C. and Pock, T. and Bischof, H.},
   editor    = {Hamprecht, Fred A. and Schn{\"o}rr, Christoph and J{\"a}hne, Bernd},
   year      = {2007},
   series    = {Lecture {{Notes}} in {{Computer Science}}},
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/activation.ipynb` & `opticalmapping-0.2.2/docs/tutorials/activation.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975626159554731%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 4: "*

 * *            '{\'source\': {insert: [(4, "filename = '*

 * *            'om.download_example_data(\'Sinus_Rabbit_1.npy\')\\n"), (5, \'video = '*

 * *            "om.load_video(filename, frames=20)\\n')], delete: [7, 5, 4]}}, 8: {'source': "*

 * *            '[\'om.show_video_pair(vid […]*

```diff
@@ -22,27 +22,27 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -74,18 +74,17 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "filename = om.utils.retrieve_example_data('Example_01_Sinus_Rabbit_Basler.npy')\n",
-                "video = om.load_video(filename)\n",
+                "filename = om.download_example_data('Sinus_Rabbit_1.npy')\n",
+                "video = om.load_video(filename, frames=20)\n",
                 "video = om.video.rotate_left(video)\n",
-                "video=video[:20]  # only use first 20 frames\n",
                 "\n",
                 "# motion compensation and normalization\n",
                 "video_warped = om.motion.motion_compensate(video, 5, ref_frame=0)\n",
                 "video_warped_norm = om.video.normalize_pixelwise(video_warped)"
             ]
         },
         {
@@ -121,28 +120,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play2(video, video_warped_norm, title1=\"original video\", title2=\"warped, normalized video\", interval=100);"
+                "om.show_video_pair(video, video_warped_norm, title1=\"original video\", title2=\"warped, normalized video\", interval=100);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play2(video, video_warped_norm, title1=\"original video\", title2=\"warped, normalized video\", interval=250))"
+                "render_ani_func(lambda: om.show_video_pair(video, video_warped_norm, title1=\"original video\", title2=\"warped, normalized video\", interval=250))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's plot some of the video frames as the wave propagates across the ventricles:"
@@ -201,15 +200,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "positions =  [(227, 181), (199, 162), (213, 171), (240, 189), (176, 146), (188, 153)]\n",
                 "fig, axs = plt.subplots(1, 2, figsize=(10,5))\n",
-                "om.trace.show_positions(video[0], positions, ax=axs[0])\n",
+                "om.trace.show_positions(positions, video[0], ax=axs[0])\n",
                 "traces = om.extract_traces(video_warped_norm,\n",
                 "                           positions,\n",
                 "                           fps=500,\n",
                 "                           ax=axs[1])\n",
                 "axs[1].axhline(y=0.5, color='r', linestyle='dashed', label='threshold')\n",
                 "axs[1].text(0.030, 0.52, 'threshold', color='r')\n",
                 "plt.show()"
@@ -320,28 +319,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play2(video, video_diff_norm, title1=\"original video\", title2=\"warped, frame-wise diff video\", interval=100);"
+                "om.show_video_pair(video, video_diff_norm, title1=\"original video\", title2=\"warped, frame-wise diff video\", interval=100);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play2(video, video_diff_norm, title1=\"original video\", title2=\"warped, frame-wise diff video\", interval=250))"
+                "render_ani_func(lambda: om.show_video_pair(video, video_diff_norm, title1=\"original video\", title2=\"warped, frame-wise diff video\", interval=250))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's visualize the wavefront as an overlay over the raw (motion-stabilized) video. We will need to further post-process the data as follows: "
@@ -370,28 +369,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play_with_overlay(video_warped, video_diff_norm, vmin_overlay=-1, vmax_overlay=1)"
+                "om.video.show_video_overlay(video_warped, video_diff_norm, vmin_overlay=-1, vmax_overlay=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play_with_overlay(video_warped, video_diff_norm, vmin_overlay=-1, vmax_overlay=1, interval=200))"
+                "render_ani_func(lambda: om.video.show_video_overlay(video_warped, video_diff_norm, vmin_overlay=-1, vmax_overlay=1, interval=200))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We will now compute an activation map from the frame-wise difference video:\n",
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/apd.ipynb` & `opticalmapping-0.2.2/docs/tutorials/cv.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933779761904762%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(1, 'Download this tutorial as a {download}`Jupyter notebook "*

 * *            '<converted/cv.ipynb>`, or as a {download}`python script <converted/cv.py>` with code '*

 * *            'cells. We highly recommend using [Visual Studio Code](#vsc […]*

```diff
@@ -22,54 +22,54 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "source": [
                 "```{tip}\n",
-                "Download this tutorial as a {download}`Jupyter notebook <converted/apd.ipynb>`, or a {download}`python script <converted/apd.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
+                "Download this tutorial as a {download}`Jupyter notebook <converted/cv.ipynb>`, or as a {download}`python script <converted/cv.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 8: Action Potential Duration\n",
+                "# Tutorial 6: Conduction Velocity\n",
                 "\n",
-                "This tutorial will discuss how to compute action potential durations and action potential duration maps from cardiac optical mapping data using ``optimap``. \n",
+                "This tutorial will discuss how to compute conduction velocities from cardiac optical mapping data using ``optimap``. \n",
                 "\n",
                 "```{warning}\n",
-                "This tutorial is currently work in progress. We will add more information soon.\n",
+                "This tutorial is currently under development. We will add more information soon.\n",
                 "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/basics.ipynb` & `opticalmapping-0.2.2/docs/tutorials/01_overview.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935406088764007%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(1, 'Download this tutorial as a {download}`Jupyter notebook "*

 * *            '<converted/01_overview.ipynb>`, or a {download}`python script '*

 * *            '<converted/01_overview.py>` with code cells. We highly recommend using [Visual St […]*

```diff
@@ -22,53 +22,53 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "source": [
                 "```{tip}\n",
-                "Download this tutorial as a {download}`Jupyter notebook <converted/basics.ipynb>`, or a {download}`python script <converted/basics.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial. Alternatively, you could run the Python script in a terminal with ``python3 basics.py`` from the folder where the file is located.\n",
+                "Download this tutorial as a {download}`Jupyter notebook <converted/01_overview.ipynb>`, or a {download}`python script <converted/01_overview.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial. Alternatively, you could run the Python script in a terminal with ``python3 01_overview.py`` from the folder where the file is located.\n",
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 1: Basics\n",
+                "# Tutorial 1: Overview\n",
                 "\n",
-                "This tutorial will walk you through the basics of ``optimap``. \n",
+                "This tutorial will walk you through an basic overview of ``optimap``. ``optimap`` is a package that can be imported and used in [Python](https://en.wikipedia.org/wiki/Python_programming_language) scripts or notebooks. Download the tutorial from the link at the top of the page and follow along.\n",
                 "\n",
-                "``optimap`` is a package that can be imported and used in Python scripts. [Python](https://en.wikipedia.org/wiki/Python_programming_language) is a freely available programming language that is also very popular in scientific computing. The simplest way to access the functionality of ``optimap`` is to import it at the beginning of a new Python script as follows:"
+                "Let's import ``optimap`` and name it ``om`` for short:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -76,17 +76,17 @@
                 "import optimap as om"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "When running this command in a terminal / Python shell or as part of a Python script and ``optimap`` was installed correctly, there should be no further output. We now have access to all the functions in the `optimap` package, and it can then be accessed by typing `om.` followed by a specific function as shown below (e.g. `om.load_video()`). If the import produces an error then ``optimap`` was  not installed correctly, see [Installation Guide](#installing) for further details. \n",
+                "When running this command and ``optimap`` was installed correctly, there should be no further output. We now have access to all the functions in the `optimap` package, and it can then be accessed by typing `om.` followed by a specific function as shown below (e.g. `om.load_video()`). If the import produces an error then ``optimap`` was  not installed correctly, see [Installation Guide](#installing) for further details. \n",
                 "\n",
-                "``optimap`` relies heavily on other open-source software packages and libraries, foremost [NumPy](https://numpy.org/), which is a numerical programming library, [Matplotlib](https://matplotlib.org/), which is a library for plotting data, and [OpenCV](https://opencv.org/), which is a library for computer vision. In this example, we will import ``numpy`` and ``matplotlib`` right after ``optimap`` as follows:"
+                "``optimap`` relies heavily on other open-source software packages and libraries, foremost [NumPy](https://numpy.org/), which is a numerical programming library, [Matplotlib](https://matplotlib.org/), which is a library for plotting data, and [OpenCV](https://opencv.org/), which is a library for computer vision. In this example, we will import ``numpy`` and ``matplotlib`` as they will be used in the tutorial."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -95,112 +95,102 @@
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You do not necessarily have to import `numpy` and `matplotlib` in your analysis scripts as it will be imported internally by `optimap`. Here we imported these packages to be able to work directly with some of their functions in our script and write some custom code for analysis and plotting.\n",
-                "\n",
-                "If you encounter any issues with the steps above please see the [Installation Guide](https://optimap.readthedocs.io/en/latest/chapters/getting_started/)."
+                "If you encounter any issues with the steps above please see the [Installation Guide](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) or create an [Issue](https://github.com/cardiacvision/optimap/issues) on GitHub."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Loading a Video file\n",
+                "## Loading a video file\n",
                 "\n",
-                "The following file formats are currently supported by ``optimap``:\n",
+                "The following video file formats are currently supported by ``optimap``:\n",
                 "\n",
-                "* .tif, .tiff (TIFF stack or folder with a series of individual TIFFs)\n",
-                "* .png (folder with a series of PNGs)\n",
+                "* .tif, .tiff (TIFF) image stacks\n",
+                "* Folder containing sequence of TIFF or .png (PNG) images\n",
                 "* .gsd, .gsh (SciMedia MiCAM 05)\n",
                 "* .rsh, .rsm, .rsd (SciMedia MiCAM ULTIMA)\n",
                 "* .dat (MultiRecorder)\n",
                 "* .npy (numpy array)\n",
                 "* .mat (MATLAB), loads the first field in the file\n",
                 "\n",
-                "We can use the `optimap.load_video` function to load a video file, see also [Tutorial 13](io.ipynb). The code below will automatically download an example file from our website [cardiacvision.ucsf.edu](https://cardiacvision.ucsf.edu) and load it into our workspace as a video. Alternatively, you could load your own file by replacing `filepath` with the filename of your video which you have stored somewhere on your computer. After loading, the video corresponds to a three-dimensional `NumPy`-array where the first dimension is time and the other two dimensions are the x- and y-dimensions, respectively. The example file shows a fibrillating, weakly contracting rabbit heart stained with voltage-sensitive dye (Di-4-ANEPPS) imaged using a Basler acA720-520um camera at 500fps. Due to the staining, the action potential wave is inverted, i.e. an upstroke is observed as a negative deflection. The data is from {cite}`Chowdhary2023` and we extracted a short part of the original recording and saved the otherwise unprocessed raw video data as a numpy file (`.npy`).  Experimenters: Jan Lebert, Shrey Chowdhary & Jan Christoph (University of California, San Francisco, USA), 2023."
+                "which can be loaded with the function {func}`load_video`, see [](io.ipynb) for further details.\n",
+                "\n",
+                "The code below will automatically download an example video recording from our website [cardiacvision.ucsf.edu](https://cardiacvision.ucsf.edu) and save it a folder named `optimap_example_data`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy')\n",
-                "# alternative if you downloaded the file to your desktop\n",
-                "# filepath = '/Users/userxyz/Desktop/Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy'\n",
-                "video = om.load_video(filepath)\n",
+                "filename = om.download_example_data(\"VF_Rabbit_1.npy\")\n",
+                "# alternative if for using your own data\n",
+                "# filename = \"example.tif\"\n",
+                "video = om.load_video(filename)\n",
                 "\n",
                 "om.print_properties(video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`optimap` imports video data as three-dimensional numpy arrays with shape (Time, Height, Width). This convention is used throughout the library. The function `optimap.print_properties()` displays the dimensions and maximal and minimal intensity values of a video. Our example file has 1040 video frames. See {func}`load_video` for additional arguments, e.g. to load only a subset of the frames or to use memory mapping to reduce memory usage.\n",
-                "\n",
-                "```python\n",
-                "video = om.load_video('Example.dat', start_frame=100, frames=1000, step=2, use_mmap=True)\n",
-                "```\n",
-                "\n",
-                "For some file formats, optimap can also load the corresponding metadata using {func}`load_metadata`. For example, the following code loads the metadata of a MiCAM ULTIMA recording:\n",
-                "\n",
-                "```python\n",
-                "metadata = om.load_metadata('Example.rsh')\n",
-                "```\n",
-                "\n",
-                "To crop, rotate, or flip a video see {mod}`optimap.video` for a list of available functions.\n",
+                "`optimap` imports video data as three-dimensional NumPy array,  where the first dimension is time and the other two dimensions are the x- and y-dimensions, respectively. This convention is used throughout the library. The function {func}`print_properties()` displays the dimensions and maximal and minimal intensity values of a video. Our example file has 1040 video frames. See {func}`load_video` for additional arguments, e.g. to load only a subset of the frames or to use memory mapping to reduce memory usage.\n",
                 "\n",
                 "## Playing Videos\n",
                 "Videos can be viewed using either:\n",
-                "1. the built-in viewer {func}`play_video` based on matplotlib\n",
-                "2. Monochrome, which is a more advanced and performant viewer with better interactive features\n",
+                "1. the built-in viewer {func}`show_video` based on matplotlib\n",
+                "2. [Monochrome](https://monochrome.readthedocs.io/latest/), which is a more advanced and performant viewer with better interactive features\n",
                 "\n",
                 "### Using the built-in Viewer"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.play_video(video, skip_frame=3);"
+                "om.show_video(video, title='Recording', skip_frame=3);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = video[:1000]\n",
-                "render_ani_func(lambda: om.video.play(video, interval=15))"
+                "render_ani_func(lambda: om.show_video(video, title='Recording', interval=15))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "See API documentation for {func}`play_video` for a list of available arguments. For instance, it is possible to specify a title, a range (vmin=0, vmax=1) and colormap:\n",
+                "The example video shows a fibrillating, weakly contracting rabbit heart stained with voltage-sensitive dye (Di-4-ANEPPS) imaged at 500 frames per second. Due to the staining, the action potential wave is inverted, i.e. an upstroke is observed as a negative deflection. The data is from {cite}`Chowdhary2023` and we extracted a short part of the original recording and saved the otherwise unprocessed raw video data as a numpy file (`.npy`).\n",
+                "\n",
+                "See API documentation for {func}`show_video` for a list of available arguments. For instance, it is possible to specify a title, a range \n",
+                "(vmin=0, vmax=1) and colormap:\n",
                 "```python\n",
-                "om.play_video(video, title='Example video', vmin=0, vmax=1, cmap='gray', interval=20)\n",
+                "om.show_video(video, title='Example video', vmin=0, vmax=1, cmap='gray', interval=20)\n",
                 "```\n",
                 "\n",
                 "\n",
                 "\n",
                 "### Using Monochrome\n",
                 "Monochrome needs to be installed separately. We will provide installation instructions soon."
             ]
@@ -212,22 +202,22 @@
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "import monochrome as mc\n",
-                "mc.show(video, \"raw video\")"
+                "mc.show(video, \"Recording\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "See the {doc}`monochrome` documentation and {func}`monochrome.show` for more information. For example, click in the video to view time traces at the selected positions.\n",
+                "See the [Monochrome documentation](https://monochrome.readthedocs.io) and {func}`monochrome.show` for more information. For example, click in the video to view time traces at the selected positions.\n",
                 "\n",
                 "## Viewing and Extracting Traces\n",
                 "\n",
                 "Using `optimap` it is possible to quickly extract and display optical traces from any location in a video and display them using the built-in player. With the {func}`select_traces` it is possible to interactively select, extract and view an optical trace. Click on the video image on the left to select a single position or multiple positions. Right click to remove positions. Close the window to continue."
             ]
         },
         {
@@ -252,15 +242,15 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "positions = [(127, 147), (130, 209), (202, 136)]\n",
                 "\n",
                 "fig, axs = plt.subplots(1,2, figsize=(11,4))\n",
-                "om.trace.show_positions(video[0], positions, ax=axs[0])\n",
+                "om.trace.show_positions(positions, video[0], ax=axs[0])\n",
                 "traces = om.trace.extract_traces(video, positions, size=5, ax=axs[1], show=True, fps=500)\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -288,15 +278,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, axs = plt.subplots(1, 2, figsize=(10,5))\n",
                 "\n",
-                "om.trace.show_positions(video[0], positions, ax=axs[0])\n",
+                "om.trace.show_positions(positions, video[0], ax=axs[0])\n",
                 "\n",
                 "x_axis_ms = (np.arange(video.shape[0]) / 500.0) * 1000\n",
                 "traces = om.extract_traces(video[:300],\n",
                 "                           positions,\n",
                 "                           x=x_axis_ms[:300],\n",
                 "                           size=5,\n",
                 "                           window='disc',\n",
@@ -323,61 +313,61 @@
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped = om.motion_compensate(video,\n",
-                "                              contrast_kernel=5,\n",
-                "                              presmooth_spatial=1,\n",
-                "                              presmooth_temporal=1)"
+                "                                    contrast_kernel=5,\n",
+                "                                    presmooth_spatial=1,\n",
+                "                                    presmooth_temporal=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "# load pre-computed warped video to speed up docs build time\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped.npy', silent=True)\n",
+                "filepath = om.utils.download_example_data('Example_02_warped.npy', silent=True)\n",
                 "video_warped = om.load_video(filepath, use_mmap=True)[:1000]\n",
                 "# fake tqdm progress bar\n",
                 "from tqdm import tqdm\n",
                 "from time import sleep\n",
                 "for _ in tqdm(range(1000), desc='Computing flows (CPU)'):\n",
                 "    sleep(1/500.0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The `video_warped` is the motion-stabilized version of the original video. The other parameters are explained in more detail in [](motion_compensation). You will also find further background information about the motion tracking and compensation routines in {cite}`Christoph2018a` and {cite}`Lebert2022`. Let's view the original video and the motion-compensated video side by side using {func}`optimap.video.play2`:"
+                "The `video_warped` is the motion-stabilized version of the original video. The other parameters are explained in more detail in [](motion_compensation). You will also find further background information about the motion tracking and compensation routines in {cite}`Christoph2018a` and {cite}`Lebert2022`. Let's view the original video and the motion-compensated video side by side using {func}`optimap.show_video_pair`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play2(video,\n",
-                "               video_warped,\n",
-                "               title1=\"with motion\",\n",
-                "               title2=\"without motion\",\n",
-                "               skip_frame=3);"
+                "om.show_video_pair(video,\n",
+                "                   video_warped,\n",
+                "                   title1=\"with motion\",\n",
+                "                   title2=\"without motion\",\n",
+                "                   skip_frame=3);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -543,14 +533,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.12.2"
         },
         "test_name": "notebook1"
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/cv.ipynb` & `opticalmapping-0.2.2/docs/tutorials/strain.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941881613756614%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(1, 'Download this tutorial as a {download}`Jupyter notebook "*

 * *            '<converted/plotting.ipynb>`, or a {download}`python script <converted/plotting.py>` '*

 * *            'with code cells. We highly recommend using [Visual Studio C […]*

```diff
@@ -22,51 +22,51 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "source": [
                 "```{tip}\n",
-                "Download this tutorial as a {download}`Jupyter notebook <converted/cv.ipynb>`, or a {download}`python script <converted/cv.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
+                "Download this tutorial as a {download}`Jupyter notebook <converted/plotting.ipynb>`, or a {download}`python script <converted/plotting.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 6: Conduction Velocity\n",
+                "# Tutorial 10: Strain\n",
                 "\n",
-                "This tutorial will discuss how to compute conduction velocities from cardiac optical mapping data using ``optimap``. \n",
+                "This tutorial demonstrates how to calculate strain.\n",
                 "\n",
                 "```{warning}\n",
                 "This tutorial is currently under development. We will add more information soon.\n",
                 "```"
             ]
         }
     ],
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/io.ipynb` & `opticalmapping-0.2.2/docs/tutorials/io.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9532692636580358%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(1, 'Download this tutorial as a {download}`Jupyter notebook "*

 * *            '<converted/io.ipynb>`, or as a {download}`python script <converted/io.py>` with code '*

 * *            "cells.\\n')], delete: [1]}}, 3: {'source': {insert: [(2, ' […]*

```diff
@@ -22,470 +22,463 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "source": [
                 "```{tip}\n",
-                "Download this tutorial as a {download}`Jupyter notebook <converted/smoothing.ipynb>`, or a {download}`python script <converted/smoothing.py>` with code cells.\n",
+                "Download this tutorial as a {download}`Jupyter notebook <converted/io.ipynb>`, or as a {download}`python script <converted/io.py>` with code cells.\n",
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Tutorial 13: Import / Export (I/O)\n",
                 "\n",
-                "Using ``optimap`` you can import, export or convert various video or image file formats acquired with different cameras and software packages. For instance, you can load .rsh videos acquired with SciMedia cameras and save them as Matlab files using the following few lines of code:"
+                "Using ``optimap`` you can import, export or convert various video or image file formats acquired with different cameras and software packages. For instance, you can load `.rsh` videos acquired with SciMedia cameras and save them as Matlab files using the following few lines of code:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "\n",
-                "video = om.load_video('filename_of_input_video.rsh')\n",
-                "video = video[:100] # store only the first 100 frames, optional\n",
-                "om.video.save_video('video.mat', video)"
+                "video = om.load_video(\"filename_of_input_video.rsh\")\n",
+                "om.video.save_video(\"video.mat\", video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Many more file formats can be imported, saved or exported. More detailed instructions are provided below. To test whether you can load your own example video file (e.g. an .rsh file), make sure that the video is located in the appropriate folder, copy and paste the code above into a python script, modify the filename to match your filename and execute the script.\n",
                 "\n",
                 "## Importing Videos\n",
                 "\n",
                 "The following file formats can be imported with ``optimap``:\n",
                 "\n",
-                "* .tif, .tiff (TIFF)\n",
-                "* .png (PNG)\n",
+                "* .tif, .tiff (TIFF) image stacks\n",
+                "* Folder containing sequence of TIFF or .png (PNG) images\n",
                 "* .gsd, .gsh (SciMedia MiCAM 05)\n",
                 "* .rsh, .rsm, .rsd (SciMedia MiCAM ULTIMA)\n",
                 "* .dat (MultiRecorder)\n",
-                "* .npy (numpy array)\n",
+                "* .npy (NumPy array)\n",
                 "* .mat (MATLAB), loads the first field in the file\n",
                 "\n",
                 "Additional file formats will be added in the future (and upon request). All files can be imported using the same {func}`load_video` function, with which it is also possible to load only a specific number of frames or range of the data (e.g. from a specific frame to another), see below. \n",
                 "\n",
-                "### TIFF Images\n",
+                "````{dropdown} TIFF Stacks\n",
+                ":open:\n",
                 "\n",
-                "``optimap`` can read .tif / .tiff (TIFF) saved as an image stack (a single file) or an image series in a folder (8-bit and 16-bit). Simply provide the filename with the .tif or .tiff ending to load a single TIFF stack:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "video = om.load_video('filename.tif')"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "or the name of the folder containing the images to load a series of .tif images:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "video = om.load_video('folder_containing_tif_images/')"
+                "``optimap`` can read .tif / .tiff (TIFF) saved as an image stack (a single file):\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.tif\")\n",
+                "```\n",
+                "````\n",
+                "\n",
+                "\n",
+                "````{dropdown} Folder of TIFF/PNG Images\n",
+                "Optimap can read a series of .tif / .tiff (TIFF) or .png (PNG) images stored in a folder. Simply provide the path to folder containing the image series. 16-bit TIFF or PNG images are supported.\n",
+                "    \n",
+                "```python\n",
+                "video = om.load_video(\"example_folder\")\n",
+                "```\n",
+                "\n",
+                "The images filenames in the folder will be sorted in natural order (i.e `frame_2.png` comes before `frame_10.png`) and loaded in that order.\n",
+                "\n",
+                "If a folder contains several image series, use {func}`video.load_image_folder` instead:\n",
+                "```python\n",
+                "video = om.load_image_folder(\"example_folder\", prefix=\"frame_\")\n",
+                "```\n",
+                "where `prefix` is the common prefix of the image series filenames.\n",
+                "````\n",
+                "\n",
+                "````{dropdown} SciMedia\n",
+                "Optimap can read the different SciMedia file formats, including video files acquired with single- and dual-camera systems.\n",
+                "\n",
+                "To import Scimedia MiCAM ULTIMA video files provide the path to an .rsh or .rsm file:\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.rsh\")\n",
+                "```\n",
+                "\n",
+                "See the {class}`video.MiCAM_ULTIMA_Importer` class for more details and options.\n",
+                "\n",
+                "For Scimedia MiCAM 05 video files provide the path to an .gsd or .gsh file:\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.gsh\")\n",
+                "```\n",
+                "\n",
+                "See the {class}`video.MiCAM05_Importer` class for more details and options.\n",
+                "\n",
+                "For both MiCAM Ultima or MiCam 05 you can load the metadata of the video file with {func}`video.load_metadata`:\n",
+                "```python\n",
+                "metadata = om.load_metadata(\"example.rsh\")\n",
+                "print(metadata)\n",
+                "```\n",
+                "````\n",
+                "\n",
+                "````{dropdown} MultiRecorder\n",
+                "optimap can import .dat video files acquired with MultiRecorder (developed by J. Schr\u00f6der-Schetelig, Max Planck Institute for Dynamics and Self-Organization).\n",
+                "```python\n",
+                "video = om.load_video(\"example.dat\")\n",
+                "```\n",
+                "\n",
+                "See the {class}`video.MultiRecorderImporter` class for more details and options.\n",
+                "\n",
+                "The metadata of the video file can be loaded with {func}`video.load_metadata`:\n",
+                "```python\n",
+                "metadata = om.load_metadata(\"example.dat\")\n",
+                "print(metadata)\n",
+                "```\n",
+                "````\n",
+                "\n",
+                "````{dropdown} NumPy\n",
+                "Videos stored as numpy arrays can easily be imported using:\n",
+                "```python\n",
+                "video = om.load_video(\"example.npy\")\n",
+                "```\n",
+                "````\n",
+                "\n",
+                "````{dropdown} MATLAB\n",
+                "Videos stored as arrays in the Matlab file format (.mat) can easily be imported using\n",
+                "    \n",
+                "```python\n",
+                "video = om.load_video(\"example.mat\")\n",
+                "```\n",
+                "\n",
+                "This will load the first field in the file. To load a specific field/variable, use the following syntax:\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.mat\", fieldname=\"field_name\")\n",
+                "```\n",
+                "````"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### PNG Images\n",
+                "In all cases, it is possible to import only parts of a video to reduce loading times using the following optional arguments:\n",
+                "\n",
+                "* `start_frame`: The first frame to load (default: 0)\n",
+                "* `frames`:  Number of frames to load (default: all)\n",
+                "* `step`:  Load every `step`-th frame (default: 1)\n",
                 "\n",
-                "``optimap`` can read a series of .png (PNG) images stored in a folder. Simply provide the name of the folder containing the image series."
+                "For instance, load 1000 frames and only every 2nd frame starting from frame 100:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = om.load_video('folder_containing_png_images/')"
+                "video = om.load_video(\"filename.tif\", frames=1000, step=2, start_frame=100)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### SciMedia\n",
+                "This will load frames 100, 102, 104, 106, ..., 2098.\n",
                 "\n",
-                "``optimap`` can read the different SciMedia file formats, including video files acquired with single- and dual-camera systems. To import Scimedia MiCAM ULTIMA video files you only need to provide the filename with the .rsh ending of the header file (assuming it is located in the same location as the .rsd files):"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "video = om.load_video('filename.rsh')"
+                "\n",
+                "Some formats can be loaded using memory mapping, which can be useful to reduce memory usage or loading times when working with large or numerous video files. This is enabled by setting the `use_mmap` argument to `True`:\n",
+                "```python\n",
+                "video = om.load_video(\"example.npy\", use_mmap=True)\n",
+                "```\n",
+                "This will load the video as a read-only memory-mapped array, which means that the data is not loaded into memory until it is accessed. `use_mmap` is disabled by default and only supported for TIFF stacks, MultiRecorder .dat files and NumPy .npy files.\n",
+                "\n",
+                "````{note}\n",
+                "Imported videos retain the same data type as the original file. For instance, 16-bit TIFF images will be loaded as 16-bit arrays, and 8-bit images as 8-bit arrays.\n",
+                "\n",
+                "Often it is useful to convert the data to 32-bit floating point arrays and to normalize the data to the range [0, 1]. This can be done using the {func}`video.normalize` method.\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.tif\")\n",
+                "video = om.video.normalize(video)\n",
+                "```\n",
+                "This will convert the video to 32-bit floating point arrays and normalize the data to the range [0, 1] based on the minimum and maximum values in the video.\n",
+                "\n",
+                "To specify a custom range for normalization to [0, 1], use the `vmin` and `vmax` arguments:\n",
+                "\n",
+                "```python\n",
+                "video = om.load_video(\"example.dat\")\n",
+                "# 12-bit data, normalize to [0, 1]\n",
+                "video = om.video.normalize(video, vmin=0, vmax=4095)\n",
+                "```\n",
+                "````"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To import Scimedia MiCAM 05 video files you only need to provide the filename with the .gsh ending of the header file:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "video = om.load_video('filename.gsh')"
+                "## Importing Images and Masks\n",
+                "\n",
+                "Individual images (.tif, .png, .jpg, .npy, ...) can be imported using {func}`load_image`:\n",
+                "\n",
+                "```python\n",
+                "image = om.load_image(\"example.tif\")\n",
+                "```\n",
+                "the `as_grey` argument can be used to convert the image to a grayscale image (if it is not already).\n",
+                "\n",
+                "Segmentation masks can be imported using {func}`load_mask`:\n",
+                "```python\n",
+                "mask = om.load_mask(\"mask.png\")\n",
+                "```\n",
+                "See [Tutorial 3: Masking / Segmentation](/tutorials/mask) for more details on how to load, create and use masks."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### MultiRecorder\n",
+                "## Saving / Exporting Videos\n",
+                "\n",
+                "The following file formats can be saved / exported with ``optimap``:\n",
+                "\n",
+                "* videos as raw data (TIFF stacks, NumPy or Matlab files)\n",
+                "* image sequences in a folder\n",
+                "* rendered videos with or without colormap (e.g. .mp4 videos)\n",
+                "* multiple videos rendered next to each other\n",
+                "* video rendered with overlays\n",
+                "\n",
+                "``optimap`` distinguishes saving and exporting files. Saving files saves them as raw data (e.g. three-dimensional arrays), while exporting renders videos for visualization purposes (such as a .mp4 file). Saving videos prevents data loss (e.g. floating point or integer precision is preserved) and one can reload and continue to process the saved videos later. Exporting data is associated with data loss (e.g. loss of floating point precision) as the recording is rendered using a video encoder.\n",
                 "\n",
-                "``optimap`` can import .dat video files acquired with MultiRecorder (developed by J. Schr\u00f6der-Schetelig, Max Planck Institute for Dynamics and Self-Organization)."
+                "### Saving Videos\n",
+                "\n",
+                "The default mode in ``optimap`` is to save videos as arrays in numpy (.npy) or Matlab (.mat) file formats. This saves the data in its rawest form without information loss:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = om.load_video('filename.dat')"
+                "# NumPy NPY format\n",
+                "om.save_video('video.npy', video)\n",
+                "# TIFF image stack\n",
+                "om.save_video('video.tif', video)\n",
+                "# MATLAB\n",
+                "om.save_video('video.mat', video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Numpy\n",
+                "The videos can later be imported and further processed or used in other applications. The {func}`save_video` function preserves the data type (e.g. floating point or integer precision).\n",
                 "\n",
-                "Videos stored as numpy arrays can easily be imported using:"
+                "Another way to save video data is to save them as a TIFF or PNG image series in a folder (here called ``\"my_folder\"``):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = om.load_video('filename.npy')"
+                "om.save_image_sequence(\".\", video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Matlab\n",
-                "\n",
-                "Videos stored as arrays in the Matlab file format (.mat) can easily be imported using:"
+                "Will create files `frame_0000.png`, `frame_0001.png`, ... in the current working directory. The `prefix` argument can be used to specify a custom prefix for the filenames, and the `format` argument can be used to specify the file format (`.png` by default)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = om.load_video('filename.mat')"
+                "om.save_image_sequence(r\"C:\\example_directory\", video, filepattern=\"frame-{:04d}\", format=\".tif\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "It is possible to import only parts of a video, for instance, only 1000 frames and only every 2nd frame starting from frame 100:"
+                "The resulting images will have the same resolution as the video. If the videos are 8- or 16-bit, then the resulting .tif or .png images will automatically be 8- or 16-bit, correspondingly. It is recommended to save your video as 16-bit to prevent data loss. If the images are all black, all white, show salt and pepper noise or look weird in any way it is likely that your video was formatted incorrectly (e.g. is an integer video even though the original video was floating point). For instance, 8-bit videos can only contain integer values between 0-255. You can use the code snippet below to format your video data before saving it as an image series:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video = om.load_video('filename.npy', start_frame=100, frames=1000, step=2, use_mmap=False)"
+                "# Convert to uint8 data type with has value range [0-255]\n",
+                "video = om.video.normalize(video, dtype=\"uint8\")\n",
+                "om.print_properties(video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This option is available for all file formats including image series. Please refer to the Documentation for more information.\n",
-                "\n",
-                "## Saving / Exporting Videos\n",
-                "\n",
-                "The following file formats can be saved / exported with ``optimap``:\n",
-                "\n",
-                "* videos as raw data (numpy or Matlab arrays)\n",
-                "* rendered videos (e.g. .mp4 videos)\n",
-                "* images as raw data (numpy or Matlab arrays)\n",
-                "* multiple videos rendered next to each other (e.g. .mp4 videos)\n",
-                "* image sequences in a folder\n",
+                "With the normalization (the subtraction of the minimum and the division by the maximum) in the code snippet above it is ensured that no values are below 0 or above 255 (or 65536, respectively).\n",
                 "\n",
-                "``optimap`` distinguishes saving and exporting files. Saving files saves them as raw data (e.g. three-dimensional arrays), while exporting renders videos for visualization purposes (such as a .mp4 file). Saving videos prevents data loss (e.g. floating point or integer precision is preserved) and one can reload and continue to process the saved videos later. Exporting data is associated with data loss (e.g. loss of floating point precision) and compression because the video is rendered using a video encoder.\n",
+                "### Video Export\n",
                 "\n",
-                "### Saving Videos\n",
+                "The main purpose of exporting videos is to generate or render videos in a file format (.mp4) that can be played with an external video player application (e.g. Quicktime, VLC, Windows Media Player etc.) or be included in slideshows (e.g. Powerpoint). You can export videos in several ways: \n",
                 "\n",
-                "The default mode in ``optimap`` is to save videos as arrays in numpy (.npy) or Matlab (.mat) file formats. This saves the data in its rawest form without information loss:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "om.save_video('video.npy',video)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "om.save_video('video.mat',video)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The videos can later be imported and further processed or used in other applications. The {func}`save_video` function preserves the data type (e.g. floating point precision).\n",
+                "* a single grayscale video (e.g. showing the original or normalized video)\n",
+                "* a processed video (e.g. phase maps) with a special colormap (e.g. hsv, jet, magma, etc.)\n",
+                "* an overlay of 2 videos on top of each other (e.g. original grayscale video plus calcium waves highlighted in a particular color)\n",
+                "* multiple videos rendered next to each other (e.g. original grayscale video plus motion-stabilized video or original grayscale video and processed video in a different colorcode)\n",
                 "\n",
-                "Another way to save video data is to save them as a TIFF or PNG image series in a folder (here called ``\"my_folder\"``):"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "om.save_image_sequence(video, filepattern=\"frame-{:04d}\", directory=\"my_folder\", suffix=\".tif\")"
+                "The most straight-forward way to export a video is:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.save_image_sequence(video, filepattern=\"frame-{:04d}\", directory=\"my_folder\", suffix=\".png\")"
+                "om.export_video('video.mp4', video)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The resulting images will have the same dimension as the video (e.g. 100x100 or 128x128 pixels). The `filepattern` can be modified, e.g. the `\"frame-\"` can be left out to obtain only zero-padded numbers (you want to change `:04d` to `:05d` if your video has more than 9999 frames). If the videos are 8- or 16-bit, then the resulting .tif or .png images will automatically be 8- or 16-bit, correspondingly. Accordingly, it is possible to prevent data loss if your raw video is 16-bit. If the images are all black, all white, show salt and pepper noise or look weird, then you need make sure that your video contains values which are normalized and formatted correctly. For instance, 8-bit videos can only contain integer values between 0-255. You can use the code snippet below to format your video data before saving it as an image series:"
+                "This will generate a .mp4 video file containing the entire video data at the original resolution with a display framerate of 60fps (default). You can customize the video export as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "import numpy as np\n",
-                "\n",
-                "om.print_properties(video)\n",
-                "video = video.astype(np.float32)\n",
-                "video = (video-np.min(video))/np.max(video)*255 # alternatively *65536 for 16-bit\n",
-                "om.print_properties(video)\n",
-                "video = video.astype(np.uint8) # alternatively np.uint16 for 16-bit\n",
-                "om.print_properties(video)"
+                "om.export_video(\"video.mp4\", video[100:500], fps=30, skip_frames=2,\n",
+                "                cmap=\"viridis\", vmin=0.1, vmax=0.9)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "With the normalization (the subtraction of the minimum and the division by the maximum) in the code snippet above it is ensured that no values are below 0 or above 255 (or 65536, respectively).\n",
-                "\n",
-                "### Video Export\n",
-                "\n",
-                "The main purpose of exporting videos is to generate or render videos in a file format (.mp4) that can be played with an external video player application (e.g. Quicktime, VLC, Windows Media Player etc.). You can export videos in several ways: \n",
-                "\n",
-                "* a single grayscale video (e.g. showing the original or normalized video)\n",
-                "* a processed video (e.g. phase maps) with a special colormap (e.g. hsv, jet, magma, etc.)\n",
-                "* an overlay of 2 videos on top of each other (e.g. original grayscale video plus calcium waves highlighted in a particular color)\n",
-                "* multiple videos rendered next to each other (e.g. original grayscale video plus motion-stabilized video)\n",
+                "Here, only every 2nd frame from frames 100-500 are exported to a video with a framerate of 30fps, `vmin` and `vmax` define the dynamic range of pixel values (0.1 is black and 0.9 white with the grayscale colormap) and the `viridis` colormap.\n",
                 "\n",
-                "The most straight-forward way to export a video is:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "skip-execution"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "om.export_video('video.mp4', video)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "This will generate a rendered .mp4 video containing the entire video data at a framerate of 60fps and at the original resolution (e.g. 100x100 or 128x128 pixels). You can customize the video export as follows:"
+                "You can overlay a processed video, for instance, a pixel-wise normalized video which shows action potential or calcium waves, see [Tutorial 2](signal_extraction.ipynb), on top of the original grayscale video as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.export_video(\"video.mp4\", video[123:323], fps=30, skip_frames=2, vmin=0.1, vmax=0.9, cmap=\"viridis\")"
+                "video_waves = om.video.normalize_pixelwise(video)\n",
+                "om.video.export_video_with_overlay(\"video.mp4\", video, video_waves)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here, only every 2nd frame from frames 123-323 are exported at a framerate of 30fps, `vmin` and `vmax` define the dynamic range of pixel values (0.1 is black and 0.9 white with the grayscale colormap) and `viridis` is a different colormap than just a grayscale colormap.\n",
-                "\n",
-                "You can overlay a processed video, for instance, a pixel-wise normalized video which shows action potential or calcium waves, see [Tutorial 2](signal_extraction.ipynb), on top of the original grayscale video as follows:"
+                "Lastly, you can export animated plots, such as two videos in two sublots next to each other, as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "video_waves = om.video.normalize_pixelwise(video)\n",
-                "om.export_video_with_overlay(\"video.mp4\", video, video_waves)"
+                "animated_plot = om.show_video_pair(video, video_waves, title1='Video 1', title2='Video 2')\n",
+                "animated_plot.save(\"Exported Animation with 2 Videos.mp4\")\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "```{warning}\n",
-                "This tutorial is currently work in progress. We will add more information soon.\n",
-                "```"
+                "You can also export various other animated plots using the same code snippet from above."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/mask.ipynb` & `opticalmapping-0.2.2/docs/tutorials/mask.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962412698412698%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(1, 'Download this tutorial as a {download}`Jupyter notebook "*

 * *            '<converted/mask.ipynb>`, or as a {download}`python script <converted/mask.py>` with '*

 * *            'code cells. We highly recommend using [Visual Studio Code]( […]*

```diff
@@ -22,68 +22,68 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "source": [
                 "```{tip}\n",
-                "Download this tutorial as a {download}`Jupyter notebook <converted/mask.ipynb>`, or a {download}`python script <converted/mask.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
+                "Download this tutorial as a {download}`Jupyter notebook <converted/mask.ipynb>`, or as a {download}`python script <converted/mask.py>` with code cells. We highly recommend using [Visual Studio Code](#vscode) to execute this tutorial.\n",
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Tutorial 3: Masking / Segmentation\n",
                 "\n",
                 "This tutorial explains how to select a region of interest in a video using ``optimap``. For instance, it is possible to use ``optimap`` to automatically select the heart surface, to manually draw a region of interest in the video image, or to ignore parts of the video close to the boundary. The post-processing can then be applied to  the masked or segmented part of the video image, for instance. ``optimap`` provides several easy-to-use routines for these purposes.\n",
                 "\n",
-                "We will first load an example video file using the following code (done automatically):"
+                "We will first load an example video file using the following code:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped.npy')\n",
+                "filepath = om.download_example_data('VF_Rabbit_1_warped.npy')\n",
                 "video_warped = om.load_video(filepath)\n",
                 "om.print_properties(video_warped)\n",
                 "\n",
                 "frame = video_warped[0]  # first frame"
             ]
         },
         {
@@ -192,15 +192,15 @@
                 "tags": [
                     "remove-input",
                     "remove-output"
                 ]
             },
             "outputs": [],
             "source": [
-                "fn = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped_mask.npy', silent=True)\n",
+                "fn = om.download_example_data('VF_Rabbit_1_warped_mask.npy', silent=True)\n",
                 "manual_mask = om.load_mask(fn)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -312,28 +312,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.play_video(video_warped)"
+                "om.show_video(video_warped)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.play_video(video_warped))"
+                "render_ani_func(lambda: om.show_video(video_warped))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -345,14 +345,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.12.2"
         },
         "test_name": "notebook1"
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/phase.ipynb` & `opticalmapping-0.2.2/docs/tutorials/phase.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996322007063695%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(11, '        ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [16, 4, 3]}}, 4: "*

 * *            '{\'source\': {insert: [(3, "filepath = '*

 * *            'om.download_example_data(\'VF_Rabbit_1.npy\')\\n"), (4, \'video = '*

 * *            "om.load_video(filepath, frames=500)\\n'), (10, 'video_warped_normalized = "*

 * *            "om.video.normalize_pixelwise_slidingwindow(video_warped, window_size=60)')], delete: "*

 * *   […]*

```diff
@@ -22,28 +22,27 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -73,25 +72,22 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "import numpy as np\n",
                 "\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy')\n",
-                "# alterantively set filepath = '/folder_on_your_computer/Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy'\n",
-                "video = om.load_video(filepath)[:500]\n",
+                "filepath = om.download_example_data('VF_Rabbit_1.npy')\n",
+                "video = om.load_video(filepath, frames=500)\n",
                 "video_warped = om.motion_compensate(video,\n",
                 "                              contrast_kernel=5,\n",
                 "                              presmooth_spatial=1,\n",
                 "                              presmooth_temporal=1)\n",
                 "\n",
-                "video_warped_normalized = om.video.normalize_pixelwise_slidingwindow(video_warped, window_size=60)\n",
-                "\n",
-                "#del video, video_warped"
+                "video_warped_normalized = om.video.normalize_pixelwise_slidingwindow(video_warped, window_size=60)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The pixel-wise normalized motion-stabilized video displays action potential vortex waves as black waves (when using a black-and-white colormap):"
@@ -103,28 +99,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play(video_warped_normalized, interval=40);"
+                "om.show_video(video_warped_normalized, interval=40);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play(video_warped_normalized, interval=40))"
+                "render_ani_func(lambda: om.show_video(video_warped_normalized, interval=40))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Next, we will first compute and display a phase video from the pixel-wise normalized video. Alternatively to a pixel-wise normalized video one could also compute phase maps from a frame-wise differentiated video, see below. We will then smooth the phase video using spatio-temporal phase smoothing filters, and ,lastly, calculate and track phase singularities through the video."
@@ -178,28 +174,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play(video_phase, title='phase video', cmap='hsv', interval=40);"
+                "om.show_video(video_phase, title='phase video', cmap='hsv', interval=40);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play(video_phase, title='phase video', cmap='hsv', interval=40))"
+                "render_ani_func(lambda: om.show_video(video_phase, title='phase video', cmap='hsv', interval=40))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We chose the continuous colormap 'hsv' which displays both $-\\pi$ and $\\pi$ in red. The 'hsv' colormap has the following advantages: 1) there is no discontinuity at the phase shift from $-\\pi$ to $\\pi$, 2) all lines of equal phase are displayed by lines of equal color, 3) it is easier to identify pinwheel patterns or 'rotors'. \n",
@@ -245,28 +241,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play(video_phase_filtered, title='removed outliers', cmap='hsv', interval=40);"
+                "om.show_video(video_phase_filtered, title='removed outliers', cmap='hsv', interval=40);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play(video_phase_filtered, title='removed outliers', cmap='hsv', interval=40))"
+                "render_ani_func(lambda: om.show_video(video_phase_filtered, title='removed outliers', cmap='hsv', interval=40))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we can infill all NaN pixels with interpolated phase values from the surrounding tissue, which we compute using the {func}`phasefilter_fillsmooth` function that operates on the complex phase values:\n",
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/plotting.ipynb` & `opticalmapping-0.2.2/docs/tutorials/plotting.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978050595238095%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}, 3: "*

 * *            "{'source': {insert: [(0, '# Tutorial 11: Plotting Optical Traces\\n')], delete: "*

 * *            '[0]}}}'}*

```diff
@@ -22,27 +22,27 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -56,15 +56,15 @@
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 11: Plotting Traces\n",
+                "# Tutorial 11: Plotting Optical Traces\n",
                 "\n",
                 "This tutorial will discuss how to plot and visualize optical traces from cardiac optical mapping data using ``optimap``. \n",
                 "\n",
                 "```{warning}\n",
                 "This tutorial is currently under development. We will add more information soon.\n",
                 "```"
             ]
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/ratiometry.ipynb` & `opticalmapping-0.2.2/docs/tutorials/ratiometry.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785517250881834%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(11, '        ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [16, 4, 3]}}, 2: "*

 * *            "{'source': {insert: [(6, '## Combining Numerical Motion Compensation and "*

 * *            "Ratiometry\\n'), (8, 'In this tutorial, we will discuss the analysis of ratiometric "*

 * *            'optical mapping data and the benefits of combining numerical motion tracking with '*

 * *            'ratiometric imaging. Ratiomet […]*

```diff
@@ -22,60 +22,59 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```{tip}\n",
                 "Download this tutorial as a {download}`Jupyter notebook <converted/ratiometry.ipynb>`, or a {download}`python script <converted/ratiometry.py>` with code cells.\n",
                 "```\n",
                 "\n",
                 "# Tutorial 7: Ratiometry\n",
                 "\n",
-                "## Combining Numerical Motion Compensation and Ratiometry with Di-4-ANEPPS\n",
+                "## Combining Numerical Motion Compensation and Ratiometry\n",
                 "\n",
-                "In this tutorial, we will discuss the analysis of ratiometric optical mapping data and the benefits of a combined approach consisting of numerical motion tracking and ratiometric imaging. Numerical motion tracking and motion-stabilization alone cannot inhibit motion artifacts entirely, see Tutorials [1](basics.ipynb) & [4](motion_compensation.ipynb). Numerical motion tracking alone cannot remove all motion artifacts alone, because it does not remove the relative motion between the tissue and the light sources used to excite the fluorescent dye. Motion tracking is merely a change of the frame of reference. The physical relative motion persists afer numerical motion-stabilization and causes fluctuations in the illumination. Typically, what can be seen in motion-stabilized videos is that the illumination (e.g. a Gaussian intensity distribution) moves back and forth across the tissue which leads to illumination artifacts. Motion artifacts therefore often have two components: dissociation-related motion artifacts and illumination artifacts. To achieve better artifact compensation, particularly with stronger motion, it is therefore required to combine numerical motion tracking with ratiometric imaging, as described in {cite:t}`Kappadan2020` or in {cite:t}`Zhang2016`. \n",
+                "In this tutorial, we will discuss the analysis of ratiometric optical mapping data and the benefits of combining numerical motion tracking with ratiometric imaging. Ratiometry can help suppress motion artifacts, as it exploits that some fluorescent indicators, such as Di-4-ANEPPS or Di-4-ANBDQPQ, respond differently to different excitation wavelengths and/or produce different signals with different emission filters. {cite:t}`Knisley2000` and {cite:t}`Bachtel2011` demonstrated ratiometric voltage-sensitive optical mapping with Di-4-ANEPPS and showed that it is possible to effectively inhibit motion artifacts by separating signal from non-signal components. With the right emission filter, Di-4-ANEPPS produces positive and negative signals at different excitation wavelengths/channels (e.g. blue vs. green), while non-signal components appear equally in both wavelengths/channels, see [{footcite:t}`Kappadan2020,Bachtel2011,Zhang2016`]. Non-signal components can be removed by calculating the ratio between the two signals. The non-signal components are usually caused by motion. Ratiometry is ideally combined with numerical motion compensation, because either technique alone cannot fully compensate motion artifacts, see also Tutorials [1](basics.ipynb) and [4](motion_compensation.ipynb). Numerical motion tracking and compensation does not remove physical motion between the tissue and the illumination, it just removes the motion virtually. The motion can cause illumination changes (e.g. the heart moves back and forth between two LEDs), which persist in the motion-stabilized videos and modulate and distort the signal that we aim to measure. Vice versa, ratiometry alone does not extract the signal in a co-moving frame of reference which is essential when aiming to inhibit motion artifacts. However, taken together, these two techniques can measure the signal in a co-moving frame of reference and compensate the non-stationary illumination in the motion-stabilized videos. \n",
                 "\n",
-                "In the example below, the heart was stained with Di-4-ANEPPS and imaged using alternating green and blue illumination at 500fps. More specifically, the tissue was illuminated in every odd frame with green light and in every even frame with blue light, respectively. This approach is also referred to as 'excitation ratiometry'. After numerical motion tracking and stabilization, the green and blue videos are divided by each other to obtain a motion-stabilized ratiometric video. Using this method, both motion artifacts as well as illumination artifacts (which also lead to motion artifacts) can be significantly reduced. \n",
+                "In the example below, the heart was stained with Di-4-ANEPPS and imaged using alternating green and blue illumination at 500fps. More specifically, the tissue was illuminated in every odd frame with green light and in every even frame with blue light, respectively. This approach is also referred to as 'excitation ratiometry'. After numerical motion tracking and stabilization, the green and blue videos are divided by each other to obtain a motion-stabilized ratiometric video. Using this method, both motion artifacts as well as illumination artifacts (which also lead to motion artifacts) can be significantly reduced.\n",
                 "\n",
                 "First, we load the video data, which is stored as a single file (`Example_05_Ratiometry.npy`) containing the two green and blue videos in an interleaved fashion (frame 1 = green, frame 2 = blue, frame 3 = green, etc.). Using optimap's {func}`load_video()` function, we can specify to load only every 2nd frame and to start reading from the first or the second frame, respectively:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "\n",
-                "filename = om.utils.retrieve_example_data('Example_05_Ratiometry.npy')\n",
+                "filename = om.download_example_data(\"Ratiometry_1.npy\")\n",
                 "video_blue = om.load_video(filename, start_frame=0, step=2)\n",
                 "video_green = om.load_video(filename, start_frame=1, step=2)\n",
                 "\n",
                 "om.print_properties(video_blue)\n",
                 "om.print_properties(video_green)\n"
             ]
         },
@@ -94,30 +93,30 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play2(video_green, video_blue,\n",
-                "               title1=\"green video with signal\",\n",
-                "               title2=\"blue video without signal\");"
+                "om.show_video_pair(video_green, video_blue,\n",
+                "                   title1=\"green video with signal\",\n",
+                "                   title2=\"blue video without signal\");"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play2(video_green, video_blue, title1=\"green video with signal\", title2=\"blue video without signal\", interval=20))"
+                "render_ani_func(lambda: om.show_video_pair(video_green, video_blue, title1=\"green video with signal\", title2=\"blue video without signal\", interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If we plot and compare two optical traces from the green and blue videos respectively, we can see not in all but in most areas stronger intensity fluctuations in the green video:"
@@ -169,15 +168,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "om.show_positions(video_green[0], positions)"
+                "om.show_positions(positions, video_green[0])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now let's perform numerical motion tracking and motion-stabilization with the green and blue videos:"
@@ -192,15 +191,15 @@
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped_green = om.motion_compensate(video_green, contrast_kernel=5, ref_frame=0)\n",
                 "video_warped_blue = om.motion_compensate(video_blue, contrast_kernel=5, ref_frame=0)\n",
-                "om.video.playn([video_green, video_warped_green, video_blue, video_warped_blue],\n",
+                "om.show_videos([video_green, video_warped_green, video_blue, video_warped_blue],\n",
                 "               titles=[\"video green\", \"stabilized video green\", \"video blue\", \"stabilized video blue\"],\n",
                 "               figsize=(8, 3));"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -209,15 +208,15 @@
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped_green = om.motion_compensate(video_green, contrast_kernel=5, ref_frame=0)\n",
                 "video_warped_blue = om.motion_compensate(video_blue, contrast_kernel=5, ref_frame=0)\n",
-                "render_ani_func(lambda: om.video.playn([video_green, video_warped_green, video_blue, video_warped_blue],\n",
+                "render_ani_func(lambda: om.show_videos([video_green, video_warped_green, video_blue, video_warped_blue],\n",
                 "               titles=[\"video green\", \"stabilized video green\", \"video blue\", \"stabilized video blue\"],\n",
                 "               figsize=(8, 3)))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -296,15 +295,15 @@
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped_ratio = video_warped_green/video_warped_blue\n",
-                "om.video.playn([video_green, video_warped_green, video_warped_blue, video_warped_ratio],\n",
+                "om.show_videos([video_green, video_warped_green, video_warped_blue, video_warped_ratio],\n",
                 "               titles=[\"video green\", \"stabilized video green\", \"stabilized video blue\", \"stabilized video ratio\"],\n",
                 "               figsize=(8, 3));"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -312,15 +311,15 @@
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped_ratio = video_warped_green/video_warped_blue\n",
-                "render_ani_func(lambda: om.video.playn([video_green, video_warped_green, video_warped_blue, video_warped_ratio],\n",
+                "render_ani_func(lambda: om.show_videos([video_green, video_warped_green, video_warped_blue, video_warped_ratio],\n",
                 "               titles=[\"video green\", \"stabilized video green\", \"stabilized video blue\", \"stabilized video ratio\"], \n",
                 "               figsize=(8, 3),\n",
                 "               interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
@@ -350,84 +349,36 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "om.compare_traces([video_warped_green_norm, video_warped_ratio_norm],\n",
+                "om.compare_traces([video_warped_green_norm[:200], video_warped_ratio_norm[:200]],\n",
                 "                  positions,\n",
                 "                  labels=['warped green','ratio'],\n",
                 "                  size=3,\n",
                 "                  colors=['g', 'k'])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "These subtle improvements become more evident when you explore the data yourself:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "om.compare_traces([video_warped_green_norm, video_warped_ratio_norm],\n",
-                "                  labels=['green','ratio'],\n",
-                "                  size=3,\n",
-                "                  colors=['green', 'k'],\n",
-                "                  fps=250)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "and zoom in:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "t = 150\n",
-                "om.compare_traces([video_warped_green_norm[:t], video_warped_ratio_norm[:t]],\n",
-                "                  labels=['green','ratio'],\n",
-                "                  colors=['green', 'k'],\n",
-                "                  size=3,\n",
-                "                  fps=250)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "The action potential duration (APD) is more heterogeneous in non-ratiometric motion-stabilized videos."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "traces_blue, positions = om.select_traces(video_blue)\n",
-                "traces_green = om.extract_traces(video_green, positions)"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "TO DO: use flow field from blue channle to compensate the green channel"
+                "TO DO: use flow field from blue channle to compensate the green channel\n",
+                "\n",
+                "```{footbibliography}\n",
+                "```"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "napari",
             "language": "python",
@@ -439,14 +390,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.9"
+            "version": "3.12.2"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/signal_extraction.ipynb` & `opticalmapping-0.2.2/docs/tutorials/signal_extraction.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967987964416536%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(11, '        ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [16, 4, 3]}}, 4: "*

 * *            '{\'source\': {insert: [(3, "filepath = '*

 * *            'om.download_example_data(\'VF_Rabbit_1.npy\')\\n"), (9, \'om.show_video(video_warped, '*

 * *            'title="recording without motion", skip_frame=3);\')], delete: [10, 4, 3]}}, 5: '*

 * *            '{\'source\': {insert: [(5, "filepath = '*

 * *            'om.downloa […]*

```diff
@@ -22,28 +22,27 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -75,22 +74,21 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "import optimap as om\n",
                 "import numpy as np\n",
                 "\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy')\n",
-                "# alterantively set filepath = '/folder_on_your_computer/Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy'\n",
+                "filepath = om.download_example_data('VF_Rabbit_1.npy')\n",
                 "video = om.load_video(filepath)\n",
                 "video_warped = om.motion_compensate(video,\n",
                 "                              contrast_kernel=5,\n",
                 "                              presmooth_spatial=1,\n",
                 "                              presmooth_temporal=1)\n",
-                "om.video.play(video_warped, title=\"recording without motion\", skip_frame=3);"
+                "om.show_video(video_warped, title=\"recording without motion\", skip_frame=3);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -100,19 +98,19 @@
             "outputs": [],
             "source": [
                 "# Hidden, same as above but shorten the video slightly\n",
                 "\n",
                 "import optimap as om\n",
                 "import numpy as np\n",
                 "\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy')\n",
-                "video = om.load_video(filepath, use_mmap=True)[:500]\n",
-                "filepath = om.utils.retrieve_example_data('Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped.npy', silent=True)\n",
-                "video_warped = om.load_video(filepath, use_mmap=True)[:500]\n",
-                "render_ani_func(lambda: om.video.play(video_warped, title=\"recording without motion\", skip_frame=1, interval=20))"
+                "filepath = om.download_example_data('VF_Rabbit_1.npy')\n",
+                "video = om.load_video(filepath, use_mmap=True, frames=500)\n",
+                "filepath = om.download_example_data('VF_Rabbit_1_warped.npy', silent=True)\n",
+                "video_warped = om.load_video(filepath, use_mmap=True, frames=500)\n",
+                "render_ani_func(lambda: om.show_video(video_warped, title=\"recording without motion\", skip_frame=1, interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Measuring action potentials or calcium transients in cardiac optical mapping videos is conventionally performed pixel-by-pixel. In the absence of motion, either with Blebbistatin or after numerical motion inhibition, each pixel shows the same tissue segment throughout the video. This condition is a prerequisite for the following processing routines."
@@ -182,28 +180,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play(video_warped_pnorm, title=\"pixel-wise normalization\", interval=20);"
+                "om.show_video(video_warped_pnorm, title=\"pixel-wise normalization\", interval=20);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play(video_warped_pnorm, title=\"pixel-wise normalization\", interval=20))"
+                "render_ani_func(lambda: om.show_video(video_warped_pnorm, title=\"pixel-wise normalization\", interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The pixel-wise normalization amplifies temporal fluctuations and therefore emphasizes action potential waves (or equally calcium waves). In our case, the action potential waves correspond to dark/black waves due to the particular staining. The normalization presrves the shape of the action potential (vs. method 3 detailed further below). The shape of the negative excursion corresponds to the shape of the action potential (in our case inverted due to the staining and emission filter). Regions without signal become noise (e.g. the background). You may have noticed that the video gets darker towards the end. The pixel-wise normalization does not account for overall brightness changes or baseline drifts as the maximal and minimal values are only determined once from the entire time-series. Correspondingly, the optical traces sampled from the pixel-wise normalized video look as follows:"
@@ -267,28 +265,28 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play(video_warped_spnorm, title=\"sliding window normalization\", interval=20);"
+                "om.show_video(video_warped_spnorm, title=\"sliding window normalization\", interval=20);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "render_ani_func(lambda: om.video.play(video_warped_spnorm, title=\"sliding window normalization\", interval=20))"
+                "render_ani_func(lambda: om.show_video(video_warped_spnorm, title=\"sliding window normalization\", interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The differences between the sliding-window pixel-wise normalized and the pixel-wise normalized videos are subtle but you may notice that unlike the simply pixel-wise normalized video this video does not get darker towards the end. Accordingly, the optical traces sampled from the sliding-window pixel-wise normalized video show much less of a baseline drift:"
@@ -344,29 +342,29 @@
             },
             "outputs": [],
             "source": [
                 "n = 5\n",
                 "diff = om.video.temporal_difference(video_warped, n)\n",
                 "#diff[:, background_mask] = np.nan\n",
                 "abs_max = 0.33*np.nanmax(np.abs(diff))\n",
-                "om.video.play(diff, title=\"temporal difference\", cmap=\"PiYG\", vmin=-abs_max, vmax=abs_max, interval=20);"
+                "om.show_video(diff, title=\"temporal difference\", cmap=\"PiYG\", vmin=-abs_max, vmax=abs_max, interval=20);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "diff[diff > 0] = 0\n",
-                "om.video.play(diff, title=\"temporal difference\", cmap=\"PiYG\", vmin=-abs_max, vmax=abs_max, interval=20);"
+                "om.show_video(diff, title=\"temporal difference\", cmap=\"PiYG\", vmin=-abs_max, vmax=abs_max, interval=20);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can compare the sliding-window pixel-wise normalization and frame difference methods next to each other:"
@@ -378,15 +376,15 @@
             "metadata": {
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
-                "om.video.play2(video_warped_spnorm, diff, title1=\"Sliding Window\", title2=\"Frame Difference\", vmin1=0, vmax1=1, cmap2='gray', vmin2=0.2*np.nanmin(diff), vmax2=0, interval=20);"
+                "om.show_video_pair(video_warped_spnorm, diff, title1=\"Sliding Window\", title2=\"Frame Difference\", vmin1=0, vmax1=1, cmap2='gray', vmin2=0.2*np.nanmin(diff), vmax2=0, interval=20);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can and should also renormalize the frame difference video and compare the sliding-window pixel-wise normalization and sliding-window pixel-wise normalized frame difference methods next to each other:"
@@ -399,15 +397,15 @@
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "diff_norm = om.video.normalize_pixelwise_slidingwindow(diff, window_size=60)\n",
-                "om.video.play2(video_warped_spnorm, diff_norm, vmin1=0, vmax1=1, cmap2='gray', vmin2=0, vmax2=1, interval=20);"
+                "om.show_video_pair(video_warped_spnorm, diff_norm, vmin1=0, vmax1=1, cmap2='gray', vmin2=0, vmax2=1, interval=20);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -416,15 +414,15 @@
             },
             "outputs": [],
             "source": [
                 "diff = om.video.temporal_difference(video_warped, 10)\n",
                 "diff[diff > 0] = 0\n",
                 "#diff[:, background_mask] = np.nan\n",
                 "diff_norm = om.video.normalize_pixelwise_slidingwindow(-diff, window_size=60)\n",
-                "om.video.play_with_overlay(video_warped_norm, diff_norm, vmin_overlay=-1, vmax_overlay=1)"
+                "om.video.show_video_overlay(video_warped, diff_norm, vmin_overlay=-1, vmax_overlay=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -433,15 +431,15 @@
             },
             "outputs": [],
             "source": [
                 "diff = om.video.temporal_difference(video_warped, 10)\n",
                 "diff[diff > 0] = 0\n",
                 "#diff[:, background_mask] = np.nan\n",
                 "diff_norm = om.video.normalize_pixelwise_slidingwindow(-diff, window_size=60)\n",
-                "render_ani_func(lambda: om.video.play_with_overlay(video_warped, diff_norm, vmin_overlay=-1, vmax_overlay=1, interval=20))"
+                "render_ani_func(lambda: om.video.show_video_overlay(video_warped, diff_norm, vmin_overlay=-1, vmax_overlay=1, interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 3. Post-Processing\n",
@@ -467,15 +465,15 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "\n",
                 "video_warped_spnorm[:, background_mask] = np.nan\n",
                 "\n",
-                "om.video.play(video_warped_spnorm, title=\"sliding window normalization\", interval=20);"
+                "om.show_video(video_warped_spnorm, title=\"sliding window normalization\", interval=20);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
@@ -483,15 +481,15 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "video_warped_spnorm = om.video.normalize_pixelwise_slidingwindow(video_warped, window_size=60)\n",
                 "video_warped_spnorm[:, background_mask] = np.nan\n",
                 "\n",
-                "render_ani_func(lambda: om.video.play(video_warped_spnorm, title=\"sliding window normalization\", interval=20))"
+                "render_ani_func(lambda: om.show_video(video_warped_spnorm, title=\"sliding window normalization\", interval=20))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For better visualization in the next steps we'll need a mask of the background. Here we use {func}`background_mask` to create a mask of the background from the first frame of the data using an automatic threshold.\n",
@@ -506,29 +504,29 @@
                 "tags": [
                     "skip-execution"
                 ]
             },
             "outputs": [],
             "source": [
                 "alpha = om.video.normalize(video_warped_spnorm, vmin=0.5, vmax=0)\n",
-                "om.video.play_with_overlay(video_warped, 1-video_warped_spnorm, alpha=alpha, vmin_overlay=0, vmax_overlay=1, interval=30);"
+                "om.video.show_video_overlay(video_warped, 1-video_warped_spnorm, alpha=alpha, vmin_overlay=0, vmax_overlay=1, interval=30);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": [
                     "remove-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "alpha = om.video.normalize(video_warped_spnorm, vmin=0.5, vmax=0)\n",
-                "render_ani_func(lambda: om.video.play_with_overlay(video_warped, (1-video_warped_spnorm), alpha=alpha, interval=20))"
+                "render_ani_func(lambda: om.video.show_video_overlay(video_warped, (1-video_warped_spnorm), alpha=alpha, interval=20))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `opticalmapping-0.2.0/docs/tutorials/smoothing.ipynb` & `opticalmapping-0.2.2/docs/tutorials/smoothing.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991071428571429%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'import matplotlib.pyplot as plt\\n'), (11, '        "*

 * *            "ani.repeat = True\\n'), (15, '    vid = "*

 * *            "HTML(ani.to_html5_video(embed_limit=2**128))\\n')], delete: [15, 4, 3]}}}"}*

```diff
@@ -22,27 +22,27 @@
                 ]
             },
             "outputs": [],
             "source": [
                 "# Code snippet for rendering animations in the docs\n",
                 "from IPython.display import HTML\n",
                 "import warnings\n",
-                "import matplotlib\n",
-                "matplotlib.rcParams['animation.embed_limit'] = 2**128\n",
+                "import matplotlib.pyplot as plt\n",
                 "\n",
                 "def render_ani_func(f):\n",
                 "    om.utils.disable_interactive_backend_switching()\n",
                 "    plt.switch_backend('Agg')\n",
                 "    with warnings.catch_warnings():\n",
                 "        warnings.simplefilter(\"ignore\")\n",
                 "        ani = f()\n",
+                "        ani.repeat = True\n",
                 "    %matplotlib inline\n",
                 "    om.utils.enable_interactive_backend_switching()\n",
                 "\n",
-                "    vid = HTML(ani.to_html5_video())\n",
+                "    vid = HTML(ani.to_html5_video(embed_limit=2**128))\n",
                 "    plt.close('all')\n",
                 "    return vid"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
```

### Comparing `opticalmapping-0.2.0/opticalmapping.egg-info/PKG-INFO` & `opticalmapping-0.2.2/opticalmapping.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opticalmapping
-Version: 0.2.0
+Version: 0.2.2
 Summary: A toolbox for analyzing optical mapping and fluorescence imaging data.
 Home-page: https://github.com/cardiacvision/optimap
 Author: Jan Lebert
 Author-email: jan.lebert@ucsf.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -31,14 +31,16 @@
 Requires-Dist: scikit-image
 Requires-Dist: scikit-video
 Requires-Dist: tqdm
 Requires-Dist: pooch
 Requires-Dist: seasonal
 Requires-Dist: static_ffmpeg
 Requires-Dist: mpl-pan-zoom
+Requires-Dist: monochrome-viewer
+Requires-Dist: Pillow>=10.0.1
 Provides-Extra: all
 Requires-Dist: opencv-contrib-python; extra == "all"
 Requires-Dist: PySide6; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
@@ -48,54 +50,60 @@
 Requires-Dist: sphinx-autobuild; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-codeautolink; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst_nb>=1.0.0; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: jupyter-cache; extra == "docs"
+Requires-Dist: sphinx-remove-toctrees; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
 
 # optimap
 
 [![docs](https://readthedocs.org/projects/optimap/badge/?version=latest&style=)](https://optimap.readthedocs.org)
 [![tests](https://github.com/cardiacvision/optimap/actions/workflows/main.yml/badge.svg)](https://github.com/cardiacvision/optimap/actions/workflows/main.yml)
 [![PyPI](https://img.shields.io/pypi/v/opticalmapping.svg)](https://pypi.org/project/opticalmapping/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/opticalmapping.svg)](https://python.org)
 [![DOI](https://zenodo.org/badge/677528623.svg)](https://zenodo.org/badge/latestdoi/677528623)
 
 ### optimap: An open-source library for the processing of fluorescence video data
 
-`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more detailed information about optimap's usage and features.
+`optimap` is an open-source Python toolbox for exploring, visualizing, and analyzing high-speed fluorescence imaging data with a focus on cardiac optical mapping data. It includes modules for loading, processing and exporting videos, extracting and measuring optical traces, visualizing action potential or calcium waves, tracking motion and compensating motion artifacts, computing activation maps, conduction velocities, action potential durations, as well as measuring contractility and further analyzing and visualizing the results. Refer to the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) and the [Documentation](https://optimap.readthedocs.io/en/latest/) for more information about optimap's features.
 
 > ⚠️ optimap is currently in early development, expect breaking changes and bugs.
 
 ## Installation
 
-`optimap` is available for Mac OSX, Windows and Linux, see [Installing optimap](https://optimap.readthedocs.io/en/latest/chapters/getting_started/#installing-optimap) for more detailed information.
+`optimap` is available for macOS, Windows and Linux, see the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for more information.
 
-### Installing pre-built binaries (Mac OSX, Windows, Linux)
+### Installing pre-built binaries (macOS, Windows, Linux)
 
 Pre-built binaries can be installed using pip:
 
 ```bash
 pip install opticalmapping[all]
 ```
 
 The above command will install optimap and all recommended dependencies including OpenCV and PySide2. If you wish to install your own version of OpenCV (e.g. for CUDA support) or Qt implementation use:
 
 ```bash
 pip install opticalmapping
 ```
 
-## Getting Started
+To update optimap to the latest version run
 
-See [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/) and the [Getting Started](https://optimap.readthedocs.io/en/latest/chapters/getting_started/) guide for an introduction to optimap and installation instructions.
+```bash
+pip install --upgrade opticalmapping[all]
+```
 
 ## About optimap
 
-`optimap` is a script-based software, which means that you run Python-based analysis scripts rather than using a graphical user interface. We provide several example scripts which explain the usage of `optimap`, see [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/basics/). The example scripts can also be downloaded directly by clicking on the right link in the green box at the top of each tutorial page. `optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). `optimap` was created for cardiovascular scientists in particular, but might also be useful for scientists in other fields, for instance, when performing calcium imaging or physiological research with moving cells or tissues. `optimap` is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, matplotlib and OpenCV.
+`optimap` is an interactive, script or notebook-based software library created for cardiovascular scientists in particular, but might also be useful for scientists in other fields. For instance, when performing calcium imaging or physiological research with moving cells or tissues. It is designed to be a flexible and customizable analysis workflow toolkit, which allows for a wide range of analyses and visualizations. See the [Tutorials](https://optimap.readthedocs.io/en/latest/tutorials/) for examples and more information about the usage of `optimap`. The tutorials can be downloaded by clicking on the link in the green box at the top of each tutorial page.
+
+`optimap` is developed by members of the [Cardiac Vision Laboratory](https://cardiacvision.ucsf.edu) at the [University of California, San Franicsco](https://www.ucsf.edu). It is open-source, freely available, and relies on open-source packages such as NumPy, SciPy, Matplotlib and OpenCV.
 
 ## Links
 
 - [Documentation](https://optimap.readthedocs.io)
 - [Issue tracker](https://github.com/cardiacvision/optimap/issues)
 - [Source code](https://github.com/cardiacvision/optimap)
```

### Comparing `opticalmapping-0.2.0/opticalmapping.egg-info/SOURCES.txt` & `opticalmapping-0.2.2/opticalmapping.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,32 @@
 docs/.gitignore
 docs/Makefile
 docs/api.md
 docs/conf.py
 docs/index.md
 docs/make.bat
 docs/refs.bib
+docs/rename_example_files.py
+docs/_static/flow diagram tracking Lebert et al.png
 docs/_static/vscode-code-cells.png
 docs/_static/vscode-plot-viewer.gif
 docs/_templates/custom-module-template.rst
 docs/chapters/bibliography.md
 docs/chapters/contributing.md
 docs/chapters/getting_started.md
 docs/chapters/installation.md
 docs/chapters/misc.md
 docs/tutorials/.gitignore
+docs/tutorials/01_overview.ipynb
 docs/tutorials/activation.ipynb
 docs/tutorials/apd.ipynb
 docs/tutorials/basics.ipynb
 docs/tutorials/cv.ipynb
+docs/tutorials/example_files.ipynb
+docs/tutorials/index.md
 docs/tutorials/io.ipynb
 docs/tutorials/mask.ipynb
 docs/tutorials/motion_compensation.ipynb
 docs/tutorials/phase.ipynb
 docs/tutorials/plotting.ipynb
 docs/tutorials/ratiometry.ipynb
 docs/tutorials/signal_extraction.ipynb
@@ -170,14 +175,16 @@
 optimap/_cpp/include/xtl/xtl_config.hpp
 optimap/_cpp/include/xtl/xtype_traits.hpp
 optimap/_cpp/include/xtl/xvariant.hpp
 optimap/_cpp/include/xtl/xvariant_impl.hpp
 optimap/_cpp/include/xtl/xvisitor.hpp
 optimap/activation/__init__.py
 optimap/activation/_core.py
+optimap/apd/__init__.py
+optimap/apd/_apd.py
 optimap/assets/README.md
 optimap/assets/draw_symbol.png
 optimap/assets/eraser_symbol.png
 optimap/assets/invert_symbol.png
 optimap/assets/redo_symbol.png
 optimap/assets/undo_symbol.png
 optimap/assets/visibility_off_symbol.png
```

### Comparing `opticalmapping-0.2.0/optimap/__init__.py` & `opticalmapping-0.2.2/optimap/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,26 +32,31 @@
     compare_traces,
     extract_traces,
     select_positions,
     select_traces,
     show_positions,
     show_traces,
 )
-from .utils import is_verbose, print_bar, print_properties, set_verbose
+from .utils import is_verbose, print_bar, print_properties, set_verbose, download_example_data
 from .video import (
     export_video,
     load_metadata,
     load_video,
     save_image_sequence,
     save_video,
+    show_video,
+    show_video_pair,
+    show_videos,
 )
 from .video import (
     play as play_video,
 )
-
+from .apd import (
+    detect_apd
+)
 __all__ = [
     "__version__",
     "__version_tuple__",
 
     # submodules
     "motion",
     "phase",
@@ -69,14 +74,17 @@
     "load_mask",
 
     "show_image",
     "show_mask",
     "show_positions",
     "show_traces",
     "play_video",
+    "show_video",
+    "show_video_pair",
+    "show_videos",
 
     "save_image",
     "save_image_sequence",
     "save_mask",
     "save_video",
     "export_video",
 
@@ -91,12 +99,14 @@
     "background_mask",
     "foreground_mask",
     "invert_mask",
 
     "compute_phase",
     "compute_activation_map",
 
+    "download_example_data",
     "set_verbose",
     "is_verbose",
     "print_bar",
     "print_properties",
+    "detect_apd"
 ]
```

### Comparing `opticalmapping-0.2.0/optimap/_cpp/.clang-format` & `opticalmapping-0.2.2/optimap/_cpp/.clang-format`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/contrast_enhancement.h` & `opticalmapping-0.2.2/optimap/_cpp/contrast_enhancement.h`

 * *Files 20% similar despite different names*

```diff
@@ -9,99 +9,116 @@
 
 #include "xtensor/xtensor.hpp"
 #include "xtensor/xview.hpp"
 
 #include "definitions.h"
 #include "vectors.h"
 
-
-template <typename Derived, typename Derived2>
-auto minmax_masked(const Derived &block, const Derived2 &mask) {
-  assert(mask.shape() == block.shape());
+template <typename Derived, typename Derived2, typename Derived3>
+auto minmax_kernel(const Derived &block, const Derived2 &kernel, const Derived3 &mask) {
+  assert(kernel.shape() == block.shape());
+  static_assert(std::is_same_v<typename Derived2::value_type, bool>);
+  static_assert(std::is_same_v<typename Derived3::value_type, bool>);
 
   using Scalar = typename Derived::value_type;
   Scalar max   = std::numeric_limits<Scalar>::lowest();
   Scalar min   = std::numeric_limits<Scalar>::max();
 
-  for (int row = 0; row < mask.shape(0); row++) {
-    for (int col = 0; col < mask.shape(1); col++) {
-      if (mask(row, col)) {
+  for (size_t row = 0; row < kernel.shape(0); row++) {
+    for (size_t col = 0; col < kernel.shape(1); col++) {
+      bool in_mask = mask.size() <= 1 || mask(row, col);
+      if (kernel(row, col) && in_mask) {
         max = std::max(max, block(row, col));
         min = std::min(min, block(row, col));
       }
     }
   }
+
+  if (max == std::numeric_limits<Scalar>::lowest() || min == std::numeric_limits<Scalar>::max()) {
+    max = 0;
+    min = 0;
+  }
   return std::make_pair(min, max);
 }
 
 auto genCircleMask(const int kernel_size) {
   const bool is_odd = static_cast<bool>(kernel_size % 2);
   if (!is_odd) {
-    return Mask2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, true);
+    return Array2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)},
+                   true);
   }
 
   const Vec2i center         = {kernel_size / 2, kernel_size / 2};
   const unsigned int radius2 = (kernel_size / 2 + 1) * (kernel_size / 2);
 
-  Mask2b circleblock = Mask2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, false);
+  Array2b circleblock =
+      Array2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, false);
   for (long row = 0; row < kernel_size; row++) {
     for (long col = 0; col < kernel_size; col++) {
       const auto v          = Vec2i(row, col) - center;
-      circleblock(row, col) = v.length_squared() <= radius2;
+      circleblock(row, col) = static_cast<size_t>(v.length_squared()) <= radius2;
     }
   }
 
   return circleblock;
 }
 
 auto genCircleMask2(const int kernel_size) {
   const bool is_odd = static_cast<bool>(kernel_size % 2);
   if (!is_odd) {
 
-    return Mask2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, true);
+    return Array2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)},
+                   true);
   }
 
   const Vec2i center         = {kernel_size / 2, kernel_size / 2};
   const unsigned int radius2 = (kernel_size / 2) * (kernel_size / 2);
 
-  Mask2b circleblock = Mask2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, false);
+  Array2b circleblock =
+      Array2b({static_cast<std::size_t>(kernel_size), static_cast<std::size_t>(kernel_size)}, false);
   for (long row = 0; row < kernel_size; row++) {
     for (long col = 0; col < kernel_size; col++) {
       const auto v          = Vec2i(row, col) - center;
-      circleblock(row, col) = v.length_squared() <= radius2;
+      circleblock(row, col) = static_cast<size_t>(v.length_squared()) <= radius2;
     }
   }
 
   return circleblock;
 }
 
-auto circleMaskFactory(std::size_t kernel_size, std::string kernel_type) {
-  Mask2b mask;
+auto kernel_factory(std::size_t kernel_size, std::string kernel_type) {
+  Array2b mask;
   if (kernel_type == "block") {
-    mask = Mask2b({kernel_size, kernel_size}, true);
+    mask = Array2b({kernel_size, kernel_size}, true);
   } else if (kernel_type == "circle") {
     mask = genCircleMask(kernel_size);
   } else if (kernel_type == "circle2") {
     mask = genCircleMask2(kernel_size);
   } else {
     throw std::logic_error(
         "Invalid value for 'kernel_type', has to be one of ['block', 'circle', 'circle2']");
   }
   return mask;
 }
 
 template <typename T>
-void _contrast_enhancement_padded(const Array2f &img, const Mask2b &mask, T &out) {
+void _contrast_enhancement_padded(T &out,
+                                  const Array2f &img,
+                                  const Array2b &kernel,
+                                  const Array2b &mask) {
   assert(img.dimension() == out.dimension());
   assert(img.shape(0) == out.shape(0) && img.shape(1) == out.shape(1));
-  assert(mask.shape(0) == mask.shape(1));
+  assert(kernel.shape(0) == kernel.shape(1));
+  if (mask.size() > 1) {
+    assert(mask.shape(0) == img.shape(0) && mask.shape(1) == img.shape(1));
+  }
 
   const int Nx          = img.shape(0);
   const int Ny          = img.shape(1);
-  const int kernel_size = mask.shape(0);
+  const int kernel_size = kernel.shape(0);
 
   const int offset = (kernel_size - 1) / 2;
   for (int row = 0; row < Nx; row++) {
     for (int col = 0; col < Ny; col++) {
       int startx  = row - offset;
       int starty  = col - offset;
       int endx    = startx + kernel_size;
@@ -121,54 +138,62 @@
       }
       if (endy > Ny) {
         mendy -= endy - Ny;
         endy = Ny;
       }
 
       const auto block = xt::view(img, xt::range(startx, endx), xt::range(starty, endy));
-      const auto maskv = xt::view(mask, xt::range(mstartx, mendx), xt::range(mstarty, mendy));
+      const auto kernel_block = xt::view(kernel, xt::range(mstartx, mendx), xt::range(mstarty, mendy));
+      const auto mask_block = (mask.size() > 1)? xt::view(mask, xt::range(startx, endx), xt::range(starty, endy)) : Array2b();
 
-      const auto [min, max] = minmax_masked(block, maskv);
-      if (max != min) {
+      const bool in_mask = mask.size() <= 1 || mask(row, col);
+      auto [min, max]    = minmax_kernel(block, kernel_block, mask_block);
+      if (max != min && in_mask) {
         out(row, col) = (img(row, col) - min) / (max - min);
       } else {
         out(row, col) = 0;
       }
     }
   }
 }
 
 Array2f contrast_enhancement_img(const Array2f &img,
                                  std::size_t kernel_size,
+                                 const Array2b &mask,
                                  std::string kernel_type) {
   if (bool is_odd = kernel_size % 2; !is_odd) {
     throw std::runtime_error("only odd kernel sizes supported!");
   }
 
   Array2f out(img.shape(), std::numeric_limits<float>::quiet_NaN());
-  auto mask = circleMaskFactory(kernel_size, kernel_type);
-  _contrast_enhancement_padded(img, mask, out);
+  const auto kernel = kernel_factory(kernel_size, kernel_type);
+  _contrast_enhancement_padded(out, img, kernel, mask);
 
   return out;
 }
 
 Array3f contrast_enhancement_video(const Array3f &video,
                                    std::size_t kernel_size,
+                                   const Array3b &mask,
                                    std::string kernel_type) {
   if (bool is_odd = kernel_size % 2; !is_odd) {
     throw std::runtime_error("only odd kernel sizes supported!");
   }
 
   Array3f out(video.shape(), std::numeric_limits<float>::quiet_NaN());
-  const auto mask = circleMaskFactory(kernel_size, kernel_type);
-  const auto Nt   = video.shape(0);
+  const auto kernel = kernel_factory(kernel_size, kernel_type);
+  const auto Nt     = video.shape(0);
 #ifdef USE_OMP
 #pragma omp parallel for
 #endif
   for (int t = 0; t < Nt; t++) {
     auto img     = xt::view(video, t, xt::all(), xt::all());
     auto out_img = xt::view(out, t, xt::all(), xt::all());
-    _contrast_enhancement_padded(img, mask, out_img);
+    if (mask.size() > 1) {
+      _contrast_enhancement_padded(out_img, img, kernel, xt::view(mask, t, xt::all(), xt::all()));
+    } else {
+      _contrast_enhancement_padded(out_img, img, kernel, Array2b());
+    }
   }
 
   return out;
 }
```

### Comparing `opticalmapping-0.2.0/optimap/_cpp/definitions.h` & `opticalmapping-0.2.2/optimap/_cpp/definitions.h`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 
 template <class T, std::size_t N>
 using Array   = xt::xtensor<T, N, xt::layout_type::row_major>;
 using Array2f = Array<float, 2>;
 using Array3f = Array<float, 3>;
 using Array4f = Array<float, 4>;
 using Array5f = Array<float, 5>;
-using Mask2b  = Array<bool, 2>;
+using Array2b = Array<bool, 2>;
+using Array3b = Array<bool, 3>;
 
 template <class T, std::size_t N>
 using PyArray   = xt::pytensor<T, N, xt::layout_type::row_major>;
 using PyArray2f = PyArray<float, 2>;
 using PyArray3f = PyArray<float, 3>;
 using PyArray4f = PyArray<float, 4>;
-using PyArray5f = PyArray<float, 5>;
+using PyArray5f = PyArray<float, 5>;
+using PyArray2b = PyArray<bool, 2>;
+using PyArray3b = PyArray<bool, 3>;
```

### Comparing `opticalmapping-0.2.0/optimap/_cpp/filters.h` & `opticalmapping-0.2.2/optimap/_cpp/filters.h`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/flow_filters.h` & `opticalmapping-0.2.2/optimap/_cpp/flow_filters.h`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/LICENSE` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaccessible.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaccessible.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaccumulator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaccumulator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xadapt.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xadapt.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xarray.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xarray.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xassign.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xassign.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaxis_iterator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaxis_iterator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xaxis_slice_iterator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xaxis_slice_iterator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xblockwise_reducer.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xblockwise_reducer.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xblockwise_reducer_functors.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xblockwise_reducer_functors.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbroadcast.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbroadcast.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbuffer_adaptor.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbuffer_adaptor.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xbuilder.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xbuilder.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_array.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_array.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_assign.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_assign.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xchunked_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xchunked_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcomplex.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcomplex.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcontainer.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcontainer.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xcsv.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xcsv.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xdynamic_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xdynamic_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xeval.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xeval.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexception.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexception.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression_holder.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression_holder.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xexpression_traits.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xexpression_traits.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfixed.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfixed.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfunction.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfunction.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xfunctor_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xfunctor_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xgenerator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xgenerator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xhistogram.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xhistogram.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xindex_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xindex_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xinfo.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xinfo.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xio.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xio.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xiterable.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xiterable.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xiterator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xiterator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xjson.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xjson.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xlayout.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xlayout.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmanipulation.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmanipulation.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmasked_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmasked_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmath.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmath.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmime.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmime.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xmultiindex_iterator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xmultiindex_iterator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnoalias.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnoalias.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnorm.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnorm.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xnpy.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xnpy.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoffset_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoffset_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoperation.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoperation.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly_base.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly_base.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xoptional_assembly_storage.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xoptional_assembly_storage.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xpad.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xpad.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xrandom.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xrandom.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xreducer.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xreducer.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xrepeat.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xrepeat.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xscalar.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xscalar.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xsemantic.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xsemantic.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xset_operation.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xset_operation.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xshape.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xshape.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xslice.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xslice.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xsort.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xsort.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstorage.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstorage.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrided_view.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrided_view.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrided_view_base.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrided_view_base.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xstrides.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xstrides.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_config.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_config.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_forward.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_forward.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xtensor_simd.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xtensor_simd.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xutils.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xutils.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xvectorize.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xvectorize.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xview.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xview.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor/xview_utils.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor/xview_utils.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/LICENSE` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyarray.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyarray.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyarray_backstrides.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyarray_backstrides.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pycontainer.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pycontainer.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pynative_casters.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pynative_casters.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pystrides_adaptor.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pystrides_adaptor.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pytensor.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pytensor.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/pyvectorize.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/pyvectorize.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/xtensor_python_config.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/xtensor_python_config.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtensor-python/xtensor_type_caster_base.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtensor-python/xtensor_type_caster_base.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/LICENSE` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/LICENSE`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xany.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xany.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xbase64.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xbase64.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xbasic_fixed_string.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xbasic_fixed_string.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xclosure.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xclosure.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcompare.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcompare.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcomplex.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcomplex.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xcomplex_sequence.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xcomplex_sequence.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xdynamic_bitset.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xdynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xfunctional.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xfunctional.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhalf_float.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhalf_float.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhalf_float_impl.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhalf_float_impl.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhash.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhash.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xhierarchy_generator.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xhierarchy_generator.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xiterator_base.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xiterator_base.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xjson.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xjson.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmasked_value.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmasked_value.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmasked_value_meta.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmasked_value_meta.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmeta_utils.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmeta_utils.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xmultimethods.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xmultimethods.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional_meta.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional_meta.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xoptional_sequence.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xoptional_sequence.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xplatform.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xplatform.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xproxy_wrapper.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xproxy_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xsequence.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xsequence.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xspan.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xspan.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xspan_impl.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xspan_impl.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xsystem.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xsystem.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xtl_config.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xtl_config.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xtype_traits.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xtype_traits.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvariant.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvariant.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvariant_impl.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvariant_impl.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/include/xtl/xvisitor.hpp` & `opticalmapping-0.2.2/optimap/_cpp/include/xtl/xvisitor.hpp`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/lib.cpp` & `opticalmapping-0.2.2/optimap/_cpp/lib.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -23,26 +23,31 @@
   return false;
 #endif
 }
 
 /* contrast enhancement */
 PyArray2f py_contrast_enhancement_img(const PyArray2f &img,
                                       std::size_t kernel_size,
+                                      const PyArray2b &mask,
                                       std::string kernel_type) {
-  return contrast_enhancement_img(img, kernel_size, kernel_type);
+  return contrast_enhancement_img(img, kernel_size, mask, kernel_type);
 }
 
 PyArray3f py_contrast_enhancement_video(const PyArray3f &video,
                                         std::size_t kernel_size,
+                                        const PyArray3b &mask,
                                         std::string kernel_type) {
-  return contrast_enhancement_video(video, kernel_size, kernel_type);
+  return contrast_enhancement_video(video, kernel_size, mask, kernel_type);
 }
 
 /* regular filters */
-PyArray3f py_normalizePixelwiseSlidingWindow(const PyArray3f &video, int wt, float ymin, float ymax) {
+PyArray3f py_normalizePixelwiseSlidingWindow(const PyArray3f &video,
+                                             int wt,
+                                             float ymin,
+                                             float ymax) {
   return normalizePixelwiseSlidingWindow(video, wt, ymin, ymax);
 }
 
 /* phase filters */
 PyArray3f py_filterPhaseAngleThreshold(
     const PyArray3f &phase, int wx, int wy, int wt, float tr_angle, PyArray2f mask) {
   return filterPhaseAngleThreshold(phase, wx, wy, wt, tr_angle, mask);
@@ -84,19 +89,20 @@
            filterPhaseFillSmooth
            spatiotemporalFlowFilter
     )doc";
 
   m.def("is_openmp_enabled", is_openmp_enabled, "");
 
   m.def("contrast_enhancement_img", py_contrast_enhancement_img, "img"_a, "kernel_size"_a,
-        "kernel_type"_a = std::string("circle"));
+        "mask"_a = PyArray2b(), "kernel_type"_a = std::string("circle"));
   m.def("contrast_enhancement_video", py_contrast_enhancement_video, "video"_a, "kernel_size"_a,
-        "kernel_type"_a = std::string("circle"));
+        "mask"_a = PyArray3b(), "kernel_type"_a = std::string("circle"));
 
-  m.def("normalize_pixelwise_slidingwindow", py_normalizePixelwiseSlidingWindow, "video"_a, "wt"_a, "ymin"_a = 0, "ymax"_a = 1);
+  m.def("normalize_pixelwise_slidingwindow", py_normalizePixelwiseSlidingWindow, "video"_a, "wt"_a,
+        "ymin"_a = 0, "ymax"_a = 1);
 
   m.def("phasefilter_angle_threshold", py_filterPhaseAngleThreshold,
         "Remove outliers in a phase video by comparing them against their neighbors", "phase"_a,
         "wx"_a, "wy"_a, "wt"_a, "tr_angle"_a, "mask"_a = PyArray2f());
   m.def("phasefilter_disc", py_filterPhaseDisc, "phase"_a, "wx"_a, "wy"_a, "wt"_a,
         "mask"_a = PyArray2f());
   m.def("phasefilter_fillsmooth", py_filterPhaseFillSmooth, "phase"_a, "wx"_a, "wy"_a, "wt"_a,
```

### Comparing `opticalmapping-0.2.0/optimap/_cpp/phase_filters.h` & `opticalmapping-0.2.2/optimap/_cpp/phase_filters.h`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/vec2.h` & `opticalmapping-0.2.2/optimap/_cpp/vec2.h`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/_cpp/vectors.h` & `opticalmapping-0.2.2/optimap/_cpp/vectors.h`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/activation/_core.py` & `opticalmapping-0.2.2/optimap/activation/_core.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/image/_GHT.py` & `opticalmapping-0.2.2/optimap/image/_GHT.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/image/__init__.py` & `opticalmapping-0.2.2/optimap/image/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Functions for loading, saving, and displaying images, and for creating masks."""
 
-from ._core import load_image, load_mask, save_image, save_mask, show_image, smooth_gaussian, collage
+from ._core import collage, load_image, load_mask, save_image, save_mask, show_image, smooth_gaussian
 from ._edit import crop, flip_left_right, flip_up_down, pad, resize, rotate_left, rotate_right
 from ._mask import (
     background_mask,
     close_mask,
     detect_background_threshold,
     dilate_mask,
     disc_mask,
@@ -13,14 +13,15 @@
     foreground_mask,
     interactive_mask,
     invert_mask,
     largest_mask_component,
     open_mask,
     show_mask,
 )
+from ..video import normalize
 
 __all__ = [
     "show_image",
     "show_mask",
     "save_image",
     "save_mask",
     "load_image",
```

### Comparing `opticalmapping-0.2.0/optimap/image/_core.py` & `opticalmapping-0.2.2/optimap/image/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         sigma = (sigma, sigma, 0)
 
     return ndimage.gaussian_filter(image, sigma=sigma, **kwargs)
 
 
 def collage(images, ncols=6, padding=0, padding_value=0):
     """Create a collage from a list or array of images/masks that have the same shape.
-    
+
     Creates a numpy array with the images arranged in a grid, with a specified number of images per row.
     Optionally, padding can be added between the images.
 
     See :func:`export_video_collage` to save a video collage to a video file.
 
     Parameters
     ----------
@@ -282,28 +282,27 @@
     -------
     np.ndarray
         Collage image
 
     Examples
     --------
     .. code-block:: python
-    
+
             import optimap as om
             import numpy as np
-    
+
             # create a collage of 3x3 random images
             images = [np.random.rand(100, 100) for _ in range(9)]
             collage = om.image.collage(images, ncols=3, padding=10)
             om.image.show_image(collage)
     """
-
     for image in images:
         if image.shape != images[0].shape:
             raise ValueError("All images must have the same shape")
-    
+
     blank_image = np.full((images[0].shape[0], padding) + images[0].shape[2:],
                           padding_value, dtype=images[0].dtype)
 
     collage_rows = []
     current_index = 0
     while current_index < len(images):
         end_index = min(current_index + ncols, len(images))
@@ -311,15 +310,15 @@
 
         if padding > 0:
             for i in range(len(row_images) - 1):
                 row_images.insert(2 * i + 1, blank_image)
 
         collage_rows.append(np.hstack(row_images))
         current_index = end_index
-    
+
     if padding > 0 and len(collage_rows) > 1:
         row_space = np.full((padding,) + collage_rows[0].shape[1:],
                             padding_value, dtype=collage_rows[0].dtype)
         for i in range(len(collage_rows) - 1):
             collage_rows.insert(2 * i + 1, row_space)
 
     collage_image = np.vstack(collage_rows)
```

### Comparing `opticalmapping-0.2.0/optimap/image/_edit.py` & `opticalmapping-0.2.2/optimap/image/_edit.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/image/_mask.py` & `opticalmapping-0.2.2/optimap/image/_mask.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/image/_segmenter.py` & `opticalmapping-0.2.2/optimap/image/_segmenter.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/motion/__init__.py` & `opticalmapping-0.2.2/optimap/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/motion/_core.py` & `opticalmapping-0.2.2/optimap/motion/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,44 @@
 
 from .. import _cpp
 from ..video import smooth_spatiotemporal
 from ._flowestimator import FlowEstimator
 from ._warping import warp_video
 
 
-def contrast_enhancement(video_or_img: np.ndarray, kernel_size: int):
+def contrast_enhancement(video_or_img: np.ndarray, kernel_size: int, mask: np.ndarray = None):
     """Amplifies local contrast to maximum to remove fluorescence signal for motion estimation.
     See :cite:t:`Christoph2018a` for details.
 
-    :param video_or_img: {t, x, y} or {x, y} ndarray
-    :param kernel_size: int kernel size for local contrast enhancement (must be odd)
-    :return: {t, x, y} or {x, y} ndarray
+    Parameters
+    ----------
+    video_or_img : np.ndarray
+        {t, x, y} or {x, y} ndarray
+    kernel_size : int
+        Kernel size for local contrast enhancement (must be odd)
+    mask : np.ndarray, optional
+        valid values mask of shape {x, y} or {t, x, y}, by default None
+
+    Returns
+    -------
+    np.ndarray
+        {t, x, y} or {x, y} ndarray of dtype np.float32
     """
     if video_or_img.ndim == 2:
-        return _cpp.contrast_enhancement_img(np.ascontiguousarray(video_or_img), kernel_size)
+        if mask is None:
+            return _cpp.contrast_enhancement_img(np.ascontiguousarray(video_or_img), kernel_size)
+        else:
+            return _cpp.contrast_enhancement_img(np.ascontiguousarray(video_or_img), kernel_size, np.ascontiguousarray(mask))
     else:
-        return _cpp.contrast_enhancement_video(np.ascontiguousarray(video_or_img), kernel_size)
+        if mask is None:
+            return _cpp.contrast_enhancement_video(np.ascontiguousarray(video_or_img), kernel_size)
+        else:
+            if mask.ndim == 2:
+                mask = mask[None, ...].repeat(video_or_img.shape[0], axis=0)
+            return _cpp.contrast_enhancement_video(np.ascontiguousarray(video_or_img), kernel_size, np.ascontiguousarray(mask))
 
 
 def smooth_displacements(
     displacements,
     wx: int,
     wy: int,
     wt: int,
```

### Comparing `opticalmapping-0.2.0/optimap/motion/_flowestimator.py` & `opticalmapping-0.2.2/optimap/motion/_flowestimator.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/motion/_plot.py` & `opticalmapping-0.2.2/optimap/motion/_plot.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/motion/_warping.py` & `opticalmapping-0.2.2/optimap/motion/_warping.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/phase/_core.py` & `opticalmapping-0.2.2/optimap/phase/_core.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/phase/_singularities.py` & `opticalmapping-0.2.2/optimap/phase/_singularities.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/trace/__init__.py` & `opticalmapping-0.2.2/optimap/trace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Functions for extracting time-series from videos."""
 
 from ._compare import compare_traces
 from ._core import (
+    collage_positions,
     extract_traces,
     get_default_trace_window,
     set_default_trace_window,
     show_positions,
     show_trace,
     show_traces,
-    collage_positions
 )
 from ._detrend import detrend_timeseries
 from ._interactive import select_positions, select_traces
 from ._points import positions_from_A_to_B, random_positions
 
 __all__ = [
     "select_traces",
```

### Comparing `opticalmapping-0.2.0/optimap/trace/_compare.py` & `opticalmapping-0.2.2/optimap/trace/_compare.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/trace/_core.py` & `opticalmapping-0.2.2/optimap/trace/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import matplotlib.pyplot as plt
 import numpy as np
 
 from ..image import disc_mask
 
 TRACE_TYPE = "rect"
 
@@ -110,27 +112,29 @@
         traces = traces[..., 0]
 
     if show or "ax" in kwargs:
         show_traces(traces, **kwargs)
     return traces
 
 
-def show_positions(image, positions, size=None, cmap="gray", vmin=None, vmax=None, ax=None, **kwargs):
+def show_positions(positions, image=None, size=None, color=None, cmap="gray", vmin=None, vmax=None, ax=None, **kwargs):
     """Overlay positions on an image.
 
     Parameters
     ----------
-    image : 2D array
-        Image to overlay positions on
     positions : list of tuples
         List of positions to overlay
+    image : 2D array
+        Image to overlay positions on, optional
     size : float or array-like, shape (n, ), optional
         Size of the points, see `s` parameter in :py:func:`matplotlib.pyplot.scatter` for more information
+    color : str or list of str, optional
+        Color of the points, by default None
     cmap : str, optional
-        Colormap to use, by default 'gray'
+        Colormap to use for image, by default 'gray'
     vmin : float, optional
         Minimum value for the colormap, by default None
     vmax : float, optional
         Maximum value for the colormap, by default None
     ax : matplotlib.axes.Axes, optional
         Axes to plot on. If None, a new figure is created.
     kwargs : dict, optional
@@ -141,19 +145,29 @@
     matplotlib.axes.Axes
     """
     if ax is None:
         fig, ax = plt.subplots()
         show = True
     else:
         show = False
-
-    ax.imshow(image, cmap=cmap, vmin=vmin, vmax=vmax, interpolation="none")
-    ax.axis("off")
-    for pos in positions:
-        ax.scatter(pos[0], pos[1], s=size, **kwargs)
+    
+    if isinstance(image, np.ndarray) and image.ndim == 2 and image.shape[1] == 2:
+        image, positions = positions, image
+        warnings.warn("The order of arguments for optimap.show_positions() has changed.", DeprecationWarning)
+
+    if image is not None:
+        ax.imshow(image, cmap=cmap, vmin=vmin, vmax=vmax, interpolation="none")
+        ax.axis("off")
+
+    if isinstance(color, str) or color is None:
+        color = [color, ] * len(positions)
+    if isinstance(size, (int, float)) or size is None:
+        size = [size, ] * len(positions)
+    for pos, s, c in zip(positions, size, color):
+        ax.scatter(pos[0], pos[1], s=s, c=c, **kwargs)
     if show:
         plt.show()
     return ax
 
 
 def show_traces(traces, x=None, fps=None, colors=None, labels=None, ax=None, **kwargs):
     """Plot one or more traces.
@@ -226,24 +240,24 @@
     return show_traces(*args, **kwargs)
 
 
 def collage_positions(positions, image_shape, ncols=6):
     """Correspondant to :func:`image.collage` but for positions. Collages the positions in the same way as the images would be collaged.
 
     `positions` is a list of list of tuples, i.e. one list of positions for each image. The function collages the positions in the same way as the images would be collaged and returns a list of tuples where the positions have been offset to the correct position in the collage. All images are assumed to have the same shape `image_shape`.
-    
+
     Parameters
     ----------
     positions : list of arrays
         List of list of positions to collage
     image_shape : tuple
         Shape of the images where the positions are from
     ncols : int, optional
         Number of columns, by default 6
-    
+
     Returns
     -------
     list of tuples
         Collaged positions
     """
     collage = []
     n = 0
@@ -256,8 +270,8 @@
             points[:, 1] += offset_x
             points[:, 0] += offset_y
             offset_x += image_shape[0]
             collage.extend(points)
         n += stop
         offset_x = 0
         offset_y += image_shape[1]
-    return collage
+    return collage
```

### Comparing `opticalmapping-0.2.0/optimap/trace/_detrend.py` & `opticalmapping-0.2.2/optimap/trace/_detrend.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/trace/_interactive.py` & `opticalmapping-0.2.2/optimap/trace/_interactive.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/trace/_point_clicker.py` & `opticalmapping-0.2.2/optimap/trace/_point_clicker.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/trace/_points.py` & `opticalmapping-0.2.2/optimap/trace/_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     if isinstance(shape_or_mask, np.ndarray):
         mask = shape_or_mask.astype(bool)
         shape = mask.shape
     else:
         mask = np.full(shape_or_mask, True, dtype=bool)
         shape = shape_or_mask
     mask = mask / mask.sum()
-    
+
     rng = np.random.default_rng()
     idxs = rng.choice(
         np.arange(mask.size),
         p=mask.flatten(),
         size=N,
         replace=False
     )
```

### Comparing `opticalmapping-0.2.0/optimap/utils.py` & `opticalmapping-0.2.2/optimap/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 __all__ = [
     "set_verbose",
     "is_verbose",
     "print_bar",
     "print_properties",
     "enable_interactive_backend_switching",
     "disable_interactive_backend_switching",
-    "retrieve_example_data",
+    "download_example_data",
 ]
 
 import functools
 import urllib.parse
 import warnings
+from pathlib import Path
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pooch
 
 from ._version import __version__
 
 VERBOSE = False
 INTERACTIVE_BACKEND = "QtAgg"
 INTERACTIVE_BACKEND_SWITCHING = True
-FILE_HASHES = {
+
+# old example file names and hashes, will be removed in the future
+OLD_FILE_HASHES = {
     "Example_01_Sinus_Rabbit_Basler.npy":
         "sha256:5c692cca0459c931b7f767c27162a42b31e3df90a6aeac53bb182affa2135678",
     "Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy":
         "sha256:6252da91db434cad95758830fdf7c13a9db6793da30dd8e85e6878736e20787e",
     "Example_03_Pacing_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy":
         "sha256:50113334e6955f5abb3658b5027447f507fd9eef6bfef766a628c2365ff848be",
     "Example_04_Pacing_Rabbit_Di-4-ANEPPS_Basler_acA720-520um.npy":
@@ -38,15 +41,52 @@
     # used in tests
     "optimap-test-download-file.npy":
         "sha256:0d3cfca36d8e3ad935de4d0681ddd510c1590212a99dccb196353c8ce85b7491",
     # warped version of Example_02, used to speed up documentation build
     "Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped.npy":
         "sha256:a1781582b669a69a9753b1c43d23e0acf26fb372426eeb6d880d2e66420b2107",
     "Example_02_VF_Rabbit_Di-4-ANEPPS_Basler_acA720-520um_warped_mask.npy":
-        "sha256:3f5d8402c8251f3cb8e8d235b459264ff7e7e2cf2b81f08129f0897baa262db6"
+        "sha256:3f5d8402c8251f3cb8e8d235b459264ff7e7e2cf2b81f08129f0897baa262db6",
+    # # VF
+    # "optimap-example-file-02.npy":
+    #     "https://cardiacvision.ucsf.edu/sites/g/files/tkssra6821/f/optimap-example-file-02.npy_.webm",
+    # # voltage-calcium with Blebbistatin:
+    # "optimap-example-file-03.npy":
+    #     "https://cardiacvision.ucsf.edu/sites/g/files/tkssra6821/f/optimap-example-file-03.npy_.webm",
+    # # ratiometry:
+    # "optimap-example-file-04.npy":
+    #     "https://cardiacvision.ucsf.edu/sites/g/files/tkssra6821/f/optimap-example-file-04.npy_.webm",
+}
+
+# New example file names and hashes
+FILE_HASHES = {
+    "Sinus_Rabbit_1.npy":
+        "sha256:5c692cca0459c931b7f767c27162a42b31e3df90a6aeac53bb182affa2135678",
+    "VF_Rabbit_1.npy":
+        "sha256:e043bf88a1af6995d2b2208431ce36e4eea7204267df5d3fc4fc1e8f04f34769",
+    # "Pacing_Rabbit_1.npy"
+    "Dualchannel_1.zip":
+        "sha256:68761acc4a4fcf7df889074590d9fd57f034cdc8ab0d3c3a692416ceb0555868",
+    "Dualchannel_1.npy":
+        "sha256:908eebb35a9853f5a9b0ae1bb40df40fede600ed11a53ca17d7049ed8ac22268",
+    "Ratiometry_1.npy":
+        "sha256:10a59863ee23abc689d8ee4cd27542ef1b7b8b8eb5668a7f2dc49572f18319f2",
+    # warped version of VF_Rabbit_1, used to speed up documentation build
+    "VF_Rabbit_1_warped.npy":
+        "sha256:48f7e556ac6861e34dc42e0510523c8fdc57d6382e0beeead9555b184e92765d",
+    # used in mask tutorial
+    "VF_Rabbit_1_warped_mask.npy":
+        "sha256:3f5d8402c8251f3cb8e8d235b459264ff7e7e2cf2b81f08129f0897baa262db6",
+    # used in unit tests
+    "test-download-file.npy":
+        "sha256:0d3cfca36d8e3ad935de4d0681ddd510c1590212a99dccb196353c8ce85b7491",
+    # "Example_03_Pacing.npy":
+    #     "sha256:50113334e6955f5abb3658b5027447f507fd9eef6bfef766a628c2365ff848be",
+    # "Example_04_Pacing.npy":
+    #     "sha256:674603f64ccf754f73a264986e0bf1ee93d03ce3a9ea88f248620632046e3c40","
 }
 
 
 def set_verbose(state=True):
     """Set verbosity of optimap.
 
     Parameters
@@ -91,15 +131,15 @@
     if not isinstance(array, np.ndarray):
         raise TypeError("array must be a numpy array")
     print_bar(force=True)
     print(f"array with dimensions: {array.shape}")
     print(f"datatype of array: {array.dtype}")
     print(f"minimum value in entire array: {np.nanmin(array)}")
     print(f"maximum value in entire array: {np.nanmax(array)}")
-    if nans := np.sum(np.isnan(array)) > 0:
+    if (nans := np.sum(np.isnan(array))) > 0:
         print(f"number of NaNs in array: {nans}")
     print_bar(force=True)
 
 
 def enable_interactive_backend_switching():
     """Enable automatic switching of the matplotlib backend to Qt when necessary.
 
@@ -113,14 +153,32 @@
 
     See also :py:func:`enable_interactive_backend_switching`.
     """
     global INTERACTIVE_BACKEND_SWITCHING
     INTERACTIVE_BACKEND_SWITCHING = False
 
 
+def deprecated(reason):
+    """Function decorator to mark a function as deprecated.
+
+    Parameters
+    ----------
+    reason : str
+        Reason why the function is deprecated.
+    """
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            warnings.warn(f"Function '{func.__name__}' is deprecated: {reason}", DeprecationWarning)
+            return func(*args, **kwargs)
+
+        return wrapper
+    return decorator
+
+
 def interactive_backend(func):
     """Function decorator to change backend temporarily in Ipython session.
 
     Switches to QtAgg backend if in Ipython session and back to inline afterwards.
     """
 
     def get_ipython():
@@ -153,15 +211,20 @@
             _print("Switching matplotlib backend to inline")
             plt.switch_backend(current_backend)
             ipython.run_line_magic("matplotlib", "inline")
         return result
 
     return wrapper
 
-def retrieve_example_data(name, directory="./example_data", silent=False):
+@deprecated("Use download_example_data instead")
+def retrieve_example_data(name, directory="./optimap_example_data", silent=False):
+    return download_example_data(name, directory=directory, silent=silent)
+
+
+def download_example_data(name, directory="./optimap_example_data", silent=False):
     """Download example data if not already present.
 
     Parameters
     ----------
     name : str
         Name of the file to download.
     directory : str
@@ -170,29 +233,43 @@
         If True, set logging level to WARNING.
 
     Returns
     -------
     str
         Path to the file.
     """
-    known_hash = FILE_HASHES.get(name, None)
-    if known_hash is None:
-        warnings.warn(f"WARNING: Example file '{name}' is not known. Attempting to download it anyway.", UserWarning)
     if silent:
         silent = pooch.get_logger().level
         pooch.get_logger().setLevel("WARNING")
 
+    known_hash = FILE_HASHES.get(name, None)
+    remote_path = urllib.parse.quote(f"optimap-{name}", safe="")
+
+    # Compatibility with old file names, will be removed in the future
+    if known_hash is None and name in OLD_FILE_HASHES:
+        known_hash = OLD_FILE_HASHES[name]
+        remote_path = urllib.parse.quote(f"{name}", safe="")
+
+    if known_hash is None:
+        warnings.warn(f"WARNING: Example file '{name}' is not known. Attempting to download it anyway.", UserWarning)
+
     # The CMS server only allows files with a certain extensions to be uploaded.
     # We use .webm as dummy extension to upload the files, and rename them after download.
-    remote_path = urllib.parse.quote(f"{name}", safe="")
     url = f"https://cardiacvision.ucsf.edu/sites/g/files/tkssra6821/f/{remote_path}_.webm"
 
+    is_zip = Path(name).suffix == ".zip"
     path = pooch.retrieve(
         url=url,
         known_hash=known_hash,
         fname=name,
         path=directory,
+        processor=pooch.Unzip(extract_dir=Path(name).stem) if is_zip else None,
     )
 
     if silent:
         pooch.get_logger().setLevel(silent)
+
+    if is_zip:
+        path = Path(path[0]).parent
+    else:
+        path = Path(path)
     return path
```

### Comparing `opticalmapping-0.2.0/optimap/video/_edit.py` & `opticalmapping-0.2.2/optimap/video/_edit.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/optimap/video/_export.py` & `opticalmapping-0.2.2/optimap/video/_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import warnings
 from pathlib import Path
-from typing import Iterable, Union, List
+from typing import Iterable, List, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import skvideo
 import skvideo.io
 import static_ffmpeg.run
 from matplotlib.colors import Normalize, to_rgba
@@ -106,16 +106,17 @@
     filename: Union[str, Path],
     video: Union[np.ndarray, Iterable[np.ndarray]],
     fps: int = 60,
     skip_frames: int = 1,
     cmap = "gray",
     vmin : float = None,
     vmax : float = None,
-    ffmpeg_encoder : str = None,
     progress_bar : bool = True,
+    ffmpeg_encoder : str = None,
+    pad_mode : str = "edge",
 ):
     """Export a video numpy array to a video file (e.g. ``.mp4``) using `ffmpeg <https://www.ffmpeg.org>`_.
 
     Downloads pre-built ffmpeg automatically if ffmpeg is not installed.
 
     Example
     -------
@@ -141,19 +142,22 @@
         Only export every ``skip_frames`` frames, by default 1
     cmap : str, optional
         The matplotlib colormap to use, by default "gray"
     vmin : float, optional
         The minimum value for the colormap, by default None
     vmax : float, optional
         The maximum value for the colormap, by default None
+    progress_bar : bool, optional
+        Whether to show a progress bar, by default True
     ffmpeg_encoder : str, optional
         The ffmpeg encoder to use, by default ``'libx264'``. See :func:`set_default_ffmpeg_encoder` and
         :func:`set_ffmpeg_defaults` for more information.
-    progress_bar : bool, optional
-        Whether to show a progress bar, by default True
+    pad_mode : str, optional
+        Odd-sized videos need to be padded to even dimensions, otherwise ffmpeg will error. The padding mode to use,
+        by default "edge". See :func:`numpy.pad` for more information.
     """
     if isinstance(video, (str, os.PathLike)):
         filename, video = video, filename
         warnings.warn("WARNING: The order of arguments for optimap.export_video() has changed. "
                       "Please use export_video(filename, video, ...) instead of export_video(video, filename, ...).",
                       DeprecationWarning)
     if ffmpeg_encoder is None:
@@ -174,25 +178,32 @@
 
     for frame in tqdm(video, desc="exporting video", disable=not progress_bar):
         if frame.ndim == 2:
             frame = cmap(norm(frame))
 
         if frame.dtype != np.uint8:
             frame = (frame * 255).astype(np.uint8)
+
+        # pad odd-sized frames to even dimension, otherwise ffmpeg will error
+        if frame.shape[0] % 2 == 1:
+            frame = np.pad(frame, ((0, 1), (0, 0), (0, 0)), mode=pad_mode)
+        if frame.shape[1] % 2 == 1:
+            frame = np.pad(frame, ((0, 0), (0, 1), (0, 0)), mode=pad_mode)
+
         writer.writeFrame(frame)
     writer.close()
     print(f"video exported to {filename}")
 
 
 def export_video_collage(
         filename: Union[str, Path],
         videos: Union[np.ndarray, List[np.ndarray]],
         ncols: int = 6,
         padding: int = 0,
-        padding_color = 'black',
+        padding_color = "black",
         fps: int = 60,
         skip_frames: int = 1,
         cmaps: Union[str, List[str]] = "gray",
         vmins : Union[float, List[float]] = None,
         vmaxs : Union[float, List[float]] = None,
         ffmpeg_encoder : str = None,
         progress_bar : bool = True,
@@ -215,15 +226,15 @@
             np.random.rand(100, 100, 100),
             np.random.rand(100, 100, 100),
         ]
 
         cmaps = ["gray", "viridis", "plasma", "inferno"]
         om.export_video_collage("collage.mp4", videos, ncols=2, padding=10,
                                 padding_color="white", cmaps=cmaps)
-    
+
     Parameters
     ----------
     filename : str or Path
         Video file path for writing.
     videos : np.ndarray or List[np.ndarray]
         The videos to export. Should be of shape (frames, height, width, channels) or (frames, height, width).
         If the video is grayscale, the colormap will be applied. If it's an RGB video, its values should range
@@ -268,25 +279,25 @@
         cmaps = plt.get_cmap(cmaps)
     if not isinstance(cmaps, list):
         cmaps = [cmaps] * len(videos)
     if not isinstance(vmins, list):
         vmins = [vmins] * len(videos)
     if not isinstance(vmaxs, list):
         vmaxs = [vmaxs] * len(videos)
-    
+
     if len(videos) != len(cmaps) != len(vmins) != len(vmaxs):
         raise ValueError("videos, cmaps, vmins, and vmaxs must have the same length")
 
     def transform_frame(frame, cmap, vmin, vmax):
         if frame.ndim == 2:
             frame = cmap(Normalize(vmin=vmin, vmax=vmax, clip=True)(frame))
         if frame.dtype != np.uint8:
             frame = (frame * 255).astype(np.uint8)
         return frame
-    
+
     if isinstance(padding_color, str):
         padding_color = np.array(to_rgba(padding_color))
         padding_color = (padding_color * 255).astype(np.uint8)
 
     writer = FFmpegWriter(
         filename,
         inputdict={"-r": f"{fps}"},
```

### Comparing `opticalmapping-0.2.0/optimap/video/_importers.py` & `opticalmapping-0.2.2/optimap/video/_importers.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
         self._meta["framerate"] = float(self._meta["Frame rate (Hz)"])
         try:
             self._meta["date"] = datetime.strptime(self._meta["Date created"], "%d/%m/%Y %H:%M:%S")
         except ValueError:
             self._meta["date"] = self._meta["Date created"]
 
     def load_video(self, start_frame=0, frames=None, step=1):
+        """Returns a 3D numpy array containing the loaded video."""
         if frames is not None:
             end_frame = start_frame + frames
             if end_frame > self._Nt:
                 warnings.warn(f"Requested {frames} frames, but only {self._Nt - start_frame} frames available. "
                               "Loading all available frames.", UserWarning)
                 end_frame = None
         else:
```

### Comparing `opticalmapping-0.2.0/optimap/video/_load.py` & `opticalmapping-0.2.2/optimap/video/_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     dat = MiCAM_ULTIMA_Importer(filename)
     return dat.load_video(start_frame=start_frame, frames=frames, step=step)
 
 def load_SciMedia_MiCAMULTIMA_metadata(filename):
     dat = MiCAM_ULTIMA_Importer(filename)
     return dat.get_metadata()
 
-def load_video(path, start_frame=0, frames=None, step=1, use_mmap=False):
+def load_video(path, start_frame=0, frames=None, step=1, use_mmap=False, **kwargs):
     """Loads a video from a file or folder, automatically detecting the file type.
 
     If ``path`` is a folder, it will load a video from a series of images in the folder.
 
     Supported file types:
 
     - .tif, .tiff (TIFF stack)
@@ -191,14 +191,16 @@
     frames : int or None, optional
         Number of frames to load. If None, loads all frames till the end.
     step : int, optional
         Steps between frames. If greater than 1, it will skip frames. Defaults to 1.
     use_mmap : bool, optional
         If True, uses memory mapping to load the video in read-only mode, defaults to False.
         Only supported for some file types.
+    **kwargs : dict
+        Additional arguments to pass to the video loader function
 
     Returns
     -------
     video : {t, x, y} ndarray
         Video array
     """
     path = Path(path)
@@ -212,27 +214,27 @@
     else:
         end_frame = None
 
     if not path.exists():
         msg = f"File or folder '{path}' does not exist"
         raise FileNotFoundError(msg)
     elif path.is_dir():
-        return load_image_folder(path, start_frame=start_frame, end_frame=end_frame, step=step)
+        return load_image_folder(path, start_frame=start_frame, end_frame=end_frame, step=step, **kwargs)
     elif suffix in [".tif", ".tiff"]:
-        return load_tiff(path, start_frame=start_frame, end_frame=end_frame, step=step, use_mmap=use_mmap)
+        return load_tiff(path, start_frame=start_frame, end_frame=end_frame, step=step, use_mmap=use_mmap, **kwargs)
     elif suffix in [".mat"]:
-        return load_MATLAB(path, start_frame=start_frame, end_frame=end_frame, step=step)
+        return load_MATLAB(path, start_frame=start_frame, end_frame=end_frame, step=step, **kwargs)
     elif suffix in [".gsd", ".gsh"]:
-        return load_SciMedia_MiCAM05(path, start_frame=start_frame, frames=frames, step=step)
+        return load_SciMedia_MiCAM05(path, start_frame=start_frame, frames=frames, step=step, **kwargs)
     elif suffix in [".rsh", ".rsm", ".rsd"]:
-        return load_SciMedia_MiCAMULTIMA(path, start_frame=start_frame, frames=frames, step=step)
+        return load_SciMedia_MiCAMULTIMA(path, start_frame=start_frame, frames=frames, step=step, **kwargs)
     elif suffix in [".dat"]:
-        return load_MultiRecorder(path, start_frame=start_frame, frames=frames, step=step, use_mmap=use_mmap)
+        return load_MultiRecorder(path, start_frame=start_frame, frames=frames, step=step, use_mmap=use_mmap, **kwargs)
     elif suffix in [".npy"]:
-        return load_numpy(path, start_frame=start_frame, end_frame=end_frame, step=step, use_mmap=use_mmap)
+        return load_numpy(path, start_frame=start_frame, end_frame=end_frame, step=step, use_mmap=use_mmap, **kwargs)
     else:
         msg = f"Unable to find videoloader for file extension {suffix} (for file '{path}')"
         raise ValueError(msg)
 
 def load_metadata(filename):
     """Loads metadata information from a recording, automatically detecting the file type.
```

### Comparing `opticalmapping-0.2.0/optimap/video/_play.py` & `opticalmapping-0.2.2/optimap/video/_play.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,44 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import animation
 from matplotlib.colors import Colormap
 
-from ..utils import interactive_backend
+from ..utils import deprecated, interactive_backend
 from ._export import iter_alpha_blend_videos
 from ._player import InteractivePlayer
 
-
+@deprecated("use optimap.show_video instead")
 def play(video, skip_frame=1, title="", vmin=None, vmax=None, cmap="gray", interval=10, **kwargs):
+    """Deprecated alias for :py:func:`optimap.video.show_video`."""
+    return show_video(video, skip_frame=skip_frame, title=title, vmin=vmin, vmax=vmax,
+                      cmap=cmap, interval=interval, **kwargs)
+
+
+@deprecated("use optimap.show_video_pair instead")
+def play2(video1, video2, skip_frame=1, title1="", title2="", vmin1=None, vmax1=None, vmin2=None, vmax2=None, cmap1="gray", cmap2="gray", interval=10, **kwargs):
+    """Deprecated alias for :py:func:`optimap.video.show_video_pair`."""
+    return show_video_pair(video1, video2, skip_frame=skip_frame, title1=title1, title2=title2,
+                           vmin1=vmin1, vmax1=vmax1, vmin2=vmin2, vmax2=vmax2, cmap1=cmap1, cmap2=cmap2,
+                           interval=interval, **kwargs)
+
+
+@deprecated("use optimap.show_videos instead")
+def playn(videos, skip_frame=1, titles=None, cmaps="gray", vmins=None, vmaxs=None, interval=10, **kwargs):
+    """Deprecated alias for :py:func:`optimap.video.show_videos`."""
+    return show_videos(videos, skip_frame=skip_frame, titles=titles, cmaps=cmaps, vmins=vmins, vmaxs=vmaxs, interval=interval, **kwargs)
+
+
+@deprecated("use optimap.show_videos instead")
+def play_with_overlay(*args, **kwargs):
+    """Deprecated alias for :py:func:`optimap.video.show_video_overlay`."""
+    return show_video_overlay(*args, **kwargs)
+
+
+def show_video(video, skip_frame=1, title="", vmin=None, vmax=None, cmap="gray", interval=10, **kwargs):
     """Simple video player based on matplotlib's animate function.
 
     See :py:func:`optimap.video.play2` for a player for two videos side-by-side, and :py:func:`optimap.video.playn`
     for a player for `n` videos side-by-side.
 
     .. note::
         Using Monochrome is an alternative to this function, which allows for more control over the video player.
@@ -40,29 +66,29 @@
         Delay between frames in ms, by default 10.
         This is not the actual framerate, but the delay between frames.
     **kwargs
         Additional keyword arguments passed to :func:`matplotlib.pyplot.subplots`
 
     Returns
     -------
-    matplotlib.animation.FuncAnimation
+    InteractivePlayer
     """
-    return playn(
+    return show_videos(
         [video],
         skip_frame=skip_frame,
         titles=[title],
         cmaps=[cmap],
         vmins=[vmin],
         vmaxs=[vmax],
         interval=interval,
         **kwargs,
     )
 
 
-def play2(
+def show_video_pair(
     video1,
     video2,
     skip_frame=1,
     title1="video1",
     title2="video2",
     cmap1="gray",
     cmap2="gray",
@@ -102,36 +128,35 @@
     interval : int, optional
         Delay between frames in ms, by default 10. This is not the actual framerate, but the delay between frames.
     **kwargs
         Additional keyword arguments passed to :func:`matplotlib.pyplot.subplots`
 
     Returns
     -------
-    matplotlib.animation.FuncAnimation
+    InteractivePlayer
     """
     if vmin1 is None and vmin2 is None:
         vmins = None
     else:
         vmins = [vmin1, vmin2]
     if vmax1 is None and vmax2 is None:
         vmaxs = None
     else:
         vmaxs = [vmax1, vmax2]
-    return playn([video1, video2],
+    return show_videos([video1, video2],
                  skip_frame=skip_frame,
                  titles=[title1, title2],
                  cmaps=[cmap1, cmap2],
                  vmins=vmins,
                  vmaxs=vmaxs,
                  interval=interval,
                  **kwargs)
 
-
 @interactive_backend
-def playn(videos, skip_frame=1, titles=None, cmaps="gray", vmins=None, vmaxs=None, interval=10, **kwargs):
+def show_videos(videos, skip_frame=1, titles=None, cmaps="gray", vmins=None, vmaxs=None, interval=10, **kwargs):
     """Video player for `n` side-by-side videos based on matplotlib's animate function.
 
     Parameters
     ----------
     videos: list of {t, x, y} np.ndarray
         Videos to play.
     skip_frame : int, optional
@@ -147,23 +172,25 @@
     interval : int, optional
         Delay between frames in ms, by default 10. This is not the actual framerate, but the delay between frames.
     **kwargs
         Additional keyword arguments passed to :func:`matplotlib.pyplot.subplots`
 
     Returns
     -------
-    matplotlib.animation.FuncAnimation
+    InteractivePlayer
     """
     n = len(videos)
     nt = len(videos[0])
     for i in range(n):
+        if videos[i].ndim < 3 or videos[i].ndim > 4:
+            msg = f"Video {i} is not a video, it has shape {videos[i].shape}! Use show_image or show_traces instead."
+            raise ValueError(msg)
         if len(videos[i]) < nt:
             msg = "videos have to be same length!"
             raise ValueError(msg)
-        videos[i] = videos[i]
 
     if titles is None:
         titles = [f"Video {i}" for i in range(n)]
     if isinstance(cmaps, (Colormap, str)):
         cmaps = [cmaps for i in range(n)]
 
     if vmins is None:
@@ -204,30 +231,30 @@
         interval=interval,
     )
     plt.show(block=True)
     return ani
 
 
 @interactive_backend
-def play_with_overlay(
+def show_video_overlay(
     base: np.ndarray,
     overlay: np.ndarray,
     alpha: np.ndarray = None,
     skip_frames: int = 1,
     cmap_base="gray",
     cmap_overlay="Purples",
     vmin_base=None,
     vmax_base=None,
     vmin_overlay=None,
     vmax_overlay=None,
     interval=10,
     **kwargs,
 ):
     """Play a video with an overlay. See :func:`export_video_with_overlay` and :func:`iter_alpha_blend_videos` for more information.
-    
+
     Parameters
     ----------
     base : np.ndarray
         Base video to play.
     overlay : np.ndarray
         Video to overlay on the base video.
     alpha : np.ndarray, optional
@@ -246,15 +273,15 @@
         Minimum value for the colorbar of the overlay video, by default None
     vmax_overlay : float, optional
         Maximum value for the colorbar of the overlay video, by default None
     interval : int, optional
         Delay between frames in ms, by default 10. This is not the actual framerate, but the delay between frames.
     **kwargs
         Additional keyword arguments passed to :func:`matplotlib.pyplot.subplots`
-    
+
     Returns
     -------
     matplotlib.animation.FuncAnimation
     """
     fig, ax = plt.subplots(**kwargs)
 
     suptitle = fig.suptitle(f"Frame {0:4d}", font="monospace")
```

### Comparing `opticalmapping-0.2.0/optimap/video/_player.py` & `opticalmapping-0.2.2/optimap/video/_player.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         start=0,
         end=100,
         step=1,
         interval=25,
         gui_pos=(0.125, 0.92),
         **kwargs,
     ):
-        self.i = 0
+        self.i = start - step
         self.min = start
         self.max = end
         self.runs = True
         self.forwards = True
         self.step = step
         self.fig = fig
         self.func = func
@@ -92,23 +92,23 @@
             interval=interval,
             **kwargs,
         )
 
     def play(self):
         while self.runs:
             self.i = self.i + self.step
-            if self.i > self.min and self.i < self.max:
+            if self.i >= self.min and self.i < self.max:
                 yield self.i
             else:
                 if self.saving:
                     break
                 elif self.i >= self.max:
                     yield self.min
                 else:
-                    yield self.max
+                    yield self.min
 
     def update(self, i):
         self.slider.set_val(i)
         if self.saving:
             self.suptitle.set_text(f"Frame {i:4d}")
 
     def set_pos(self, i):
@@ -159,28 +159,43 @@
     def setup_gui(self, pos):
         self.ax_player = self.fig.add_axes([pos[0], pos[1], 0.64, 0.04])
         divider = make_axes_locatable(self.ax_player)
         self.ax_slider = divider.append_axes("right", size="500%", pad=0.07)
         self.button_stop = matplotlib.widgets.Button(self.ax_player, label="■")
         self.button_stop.on_clicked(self.toggle_play)
         self.slider = matplotlib.widgets.Slider(
-            self.ax_slider, "", self.min, self.max, valinit=self.i,
+            self.ax_slider, "", self.min, self.max - 1, valinit=self.min,
         )
         self.slider.on_changed(self.set_pos)
 
-    def save(self, *args, **kwargs):
+    def save(self, *args, hide_slider=True, hide_buttons=True, hide_framecounter=False, **kwargs):
         """Save the animation as a movie file, but hide the GUI buttons and slider.
-        
-        See FuncAnimation's :meth:`~matplotlib.animation.Animation.save` for arguments.
-        """
 
+        Parameters
+        ----------
+        *args :
+            See FuncAnimation's :meth:`~matplotlib.animation.Animation.save` for arguments.
+        hide_slider : bool, optional
+            Hide the slider, by default True
+        hide_buttons : bool, optional
+            Hide the play/pause button, by default True
+        hide_framecounter : bool, optional
+            Hide the frame counter, by default False
+        **kwargs :
+            See FuncAnimation's :meth:`~matplotlib.animation.Animation.save` for arguments.
+        """
+        self.i = self.min - self.step
         self.saving = True
-        # self.save_count = self.max // self.step
-
-        self.ax_player.set_visible(False)
-        self.ax_slider.set_visible(False)
+        self._save_count = (self.max - self.min) // self.step
+        if hide_buttons:
+            self.ax_player.set_visible(False)
+        if hide_slider:
+            self.ax_slider.set_visible(False)
+        if hide_framecounter:
+            self.suptitle.set_visible(False)
         super().save(*args, **kwargs)
 
         self.saving = False
-        # self.save_count = None
+        self._save_count = None
         self.ax_player.set_visible(True)
         self.ax_slider.set_visible(True)
+        self.suptitle.set_visible(True)
```

### Comparing `opticalmapping-0.2.0/pyproject.toml` & `opticalmapping-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,18 @@
 
 [tool.setuptools_scm]
 write_to = "optimap/_version.py"
 fallback_version = "0.1.0"
 
 [tool.cibuildwheel]
 archs = ["auto64"]  # 64-bit only
-skip = "pp* *musllinux*"  # disable PyPy, musl-based wheels, and Python 3.12 (waiting for dependencies to catch up)
+skip = "pp* *musllinux*"  # disable PyPy, musl-based wheels
 test-requires = ["pytest", "opencv-python-headless"]
 test-command = "pytest {project}/tests"
 
-[tool.cibuildwheel.macos]
-# https://cibuildwheel.readthedocs.io/en/stable/faq/#apple-silicon
-archs = ["x86_64", "universal2"]
-test-skip = ["*_arm64", "*_universal2:arm64"]
-
 [tool.ruff]
 exclude = [
   "docs",
 ]
 select = ['E', 'F', 'W', 'A', 'PLC', 'PLE', 'PLW', 'I', 'D', 'Q']
 target-version = "py39"
 line-length = 120
```

### Comparing `opticalmapping-0.2.0/setup.py` & `opticalmapping-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         "scikit-image",
         "scikit-video",
         "tqdm",
         "pooch",
         "seasonal",
         "static_ffmpeg",
         "mpl-pan-zoom",
+        "monochrome-viewer",
+        "Pillow>=10.0.1"  # not a strict requirement, but it makes importing 16-bit PNGs more consistent
     ],
     tests_require=["pytest"],
     ext_modules=[cpp_module],
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     extras_require={
         "all": [
@@ -82,10 +84,12 @@
             "sphinx-autobuild",
             "sphinx-copybutton",
             "sphinx-codeautolink",
             "furo",
             "myst_nb>=1.0.0",
             "jupytext",
             "jupyter-cache",
+            "sphinx-remove-toctrees",
+            "sphinx-design",
         ],
     },
 )
```

### Comparing `opticalmapping-0.2.0/tests/test_cpp.py` & `opticalmapping-0.2.2/tests/test_cpp.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     img = np.ones((64, 32), dtype=np.uint16)
     out = cpp.contrast_enhancement_img(img, 3)
     assert out.shape == img.shape
     assert out.dtype == np.float32
     assert np.all(out == 0)
 
     pytest.raises(RuntimeError, cpp.contrast_enhancement_img, img, 2)
+    
+    mask = np.ones((64, 32), dtype=bool)
+    out = cpp.contrast_enhancement_img(img, 3, mask)
 
 def test_contrastEnhanceVideo():
     vid = np.ones((100, 64, 32), dtype=np.uint16)
     out = cpp.contrast_enhancement_video(vid, 3)
     assert out.shape == vid.shape
     assert out.dtype == np.float32
     assert np.all(out == 0)
```

### Comparing `opticalmapping-0.2.0/tests/test_image.py` & `opticalmapping-0.2.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/tests/test_motion.py` & `opticalmapping-0.2.2/tests/test_motion.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,19 +6,48 @@
 def test_contrast_enhancement():
     img = np.ones((64, 32), dtype=np.uint16)
     vid = np.ones((10, 32, 32), dtype=np.float32)
     out = om.motion.contrast_enhancement(img, 3)
     assert out.shape == img.shape
     assert out.dtype == np.float32
     assert np.all(out == 0)
+
+    mask = np.ones_like(img, dtype=bool)
+    out2 = om.motion.contrast_enhancement(img, 3, mask)
+    assert np.all(out2 == out)
+
     out = om.motion.contrast_enhancement(vid, 3)
     assert out.shape == vid.shape
     assert out.dtype == np.float32
     assert np.all(out == 0)
 
+    mask = np.ones_like(vid, dtype=bool)
+    out2 = om.motion.contrast_enhancement(vid, 3, mask)
+    assert np.all(out2 == out)
+
+    mask = np.zeros_like(vid, dtype=bool)
+    out2 = om.motion.contrast_enhancement(vid, 3, mask)
+    assert np.all(out2 == 0)
+
+    mask = mask[0]
+    out2 = om.motion.contrast_enhancement(vid, 3, mask)
+    assert np.all(out2 == 0)
+
+    vid = np.random.random((10, 32, 32)).astype(np.float32)
+    out = om.motion.contrast_enhancement(vid, 3)
+    assert out.shape == vid.shape
+    assert out.min() == 0
+    assert out.max() == 1
+
+    mask = np.random.random((10, 32, 32)) > 0.5
+    out = om.motion.contrast_enhancement(vid, 3, mask)
+    assert out.shape == vid.shape
+    assert out.min() == 0
+    assert out.max() == 1
+
 def test_flowestimator():
     estimator = om.motion.FlowEstimator()
     vid = np.ones((10, 128, 128), dtype=np.float32)
     ref = np.ones((128, 128), dtype=np.float32)
     out = estimator.estimate(vid, ref)
     assert out.shape == vid.shape + (2,)
     assert out.dtype == np.float32
```

### Comparing `opticalmapping-0.2.0/tests/test_trace.py` & `opticalmapping-0.2.2/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `opticalmapping-0.2.0/tests/test_video.py` & `opticalmapping-0.2.2/tests/test_video.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,25 @@
     vid = (np.random.random((10, 128, 128)) * 8000).astype(np.uint16)
     out = om.video.normalize(vid, -0.5, 0.5)
     assert out.shape == vid.shape
     assert out.dtype == np.float32
     assert np.all(out >= -0.5)
     assert np.all(out <= 0.5)
 
+    vid = vid.astype(np.float64)
+    out = om.video.normalize(vid, dtype="float64")
+    assert out.dtype == np.float64
+    assert np.allclose(out.max(), 1.0)
+    assert np.allclose(out.min(), 0.0)
+
+    out = om.video.normalize(vid, dtype="uint8")
+    assert out.dtype == np.uint8
+    assert out.min() == 0
+    assert out.max() == 255
+
 def test_normalize_pixelwise():
     vid = (np.random.random((10, 128, 128)) * 8000).astype(np.uint16)
     out = om.video.normalize_pixelwise(vid, -0.5, 0.5)
     assert out.shape == vid.shape
     assert out.dtype == np.float32
     assert np.all(out >= -0.5)
     assert np.all(out <= 0.5)
@@ -49,23 +60,29 @@
     out2 = om.video.normalize_pixelwise(vid)
     assert np.allclose(out, out2)
 
 def test_temporal_difference():
     video = np.zeros((10, 128, 128), dtype=np.uint16)
     for i in range(1, 10):
         video[i] = i
-    out = om.video.temporal_difference(video, 1)
+    out = om.video.temporal_difference(video, 1, fill_value=np.inf)
     assert out.shape == video.shape
     assert out.dtype == np.float32
-    assert np.all(out[0] == 0)
+    assert np.all(out[0] == np.inf)
     assert np.all(out[1:] == 1)
 
     out = om.video.temporal_difference(video, 2)
     assert np.all(out[2:] == 2)
 
+    out = om.video.temporal_difference(video, 2, fill_value=np.inf, center=True)
+    assert out.shape == video.shape
+    assert out.dtype == np.float32
+    assert np.all(out[0] == np.inf) and np.all(out[-1] == np.inf)
+    assert np.all(out[1:-1] == 2)
+
 
 def test_resize():
     video = np.zeros((10, 128, 128), dtype=np.float32)
     out = om.video.resize(video, shape=(64, 64))
     assert out.shape == (10, 64, 64)
     assert out.dtype == np.float32
```

### Comparing `opticalmapping-0.2.0/tests/test_video_io.py` & `opticalmapping-0.2.2/tests/test_video_io.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     assert np.all(video == vid)
     assert video.flags["WRITEABLE"] is False
 
 
 def test_tiff_folder(tmpdir):
     vid = np.random.random((10, 4, 6)).astype(np.float32)
 
-    om.save_image_sequence(vid, directory=tmpdir, suffix=".tiff")
+    om.save_image_sequence(tmpdir, vid, format=".tiff")
     assert len(list(Path(tmpdir).glob("*.tiff"))) == 10
 
     video = om.load_video(tmpdir)
     assert video.shape == vid.shape
     assert video.dtype == vid.dtype
     assert np.all(video == vid)
 
@@ -53,15 +53,15 @@
     assert np.all(video == vid[1:6:2])
 
 
 def test_png_folder(tmpdir):
     vid = np.random.random((10, 4, 6)) * 16535
     vid = vid.astype(np.uint16)
 
-    om.save_image_sequence(vid, directory=tmpdir, suffix=".png")
+    om.save_image_sequence(tmpdir, vid, format=".png")
     assert len(list(Path(tmpdir).glob("*.png"))) == 10
 
     video = om.load_video(tmpdir)
     assert video.shape == vid.shape
     assert video.dtype == vid.dtype
     assert np.all(video == vid)
 
@@ -145,27 +145,54 @@
     om.export_video(filename, video, vmin=0, vmax=1)
     assert Path(filename).exists()
     assert Path(filename).is_file()
     assert mimetypes.guess_type(filename)[0] == "video/mp4"
 
 
 @pytest.mark.skipif(skvideo._HAS_FFMPEG == 0, reason="ffmpeg not installed")
+def test_export_video_uneven(tmpdir):
+    om.video.set_default_ffmpeg_encoder("libx264")
+    video = np.random.random((10, 15, 21)).astype(np.float32)
+    filename = Path(tmpdir / "test.mp4")
+    om.export_video(filename, video, vmin=0, vmax=1)
+    assert filename.is_file() and filename.stat().st_size > 0
+    assert mimetypes.guess_type(filename)[0] == "video/mp4"
+
+
+@pytest.mark.skipif(skvideo._HAS_FFMPEG == 0, reason="ffmpeg not installed")
 def test_export_video_overlay(tmpdir):
     video = np.random.random((10, 4, 4)).astype(np.float32)
     overlay = np.random.random((10, 4, 4)).astype(np.float32)
-    filename = tmpdir / "test.mp4"
+    filename = Path(tmpdir / "test.mp4")
     om.video.export_video_with_overlay(filename, video, overlay=overlay, vmin_base=0, vmax_base=1)
-    assert Path(filename).is_file()
+    assert filename.is_file() and filename.stat().st_size > 0
     assert mimetypes.guess_type(filename)[0] == "video/mp4"
 
     om.video.export_video_with_overlay(filename, video, overlay=overlay, alpha=overlay)
-    assert Path(filename).is_file()
+    assert filename.is_file() and filename.stat().st_size > 0
     assert mimetypes.guess_type(filename)[0] == "video/mp4"
 
+
 @pytest.mark.skipif(skvideo._HAS_FFMPEG == 0, reason="ffmpeg not installed")
 def test_export_video_collage(tmpdir):
     videos = [np.random.random((10, 4, 4)).astype(np.float32) for _ in range(4)]
-    filename = tmpdir / "test.mp4"
+    filename = Path(tmpdir / "test.mp4")
 
     om.video.export_video_collage(filename, videos, vmins=0, vmaxs=1, padding=10, ncols=2, padding_color="white")
-    assert Path(filename).is_file()
+    assert filename.is_file() and filename.stat().st_size > 0
     assert mimetypes.guess_type(filename)[0] == "video/mp4"
+
+
+@pytest.mark.skipif(skvideo._HAS_FFMPEG == 0, reason="ffmpeg not installed")
+def test_interactive_player_save(tmpdir):
+    import matplotlib.pyplot as plt
+    video = np.zeros((100, 32, 32), dtype=np.float32)
+
+    fn = Path(tmpdir / "test.mp4")
+    # fn = Path('/tmp') / "test.mp4"
+    fig, ax = plt.subplots()
+    imshow = ax.imshow(video[0])
+    player = om.video.InteractivePlayer(fig, lambda i: imshow.set_data(video[i]), end=len(video))
+    player.save(fn, fps=25, hide_framecounter=True)
+    plt.close(fig)
+    assert fn.exists()
+    assert fn.is_file() and fn.stat().st_size > 0
```

