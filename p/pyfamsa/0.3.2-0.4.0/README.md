# Comparing `tmp/pyfamsa-0.3.2.tar.gz` & `tmp/pyfamsa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfamsa-0.3.2.tar", last modified: Sat Jan 27 13:58:51 2024, max compression
+gzip compressed data, was "pyfamsa-0.4.0.tar", last modified: Mon May  6 14:27:51 2024, max compression
```

## Comparing `pyfamsa-0.3.2.tar` & `pyfamsa-0.4.0.tar`

### file list

```diff
@@ -1,259 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.503548 pyfamsa-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-01-27 13:58:51.503548 pyfamsa-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.455547 pyfamsa-0.3.2/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.459547 pyfamsa-0.3.2/include/famsa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/__init__.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.463547 pyfamsa-0.3.2/include/famsa/core/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/io_service.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/params.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/profile.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/core/version.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/msa.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.463547 pyfamsa-0.3.2/include/famsa/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/tree/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/tree/abstract_tree_generator.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/tree/guide_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/tree/newick_parser.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.463547 pyfamsa-0.3.2/include/famsa/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/utils/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/utils/log.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/include/famsa/utils/memory_monotonic.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.463547 pyfamsa-0.3.2/patches/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/NewickParser.h.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/memory_monotonic.h.patch
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/msa.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/msa.h.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/sequence.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/patches/sequence.h.patch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.463547 pyfamsa-0.3.2/pyfamsa/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/_famsa.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/_famsa.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/_famsa.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.467547 pyfamsa-0.3.2/pyfamsa/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.479547 pyfamsa-0.3.2/pyfamsa/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47464 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.faa
--rw-r--r--   0 runner    (1001) docker     (127)    68569 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.sl.afa
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.sl.nwk
--rw-r--r--   0 runner    (1001) docker     (127)    70021 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.upgma.afa
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.upgma.nwk
--rw-r--r--   0 runner    (1001) docker     (127)   287439 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.faa
--rw-r--r--   0 runner    (1001) docker     (127)  2097465 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-nj.afa
--rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-nj.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  1913193 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-sl.afa
--rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-sl.nwk
--rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-slink.nwk
--rw-r--r--   0 runner    (1001) docker     (127)  2030457 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-upgma.afa
--rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/test_aligner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/pyfamsa/tests/test_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.467547 pyfamsa-0.3.2/pyfamsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10774 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyfamsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyfamsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyfamsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyfamsa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyfamsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-27 13:58:51.000000 pyfamsa-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-01-27 13:58:51.503548 pyfamsa-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    36592 2024-01-27 13:58:44.000000 pyfamsa-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.451547 pyfamsa-0.3.2/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.479547 pyfamsa-0.3.2/vendor/FAMSA/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.455547 pyfamsa-0.3.2/vendor/FAMSA/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.479547 pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/atomic_wait
--rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/barrier
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/latch
--rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/semaphore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.479547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.479547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/common_defs.h
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.483548 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.487547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (127)    25448 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h
--rw-r--r--   0 runner    (1001) docker     (127)   124274 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.h
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/lib_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/unaligned.h
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.487547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/zlib_constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/libdeflate.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.487547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/checksum.c
--rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/gzip.c
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/prog_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/prog_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_overread.c
--rw-r--r--   0 runner    (1001) docker     (127)    22742 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_util.c
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.487547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1512 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/scripts/detect.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.491547 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/windows/
--rw-r--r--   0 runner    (1001) docker     (127)    73752 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.495548 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-aligned.c
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-override.c
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-posix.c
--rw-r--r--   0 runner    (1001) docker     (127)    32874 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc.c
--rw-r--r--   0 runner    (1001) docker     (127)    19573 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/arena.c
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/bitmap.c
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/bitmap.h
--rw-r--r--   0 runner    (1001) docker     (127)    20115 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/heap.c
--rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/init.c
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h
--rw-r--r--   0 runner    (1001) docker     (127)    40784 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-override.h
--rw-r--r--   0 runner    (1001) docker     (127)    24060 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-types.h
--rw-r--r--   0 runner    (1001) docker     (127)    28550 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    22798 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/options.c
--rw-r--r--   0 runner    (1001) docker     (127)    55869 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/os.c
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/page-queue.c
--rw-r--r--   0 runner    (1001) docker     (127)    33440 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/page.c
--rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    20963 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/region.c
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/segment-cache.c
--rw-r--r--   0 runner    (1001) docker     (127)    65602 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/segment.c
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/static.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21607 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/stats.c
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.495548 pyfamsa-0.3.2/vendor/FAMSA/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.495548 pyfamsa-0.3.2/vendor/FAMSA/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/defs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/io_service.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/io_service.h
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/params.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/params.h
--rw-r--r--   0 runner    (1001) docker     (127)    47408 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/profile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/profile.h
--rw-r--r--   0 runner    (1001) docker     (127)    31900 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/profile_par.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    29543 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/profile_seq.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/queues.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/queues.h
--rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/sequence.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/sequence.h
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/core/version.h
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/famsa.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.495548 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp.h
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_classic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_classic.h
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h
--rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/msa.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/msa.h
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/msa_refinement.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.499548 pyfamsa-0.3.2/vendor/FAMSA/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/Chained.h
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/Clustering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/Clustering.h
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/DistanceCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/DistanceCalculator.h
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/FastTree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/FastTree.h
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/GuideTree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/GuideTree.h
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/IPartialGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/MSTPrim.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/MSTPrim.h
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/NeighborJoining.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/NeighborJoining.h
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/NewickParser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/NewickParser.h
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkage.h
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkageQueue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/TreeDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/UPGMA.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/tree/UPGMA.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 13:58:51.503548 pyfamsa-0.3.2/vendor/FAMSA/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/array.h
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/conversion.h
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/cpuid.h
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/deterministic_random.h
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/log.h
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/memory_monotonic.h
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/meta_oper.h
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/pooled_threads.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/pooled_threads.h
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/statistics.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/timer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/timer.h
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils_avx.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-27 13:58:45.000000 pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils_neon.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.486444 pyfamsa-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-06 14:27:51.486444 pyfamsa-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.438442 pyfamsa-0.4.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.446442 pyfamsa-0.4.0/include/famsa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.446442 pyfamsa-0.4.0/include/famsa/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/io_service.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/params.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/profile.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/sequence.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/core/version.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/msa.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.446442 pyfamsa-0.4.0/include/famsa/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/tree/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/tree/abstract_tree_generator.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/tree/guide_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/tree/newick_parser.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.446442 pyfamsa-0.4.0/include/famsa/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/utils/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/utils/log.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/include/famsa/utils/memory_monotonic.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.446442 pyfamsa-0.4.0/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/NewickParser.h.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/memory_monotonic.h.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/msa.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/msa.h.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/sequence.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/patches/sequence.h.patch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.450443 pyfamsa-0.4.0/pyfamsa/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/_famsa.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/_famsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22263 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/_famsa.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.450443 pyfamsa-0.4.0/pyfamsa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.462443 pyfamsa-0.4.0/pyfamsa/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47464 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.faa
+-rw-r--r--   0 runner    (1001) docker     (127)    68569 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.sl.afa
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.sl.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)    70021 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.upgma.afa
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)   287439 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.faa
+-rw-r--r--   0 runner    (1001) docker     (127)  2097465 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa
+-rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)  1913193 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa
+-rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)  2030457 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa
+-rw-r--r--   0 runner    (1001) docker     (127)   129095 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/test_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/pyfamsa/tests/test_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.450443 pyfamsa-0.4.0/pyfamsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyfamsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-06 14:27:51.000000 pyfamsa-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-06 14:27:51.486444 pyfamsa-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    36711 2024-05-06 14:27:46.000000 pyfamsa-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.438442 pyfamsa-0.4.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.462443 pyfamsa-0.4.0/vendor/FAMSA/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.438442 pyfamsa-0.4.0/vendor/FAMSA/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.462443 pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/atomic_wait
+-rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/barrier
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/latch
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/semaphore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.462443 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.462443 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.466443 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.470443 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25448 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)   124274 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.470443 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/zlib_constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/libdeflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.474444 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22742 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.474444 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1512 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.474444 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)    73752 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.478444 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-override.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    32874 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19573 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/arena.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/bitmap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20115 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/heap.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25391 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/init.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40784 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24060 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28550 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22798 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/options.c
+-rw-r--r--   0 runner    (1001) docker     (127)    55869 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/os.c
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11537 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/page-queue.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33440 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/page.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20963 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/region.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/segment-cache.c
+-rw-r--r--   0 runner    (1001) docker     (127)    65602 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/segment.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/static.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21607 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/stats.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.478444 pyfamsa-0.4.0/vendor/FAMSA/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.478444 pyfamsa-0.4.0/vendor/FAMSA/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/defs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/io_service.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/io_service.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/params.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/params.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47408 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/profile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/profile.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31900 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/profile_par.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29543 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/profile_seq.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/queues.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/queues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/sequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/sequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/core/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/famsa.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.482444 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_classic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/msa.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/msa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/msa_refinement.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.482444 pyfamsa-0.4.0/vendor/FAMSA/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/Chained.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/Clustering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/Clustering.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/DistanceCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/FastTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/FastTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/GuideTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/GuideTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/IPartialGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/MSTPrim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/MSTPrim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/NeighborJoining.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/NeighborJoining.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/NewickParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/NewickParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/TreeDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/UPGMA.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/tree/UPGMA.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:27:51.486444 pyfamsa-0.4.0/vendor/FAMSA/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/conversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/cpuid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/deterministic_random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/memory_monotonic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/meta_oper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/pooled_threads.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/pooled_threads.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/statistics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/timer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils_avx.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-06 14:27:47.000000 pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils_neon.cpp
```

### Comparing `pyfamsa-0.3.2/CHANGELOG.md` & `pyfamsa-0.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pyfamsa/compare/v0.3.2...HEAD
+[Unreleased]: https://github.com/althonos/pyfamsa/compare/v0.4.0...HEAD
+
+
+## [v0.4.0] - 2024-05-06
+[v0.4.0]: https://github.com/althonos/pyfamsa/compare/v0.3.2...v0.4.0
+
+### Added
+- `scoring-matrices` dependency to handle alternative scoring matrices.
+- `scoring_matrix` argument to `Aligner` constructor to use a non-default matrix ([#3](https://github.com/althonos/pyfamsa/issues/3)).
+
+### Fixed
+- Use of outdated `importlib.resources` interface in `pyfamsa.tests` package.
+- Missing defines for compilation of NEON code on non-Aarch64 Arm platforms.
 
 
 ## [v0.3.2] - 2024-01-27
 [v0.3.2]: https://github.com/althonos/pyfamsa/compare/v0.3.1...v0.3.2
 
 ### Added
 - `pickle` protocol support for `Sequence` objects.
```

### Comparing `pyfamsa-0.3.2/CONTRIBUTING.md` & `pyfamsa-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/COPYING` & `pyfamsa-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/MANIFEST.in` & `pyfamsa-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/PKG-INFO` & `pyfamsa-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfamsa
-Version: 0.3.2
+Version: 0.4.0
 Summary: Cython bindings and Python interface to FAMSA, an algorithm for ultra-scale multiple sequence alignments.
 Home-page: https://github.com/althonos/pyfamsa
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyfamsa.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyfamsa/issues
@@ -69,39 +69,42 @@
 
 PyFAMSA is a Python module that provides bindings to [FAMSA](https://github.com/refresh-bio/FAMSA)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to align protein sequences using different parameters and access
 results directly. It interacts with the FAMSA library interface, which has
 the following advantages:
 
-- **single dependency**: pyfamsa is distributed as a Python package, so you
+- **single dependency**: PyFAMSA is distributed as a Python package, so you
   can add it as a dependency to your project, and stop worrying about the
   FAMSA binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the FAMSA CLI using a
   sub-process and temporary files.
 - **friendly interface**: The different guide tree build methods and
   heuristics can be selected from the Python code with a simple keyword
   argument when configuring a new [`Aligner`](https://pyfamsa.readthedocs.io/en/stable/api/aligner.html#pyfamsa.Aligner).
+- **custom scoring matrices**: You can use any custom scoring matrix from 
+  the [`scoring-matrices`](https://pypi.org/project/scoring-matrices) library
+  in addition to the default MIQS to score the alignment. 
 
 ## 🔧 Installing
 
 PyFAMSA can be installed directly from [PyPI](https://pypi.org/project/pyfamsa/),
 which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
 and the Aarch64 architecture (Linux only), as well as the code required to
 compile from source with Cython:
 ```console
 $ pip install pyfamsa
 ```
 
-<!-- Otherwise, pyfamsa is also available as a [Bioconda](https://bioconda.github.io/)
+Otherwise, PyFAMSA is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pyfamsa
-``` -->
+```
 
 Otherwise, have a look at the [Installation page](https://pyfamsa.readthedocs.io/en/stable/install.html) of the [online documentation](https://pyfamsa.readthedocs.io/)
 
 ## 💡 Example
 
 Let's create some sequences in memory, align them using the UPGMA method,
 (without any heuristic), and simply print the alignment on screen:
```

### Comparing `pyfamsa-0.3.2/README.md` & `pyfamsa-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,39 +30,42 @@
 
 PyFAMSA is a Python module that provides bindings to [FAMSA](https://github.com/refresh-bio/FAMSA)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to align protein sequences using different parameters and access
 results directly. It interacts with the FAMSA library interface, which has
 the following advantages:
 
-- **single dependency**: pyfamsa is distributed as a Python package, so you
+- **single dependency**: PyFAMSA is distributed as a Python package, so you
   can add it as a dependency to your project, and stop worrying about the
   FAMSA binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the FAMSA CLI using a
   sub-process and temporary files.
 - **friendly interface**: The different guide tree build methods and
   heuristics can be selected from the Python code with a simple keyword
   argument when configuring a new [`Aligner`](https://pyfamsa.readthedocs.io/en/stable/api/aligner.html#pyfamsa.Aligner).
+- **custom scoring matrices**: You can use any custom scoring matrix from 
+  the [`scoring-matrices`](https://pypi.org/project/scoring-matrices) library
+  in addition to the default MIQS to score the alignment. 
 
 ## 🔧 Installing
 
 PyFAMSA can be installed directly from [PyPI](https://pypi.org/project/pyfamsa/),
 which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
 and the Aarch64 architecture (Linux only), as well as the code required to
 compile from source with Cython:
 ```console
 $ pip install pyfamsa
 ```
 
-<!-- Otherwise, pyfamsa is also available as a [Bioconda](https://bioconda.github.io/)
+Otherwise, PyFAMSA is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pyfamsa
-``` -->
+```
 
 Otherwise, have a look at the [Installation page](https://pyfamsa.readthedocs.io/en/stable/install.html) of the [online documentation](https://pyfamsa.readthedocs.io/)
 
 ## 💡 Example
 
 Let's create some sequences in memory, align them using the UPGMA method,
 (without any heuristic), and simply print the alignment on screen:
```

### Comparing `pyfamsa-0.3.2/include/famsa/core/__init__.pxd` & `pyfamsa-0.4.0/include/famsa/core/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/include/famsa/core/io_service.pxd` & `pyfamsa-0.4.0/include/famsa/core/io_service.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/include/famsa/core/params.pxd` & `pyfamsa-0.4.0/include/famsa/core/params.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/include/famsa/core/sequence.pxd` & `pyfamsa-0.4.0/include/famsa/core/sequence.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/include/famsa/msa.pxd` & `pyfamsa-0.4.0/include/famsa/msa.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from famsa.tree.abstract_tree_generator cimport AbstractTreeGenerator
 
 cdef extern from "msa.h" nogil:
 
     cdef cppclass CFAMSA:
         instruction_set_t instruction_set
         score_t avg_sim
+        vector[vector[score_t]] score_matrix
+        vector[score_t] score_vector
 
         CFAMSA(CParams& params) except +
 
         bool ComputeAlignment(tree_structure& guide_tree) except +
         # bool RefineAlignment(CProfile *&profile_to_refine)
         bool GetAlignment(vector[CGappedSequence*]& result) except +
         score_t GetScore()
@@ -33,7 +35,11 @@
         void sortAndExtendSequences(vector[CSequence]& sequences) except +
         void extendSequences(vector[CSequence]& sequences) except +
         void shrinkSequences(vector[CSequence]& sequences) except +
         void removeDuplicates(vector[CSequence*]& sorted_seqs, vector[int]& original2sorted) except +
 
         bool ComputeMSA(vector[CSequence]& sequences) except +
 
+
+cdef extern from "msa.h" namespace "CFAMSA" nogil:
+
+    const double[24][24] SM_MIQS
```

### Comparing `pyfamsa-0.3.2/include/famsa/tree/newick_parser.pxd` & `pyfamsa-0.4.0/include/famsa/tree/newick_parser.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/include/famsa/utils/memory_monotonic.pxd` & `pyfamsa-0.4.0/include/famsa/utils/memory_monotonic.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/patches/memory_monotonic.h.patch` & `pyfamsa-0.4.0/patches/memory_monotonic.h.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/patches/sequence.cpp.patch` & `pyfamsa-0.4.0/patches/sequence.cpp.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/patches/sequence.h.patch` & `pyfamsa-0.4.0/patches/sequence.h.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/_famsa.pxd` & `pyfamsa-0.4.0/pyfamsa/_famsa.pxd`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 
 # --- C imports --------------------------------------------------------------
 
 from libcpp.memory cimport shared_ptr
 from libcpp.vector cimport vector
 
 from famsa.msa cimport CFAMSA
+from famsa.core cimport NO_AMINOACIDS
 from famsa.core.params cimport CParams
 from famsa.core.sequence cimport CSequence, CGappedSequence
 from famsa.tree.guide_tree cimport GuideTree as CGuideTree
 from famsa.utils.memory_monotonic cimport memory_monotonic_safe
 
+from scoring_matrices.lib cimport ScoringMatrix
+
 # --- Allocator --------------------------------------------------------------
 
 cdef memory_monotonic_safe* MMA = new memory_monotonic_safe()
 
 # --- Classes ----------------------------------------------------------------
 
 cdef class Sequence:
@@ -32,18 +35,22 @@
 
 cdef class Alignment:
     cdef shared_ptr[CFAMSA]       _famsa
     cdef vector[CGappedSequence*] _msa
 
 
 cdef class Aligner:
-    cdef CParams _params
+    cdef          CParams       _params
+    cdef readonly ScoringMatrix scoring_matrix
+
+    cdef int _copy_matrix(self, CFAMSA* famsa) except 1 nogil
 
     cpdef Alignment align(self, object sequences)
     cpdef GuideTree build_tree(self, object sequences)
 
+
 cdef class GuideTree:
     cdef CGuideTree        _tree
     cdef vector[CSequence] _names
 
     cpdef bytes dumps(self)
     cpdef ssize_t dump(self, object file) except -1
```

### Comparing `pyfamsa-0.3.2/pyfamsa/_famsa.pyi` & `pyfamsa-0.4.0/pyfamsa/_famsa.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import datetime
 import os
 import typing
 
+from scoring_matrices import ScoringMatrix
+
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 GuideTreeMethod = Literal["sl", "slink", "upgma", "nj"]
 TreeHeuristicMethod = Literal["medoid", "part"]
 Node = typing.Tuple[int, int]
 
+FAMSA_ALPHABET: str
+MIQS: ScoringMatrix
+
 class _VersionInfo(typing.NamedTuple):
     major: int
     minor: int
     micro: int
 
 class _Info(typing.NamedTuple):
     version: str
@@ -52,14 +57,15 @@
         threads: int = 0,
         guide_tree: GuideTreeMethod = "sl",
         tree_heuristic: typing.Optional[TreeHeuristicMethod] = None,
         medoid_threshold: int = 0,
         n_refinements: int = 100,
         keep_duplicates: bool = False,
         refine: typing.Optional[bool] = None,
+        scoring_matrix: typing.Union[ScoringMatrix, str, None] = None,
     ) -> None: ...
     def align(self, sequences: typing.Iterable[Sequence]) -> Alignment: ...
     def build_tree(self, sequences: typing.Iterable[Sequence]) -> GuideTree: ...
 
 class GuideTree(typing.Sequence[Node]):
     def __init__(self) -> None: ...
     def __len__(self) -> int: ...
```

### Comparing `pyfamsa-0.3.2/pyfamsa/_famsa.pyx` & `pyfamsa-0.4.0/pyfamsa/_famsa.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,92 @@
 # coding: utf-8
 # cython: language_level=3, linetrace=True
 """Bindings to FAMSA, an algorithm for fast multiple sequence alignments.
 
+Attributes:
+    FAMSA_ALPHABET (`str`): The alphabet used by default by FAMSA to encode
+        sequences with ordinal encoding.
+    MIQS (`~scoring_matrices.ScoringMatrix`): The MIQS scoring matrix proposed
+        by Yamada & Tomii (2014), used by default in FAMSA for scoring
+        alignments.
+
 References:
     - Deorowicz, S., Debudaj-Grabysz, A., Gudyś, A. (2016)
       *FAMSA: Fast and accurate multiple sequence alignment of huge protein
       families*. Scientific Reports, 6, 33964. :doi:`10.1038/srep33964`.
+    - Yamada, K., Tomii, K. (2014).
+      *Revisiting amino acid substitution matrices for identifying distantly
+      related proteins*. Bioinformatics (Oxford, England), 30(3), 317-325.
+      :doi:`10.1093/bioinformatics/btt694`. :pmid:`24281694`.
 
 """
 
 # --- C imports --------------------------------------------------------------
 
 from cpython cimport Py_buffer
 from cpython.memoryview cimport PyMemoryView_FromMemory
 from cpython.buffer cimport PyBUF_FORMAT, PyBUF_READ
 from cpython.bytes cimport PyBytes_FromStringAndSize, PyBytes_AS_STRING
 
 from libc.stdint cimport uint32_t
 from libc.string cimport memset
+from libc.math cimport roundf
 from libcpp cimport bool
 from libcpp.memory cimport shared_ptr
 from libcpp.utility cimport move
 from libcpp.vector cimport vector
 from libcpp.string cimport string
 
 cimport famsa.core.version
-from famsa.core cimport symbol_t, GAP, GUARD
+from famsa.core cimport score_t, symbol_t, GAP, GUARD, NO_AMINOACIDS, cost_cast_factor
 from famsa.core.params cimport CParams, ON, OFF, AUTO
 from famsa.core.sequence cimport CSequence, CGappedSequence
-from famsa.msa cimport CFAMSA
+from famsa.msa cimport CFAMSA, SM_MIQS
 from famsa.tree cimport GT, node_t
 from famsa.tree.guide_tree cimport GuideTree as CGuideTree
 from famsa.tree.newick_parser cimport NewickParser
 from famsa.tree.abstract_tree_generator cimport AbstractTreeGenerator
 from famsa.utils.memory_monotonic cimport memory_monotonic_safe
 # from famsa.utils.log cimport Log, LEVEL_NORMAL, LEVEL_DEBUG, LEVEL_VERBOSE
 
+from scoring_matrices.lib cimport ScoringMatrix
 
 # --- Python imports ---------------------------------------------------------
 
 import datetime
 import collections
 import os
 
 include "_version.py"
 
 # --- Constants --------------------------------------------------------------
 
+FAMSA_ALPHABET = "ARNDCQEGHILKMFPSTWYVBZX*"
+
 cdef memory_monotonic_safe* MMA = new memory_monotonic_safe()
 
-cdef char SYMBOLS[25]
-for i, x in enumerate(b"ARNDCQEGHILKMFPSTWYVBZX*"):
-    SYMBOLS[i] = x
+cdef char SYMBOLS[NO_AMINOACIDS]
+for i, x in enumerate(FAMSA_ALPHABET):
+    SYMBOLS[i] = ord(x)
+
+cdef ScoringMatrix _make_miqs():
+    cdef list row
+    cdef list weights = []
+    for i in range(NO_AMINOACIDS):
+        row = []
+        for j in range(NO_AMINOACIDS):
+            row.append(round(SM_MIQS[i][j], 4))
+        weights.append(row)
+    return ScoringMatrix(
+        weights,
+        alphabet=FAMSA_ALPHABET,
+        name="MIQS",
+    )
+
+MIQS = _make_miqs()
 
 # Log.getInstance(LEVEL_NORMAL).enable()
 # Log.getInstance(LEVEL_VERBOSE).enable()
 # Log.getInstance(LEVEL_DEBUG).enable()
 
 
 # --- Version info about the wrapped FAMSA code ------------------------------
@@ -179,18 +210,15 @@
                 mem += 1
 
         return seq
 
     # --- Methods ------------------------------------------------------------
 
     cpdef Sequence copy(self):
-        """copy(self)\n--
-
-        Copy the sequence data, and return the copy.
-
+        """Copy the sequence data, and return the copy.
         """
         cdef Sequence seq = Sequence.__new__(Sequence)
         seq._cseq = move(CSequence(self._cseq))
         seq._shape = self._shape
         return seq
 
 
@@ -267,14 +295,22 @@
         gapped.alignment = self
         gapped._gseq = self._msa[index_]
         return gapped
 
 
 cdef class Aligner:
     """A single FAMSA aligner.
+
+    Attributes:
+        scoring_matrix (`~scoring_matrices.ScoringMatrix`): The scoring
+            matrix used for scoring alignments.
+
+    .. versionadded:: 0.4.0
+       The ``scoring_matrix`` attribute.
+
     """
 
     # --- Magic methods ------------------------------------------------------
 
     def __cinit__(self):
         self._params = CParams()
         self._params.verbose_mode = True
@@ -287,18 +323,17 @@
         int threads=0,
         object guide_tree="sl",
         object tree_heuristic=None,
         int medoid_threshold=0,
         int n_refinements=100,
         bool keep_duplicates=False,
         object refine=None,
+        object scoring_matrix=None,
     ):
-        """__init__(self, *, threads=0, guide_tree="sl", tree_heuristic=None, medoid_threshold=0, n_refinements=100, keep_duplicates=False, refine=None)\n--
-
-        Create a new aligner with the given configuration.
+        """Create a new aligner with the given configuration.
 
         Keyword Arguments:
             threads (`int`): The number of threads to use for parallel
                 computations. If *0* given (the default), use `os.cpu_count`
                 to spawn one thread per CPU on the host machine.
             guide_tree (`str`): The method for building the guide tree.
                 Supported values are: ``sl`` for MST+Prim single linkage,
@@ -309,19 +344,26 @@
                 medoid trees, ``part`` for part trees, or `None` to disable
                 heuristics.
             medoid_threshold (`int`): The minimum number of sequences a
                 set must contain for medoid trees to be used, if enabled
                 with ``tree_heuristic``.
             n_refinements (`int`): The number of refinement iterations to
                 run.
-            keep_duplicates (`bool`): Set to `True` to avoid discarding 
+            keep_duplicates (`bool`): Set to `True` to avoid discarding
                 duplicate sequences before building trees or alignments.
             refine (`bool` or `None`): Set to `True` to force refinement,
                 `False` to disable refinement, or leave as `None` to disable
                 refinement automatically for sets of more than 1000 sequences.
+            scoring_matrix (`~scoring_matrices.ScoringMatrix` or `str`): The
+                scoring matrix to use for scoring alignments. By default, the
+                *MIQS* matrix by Yamada & Tomii (2014) is used like in the
+                original FAMSA implementation.
+
+        .. versionadded:: 0.4.0
+           The ``scoring_matrix`` argument.
 
         """
         self._params.keepDuplicates = keep_duplicates
 
         if refine is True:
             self._params.refinement_mode = ON
         elif refine is False:
@@ -364,39 +406,65 @@
             raise ValueError("`medoid_threshold` argument must be positive")
 
         if n_refinements >= 0:
             self._params.n_refinements = n_refinements
         else:
             raise ValueError("`n_refinements` argument must be positive")
 
+        if scoring_matrix is None:
+            self.scoring_matrix = MIQS
+        elif isinstance(scoring_matrix, str):
+            self.scoring_matrix = ScoringMatrix.from_name(scoring_matrix).shuffle(FAMSA_ALPHABET)
+        elif isinstance(scoring_matrix, ScoringMatrix):
+            if scoring_matrix.alphabet != FAMSA_ALPHABET:
+                raise ValueError(f"invalid scoring matrix alphabet: expected {FAMSA_ALPHABET!r}, got {scoring_matrix.alphabet!r}")
+            self.scoring_matrix = scoring_matrix
+        else:
+            ty = type(scoring_matrix).__name__
+            raise TypeError(f"expected str or ScoringMatrix, found {ty}")
 
     # --- Methods ------------------------------------------------------------
 
-    cpdef Alignment align(self, object sequences):
-        """align(self, sequences)\n--
+    cdef int _copy_matrix(self, CFAMSA* famsa) except 1 nogil:
+        cdef size_t i
+        cdef size_t j
+        cdef const float** matrix = self.scoring_matrix.matrix_ptr()
+        for i in range(<size_t> NO_AMINOACIDS):
+            famsa.score_vector[i] = <score_t> roundf(cost_cast_factor * matrix[i][i])
+            for j in range(<size_t> NO_AMINOACIDS):
+                famsa.score_matrix[i][j] = <score_t> roundf(cost_cast_factor * matrix[i][j])
+        return 0
 
-        Align sequences together.
+    cpdef Alignment align(self, object sequences):
+        """Align sequences together.
 
         Arguments:
             sequences (iterable of `~pyfamsa.Sequence`): An iterable
                 yielding the digitized sequences to align.
 
         Returns:
             `~pyfamsa.Alignment`: The aligned sequences, in aligned format.
 
         """
         cdef int                      i
+        cdef int                      j
         cdef Sequence                 sequence
         cdef CSequence                cseq
         cdef vector[CSequence]        seqvec
         cdef vector[CGappedSequence*] gapvec
+        cdef const float**            matrix
         cdef Alignment                alignment = Alignment.__new__(Alignment)
+        cdef CFAMSA*                  famsa     = new CFAMSA(self._params)
 
-        # create a new aligner
-        alignment._famsa = shared_ptr[CFAMSA](new CFAMSA(self._params))
+        # copy score matrix weights
+        with nogil:
+            self._copy_matrix(famsa)
+
+        # record the aligner on the resulting alignment
+        alignment._famsa = shared_ptr[CFAMSA](famsa)
 
         # copy the aligner input and record sequence order
         for i, sequence in enumerate(sequences):
             cseq = CSequence(sequence._cseq)
             cseq.sequence_no = cseq.original_no = i
             seqvec.push_back(move(cseq))
 
@@ -405,17 +473,15 @@
             with nogil:
                 alignment._famsa.get().ComputeMSA(seqvec)
                 alignment._famsa.get().GetAlignment(alignment._msa)
 
         return alignment
 
     cpdef GuideTree build_tree(self, object sequences):
-        """build_tree(self, sequences)\n--
-
-        Build a tree from the given sequences.
+        """Build a tree from the given sequences.
 
         Arguments:
             sequences (iterable of `~pyfamsa.Sequence`): An iterable
                 yielding the digitized sequences to build a tree from.
 
         Returns:
             `~pyfamsa.GuideTree`: The guide tree obtained from the sequences.
@@ -424,31 +490,36 @@
         cdef size_t                            i
         cdef Sequence                          sequence
         cdef CSequence                         cseq
         cdef vector[CSequence]                 seqvec
         cdef vector[CSequence*]                ptrvec
         cdef shared_ptr[AbstractTreeGenerator] gen
         cdef vector[int]                       og2map
+        cdef const float**                     matrix
         cdef CFAMSA*                           famsa    = new CFAMSA(self._params)
         cdef GuideTree                         tree     = GuideTree.__new__(GuideTree)
 
+        # copy score matrix weights
+        with nogil:
+            self._copy_matrix(famsa)
+
         # copy the aligner input and record original order
         for i, sequence in enumerate(sequences):
             cseq = CSequence(sequence._cseq)
             cseq.sequence_no = cseq.original_no = i
             seqvec.push_back(move(cseq))
 
         # sort sequences and record pointers
         if seqvec.size() > 0:
             famsa.sortAndExtendSequences(seqvec)
         for i in range(seqvec.size()):
             og2map.push_back(i)
             ptrvec.push_back(&seqvec.data()[i])
             tree._names.push_back(move(CSequence(seqvec[i].id, string(), i, NULL)))
-        
+
         # remove duplicates and record sequence order
         if not self._params.keepDuplicates:
             famsa.removeDuplicates(ptrvec, og2map)
         for i in range(ptrvec.size()):
             ptrvec[i].sequence_no = i
 
         # # check enough sequences where given
@@ -505,34 +576,30 @@
         """`list` of `bytes`: The name of the leaves in the guide tree.
         """
         return [ <bytes> self._names[i].id for i in range(self._names.size()) ]
 
     # --- Methods ------------------------------------------------------------
 
     cpdef bytes dumps(self):
-        """dumps(self)\n--
-
-        Dump the tree in Newick format into a `bytes` object.
+        """Dump the tree in Newick format into a `bytes` object.
 
         Returns:
             `bytes`: The tree in Newick format, stored as an ASCII string.
 
         """
         cdef string       out
         cdef NewickParser nw
 
         with nogil:
             nw.store(self._names, self._tree.raw(), out)
 
         return <bytes> out
 
     cpdef ssize_t dump(self, object file) except -1:
-        """dump(self, file)\n--
-
-        Write the tree into a file in Newick format.
+        """Write the tree into a file in Newick format.
 
         Arguments:
             file (`str`, `bytes, `os.PathLike` or file-like object): The
                 path to a file, or a file-like object open in binary mode.
 
         """
         cdef string       out
```

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.faa` & `pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.faa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.sl.afa` & `pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.sl.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.sl.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.sl.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.upgma.afa` & `pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.upgma.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/adeno_fiber.upgma.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.faa` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.faa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-nj.afa` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-nj.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-sl.afa` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-sl.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-slink.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-upgma.afa` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk` & `pyfamsa-0.4.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/fasta.py` & `pyfamsa-0.4.0/pyfamsa/tests/fasta.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/test_doctest.py` & `pyfamsa-0.4.0/pyfamsa/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa/tests/test_sequence.py` & `pyfamsa-0.4.0/pyfamsa/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/pyfamsa.egg-info/PKG-INFO` & `pyfamsa-0.4.0/pyfamsa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfamsa
-Version: 0.3.2
+Version: 0.4.0
 Summary: Cython bindings and Python interface to FAMSA, an algorithm for ultra-scale multiple sequence alignments.
 Home-page: https://github.com/althonos/pyfamsa
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyfamsa.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyfamsa/issues
@@ -69,39 +69,42 @@
 
 PyFAMSA is a Python module that provides bindings to [FAMSA](https://github.com/refresh-bio/FAMSA)
 using [Cython](https://cython.org/). It implements a user-friendly, Pythonic
 interface to align protein sequences using different parameters and access
 results directly. It interacts with the FAMSA library interface, which has
 the following advantages:
 
-- **single dependency**: pyfamsa is distributed as a Python package, so you
+- **single dependency**: PyFAMSA is distributed as a Python package, so you
   can add it as a dependency to your project, and stop worrying about the
   FAMSA binary being present on the end-user machine.
 - **no intermediate files**: Everything happens in memory, in a Python object
   you control, so you don't have to invoke the FAMSA CLI using a
   sub-process and temporary files.
 - **friendly interface**: The different guide tree build methods and
   heuristics can be selected from the Python code with a simple keyword
   argument when configuring a new [`Aligner`](https://pyfamsa.readthedocs.io/en/stable/api/aligner.html#pyfamsa.Aligner).
+- **custom scoring matrices**: You can use any custom scoring matrix from 
+  the [`scoring-matrices`](https://pypi.org/project/scoring-matrices) library
+  in addition to the default MIQS to score the alignment. 
 
 ## 🔧 Installing
 
 PyFAMSA can be installed directly from [PyPI](https://pypi.org/project/pyfamsa/),
 which hosts some pre-built wheels for the x86-64 architecture (Linux/OSX)
 and the Aarch64 architecture (Linux only), as well as the code required to
 compile from source with Cython:
 ```console
 $ pip install pyfamsa
 ```
 
-<!-- Otherwise, pyfamsa is also available as a [Bioconda](https://bioconda.github.io/)
+Otherwise, PyFAMSA is also available as a [Bioconda](https://bioconda.github.io/)
 package:
 ```console
 $ conda install -c bioconda pyfamsa
-``` -->
+```
 
 Otherwise, have a look at the [Installation page](https://pyfamsa.readthedocs.io/en/stable/install.html) of the [online documentation](https://pyfamsa.readthedocs.io/)
 
 ## 💡 Example
 
 Let's create some sequences in memory, align them using the UPGMA method,
 (without any heuristic), and simply print the alignment on screen:
```

### Comparing `pyfamsa-0.3.2/pyfamsa.egg-info/SOURCES.txt` & `pyfamsa-0.4.0/pyfamsa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 pyfamsa/_famsa.pyx
 pyfamsa/_version.py
 pyfamsa/py.typed
 pyfamsa.egg-info/PKG-INFO
 pyfamsa.egg-info/SOURCES.txt
 pyfamsa.egg-info/dependency_links.txt
 pyfamsa.egg-info/not-zip-safe
+pyfamsa.egg-info/requires.txt
 pyfamsa.egg-info/top_level.txt
 pyfamsa/tests/__init__.py
 pyfamsa/tests/__main__.py
 pyfamsa/tests/fasta.py
 pyfamsa/tests/requirements.txt
 pyfamsa/tests/test_aligner.py
 pyfamsa/tests/test_doctest.py
```

### Comparing `pyfamsa-0.3.2/setup.cfg` & `pyfamsa-0.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,20 @@
 zip_safe = false
 packages = pyfamsa, pyfamsa.tests, pyfamsa.tests.data
 include_package_data = false
 python_requires = >=3.6
 setup_requires = 
 	setuptools >=46.4
 	cython ~=3.0
+	scoring-matrices ~=0.2
 	semantic-version ~=2.10
+install_requires = 
+	scoring-matrices ~=0.2
 tests_require = 
-	importlib-resources ; python_version < '3.7'
+	importlib-resources ; python_version < '3.9'
 
 [options.package_data]
 pyfamsa = py.typed, *.pyi
 pyfamsa.tests = requirements.txt
 pyfamsa.tests.data = *
 
 [coverage:run]
```

### Comparing `pyfamsa-0.3.2/setup.py` & `pyfamsa-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     elif platform.startswith("freebsd"):
         return "freebsd"
     return None
 
 
 # --- Utils ------------------------------------------------------------------
 
-_HEADER_PATTERN = re.compile("^@@ -(\d+),?(\d+)? \+(\d+),?(\d+)? @@$")
+_HEADER_PATTERN = re.compile(r"^@@ -(\d+),?(\d+)? \+(\d+),?(\d+)? @@$")
 
 
 def _eprint(*args, **kwargs):
     print(*args, **kwargs, file=sys.stderr)
 
 
 def _patch_osx_compiler(compiler, machine):
@@ -618,14 +618,16 @@
             if not self._simd_disabled["AVX2"] and self._check_avx2():
                 self._simd_supported["AVX2"] = True
                 self._simd_flags["AVX2"].extend(self._avx2_flags())
         elif self.target_cpu == "arm" or self.target_cpu == "aarch64":
             if not self._simd_disabled["NEON"] and self._check_neon():
                 self._simd_supported["NEON"] = True
                 self._simd_flags["NEON"].extend(self._neon_flags())
+                if self.target_cpu == "arm":
+                    self._simd_defines["NEON"].append(("__ARM_NEON", 1))
 
         # setup dispatcher of SIMD extensions
         for library in libraries:
             if self._simd_supported["AVX2"]:
                 library.define_macros.append(("SIMD", 2))
             elif self._simd_supported["AVX"]:
                 library.define_macros.append(("SIMD", 1))
```

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/LICENSE` & `pyfamsa-0.4.0/vendor/FAMSA/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/README.md` & `pyfamsa-0.4.0/vendor/FAMSA/README.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/atomic_wait` & `pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/atomic_wait`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/barrier` & `pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/barrier`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/latch` & `pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/latch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/atomic_wait/semaphore` & `pyfamsa-0.4.0/vendor/FAMSA/libs/atomic_wait/semaphore`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/COPYING` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/Makefile` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/Makefile`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/NEWS.md` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/NEWS.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/README.md` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/README.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/common_defs.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/adler32.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/lib_common.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/unaligned.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/utils.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/utils.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/libdeflate.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/libdeflate.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/benchmark.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/checksum.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/gzip.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/prog_util.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/prog_util.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_overread.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_util.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/test_util.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/scripts/detect.sh` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib` & `pyfamsa-0.4.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-aligned.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-override.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-override.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc-posix.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/alloc.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/alloc.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/arena.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/arena.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/bitmap.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/bitmap.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/bitmap.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/bitmap.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/heap.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/heap.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/init.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/init.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-override.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc-types.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/mimalloc.h` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/mimalloc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/options.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/options.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/os.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/os.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/page-queue.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/page-queue.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/page.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/page.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/random.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/random.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/region.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/region.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/segment-cache.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/segment-cache.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/segment.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/segment.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/static.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/static.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/libs/mimalloc/stats.c` & `pyfamsa-0.4.0/vendor/FAMSA/libs/mimalloc/stats.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/makefile` & `pyfamsa-0.4.0/vendor/FAMSA/makefile`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/defs.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/defs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/io_service.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/io_service.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/io_service.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/io_service.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/params.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/params.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/params.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/params.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/profile.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/profile.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/profile.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/profile.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/profile_par.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/profile_par.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/profile_seq.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/profile_seq.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/queues.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/queues.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/queues.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/queues.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/sequence.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/sequence.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/sequence.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/sequence.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/core/version.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/core/version.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/famsa.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/famsa.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_classic.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_classic.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_classic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/msa.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/msa.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/msa.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/msa.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/msa_refinement.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/msa_refinement.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/Chained.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/Chained.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/Clustering.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/Clustering.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/Clustering.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/Clustering.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/DistanceCalculator.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/DistanceCalculator.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/DistanceCalculator.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/FastTree.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/FastTree.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/FastTree.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/FastTree.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/GuideTree.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/GuideTree.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/GuideTree.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/GuideTree.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/MSTPrim.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/MSTPrim.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/MSTPrim.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/MSTPrim.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/NeighborJoining.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/NeighborJoining.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/NeighborJoining.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/NeighborJoining.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/NewickParser.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/NewickParser.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/NewickParser.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/NewickParser.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkage.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkage.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkage.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkage.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/SingleLinkageQueue.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/TreeDefs.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/TreeDefs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/UPGMA.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/UPGMA.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/tree/UPGMA.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/tree/UPGMA.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/array.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/array.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/conversion.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/conversion.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/cpuid.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/cpuid.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/deterministic_random.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/deterministic_random.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/log.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/log.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/log.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/log.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/memory_monotonic.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/memory_monotonic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/meta_oper.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/meta_oper.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/pooled_threads.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/pooled_threads.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/pooled_threads.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/pooled_threads.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/statistics.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/statistics.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/timer.cpp` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/timer.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/timer.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/timer.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.3.2/vendor/FAMSA/src/utils/utils.h` & `pyfamsa-0.4.0/vendor/FAMSA/src/utils/utils.h`

 * *Files identical despite different names*

