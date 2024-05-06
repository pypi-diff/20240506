# Comparing `tmp/camel-kenlm-2024.5.2.zip` & `tmp/camel-kenlm-2024.5.6.zip`

## zipinfo {}

```diff
@@ -1,330 +1,331 @@
-Zip file size: 555818 bytes, number of entries: 328
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/camel_kenlm.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/cmake/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/util/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/python/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/.github/
--rw-r--r--  2.0 unx      209 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/PKG-INFO
--rw-r--r--  2.0 unx     4792 b- defN 23-Apr-05 19:17 camel-kenlm-2024.5.2/CMakeLists.txt
--rw-r--r--  2.0 unx     1150 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/LICENSE
--rw-r--r--  2.0 unx     7637 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/COPYING.LESSER.3
--rw-r--r--  2.0 unx       59 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/pyproject.toml
--rw-r--r--  2.0 unx      220 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/MANIFEST.in
--rwxr-xr-x  2.0 unx       81 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/clean_query_only.sh
--rw-r--r--  2.0 unx     6359 b- defN 23-Mar-17 13:22 camel-kenlm-2024.5.2/README.md
--rw-r--r--  2.0 unx    26530 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/COPYING
--rw-r--r--  2.0 unx     4535 b- defN 24-May-02 18:04 camel-kenlm-2024.5.2/setup.py
--rw-r--r--  2.0 unx      281 b- defN 24-Jan-30 20:41 camel-kenlm-2024.5.2/.gitignore
--rw-r--r--  2.0 unx       38 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/setup.cfg
--rw-r--r--  2.0 unx    35147 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/COPYING.3
--rw-r--r--  2.0 unx    63537 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/Doxyfile
--rwxr-xr-x  2.0 unx     1154 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/compile_query_only.sh
--rw-r--r--  2.0 unx      696 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/BUILDING
--rw-r--r--  2.0 unx      209 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/camel_kenlm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     7780 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/camel_kenlm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/camel_kenlm.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-02 18:08 camel-kenlm-2024.5.2/camel_kenlm.egg-info/dependency_links.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/cmake/modules/
--rw-r--r--  2.0 unx     2821 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/cmake/KenLMFunctions.cmake
--rw-r--r--  2.0 unx      334 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/cmake/kenlmConfig.cmake.in
--rw-r--r--  2.0 unx     3185 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/cmake/modules/FindEigen3.cmake
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/util/stream/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/util/double-conversion/
--rw-r--r--  2.0 unx     2424 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file_stream.hh
--rw-r--r--  2.0 unx     1603 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/ersatz_progress.hh
--rw-r--r--  2.0 unx     6581 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/sized_iterator.hh
--rw-r--r--  2.0 unx     1778 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/string_stream_test.cc
--rw-r--r--  2.0 unx      705 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/pool.cc
--rw-r--r--  2.0 unx     5545 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/fixed_array.hh
--rw-r--r--  2.0 unx     1738 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/joint_sort_test.cc
--rw-r--r--  2.0 unx      729 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/float_to_string.cc
--rw-r--r--  2.0 unx    13507 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/mmap.cc
--rw-r--r--  2.0 unx     1887 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/multi_intersection_test.cc
--rw-r--r--  2.0 unx    10877 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file_piece.cc
--rw-r--r--  2.0 unx    13233 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/probing_hash_table.hh
--rw-r--r--  2.0 unx     1490 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/bit_packing_test.cc
--rw-r--r--  2.0 unx     4746 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file.hh
--rw-r--r--  2.0 unx     5480 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/string_piece.cc
--rw-r--r--  2.0 unx     3873 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/CMakeLists.txt
--rw-r--r--  2.0 unx     1176 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/bit_packing.cc
--rw-r--r--  2.0 unx    11091 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/usage.cc
--rw-r--r--  2.0 unx     1135 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/tokenize_piece_test.cc
--rw-r--r--  2.0 unx      461 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/parallel_read.hh
--rw-r--r--  2.0 unx     1039 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/string_stream.hh
--rw-r--r--  2.0 unx     9185 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/string_piece.hh
--rw-r--r--  2.0 unx    18350 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file.cc
--rw-r--r--  2.0 unx     3480 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/pcqueue.hh
--rw-r--r--  2.0 unx     5967 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/bit_packing.hh
--rw-r--r--  2.0 unx     1227 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/cat_compressed_main.cc
--rw-r--r--  2.0 unx     1546 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/parallel_read.cc
--rw-r--r--  2.0 unx      702 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/usage.hh
--rw-r--r--  2.0 unx     1367 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/ersatz_progress.cc
--rw-r--r--  2.0 unx     3526 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/proxy_iterator.hh
--rw-r--r--  2.0 unx     2956 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.2/util/pool.hh
--rw-r--r--  2.0 unx     2669 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/read_compressed_test.cc
--rw-r--r--  2.0 unx     6515 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file_piece.hh
--rw-r--r--  2.0 unx      609 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/float_to_string.hh
--rw-r--r--  2.0 unx     6780 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/mmap.hh
--rw-r--r--  2.0 unx     4890 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/tokenize_piece.hh
--rw-r--r--  2.0 unx      472 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/getopt.hh
--rw-r--r--  2.0 unx     5364 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/file_piece_test.cc
--rw-r--r--  2.0 unx    22498 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/integer_to_string.cc
--rw-r--r--  2.0 unx      559 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/sized_iterator_test.cc
--rw-r--r--  2.0 unx     3621 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/sorted_uniform_test.cc
--rw-r--r--  2.0 unx      751 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/spaces.cc
--rw-r--r--  2.0 unx     2034 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/read_compressed.hh
--rw-r--r--  2.0 unx    11788 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/probing_hash_table_benchmark_main.cc
--rw-r--r--  2.0 unx     4392 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/exception.hh
--rw-r--r--  2.0 unx      270 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/have.hh
--rw-r--r--  2.0 unx     3257 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/sorted_uniform.hh
--rw-r--r--  2.0 unx     4074 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/murmur_hash.cc
--rw-r--r--  2.0 unx     1959 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/integer_to_string_test.cc
--rw-r--r--  2.0 unx     1118 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/scoped.cc
--rw-r--r--  2.0 unx     4905 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/joint_sort.hh
--rw-r--r--  2.0 unx      167 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/spaces.hh
--rw-r--r--  2.0 unx    13086 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/read_compressed.cc
--rw-r--r--  2.0 unx     2765 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/exception.cc
--rw-r--r--  2.0 unx     1500 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.2/util/string_piece_hash.hh
--rw-r--r--  2.0 unx      616 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/murmur_hash.hh
--rw-r--r--  2.0 unx     3660 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/scoped.hh
--rw-r--r--  2.0 unx     3994 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/fake_ostream.hh
--rw-r--r--  2.0 unx      355 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/pcqueue_test.cc
--rw-r--r--  2.0 unx     3379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/multi_intersection.hh
--rw-r--r--  2.0 unx     2269 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/probing_hash_table_test.cc
--rw-r--r--  2.0 unx     1441 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/getopt.c
--rw-r--r--  2.0 unx     3825 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/thread_pool.hh
--rw-r--r--  2.0 unx     1636 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/integer_to_string.hh
--rw-r--r--  2.0 unx      823 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/io_test.cc
--rw-r--r--  2.0 unx     1237 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/CMakeLists.txt
--rw-r--r--  2.0 unx     3241 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/rewindable_stream.hh
--rw-r--r--  2.0 unx     1848 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/multi_progress.hh
--rw-r--r--  2.0 unx     3362 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/multi_stream.hh
--rw-r--r--  2.0 unx     3627 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/rewindable_stream.cc
--rw-r--r--  2.0 unx      899 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/rewindable_stream_test.cc
--rw-r--r--  2.0 unx      759 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/stream_test.cc
--rw-r--r--  2.0 unx     2363 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/multi_progress.cc
--rw-r--r--  2.0 unx     2420 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/block.hh
--rw-r--r--  2.0 unx     2436 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/io.cc
--rw-r--r--  2.0 unx     4367 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/chain.cc
--rw-r--r--  2.0 unx     1663 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/sort_test.cc
--rw-r--r--  2.0 unx     1606 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/config.hh
--rw-r--r--  2.0 unx      278 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/count_records.cc
--rw-r--r--  2.0 unx     1418 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/line_input.cc
--rw-r--r--  2.0 unx     1821 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/stream.hh
--rw-r--r--  2.0 unx      515 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/line_input.hh
--rw-r--r--  2.0 unx     1843 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/io.hh
--rw-r--r--  2.0 unx      732 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/typed_stream.hh
--rw-r--r--  2.0 unx     8996 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/chain.hh
--rw-r--r--  2.0 unx      300 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/count_records.hh
--rw-r--r--  2.0 unx    20450 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/stream/sort.hh
--rw-r--r--  2.0 unx    10848 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/string-to-double.h
--rw-r--r--  2.0 unx    15340 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/utils.h
--rw-r--r--  2.0 unx    24726 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/bignum.cc
--rw-r--r--  2.0 unx     2770 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.h
--rw-r--r--  2.0 unx    27857 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/string-to-double.cc
--rw-r--r--  2.0 unx     1042 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/CMakeLists.txt
--rw-r--r--  2.0 unx     1527 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/double-conversion/LICENSE
--rw-r--r--  2.0 unx     4300 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.h
--rw-r--r--  2.0 unx    15352 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.cc
--rw-r--r--  2.0 unx    22349 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/double-to-string.h
--rw-r--r--  2.0 unx     3038 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/strtod.h
--rw-r--r--  2.0 unx     5030 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/diy-fp.h
--rw-r--r--  2.0 unx    23469 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/strtod.cc
--rw-r--r--  2.0 unx     3021 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/cached-powers.h
--rw-r--r--  2.0 unx     1804 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/double-conversion.h
--rw-r--r--  2.0 unx    31645 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.cc
--rw-r--r--  2.0 unx    15851 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/double-to-string.cc
--rw-r--r--  2.0 unx     9913 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/cached-powers.cc
--rw-r--r--  2.0 unx    15223 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/ieee.h
--rw-r--r--  2.0 unx     5891 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/bignum.h
--rw-r--r--  2.0 unx     4064 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.h
--rw-r--r--  2.0 unx    27617 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.cc
--rw-r--r--  2.0 unx   450422 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.2/python/kenlm.cpp
--rw-r--r--  2.0 unx      988 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/python/CMakeLists.txt
--rw-r--r--  2.0 unx      906 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/python/score_sentence.cc
--rw-r--r--  2.0 unx      325 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/python/score_sentence.hh
--rwxr-xr-x  2.0 unx     1427 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/python/example.py
--rw-r--r--  2.0 unx     1957 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/python/_kenlm.pxd
--rw-r--r--  2.0 unx     9323 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/python/kenlm.pyx
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/wrappers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/common/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/interpolate/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/filter/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/builder/
--rw-r--r--  2.0 unx    10982 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/trie_sort.cc
--rw-r--r--  2.0 unx     3016 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/read_arpa.hh
--rw-r--r--  2.0 unx      637 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/lm_exception.cc
--rw-r--r--  2.0 unx     2045 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/value_build.cc
--rw-r--r--  2.0 unx    12931 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/binary_format.cc
--rw-r--r--  2.0 unx     4348 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/bhiksha.hh
--rw-r--r--  2.0 unx     2097 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/lm/CMakeLists.txt
--rw-r--r--  2.0 unx     7051 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/model.hh
--rw-r--r--  2.0 unx     5639 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/trie.cc
--rw-r--r--  2.0 unx     3710 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/bhiksha.cc
--rw-r--r--  2.0 unx     3440 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/state.hh
--rw-r--r--  2.0 unx     3563 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/trie.hh
--rw-r--r--  2.0 unx     1248 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/return.hh
--rw-r--r--  2.0 unx    16256 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/model.cc
--rw-r--r--  2.0 unx     4675 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/query_main.cc
--rw-r--r--  2.0 unx     1379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/blank.hh
--rw-r--r--  2.0 unx     2795 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/trie_sort.hh
--rw-r--r--  2.0 unx      358 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/weights.hh
--rw-r--r--  2.0 unx    12402 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/left_test.cc
--rw-r--r--  2.0 unx      644 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/max_order.hh
--rw-r--r--  2.0 unx     1057 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/lm_exception.hh
--rw-r--r--  2.0 unx     2694 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/test_nounk.arpa
--rw-r--r--  2.0 unx     3935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/value.hh
--rw-r--r--  2.0 unx     7543 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/read_arpa.cc
--rw-r--r--  2.0 unx     3498 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/binary_format.hh
--rw-r--r--  2.0 unx     6003 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/partial.hh
--rw-r--r--  2.0 unx     2568 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/value_build.hh
--rw-r--r--  2.0 unx    12060 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/search_hashed.cc
--rw-r--r--  2.0 unx     7749 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/quantize.hh
--rw-r--r--  2.0 unx     8154 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/build_binary_main.cc
--rw-r--r--  2.0 unx     7174 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/left.hh
--rw-r--r--  2.0 unx     8680 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/vocab.hh
--rw-r--r--  2.0 unx     4906 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/search_trie.hh
--rw-r--r--  2.0 unx     3913 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/config.hh
--rw-r--r--  2.0 unx     2780 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/test.arpa
--rw-r--r--  2.0 unx      293 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/word_index.hh
--rw-r--r--  2.0 unx      798 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/model_type.hh
--rw-r--r--  2.0 unx     2594 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/sizes.cc
--rw-r--r--  2.0 unx     6672 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/partial_test.cc
--rw-r--r--  2.0 unx      380 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/virtual_interface.cc
--rw-r--r--  2.0 unx      722 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/enumerate_vocab.hh
--rw-r--r--  2.0 unx     2544 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/facade.hh
--rw-r--r--  2.0 unx    14544 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/model_test.cc
--rw-r--r--  2.0 unx      374 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/sizes.hh
--rw-r--r--  2.0 unx     9039 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/kenlm_benchmark_main.cc
--rw-r--r--  2.0 unx     5668 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/virtual_interface.hh
--rw-r--r--  2.0 unx     1068 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/fragment_main.cc
--rw-r--r--  2.0 unx     5935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/search_hashed.hh
--rw-r--r--  2.0 unx     3743 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/quantize.cc
--rw-r--r--  2.0 unx    11083 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/vocab.cc
--rw-r--r--  2.0 unx     3534 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/ngram_query.hh
--rw-r--r--  2.0 unx    23394 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/search_trie.cc
--rw-r--r--  2.0 unx      675 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/config.cc
--rw-r--r--  2.0 unx     4261 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/wrappers/nplm.cc
--rw-r--r--  2.0 unx     1975 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/wrappers/nplm.hh
--rw-r--r--  2.0 unx      176 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/wrappers/README
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/common/test_data/
--rw-r--r--  2.0 unx     2366 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/joint_order.hh
--rw-r--r--  2.0 unx      398 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/renumber.cc
--rw-r--r--  2.0 unx     2155 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/model_buffer.hh
--rw-r--r--  2.0 unx      302 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/size_option.hh
--rw-r--r--  2.0 unx     1483 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/print.hh
--rw-r--r--  2.0 unx      889 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/CMakeLists.txt
--rw-r--r--  2.0 unx      550 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/special.hh
--rw-r--r--  2.0 unx     6078 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/compare.hh
--rw-r--r--  2.0 unx      755 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/renumber.hh
--rw-r--r--  2.0 unx     5186 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/model_buffer.cc
--rw-r--r--  2.0 unx      562 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/size_option.cc
--rw-r--r--  2.0 unx     1890 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/print.cc
--rw-r--r--  2.0 unx     2112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/ngram.hh
--rw-r--r--  2.0 unx     1872 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/ngram_stream.hh
--rw-r--r--  2.0 unx     1713 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/model_buffer_test.cc
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/
--rw-r--r--  2.0 unx      475 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/toy0.arpa
--rw-r--r--  2.0 unx      470 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/toy1.arpa
--rwxr-xr-x  2.0 unx      270 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/generate.sh
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.2
--rw-r--r--  2.0 unx      120 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.3
--rw-r--r--  2.0 unx       60 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.1
--rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.kenlm_intermediate
--rw-r--r--  2.0 unx       72 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.1
--rw-r--r--  2.0 unx       21 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.vocab
--rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.kenlm_intermediate
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.2
--rw-r--r--  2.0 unx      140 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.3
--rw-r--r--  2.0 unx       19 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.vocab
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.2
--rw-r--r--  2.0 unx      120 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.3
--rw-r--r--  2.0 unx       60 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.1
--rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.kenlm_intermediate
--rw-r--r--  2.0 unx       72 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.1
--rw-r--r--  2.0 unx       21 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.vocab
--rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.kenlm_intermediate
--rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.2
--rw-r--r--  2.0 unx      140 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.3
--rw-r--r--  2.0 unx       19 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.vocab
--rw-r--r--  2.0 unx     3222 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding_test.cc
--rw-r--r--  2.0 unx     1347 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/universal_vocab.hh
--rw-r--r--  2.0 unx     3586 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.cc
--rw-r--r--  2.0 unx      552 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/pipeline.hh
--rw-r--r--  2.0 unx     1952 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.cc
--rw-r--r--  2.0 unx     1774 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/CMakeLists.txt
--rw-r--r--  2.0 unx      512 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_matrix.hh
--rw-r--r--  2.0 unx     4571 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_instances_test.cc
--rw-r--r--  2.0 unx     1100 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/split_worker.hh
--rw-r--r--  2.0 unx     1366 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_weights.cc
--rw-r--r--  2.0 unx     5296 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/interpolate_main.cc
--rw-r--r--  2.0 unx      693 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/interpolate_info.hh
--rw-r--r--  2.0 unx      446 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_weights.hh
--rw-r--r--  2.0 unx     1235 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/split_worker.cc
--rw-r--r--  2.0 unx      572 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.hh
--rw-r--r--  2.0 unx     2758 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/normalize_test.cc
--rw-r--r--  2.0 unx      342 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/universal_vocab.cc
--rw-r--r--  2.0 unx     7645 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/pipeline.cc
--rw-r--r--  2.0 unx      913 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.hh
--rw-r--r--  2.0 unx    13813 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/normalize.cc
--rw-r--r--  2.0 unx      590 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.hh
--rw-r--r--  2.0 unx    10010 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.cc
--rw-r--r--  2.0 unx      737 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/backoff_matrix.hh
--rw-r--r--  2.0 unx     2530 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.hh
--rw-r--r--  2.0 unx    19605 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_instances.cc
--rw-r--r--  2.0 unx     4904 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification_test.cc
--rw-r--r--  2.0 unx     7430 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/streaming_example_main.cc
--rw-r--r--  2.0 unx     5950 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.cc
--rw-r--r--  2.0 unx     1101 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/normalize.hh
--rw-r--r--  2.0 unx     3969 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives_test.cc
--rw-r--r--  2.0 unx     3385 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.hh
--rw-r--r--  2.0 unx     1086 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.cc
--rw-r--r--  2.0 unx     5306 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/merge_vocab_test.cc
--rw-r--r--  2.0 unx     2956 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/interpolate/tune_instances.hh
--rw-r--r--  2.0 unx     1327 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/CMakeLists.txt
--rw-r--r--  2.0 unx     5027 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/phrase_table_vocab_main.cc
--rw-r--r--  2.0 unx     2458 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/count_io.hh
--rw-r--r--  2.0 unx     9352 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/filter_main.cc
--rw-r--r--  2.0 unx     4205 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/thread.hh
--rw-r--r--  2.0 unx     4123 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/vocab.hh
--rw-r--r--  2.0 unx     1935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/arpa_io.cc
--rw-r--r--  2.0 unx     8212 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/phrase.cc
--rw-r--r--  2.0 unx     1797 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/wrapper.hh
--rw-r--r--  2.0 unx     5778 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/phrase.hh
--rw-r--r--  2.0 unx     2816 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/arpa_io.hh
--rw-r--r--  2.0 unx     7379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/format.hh
--rw-r--r--  2.0 unx     1209 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/filter/vocab.cc
--rw-r--r--  2.0 unx     1136 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/interpolate.hh
--rw-r--r--  2.0 unx      439 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/discount.hh
--rw-r--r--  2.0 unx     2572 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/pipeline.hh
--rw-r--r--  2.0 unx    12607 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/adjust_counts.cc
--rw-r--r--  2.0 unx    11967 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/lmplz_main.cc
--rw-r--r--  2.0 unx     1625 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/output.cc
--rw-r--r--  2.0 unx     1897 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/CMakeLists.txt
--rw-r--r--  2.0 unx     1452 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/initial_probabilities.hh
--rw-r--r--  2.0 unx     1051 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/payload.hh
--rw-r--r--  2.0 unx     2529 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/output.hh
--rw-r--r--  2.0 unx      899 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/combine_counts.hh
--rw-r--r--  2.0 unx     2258 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/adjust_counts.hh
--rw-r--r--  2.0 unx    10698 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/initial_probabilities.cc
--rw-r--r--  2.0 unx      715 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/header_info.hh
--rw-r--r--  2.0 unx     6044 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/interpolate.cc
--rw-r--r--  2.0 unx     2411 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/debug_print.hh
--rw-r--r--  2.0 unx     3992 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/count_ngrams_main.cc
--rw-r--r--  2.0 unx    17887 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/pipeline.cc
--rw-r--r--  2.0 unx      152 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/TODO
--rw-r--r--  2.0 unx      826 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/README.md
--rw-r--r--  2.0 unx     9550 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/corpus_count.cc
--rw-r--r--  2.0 unx      293 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/hash_gamma.hh
--rw-r--r--  2.0 unx     2820 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/corpus_count_test.cc
--rw-r--r--  2.0 unx     1869 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/dump_counts_main.cc
--rw-r--r--  2.0 unx     3509 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/adjust_counts_test.cc
--rw-r--r--  2.0 unx     1701 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/lm/builder/corpus_count.hh
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 18:08 camel-kenlm-2024.5.2/.github/workflows/
--rw-r--r--  2.0 unx      471 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/.github/workflows/windows.yml
--rw-r--r--  2.0 unx      619 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.2/.github/workflows/ubuntu.yml
--rw-r--r--  2.0 unx      542 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.2/.github/workflows/mac.yml
-328 files, 1834275 bytes uncompressed, 501594 bytes compressed:  72.7%
+Zip file size: 556433 bytes, number of entries: 329
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/camel_kenlm.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/cmake/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/util/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/python/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/.github/
+-rw-r--r--  2.0 unx      209 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/PKG-INFO
+-rw-r--r--  2.0 unx     4792 b- defN 23-Apr-05 19:17 camel-kenlm-2024.5.6/CMakeLists.txt
+-rw-r--r--  2.0 unx     1150 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/LICENSE
+-rw-r--r--  2.0 unx     7637 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/COPYING.LESSER.3
+-rw-r--r--  2.0 unx       59 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/pyproject.toml
+-rw-r--r--  2.0 unx      220 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/MANIFEST.in
+-rwxr-xr-x  2.0 unx       81 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/clean_query_only.sh
+-rw-r--r--  2.0 unx     6359 b- defN 23-Mar-17 13:22 camel-kenlm-2024.5.6/README.md
+-rw-r--r--  2.0 unx    26530 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/COPYING
+-rw-r--r--  2.0 unx     4562 b- defN 24-May-06 07:46 camel-kenlm-2024.5.6/setup.py
+-rw-r--r--  2.0 unx      281 b- defN 24-Jan-30 20:41 camel-kenlm-2024.5.6/.gitignore
+-rw-r--r--  2.0 unx       38 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/setup.cfg
+-rw-r--r--  2.0 unx    35147 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/COPYING.3
+-rw-r--r--  2.0 unx    63537 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/Doxyfile
+-rwxr-xr-x  2.0 unx     1154 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/compile_query_only.sh
+-rw-r--r--  2.0 unx      696 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/BUILDING
+-rw-r--r--  2.0 unx      209 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/camel_kenlm.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     7809 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/camel_kenlm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/camel_kenlm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-06 07:48 camel-kenlm-2024.5.6/camel_kenlm.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/cmake/modules/
+-rw-r--r--  2.0 unx     2821 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/cmake/KenLMFunctions.cmake
+-rw-r--r--  2.0 unx      334 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/cmake/kenlmConfig.cmake.in
+-rw-r--r--  2.0 unx     3185 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/cmake/modules/FindEigen3.cmake
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/util/stream/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/util/double-conversion/
+-rw-r--r--  2.0 unx     2424 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file_stream.hh
+-rw-r--r--  2.0 unx     1603 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/ersatz_progress.hh
+-rw-r--r--  2.0 unx     6581 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/sized_iterator.hh
+-rw-r--r--  2.0 unx     1778 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/string_stream_test.cc
+-rw-r--r--  2.0 unx      705 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/pool.cc
+-rw-r--r--  2.0 unx     5545 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/fixed_array.hh
+-rw-r--r--  2.0 unx     1738 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/joint_sort_test.cc
+-rw-r--r--  2.0 unx      729 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/float_to_string.cc
+-rw-r--r--  2.0 unx    13507 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/mmap.cc
+-rw-r--r--  2.0 unx     1887 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/multi_intersection_test.cc
+-rw-r--r--  2.0 unx    10877 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file_piece.cc
+-rw-r--r--  2.0 unx    13233 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/probing_hash_table.hh
+-rw-r--r--  2.0 unx     1490 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/bit_packing_test.cc
+-rw-r--r--  2.0 unx     4746 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file.hh
+-rw-r--r--  2.0 unx     5480 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/string_piece.cc
+-rw-r--r--  2.0 unx     3873 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/CMakeLists.txt
+-rw-r--r--  2.0 unx     1176 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/bit_packing.cc
+-rw-r--r--  2.0 unx    11091 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/usage.cc
+-rw-r--r--  2.0 unx     1135 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/tokenize_piece_test.cc
+-rw-r--r--  2.0 unx      461 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/parallel_read.hh
+-rw-r--r--  2.0 unx     1039 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/string_stream.hh
+-rw-r--r--  2.0 unx     9185 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/string_piece.hh
+-rw-r--r--  2.0 unx    18350 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file.cc
+-rw-r--r--  2.0 unx     3480 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/pcqueue.hh
+-rw-r--r--  2.0 unx     5967 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/bit_packing.hh
+-rw-r--r--  2.0 unx     1227 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/cat_compressed_main.cc
+-rw-r--r--  2.0 unx     1546 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/parallel_read.cc
+-rw-r--r--  2.0 unx      702 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/usage.hh
+-rw-r--r--  2.0 unx     1367 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/ersatz_progress.cc
+-rw-r--r--  2.0 unx     3526 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/proxy_iterator.hh
+-rw-r--r--  2.0 unx     2956 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.6/util/pool.hh
+-rw-r--r--  2.0 unx     2669 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/read_compressed_test.cc
+-rw-r--r--  2.0 unx     6515 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file_piece.hh
+-rw-r--r--  2.0 unx      609 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/float_to_string.hh
+-rw-r--r--  2.0 unx     6780 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/mmap.hh
+-rw-r--r--  2.0 unx     4890 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/tokenize_piece.hh
+-rw-r--r--  2.0 unx      472 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/getopt.hh
+-rw-r--r--  2.0 unx     5364 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/file_piece_test.cc
+-rw-r--r--  2.0 unx    22498 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/integer_to_string.cc
+-rw-r--r--  2.0 unx      559 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/sized_iterator_test.cc
+-rw-r--r--  2.0 unx     3621 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/sorted_uniform_test.cc
+-rw-r--r--  2.0 unx      751 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/spaces.cc
+-rw-r--r--  2.0 unx     2034 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/read_compressed.hh
+-rw-r--r--  2.0 unx    11788 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/probing_hash_table_benchmark_main.cc
+-rw-r--r--  2.0 unx     4392 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/exception.hh
+-rw-r--r--  2.0 unx      270 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/have.hh
+-rw-r--r--  2.0 unx     3257 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/sorted_uniform.hh
+-rw-r--r--  2.0 unx     4074 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/murmur_hash.cc
+-rw-r--r--  2.0 unx     1959 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/integer_to_string_test.cc
+-rw-r--r--  2.0 unx     1118 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/scoped.cc
+-rw-r--r--  2.0 unx     4905 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/joint_sort.hh
+-rw-r--r--  2.0 unx      167 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/spaces.hh
+-rw-r--r--  2.0 unx    13086 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/read_compressed.cc
+-rw-r--r--  2.0 unx     2765 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/exception.cc
+-rw-r--r--  2.0 unx     1500 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.6/util/string_piece_hash.hh
+-rw-r--r--  2.0 unx      616 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/murmur_hash.hh
+-rw-r--r--  2.0 unx     3660 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/scoped.hh
+-rw-r--r--  2.0 unx     3994 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/fake_ostream.hh
+-rw-r--r--  2.0 unx      355 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/pcqueue_test.cc
+-rw-r--r--  2.0 unx     3379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/multi_intersection.hh
+-rw-r--r--  2.0 unx     2269 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/probing_hash_table_test.cc
+-rw-r--r--  2.0 unx     1441 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/getopt.c
+-rw-r--r--  2.0 unx     3825 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/thread_pool.hh
+-rw-r--r--  2.0 unx     1636 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/integer_to_string.hh
+-rw-r--r--  2.0 unx      823 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/io_test.cc
+-rw-r--r--  2.0 unx     1237 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/CMakeLists.txt
+-rw-r--r--  2.0 unx     3241 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/rewindable_stream.hh
+-rw-r--r--  2.0 unx     1848 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/multi_progress.hh
+-rw-r--r--  2.0 unx     3362 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/multi_stream.hh
+-rw-r--r--  2.0 unx     3627 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/rewindable_stream.cc
+-rw-r--r--  2.0 unx      899 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/rewindable_stream_test.cc
+-rw-r--r--  2.0 unx      759 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/stream_test.cc
+-rw-r--r--  2.0 unx     2363 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/multi_progress.cc
+-rw-r--r--  2.0 unx     2420 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/block.hh
+-rw-r--r--  2.0 unx     2436 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/io.cc
+-rw-r--r--  2.0 unx     4367 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/chain.cc
+-rw-r--r--  2.0 unx     1663 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/sort_test.cc
+-rw-r--r--  2.0 unx     1606 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/config.hh
+-rw-r--r--  2.0 unx      278 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/count_records.cc
+-rw-r--r--  2.0 unx     1418 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/line_input.cc
+-rw-r--r--  2.0 unx     1821 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/stream.hh
+-rw-r--r--  2.0 unx      515 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/line_input.hh
+-rw-r--r--  2.0 unx     1843 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/io.hh
+-rw-r--r--  2.0 unx      732 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/typed_stream.hh
+-rw-r--r--  2.0 unx     8996 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/chain.hh
+-rw-r--r--  2.0 unx      300 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/count_records.hh
+-rw-r--r--  2.0 unx    20450 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/stream/sort.hh
+-rw-r--r--  2.0 unx    10848 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/string-to-double.h
+-rw-r--r--  2.0 unx    15340 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/utils.h
+-rw-r--r--  2.0 unx    24726 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/bignum.cc
+-rw-r--r--  2.0 unx     2770 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.h
+-rw-r--r--  2.0 unx    27857 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/string-to-double.cc
+-rw-r--r--  2.0 unx     1042 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/CMakeLists.txt
+-rw-r--r--  2.0 unx     1527 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/double-conversion/LICENSE
+-rw-r--r--  2.0 unx     4300 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.h
+-rw-r--r--  2.0 unx    15352 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.cc
+-rw-r--r--  2.0 unx    22349 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/double-to-string.h
+-rw-r--r--  2.0 unx     3038 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/strtod.h
+-rw-r--r--  2.0 unx     5030 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/diy-fp.h
+-rw-r--r--  2.0 unx    23469 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/strtod.cc
+-rw-r--r--  2.0 unx     3021 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/cached-powers.h
+-rw-r--r--  2.0 unx     1804 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/double-conversion.h
+-rw-r--r--  2.0 unx    31645 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.cc
+-rw-r--r--  2.0 unx    15851 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/double-to-string.cc
+-rw-r--r--  2.0 unx     9913 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/cached-powers.cc
+-rw-r--r--  2.0 unx    15223 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/ieee.h
+-rw-r--r--  2.0 unx     5891 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/bignum.h
+-rw-r--r--  2.0 unx     4064 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.h
+-rw-r--r--  2.0 unx    27617 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.cc
+-rw-r--r--  2.0 unx   450422 b- defN 24-Jan-30 20:43 camel-kenlm-2024.5.6/python/kenlm.cpp
+-rw-r--r--  2.0 unx      988 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/python/CMakeLists.txt
+-rw-r--r--  2.0 unx      906 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/python/score_sentence.cc
+-rw-r--r--  2.0 unx      325 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/python/score_sentence.hh
+-rw-r--r--  2.0 unx     1177 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/python/BuildStandalone.cmake
+-rwxr-xr-x  2.0 unx     1427 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/python/example.py
+-rw-r--r--  2.0 unx     1957 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/python/_kenlm.pxd
+-rw-r--r--  2.0 unx     9323 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/python/kenlm.pyx
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/wrappers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/common/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/interpolate/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/filter/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/builder/
+-rw-r--r--  2.0 unx    10982 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/trie_sort.cc
+-rw-r--r--  2.0 unx     3016 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/read_arpa.hh
+-rw-r--r--  2.0 unx      637 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/lm_exception.cc
+-rw-r--r--  2.0 unx     2045 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/value_build.cc
+-rw-r--r--  2.0 unx    12931 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/binary_format.cc
+-rw-r--r--  2.0 unx     4348 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/bhiksha.hh
+-rw-r--r--  2.0 unx     2097 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/lm/CMakeLists.txt
+-rw-r--r--  2.0 unx     7051 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/model.hh
+-rw-r--r--  2.0 unx     5639 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/trie.cc
+-rw-r--r--  2.0 unx     3710 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/bhiksha.cc
+-rw-r--r--  2.0 unx     3440 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/state.hh
+-rw-r--r--  2.0 unx     3563 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/trie.hh
+-rw-r--r--  2.0 unx     1248 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/return.hh
+-rw-r--r--  2.0 unx    16256 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/model.cc
+-rw-r--r--  2.0 unx     4675 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/query_main.cc
+-rw-r--r--  2.0 unx     1379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/blank.hh
+-rw-r--r--  2.0 unx     2795 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/trie_sort.hh
+-rw-r--r--  2.0 unx      358 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/weights.hh
+-rw-r--r--  2.0 unx    12402 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/left_test.cc
+-rw-r--r--  2.0 unx      644 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/max_order.hh
+-rw-r--r--  2.0 unx     1057 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/lm_exception.hh
+-rw-r--r--  2.0 unx     2694 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/test_nounk.arpa
+-rw-r--r--  2.0 unx     3935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/value.hh
+-rw-r--r--  2.0 unx     7543 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/read_arpa.cc
+-rw-r--r--  2.0 unx     3498 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/binary_format.hh
+-rw-r--r--  2.0 unx     6003 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/partial.hh
+-rw-r--r--  2.0 unx     2568 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/value_build.hh
+-rw-r--r--  2.0 unx    12060 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/search_hashed.cc
+-rw-r--r--  2.0 unx     7749 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/quantize.hh
+-rw-r--r--  2.0 unx     8154 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/build_binary_main.cc
+-rw-r--r--  2.0 unx     7174 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/left.hh
+-rw-r--r--  2.0 unx     8680 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/vocab.hh
+-rw-r--r--  2.0 unx     4906 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/search_trie.hh
+-rw-r--r--  2.0 unx     3913 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/config.hh
+-rw-r--r--  2.0 unx     2780 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/test.arpa
+-rw-r--r--  2.0 unx      293 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/word_index.hh
+-rw-r--r--  2.0 unx      798 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/model_type.hh
+-rw-r--r--  2.0 unx     2594 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/sizes.cc
+-rw-r--r--  2.0 unx     6672 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/partial_test.cc
+-rw-r--r--  2.0 unx      380 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/virtual_interface.cc
+-rw-r--r--  2.0 unx      722 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/enumerate_vocab.hh
+-rw-r--r--  2.0 unx     2544 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/facade.hh
+-rw-r--r--  2.0 unx    14544 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/model_test.cc
+-rw-r--r--  2.0 unx      374 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/sizes.hh
+-rw-r--r--  2.0 unx     9039 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/kenlm_benchmark_main.cc
+-rw-r--r--  2.0 unx     5668 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/virtual_interface.hh
+-rw-r--r--  2.0 unx     1068 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/fragment_main.cc
+-rw-r--r--  2.0 unx     5935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/search_hashed.hh
+-rw-r--r--  2.0 unx     3743 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/quantize.cc
+-rw-r--r--  2.0 unx    11083 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/vocab.cc
+-rw-r--r--  2.0 unx     3534 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/ngram_query.hh
+-rw-r--r--  2.0 unx    23394 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/search_trie.cc
+-rw-r--r--  2.0 unx      675 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/config.cc
+-rw-r--r--  2.0 unx     4261 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/wrappers/nplm.cc
+-rw-r--r--  2.0 unx     1975 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/wrappers/nplm.hh
+-rw-r--r--  2.0 unx      176 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/wrappers/README
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/common/test_data/
+-rw-r--r--  2.0 unx     2366 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/joint_order.hh
+-rw-r--r--  2.0 unx      398 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/renumber.cc
+-rw-r--r--  2.0 unx     2155 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/model_buffer.hh
+-rw-r--r--  2.0 unx      302 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/size_option.hh
+-rw-r--r--  2.0 unx     1483 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/print.hh
+-rw-r--r--  2.0 unx      889 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/CMakeLists.txt
+-rw-r--r--  2.0 unx      550 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/special.hh
+-rw-r--r--  2.0 unx     6078 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/compare.hh
+-rw-r--r--  2.0 unx      755 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/renumber.hh
+-rw-r--r--  2.0 unx     5186 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/model_buffer.cc
+-rw-r--r--  2.0 unx      562 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/size_option.cc
+-rw-r--r--  2.0 unx     1890 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/print.cc
+-rw-r--r--  2.0 unx     2112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/ngram.hh
+-rw-r--r--  2.0 unx     1872 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/ngram_stream.hh
+-rw-r--r--  2.0 unx     1713 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/model_buffer_test.cc
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/
+-rw-r--r--  2.0 unx      475 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/toy0.arpa
+-rw-r--r--  2.0 unx      470 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/toy1.arpa
+-rwxr-xr-x  2.0 unx      270 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/generate.sh
+-rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.2
+-rw-r--r--  2.0 unx      120 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.3
+-rw-r--r--  2.0 unx       60 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.1
+-rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.kenlm_intermediate
+-rw-r--r--  2.0 unx       72 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.1
+-rw-r--r--  2.0 unx       21 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.vocab
+-rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.kenlm_intermediate
+-rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.2
+-rw-r--r--  2.0 unx      140 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.3
+-rw-r--r--  2.0 unx       19 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.vocab
+-rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.2
+-rw-r--r--  2.0 unx      120 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.3
+-rw-r--r--  2.0 unx       60 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.1
+-rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.kenlm_intermediate
+-rw-r--r--  2.0 unx       72 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.1
+-rw-r--r--  2.0 unx       21 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.vocab
+-rw-r--r--  2.0 unx       55 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.kenlm_intermediate
+-rw-r--r--  2.0 unx      112 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.2
+-rw-r--r--  2.0 unx      140 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.3
+-rw-r--r--  2.0 unx       19 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.vocab
+-rw-r--r--  2.0 unx     3222 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding_test.cc
+-rw-r--r--  2.0 unx     1347 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/universal_vocab.hh
+-rw-r--r--  2.0 unx     3586 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.cc
+-rw-r--r--  2.0 unx      552 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/pipeline.hh
+-rw-r--r--  2.0 unx     1952 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.cc
+-rw-r--r--  2.0 unx     1774 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/CMakeLists.txt
+-rw-r--r--  2.0 unx      512 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_matrix.hh
+-rw-r--r--  2.0 unx     4571 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_instances_test.cc
+-rw-r--r--  2.0 unx     1100 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/split_worker.hh
+-rw-r--r--  2.0 unx     1366 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_weights.cc
+-rw-r--r--  2.0 unx     5296 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/interpolate_main.cc
+-rw-r--r--  2.0 unx      693 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/interpolate_info.hh
+-rw-r--r--  2.0 unx      446 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_weights.hh
+-rw-r--r--  2.0 unx     1235 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/split_worker.cc
+-rw-r--r--  2.0 unx      572 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.hh
+-rw-r--r--  2.0 unx     2758 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/normalize_test.cc
+-rw-r--r--  2.0 unx      342 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/universal_vocab.cc
+-rw-r--r--  2.0 unx     7645 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/pipeline.cc
+-rw-r--r--  2.0 unx      913 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.hh
+-rw-r--r--  2.0 unx    13813 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/normalize.cc
+-rw-r--r--  2.0 unx      590 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.hh
+-rw-r--r--  2.0 unx    10010 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.cc
+-rw-r--r--  2.0 unx      737 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/backoff_matrix.hh
+-rw-r--r--  2.0 unx     2530 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.hh
+-rw-r--r--  2.0 unx    19605 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_instances.cc
+-rw-r--r--  2.0 unx     4904 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification_test.cc
+-rw-r--r--  2.0 unx     7430 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/streaming_example_main.cc
+-rw-r--r--  2.0 unx     5950 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.cc
+-rw-r--r--  2.0 unx     1101 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/normalize.hh
+-rw-r--r--  2.0 unx     3969 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives_test.cc
+-rw-r--r--  2.0 unx     3385 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.hh
+-rw-r--r--  2.0 unx     1086 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.cc
+-rw-r--r--  2.0 unx     5306 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/merge_vocab_test.cc
+-rw-r--r--  2.0 unx     2956 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/interpolate/tune_instances.hh
+-rw-r--r--  2.0 unx     1327 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/CMakeLists.txt
+-rw-r--r--  2.0 unx     5027 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/phrase_table_vocab_main.cc
+-rw-r--r--  2.0 unx     2458 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/count_io.hh
+-rw-r--r--  2.0 unx     9352 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/filter_main.cc
+-rw-r--r--  2.0 unx     4205 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/thread.hh
+-rw-r--r--  2.0 unx     4123 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/vocab.hh
+-rw-r--r--  2.0 unx     1935 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/arpa_io.cc
+-rw-r--r--  2.0 unx     8212 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/phrase.cc
+-rw-r--r--  2.0 unx     1797 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/wrapper.hh
+-rw-r--r--  2.0 unx     5778 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/phrase.hh
+-rw-r--r--  2.0 unx     2816 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/arpa_io.hh
+-rw-r--r--  2.0 unx     7379 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/format.hh
+-rw-r--r--  2.0 unx     1209 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/filter/vocab.cc
+-rw-r--r--  2.0 unx     1136 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/interpolate.hh
+-rw-r--r--  2.0 unx      439 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/discount.hh
+-rw-r--r--  2.0 unx     2572 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/pipeline.hh
+-rw-r--r--  2.0 unx    12607 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/adjust_counts.cc
+-rw-r--r--  2.0 unx    11967 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/lmplz_main.cc
+-rw-r--r--  2.0 unx     1625 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/output.cc
+-rw-r--r--  2.0 unx     1897 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/CMakeLists.txt
+-rw-r--r--  2.0 unx     1452 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/initial_probabilities.hh
+-rw-r--r--  2.0 unx     1051 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/payload.hh
+-rw-r--r--  2.0 unx     2529 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/output.hh
+-rw-r--r--  2.0 unx      899 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/combine_counts.hh
+-rw-r--r--  2.0 unx     2258 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/adjust_counts.hh
+-rw-r--r--  2.0 unx    10698 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/initial_probabilities.cc
+-rw-r--r--  2.0 unx      715 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/header_info.hh
+-rw-r--r--  2.0 unx     6044 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/interpolate.cc
+-rw-r--r--  2.0 unx     2411 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/debug_print.hh
+-rw-r--r--  2.0 unx     3992 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/count_ngrams_main.cc
+-rw-r--r--  2.0 unx    17887 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/pipeline.cc
+-rw-r--r--  2.0 unx      152 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/TODO
+-rw-r--r--  2.0 unx      826 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/README.md
+-rw-r--r--  2.0 unx     9550 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/corpus_count.cc
+-rw-r--r--  2.0 unx      293 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/hash_gamma.hh
+-rw-r--r--  2.0 unx     2820 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/corpus_count_test.cc
+-rw-r--r--  2.0 unx     1869 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/dump_counts_main.cc
+-rw-r--r--  2.0 unx     3509 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/adjust_counts_test.cc
+-rw-r--r--  2.0 unx     1701 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/lm/builder/corpus_count.hh
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-06 07:48 camel-kenlm-2024.5.6/.github/workflows/
+-rw-r--r--  2.0 unx      471 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/.github/workflows/windows.yml
+-rw-r--r--  2.0 unx      619 b- defN 23-Mar-04 15:18 camel-kenlm-2024.5.6/.github/workflows/ubuntu.yml
+-rw-r--r--  2.0 unx      542 b- defN 21-Dec-27 11:00 camel-kenlm-2024.5.6/.github/workflows/mac.yml
+329 files, 1835508 bytes uncompressed, 502035 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,985 +1,988 @@
-Filename: camel-kenlm-2024.5.2/
+Filename: camel-kenlm-2024.5.6/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/camel_kenlm.egg-info/
+Filename: camel-kenlm-2024.5.6/camel_kenlm.egg-info/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/cmake/
+Filename: camel-kenlm-2024.5.6/cmake/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/
+Filename: camel-kenlm-2024.5.6/util/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/
+Filename: camel-kenlm-2024.5.6/python/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/
+Filename: camel-kenlm-2024.5.6/lm/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.github/
+Filename: camel-kenlm-2024.5.6/.github/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/PKG-INFO
+Filename: camel-kenlm-2024.5.6/PKG-INFO
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/LICENSE
+Filename: camel-kenlm-2024.5.6/LICENSE
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/COPYING.LESSER.3
+Filename: camel-kenlm-2024.5.6/COPYING.LESSER.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/pyproject.toml
+Filename: camel-kenlm-2024.5.6/pyproject.toml
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/MANIFEST.in
+Filename: camel-kenlm-2024.5.6/MANIFEST.in
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/clean_query_only.sh
+Filename: camel-kenlm-2024.5.6/clean_query_only.sh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/README.md
+Filename: camel-kenlm-2024.5.6/README.md
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/COPYING
+Filename: camel-kenlm-2024.5.6/COPYING
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/setup.py
+Filename: camel-kenlm-2024.5.6/setup.py
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.gitignore
+Filename: camel-kenlm-2024.5.6/.gitignore
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/setup.cfg
+Filename: camel-kenlm-2024.5.6/setup.cfg
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/COPYING.3
+Filename: camel-kenlm-2024.5.6/COPYING.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/Doxyfile
+Filename: camel-kenlm-2024.5.6/Doxyfile
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/compile_query_only.sh
+Filename: camel-kenlm-2024.5.6/compile_query_only.sh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/BUILDING
+Filename: camel-kenlm-2024.5.6/BUILDING
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/camel_kenlm.egg-info/PKG-INFO
+Filename: camel-kenlm-2024.5.6/camel_kenlm.egg-info/PKG-INFO
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/camel_kenlm.egg-info/SOURCES.txt
+Filename: camel-kenlm-2024.5.6/camel_kenlm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/camel_kenlm.egg-info/top_level.txt
+Filename: camel-kenlm-2024.5.6/camel_kenlm.egg-info/top_level.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/camel_kenlm.egg-info/dependency_links.txt
+Filename: camel-kenlm-2024.5.6/camel_kenlm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/cmake/modules/
+Filename: camel-kenlm-2024.5.6/cmake/modules/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/cmake/KenLMFunctions.cmake
+Filename: camel-kenlm-2024.5.6/cmake/KenLMFunctions.cmake
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/cmake/kenlmConfig.cmake.in
+Filename: camel-kenlm-2024.5.6/cmake/kenlmConfig.cmake.in
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/cmake/modules/FindEigen3.cmake
+Filename: camel-kenlm-2024.5.6/cmake/modules/FindEigen3.cmake
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/
+Filename: camel-kenlm-2024.5.6/util/stream/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/
+Filename: camel-kenlm-2024.5.6/util/double-conversion/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file_stream.hh
+Filename: camel-kenlm-2024.5.6/util/file_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/ersatz_progress.hh
+Filename: camel-kenlm-2024.5.6/util/ersatz_progress.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/sized_iterator.hh
+Filename: camel-kenlm-2024.5.6/util/sized_iterator.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/string_stream_test.cc
+Filename: camel-kenlm-2024.5.6/util/string_stream_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/pool.cc
+Filename: camel-kenlm-2024.5.6/util/pool.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/fixed_array.hh
+Filename: camel-kenlm-2024.5.6/util/fixed_array.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/joint_sort_test.cc
+Filename: camel-kenlm-2024.5.6/util/joint_sort_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/float_to_string.cc
+Filename: camel-kenlm-2024.5.6/util/float_to_string.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/mmap.cc
+Filename: camel-kenlm-2024.5.6/util/mmap.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/multi_intersection_test.cc
+Filename: camel-kenlm-2024.5.6/util/multi_intersection_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file_piece.cc
+Filename: camel-kenlm-2024.5.6/util/file_piece.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/probing_hash_table.hh
+Filename: camel-kenlm-2024.5.6/util/probing_hash_table.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/bit_packing_test.cc
+Filename: camel-kenlm-2024.5.6/util/bit_packing_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file.hh
+Filename: camel-kenlm-2024.5.6/util/file.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/string_piece.cc
+Filename: camel-kenlm-2024.5.6/util/string_piece.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/util/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/bit_packing.cc
+Filename: camel-kenlm-2024.5.6/util/bit_packing.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/usage.cc
+Filename: camel-kenlm-2024.5.6/util/usage.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/tokenize_piece_test.cc
+Filename: camel-kenlm-2024.5.6/util/tokenize_piece_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/parallel_read.hh
+Filename: camel-kenlm-2024.5.6/util/parallel_read.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/string_stream.hh
+Filename: camel-kenlm-2024.5.6/util/string_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/string_piece.hh
+Filename: camel-kenlm-2024.5.6/util/string_piece.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file.cc
+Filename: camel-kenlm-2024.5.6/util/file.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/pcqueue.hh
+Filename: camel-kenlm-2024.5.6/util/pcqueue.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/bit_packing.hh
+Filename: camel-kenlm-2024.5.6/util/bit_packing.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/cat_compressed_main.cc
+Filename: camel-kenlm-2024.5.6/util/cat_compressed_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/parallel_read.cc
+Filename: camel-kenlm-2024.5.6/util/parallel_read.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/usage.hh
+Filename: camel-kenlm-2024.5.6/util/usage.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/ersatz_progress.cc
+Filename: camel-kenlm-2024.5.6/util/ersatz_progress.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/proxy_iterator.hh
+Filename: camel-kenlm-2024.5.6/util/proxy_iterator.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/pool.hh
+Filename: camel-kenlm-2024.5.6/util/pool.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/read_compressed_test.cc
+Filename: camel-kenlm-2024.5.6/util/read_compressed_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file_piece.hh
+Filename: camel-kenlm-2024.5.6/util/file_piece.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/float_to_string.hh
+Filename: camel-kenlm-2024.5.6/util/float_to_string.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/mmap.hh
+Filename: camel-kenlm-2024.5.6/util/mmap.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/tokenize_piece.hh
+Filename: camel-kenlm-2024.5.6/util/tokenize_piece.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/getopt.hh
+Filename: camel-kenlm-2024.5.6/util/getopt.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/file_piece_test.cc
+Filename: camel-kenlm-2024.5.6/util/file_piece_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/integer_to_string.cc
+Filename: camel-kenlm-2024.5.6/util/integer_to_string.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/sized_iterator_test.cc
+Filename: camel-kenlm-2024.5.6/util/sized_iterator_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/sorted_uniform_test.cc
+Filename: camel-kenlm-2024.5.6/util/sorted_uniform_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/spaces.cc
+Filename: camel-kenlm-2024.5.6/util/spaces.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/read_compressed.hh
+Filename: camel-kenlm-2024.5.6/util/read_compressed.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/probing_hash_table_benchmark_main.cc
+Filename: camel-kenlm-2024.5.6/util/probing_hash_table_benchmark_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/exception.hh
+Filename: camel-kenlm-2024.5.6/util/exception.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/have.hh
+Filename: camel-kenlm-2024.5.6/util/have.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/sorted_uniform.hh
+Filename: camel-kenlm-2024.5.6/util/sorted_uniform.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/murmur_hash.cc
+Filename: camel-kenlm-2024.5.6/util/murmur_hash.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/integer_to_string_test.cc
+Filename: camel-kenlm-2024.5.6/util/integer_to_string_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/scoped.cc
+Filename: camel-kenlm-2024.5.6/util/scoped.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/joint_sort.hh
+Filename: camel-kenlm-2024.5.6/util/joint_sort.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/spaces.hh
+Filename: camel-kenlm-2024.5.6/util/spaces.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/read_compressed.cc
+Filename: camel-kenlm-2024.5.6/util/read_compressed.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/exception.cc
+Filename: camel-kenlm-2024.5.6/util/exception.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/string_piece_hash.hh
+Filename: camel-kenlm-2024.5.6/util/string_piece_hash.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/murmur_hash.hh
+Filename: camel-kenlm-2024.5.6/util/murmur_hash.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/scoped.hh
+Filename: camel-kenlm-2024.5.6/util/scoped.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/fake_ostream.hh
+Filename: camel-kenlm-2024.5.6/util/fake_ostream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/pcqueue_test.cc
+Filename: camel-kenlm-2024.5.6/util/pcqueue_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/multi_intersection.hh
+Filename: camel-kenlm-2024.5.6/util/multi_intersection.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/probing_hash_table_test.cc
+Filename: camel-kenlm-2024.5.6/util/probing_hash_table_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/getopt.c
+Filename: camel-kenlm-2024.5.6/util/getopt.c
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/thread_pool.hh
+Filename: camel-kenlm-2024.5.6/util/thread_pool.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/integer_to_string.hh
+Filename: camel-kenlm-2024.5.6/util/integer_to_string.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/io_test.cc
+Filename: camel-kenlm-2024.5.6/util/stream/io_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/util/stream/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/rewindable_stream.hh
+Filename: camel-kenlm-2024.5.6/util/stream/rewindable_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/multi_progress.hh
+Filename: camel-kenlm-2024.5.6/util/stream/multi_progress.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/multi_stream.hh
+Filename: camel-kenlm-2024.5.6/util/stream/multi_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/rewindable_stream.cc
+Filename: camel-kenlm-2024.5.6/util/stream/rewindable_stream.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/rewindable_stream_test.cc
+Filename: camel-kenlm-2024.5.6/util/stream/rewindable_stream_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/stream_test.cc
+Filename: camel-kenlm-2024.5.6/util/stream/stream_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/multi_progress.cc
+Filename: camel-kenlm-2024.5.6/util/stream/multi_progress.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/block.hh
+Filename: camel-kenlm-2024.5.6/util/stream/block.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/io.cc
+Filename: camel-kenlm-2024.5.6/util/stream/io.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/chain.cc
+Filename: camel-kenlm-2024.5.6/util/stream/chain.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/sort_test.cc
+Filename: camel-kenlm-2024.5.6/util/stream/sort_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/config.hh
+Filename: camel-kenlm-2024.5.6/util/stream/config.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/count_records.cc
+Filename: camel-kenlm-2024.5.6/util/stream/count_records.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/line_input.cc
+Filename: camel-kenlm-2024.5.6/util/stream/line_input.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/stream.hh
+Filename: camel-kenlm-2024.5.6/util/stream/stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/line_input.hh
+Filename: camel-kenlm-2024.5.6/util/stream/line_input.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/io.hh
+Filename: camel-kenlm-2024.5.6/util/stream/io.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/typed_stream.hh
+Filename: camel-kenlm-2024.5.6/util/stream/typed_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/chain.hh
+Filename: camel-kenlm-2024.5.6/util/stream/chain.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/count_records.hh
+Filename: camel-kenlm-2024.5.6/util/stream/count_records.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/stream/sort.hh
+Filename: camel-kenlm-2024.5.6/util/stream/sort.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/string-to-double.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/string-to-double.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/utils.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/utils.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/bignum.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/bignum.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/string-to-double.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/string-to-double.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/util/double-conversion/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/LICENSE
+Filename: camel-kenlm-2024.5.6/util/double-conversion/LICENSE
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/double-to-string.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/double-to-string.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/strtod.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/strtod.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/diy-fp.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/diy-fp.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/strtod.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/strtod.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/cached-powers.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/cached-powers.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/double-conversion.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/double-conversion.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/double-to-string.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/double-to-string.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/cached-powers.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/cached-powers.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/ieee.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/ieee.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/bignum.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/bignum.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.h
+Filename: camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.h
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.cc
+Filename: camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/kenlm.cpp
+Filename: camel-kenlm-2024.5.6/python/kenlm.cpp
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/python/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/score_sentence.cc
+Filename: camel-kenlm-2024.5.6/python/score_sentence.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/score_sentence.hh
+Filename: camel-kenlm-2024.5.6/python/score_sentence.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/example.py
+Filename: camel-kenlm-2024.5.6/python/BuildStandalone.cmake
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/_kenlm.pxd
+Filename: camel-kenlm-2024.5.6/python/example.py
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/python/kenlm.pyx
+Filename: camel-kenlm-2024.5.6/python/_kenlm.pxd
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/wrappers/
+Filename: camel-kenlm-2024.5.6/python/kenlm.pyx
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/
+Filename: camel-kenlm-2024.5.6/lm/wrappers/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/
+Filename: camel-kenlm-2024.5.6/lm/common/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/
+Filename: camel-kenlm-2024.5.6/lm/interpolate/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/
+Filename: camel-kenlm-2024.5.6/lm/filter/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/trie_sort.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/read_arpa.hh
+Filename: camel-kenlm-2024.5.6/lm/trie_sort.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/lm_exception.cc
+Filename: camel-kenlm-2024.5.6/lm/read_arpa.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/value_build.cc
+Filename: camel-kenlm-2024.5.6/lm/lm_exception.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/binary_format.cc
+Filename: camel-kenlm-2024.5.6/lm/value_build.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/bhiksha.hh
+Filename: camel-kenlm-2024.5.6/lm/binary_format.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/lm/bhiksha.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/model.hh
+Filename: camel-kenlm-2024.5.6/lm/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/trie.cc
+Filename: camel-kenlm-2024.5.6/lm/model.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/bhiksha.cc
+Filename: camel-kenlm-2024.5.6/lm/trie.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/state.hh
+Filename: camel-kenlm-2024.5.6/lm/bhiksha.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/trie.hh
+Filename: camel-kenlm-2024.5.6/lm/state.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/return.hh
+Filename: camel-kenlm-2024.5.6/lm/trie.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/model.cc
+Filename: camel-kenlm-2024.5.6/lm/return.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/query_main.cc
+Filename: camel-kenlm-2024.5.6/lm/model.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/blank.hh
+Filename: camel-kenlm-2024.5.6/lm/query_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/trie_sort.hh
+Filename: camel-kenlm-2024.5.6/lm/blank.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/weights.hh
+Filename: camel-kenlm-2024.5.6/lm/trie_sort.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/left_test.cc
+Filename: camel-kenlm-2024.5.6/lm/weights.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/max_order.hh
+Filename: camel-kenlm-2024.5.6/lm/left_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/lm_exception.hh
+Filename: camel-kenlm-2024.5.6/lm/max_order.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/test_nounk.arpa
+Filename: camel-kenlm-2024.5.6/lm/lm_exception.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/value.hh
+Filename: camel-kenlm-2024.5.6/lm/test_nounk.arpa
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/read_arpa.cc
+Filename: camel-kenlm-2024.5.6/lm/value.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/binary_format.hh
+Filename: camel-kenlm-2024.5.6/lm/read_arpa.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/partial.hh
+Filename: camel-kenlm-2024.5.6/lm/binary_format.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/value_build.hh
+Filename: camel-kenlm-2024.5.6/lm/partial.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/search_hashed.cc
+Filename: camel-kenlm-2024.5.6/lm/value_build.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/quantize.hh
+Filename: camel-kenlm-2024.5.6/lm/search_hashed.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/build_binary_main.cc
+Filename: camel-kenlm-2024.5.6/lm/quantize.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/left.hh
+Filename: camel-kenlm-2024.5.6/lm/build_binary_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/vocab.hh
+Filename: camel-kenlm-2024.5.6/lm/left.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/search_trie.hh
+Filename: camel-kenlm-2024.5.6/lm/vocab.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/config.hh
+Filename: camel-kenlm-2024.5.6/lm/search_trie.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/test.arpa
+Filename: camel-kenlm-2024.5.6/lm/config.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/word_index.hh
+Filename: camel-kenlm-2024.5.6/lm/test.arpa
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/model_type.hh
+Filename: camel-kenlm-2024.5.6/lm/word_index.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/sizes.cc
+Filename: camel-kenlm-2024.5.6/lm/model_type.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/partial_test.cc
+Filename: camel-kenlm-2024.5.6/lm/sizes.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/virtual_interface.cc
+Filename: camel-kenlm-2024.5.6/lm/partial_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/enumerate_vocab.hh
+Filename: camel-kenlm-2024.5.6/lm/virtual_interface.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/facade.hh
+Filename: camel-kenlm-2024.5.6/lm/enumerate_vocab.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/model_test.cc
+Filename: camel-kenlm-2024.5.6/lm/facade.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/sizes.hh
+Filename: camel-kenlm-2024.5.6/lm/model_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/kenlm_benchmark_main.cc
+Filename: camel-kenlm-2024.5.6/lm/sizes.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/virtual_interface.hh
+Filename: camel-kenlm-2024.5.6/lm/kenlm_benchmark_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/fragment_main.cc
+Filename: camel-kenlm-2024.5.6/lm/virtual_interface.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/search_hashed.hh
+Filename: camel-kenlm-2024.5.6/lm/fragment_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/quantize.cc
+Filename: camel-kenlm-2024.5.6/lm/search_hashed.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/vocab.cc
+Filename: camel-kenlm-2024.5.6/lm/quantize.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/ngram_query.hh
+Filename: camel-kenlm-2024.5.6/lm/vocab.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/search_trie.cc
+Filename: camel-kenlm-2024.5.6/lm/ngram_query.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/config.cc
+Filename: camel-kenlm-2024.5.6/lm/search_trie.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/wrappers/nplm.cc
+Filename: camel-kenlm-2024.5.6/lm/config.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/wrappers/nplm.hh
+Filename: camel-kenlm-2024.5.6/lm/wrappers/nplm.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/wrappers/README
+Filename: camel-kenlm-2024.5.6/lm/wrappers/nplm.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/
+Filename: camel-kenlm-2024.5.6/lm/wrappers/README
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/joint_order.hh
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/renumber.cc
+Filename: camel-kenlm-2024.5.6/lm/common/joint_order.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/model_buffer.hh
+Filename: camel-kenlm-2024.5.6/lm/common/renumber.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/size_option.hh
+Filename: camel-kenlm-2024.5.6/lm/common/model_buffer.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/print.hh
+Filename: camel-kenlm-2024.5.6/lm/common/size_option.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/lm/common/print.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/special.hh
+Filename: camel-kenlm-2024.5.6/lm/common/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/compare.hh
+Filename: camel-kenlm-2024.5.6/lm/common/special.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/renumber.hh
+Filename: camel-kenlm-2024.5.6/lm/common/compare.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/model_buffer.cc
+Filename: camel-kenlm-2024.5.6/lm/common/renumber.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/size_option.cc
+Filename: camel-kenlm-2024.5.6/lm/common/model_buffer.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/print.cc
+Filename: camel-kenlm-2024.5.6/lm/common/size_option.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/ngram.hh
+Filename: camel-kenlm-2024.5.6/lm/common/print.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/ngram_stream.hh
+Filename: camel-kenlm-2024.5.6/lm/common/ngram.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/model_buffer_test.cc
+Filename: camel-kenlm-2024.5.6/lm/common/ngram_stream.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/
+Filename: camel-kenlm-2024.5.6/lm/common/model_buffer_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/toy0.arpa
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/toy1.arpa
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/toy0.arpa
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/generate.sh
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/toy1.arpa
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.2
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/generate.sh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.3
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.2
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.1
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.kenlm_intermediate
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.1
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.1
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.kenlm_intermediate
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.vocab
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.1
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy1.kenlm_intermediate
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.vocab
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.2
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy1.kenlm_intermediate
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.3
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.2
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/bigendian/toy0.vocab
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.2
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/bigendian/toy0.vocab
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.3
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.2
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.1
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.kenlm_intermediate
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.1
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.1
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.kenlm_intermediate
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.vocab
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.1
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy1.kenlm_intermediate
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.vocab
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.2
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy1.kenlm_intermediate
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.3
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.2
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/common/test_data/littleendian/toy0.vocab
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.3
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding_test.cc
+Filename: camel-kenlm-2024.5.6/lm/common/test_data/littleendian/toy0.vocab
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/universal_vocab.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/universal_vocab.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/pipeline.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/pipeline.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_matrix.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_instances_test.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_matrix.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/split_worker.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_instances_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_weights.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/split_worker.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/interpolate_main.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_weights.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/interpolate_info.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/interpolate_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_weights.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/interpolate_info.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/split_worker.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_weights.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/split_worker.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/normalize_test.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/universal_vocab.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/normalize_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/pipeline.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/universal_vocab.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/pipeline.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/normalize.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/normalize.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/backoff_matrix.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/backoff_matrix.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_instances.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification_test.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_instances.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/streaming_example_main.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/streaming_example_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/normalize.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives_test.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/normalize.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/merge_vocab_test.cc
+Filename: camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/interpolate/tune_instances.hh
+Filename: camel-kenlm-2024.5.6/lm/interpolate/merge_vocab_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/lm/interpolate/tune_instances.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/phrase_table_vocab_main.cc
+Filename: camel-kenlm-2024.5.6/lm/filter/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/count_io.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/phrase_table_vocab_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/filter_main.cc
+Filename: camel-kenlm-2024.5.6/lm/filter/count_io.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/thread.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/filter_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/vocab.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/thread.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/arpa_io.cc
+Filename: camel-kenlm-2024.5.6/lm/filter/vocab.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/phrase.cc
+Filename: camel-kenlm-2024.5.6/lm/filter/arpa_io.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/wrapper.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/phrase.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/phrase.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/wrapper.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/arpa_io.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/phrase.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/format.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/arpa_io.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/filter/vocab.cc
+Filename: camel-kenlm-2024.5.6/lm/filter/format.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/interpolate.hh
+Filename: camel-kenlm-2024.5.6/lm/filter/vocab.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/discount.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/interpolate.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/pipeline.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/discount.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/adjust_counts.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/pipeline.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/lmplz_main.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/adjust_counts.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/output.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/lmplz_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/CMakeLists.txt
+Filename: camel-kenlm-2024.5.6/lm/builder/output.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/initial_probabilities.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/CMakeLists.txt
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/payload.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/initial_probabilities.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/output.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/payload.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/combine_counts.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/output.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/adjust_counts.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/combine_counts.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/initial_probabilities.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/adjust_counts.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/header_info.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/initial_probabilities.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/interpolate.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/header_info.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/debug_print.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/interpolate.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/count_ngrams_main.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/debug_print.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/pipeline.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/count_ngrams_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/TODO
+Filename: camel-kenlm-2024.5.6/lm/builder/pipeline.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/README.md
+Filename: camel-kenlm-2024.5.6/lm/builder/TODO
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/corpus_count.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/README.md
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/hash_gamma.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/corpus_count.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/corpus_count_test.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/hash_gamma.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/dump_counts_main.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/corpus_count_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/adjust_counts_test.cc
+Filename: camel-kenlm-2024.5.6/lm/builder/dump_counts_main.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/lm/builder/corpus_count.hh
+Filename: camel-kenlm-2024.5.6/lm/builder/adjust_counts_test.cc
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.github/workflows/
+Filename: camel-kenlm-2024.5.6/lm/builder/corpus_count.hh
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.github/workflows/windows.yml
+Filename: camel-kenlm-2024.5.6/.github/workflows/
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.github/workflows/ubuntu.yml
+Filename: camel-kenlm-2024.5.6/.github/workflows/windows.yml
 Comment: 
 
-Filename: camel-kenlm-2024.5.2/.github/workflows/mac.yml
+Filename: camel-kenlm-2024.5.6/.github/workflows/ubuntu.yml
+Comment: 
+
+Filename: camel-kenlm-2024.5.6/.github/workflows/mac.yml
 Comment: 
 
 Zip file comment:
```

## Comparing `camel-kenlm-2024.5.2/CMakeLists.txt` & `camel-kenlm-2024.5.6/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/LICENSE` & `camel-kenlm-2024.5.6/LICENSE`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/COPYING.LESSER.3` & `camel-kenlm-2024.5.6/COPYING.LESSER.3`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/README.md` & `camel-kenlm-2024.5.6/README.md`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/COPYING` & `camel-kenlm-2024.5.6/COPYING`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/setup.py` & `camel-kenlm-2024.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import re
 from pathlib import Path
 
 #Does gcc compile with this header and library?
 def compile_test(header, library):
     dummy_path = os.path.join(os.path.dirname(__file__), "dummy")
-    command = "bash -c \"g++ -include " + header + " -l" + library + " -x c++ - <<<'int main() {}' -o " + dummy_path + " >/dev/null 2>/dev/null && rm " + dummy_path + " 2>/dev/null\""
+    command = "bash -c \"g++ -include " + header + " -l" + library + " -x c++ - <<<'#include <" + header + ">\nint main() {}' -o " + dummy_path + " >/dev/null 2>/dev/null && rm " + dummy_path + " 2>/dev/null\""
     return os.system(command) == 0
 
 # Use an environment variable
 max_order = os.getenv("MAX_ORDER", "6")
 
 # Try to get from --config-settings, if present
 is_max_order = [s for s in sys.argv if "--max_order" in s]
@@ -120,13 +120,13 @@
         depends = ['python/BuildStandalone.cmake'],
         libraries=LIBS, 
         extra_compile_args=ARGS),
 ]
 
 setup(
     name='camel-kenlm',
-    version='2024.05.02',
+    version='2024.05.06',
     url='https://github.com/CAMeL-Lab/camel-kenlm',
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
     include_package_data=True,
 )
```

## Comparing `camel-kenlm-2024.5.2/COPYING.3` & `camel-kenlm-2024.5.6/COPYING.3`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/Doxyfile` & `camel-kenlm-2024.5.6/Doxyfile`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/compile_query_only.sh` & `camel-kenlm-2024.5.6/compile_query_only.sh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/BUILDING` & `camel-kenlm-2024.5.6/BUILDING`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/camel_kenlm.egg-info/SOURCES.txt` & `camel-kenlm-2024.5.6/camel_kenlm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 lm/interpolate/tune_weights.cc
 lm/interpolate/tune_weights.hh
 lm/interpolate/universal_vocab.cc
 lm/interpolate/universal_vocab.hh
 lm/wrappers/README
 lm/wrappers/nplm.cc
 lm/wrappers/nplm.hh
+python/BuildStandalone.cmake
 python/CMakeLists.txt
 python/_kenlm.pxd
 python/example.py
 python/kenlm.cpp
 python/kenlm.pyx
 python/score_sentence.cc
 python/score_sentence.hh
```

## Comparing `camel-kenlm-2024.5.2/cmake/KenLMFunctions.cmake` & `camel-kenlm-2024.5.6/cmake/KenLMFunctions.cmake`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/cmake/modules/FindEigen3.cmake` & `camel-kenlm-2024.5.6/cmake/modules/FindEigen3.cmake`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file_stream.hh` & `camel-kenlm-2024.5.6/util/file_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/ersatz_progress.hh` & `camel-kenlm-2024.5.6/util/ersatz_progress.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/sized_iterator.hh` & `camel-kenlm-2024.5.6/util/sized_iterator.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/string_stream_test.cc` & `camel-kenlm-2024.5.6/util/string_stream_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/pool.cc` & `camel-kenlm-2024.5.6/util/pool.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/fixed_array.hh` & `camel-kenlm-2024.5.6/util/fixed_array.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/joint_sort_test.cc` & `camel-kenlm-2024.5.6/util/joint_sort_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/float_to_string.cc` & `camel-kenlm-2024.5.6/util/float_to_string.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/mmap.cc` & `camel-kenlm-2024.5.6/util/mmap.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/multi_intersection_test.cc` & `camel-kenlm-2024.5.6/util/multi_intersection_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file_piece.cc` & `camel-kenlm-2024.5.6/util/file_piece.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/probing_hash_table.hh` & `camel-kenlm-2024.5.6/util/probing_hash_table.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/bit_packing_test.cc` & `camel-kenlm-2024.5.6/util/bit_packing_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file.hh` & `camel-kenlm-2024.5.6/util/file.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/string_piece.cc` & `camel-kenlm-2024.5.6/util/string_piece.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/CMakeLists.txt` & `camel-kenlm-2024.5.6/util/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/bit_packing.cc` & `camel-kenlm-2024.5.6/util/bit_packing.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/usage.cc` & `camel-kenlm-2024.5.6/util/usage.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/tokenize_piece_test.cc` & `camel-kenlm-2024.5.6/util/tokenize_piece_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/string_stream.hh` & `camel-kenlm-2024.5.6/util/string_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/string_piece.hh` & `camel-kenlm-2024.5.6/util/string_piece.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file.cc` & `camel-kenlm-2024.5.6/util/file.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/pcqueue.hh` & `camel-kenlm-2024.5.6/util/pcqueue.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/bit_packing.hh` & `camel-kenlm-2024.5.6/util/bit_packing.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/cat_compressed_main.cc` & `camel-kenlm-2024.5.6/util/cat_compressed_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/parallel_read.cc` & `camel-kenlm-2024.5.6/util/parallel_read.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/usage.hh` & `camel-kenlm-2024.5.6/util/usage.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/ersatz_progress.cc` & `camel-kenlm-2024.5.6/util/ersatz_progress.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/proxy_iterator.hh` & `camel-kenlm-2024.5.6/util/proxy_iterator.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/pool.hh` & `camel-kenlm-2024.5.6/util/pool.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/read_compressed_test.cc` & `camel-kenlm-2024.5.6/util/read_compressed_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file_piece.hh` & `camel-kenlm-2024.5.6/util/file_piece.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/float_to_string.hh` & `camel-kenlm-2024.5.6/util/float_to_string.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/mmap.hh` & `camel-kenlm-2024.5.6/util/mmap.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/tokenize_piece.hh` & `camel-kenlm-2024.5.6/util/tokenize_piece.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/file_piece_test.cc` & `camel-kenlm-2024.5.6/util/file_piece_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/integer_to_string.cc` & `camel-kenlm-2024.5.6/util/integer_to_string.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/sized_iterator_test.cc` & `camel-kenlm-2024.5.6/util/sized_iterator_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/sorted_uniform_test.cc` & `camel-kenlm-2024.5.6/util/sorted_uniform_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/spaces.cc` & `camel-kenlm-2024.5.6/util/spaces.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/read_compressed.hh` & `camel-kenlm-2024.5.6/util/read_compressed.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/probing_hash_table_benchmark_main.cc` & `camel-kenlm-2024.5.6/util/probing_hash_table_benchmark_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/exception.hh` & `camel-kenlm-2024.5.6/util/exception.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/sorted_uniform.hh` & `camel-kenlm-2024.5.6/util/sorted_uniform.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/murmur_hash.cc` & `camel-kenlm-2024.5.6/util/murmur_hash.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/integer_to_string_test.cc` & `camel-kenlm-2024.5.6/util/integer_to_string_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/scoped.cc` & `camel-kenlm-2024.5.6/util/scoped.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/joint_sort.hh` & `camel-kenlm-2024.5.6/util/joint_sort.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/read_compressed.cc` & `camel-kenlm-2024.5.6/util/read_compressed.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/exception.cc` & `camel-kenlm-2024.5.6/util/exception.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/string_piece_hash.hh` & `camel-kenlm-2024.5.6/util/string_piece_hash.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/murmur_hash.hh` & `camel-kenlm-2024.5.6/util/murmur_hash.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/scoped.hh` & `camel-kenlm-2024.5.6/util/scoped.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/fake_ostream.hh` & `camel-kenlm-2024.5.6/util/fake_ostream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/multi_intersection.hh` & `camel-kenlm-2024.5.6/util/multi_intersection.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/probing_hash_table_test.cc` & `camel-kenlm-2024.5.6/util/probing_hash_table_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/getopt.c` & `camel-kenlm-2024.5.6/util/getopt.c`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/thread_pool.hh` & `camel-kenlm-2024.5.6/util/thread_pool.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/integer_to_string.hh` & `camel-kenlm-2024.5.6/util/integer_to_string.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/io_test.cc` & `camel-kenlm-2024.5.6/util/stream/io_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/CMakeLists.txt` & `camel-kenlm-2024.5.6/util/stream/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/rewindable_stream.hh` & `camel-kenlm-2024.5.6/util/stream/rewindable_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/multi_progress.hh` & `camel-kenlm-2024.5.6/util/stream/multi_progress.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/multi_stream.hh` & `camel-kenlm-2024.5.6/util/stream/multi_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/rewindable_stream.cc` & `camel-kenlm-2024.5.6/util/stream/rewindable_stream.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/rewindable_stream_test.cc` & `camel-kenlm-2024.5.6/util/stream/rewindable_stream_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/stream_test.cc` & `camel-kenlm-2024.5.6/util/stream/stream_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/multi_progress.cc` & `camel-kenlm-2024.5.6/util/stream/multi_progress.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/block.hh` & `camel-kenlm-2024.5.6/util/stream/block.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/io.cc` & `camel-kenlm-2024.5.6/util/stream/io.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/chain.cc` & `camel-kenlm-2024.5.6/util/stream/chain.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/sort_test.cc` & `camel-kenlm-2024.5.6/util/stream/sort_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/config.hh` & `camel-kenlm-2024.5.6/util/stream/config.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/line_input.cc` & `camel-kenlm-2024.5.6/util/stream/line_input.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/stream.hh` & `camel-kenlm-2024.5.6/util/stream/stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/line_input.hh` & `camel-kenlm-2024.5.6/util/stream/line_input.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/io.hh` & `camel-kenlm-2024.5.6/util/stream/io.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/typed_stream.hh` & `camel-kenlm-2024.5.6/util/stream/typed_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/chain.hh` & `camel-kenlm-2024.5.6/util/stream/chain.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/stream/sort.hh` & `camel-kenlm-2024.5.6/util/stream/sort.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/string-to-double.h` & `camel-kenlm-2024.5.6/util/double-conversion/string-to-double.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/utils.h` & `camel-kenlm-2024.5.6/util/double-conversion/utils.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/bignum.cc` & `camel-kenlm-2024.5.6/util/double-conversion/bignum.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.h` & `camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/string-to-double.cc` & `camel-kenlm-2024.5.6/util/double-conversion/string-to-double.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/CMakeLists.txt` & `camel-kenlm-2024.5.6/util/double-conversion/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/LICENSE` & `camel-kenlm-2024.5.6/util/double-conversion/LICENSE`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.h` & `camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/fixed-dtoa.cc` & `camel-kenlm-2024.5.6/util/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/double-to-string.h` & `camel-kenlm-2024.5.6/util/double-conversion/double-to-string.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/strtod.h` & `camel-kenlm-2024.5.6/util/double-conversion/strtod.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/diy-fp.h` & `camel-kenlm-2024.5.6/util/double-conversion/diy-fp.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/strtod.cc` & `camel-kenlm-2024.5.6/util/double-conversion/strtod.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/cached-powers.h` & `camel-kenlm-2024.5.6/util/double-conversion/cached-powers.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/double-conversion.h` & `camel-kenlm-2024.5.6/util/double-conversion/double-conversion.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.cc` & `camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/double-to-string.cc` & `camel-kenlm-2024.5.6/util/double-conversion/double-to-string.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/cached-powers.cc` & `camel-kenlm-2024.5.6/util/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/ieee.h` & `camel-kenlm-2024.5.6/util/double-conversion/ieee.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/bignum.h` & `camel-kenlm-2024.5.6/util/double-conversion/bignum.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/fast-dtoa.h` & `camel-kenlm-2024.5.6/util/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/util/double-conversion/bignum-dtoa.cc` & `camel-kenlm-2024.5.6/util/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/kenlm.cpp` & `camel-kenlm-2024.5.6/python/kenlm.cpp`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/CMakeLists.txt` & `camel-kenlm-2024.5.6/python/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/score_sentence.cc` & `camel-kenlm-2024.5.6/python/score_sentence.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/example.py` & `camel-kenlm-2024.5.6/python/example.py`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/_kenlm.pxd` & `camel-kenlm-2024.5.6/python/_kenlm.pxd`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/python/kenlm.pyx` & `camel-kenlm-2024.5.6/python/kenlm.pyx`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/trie_sort.cc` & `camel-kenlm-2024.5.6/lm/trie_sort.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/read_arpa.hh` & `camel-kenlm-2024.5.6/lm/read_arpa.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/lm_exception.cc` & `camel-kenlm-2024.5.6/lm/lm_exception.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/value_build.cc` & `camel-kenlm-2024.5.6/lm/value_build.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/binary_format.cc` & `camel-kenlm-2024.5.6/lm/binary_format.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/bhiksha.hh` & `camel-kenlm-2024.5.6/lm/bhiksha.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/CMakeLists.txt` & `camel-kenlm-2024.5.6/lm/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/model.hh` & `camel-kenlm-2024.5.6/lm/model.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/trie.cc` & `camel-kenlm-2024.5.6/lm/trie.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/bhiksha.cc` & `camel-kenlm-2024.5.6/lm/bhiksha.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/state.hh` & `camel-kenlm-2024.5.6/lm/state.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/trie.hh` & `camel-kenlm-2024.5.6/lm/trie.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/return.hh` & `camel-kenlm-2024.5.6/lm/return.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/model.cc` & `camel-kenlm-2024.5.6/lm/model.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/query_main.cc` & `camel-kenlm-2024.5.6/lm/query_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/blank.hh` & `camel-kenlm-2024.5.6/lm/blank.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/trie_sort.hh` & `camel-kenlm-2024.5.6/lm/trie_sort.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/left_test.cc` & `camel-kenlm-2024.5.6/lm/left_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/max_order.hh` & `camel-kenlm-2024.5.6/lm/max_order.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/lm_exception.hh` & `camel-kenlm-2024.5.6/lm/lm_exception.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/test_nounk.arpa` & `camel-kenlm-2024.5.6/lm/test_nounk.arpa`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/value.hh` & `camel-kenlm-2024.5.6/lm/value.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/read_arpa.cc` & `camel-kenlm-2024.5.6/lm/read_arpa.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/binary_format.hh` & `camel-kenlm-2024.5.6/lm/binary_format.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/partial.hh` & `camel-kenlm-2024.5.6/lm/partial.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/value_build.hh` & `camel-kenlm-2024.5.6/lm/value_build.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/search_hashed.cc` & `camel-kenlm-2024.5.6/lm/search_hashed.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/quantize.hh` & `camel-kenlm-2024.5.6/lm/quantize.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/build_binary_main.cc` & `camel-kenlm-2024.5.6/lm/build_binary_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/left.hh` & `camel-kenlm-2024.5.6/lm/left.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/vocab.hh` & `camel-kenlm-2024.5.6/lm/vocab.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/search_trie.hh` & `camel-kenlm-2024.5.6/lm/search_trie.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/config.hh` & `camel-kenlm-2024.5.6/lm/config.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/test.arpa` & `camel-kenlm-2024.5.6/lm/test.arpa`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/model_type.hh` & `camel-kenlm-2024.5.6/lm/model_type.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/sizes.cc` & `camel-kenlm-2024.5.6/lm/sizes.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/partial_test.cc` & `camel-kenlm-2024.5.6/lm/partial_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/enumerate_vocab.hh` & `camel-kenlm-2024.5.6/lm/enumerate_vocab.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/facade.hh` & `camel-kenlm-2024.5.6/lm/facade.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/model_test.cc` & `camel-kenlm-2024.5.6/lm/model_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/kenlm_benchmark_main.cc` & `camel-kenlm-2024.5.6/lm/kenlm_benchmark_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/virtual_interface.hh` & `camel-kenlm-2024.5.6/lm/virtual_interface.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/fragment_main.cc` & `camel-kenlm-2024.5.6/lm/fragment_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/search_hashed.hh` & `camel-kenlm-2024.5.6/lm/search_hashed.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/quantize.cc` & `camel-kenlm-2024.5.6/lm/quantize.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/vocab.cc` & `camel-kenlm-2024.5.6/lm/vocab.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/ngram_query.hh` & `camel-kenlm-2024.5.6/lm/ngram_query.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/search_trie.cc` & `camel-kenlm-2024.5.6/lm/search_trie.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/config.cc` & `camel-kenlm-2024.5.6/lm/config.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/wrappers/nplm.cc` & `camel-kenlm-2024.5.6/lm/wrappers/nplm.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/wrappers/nplm.hh` & `camel-kenlm-2024.5.6/lm/wrappers/nplm.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/joint_order.hh` & `camel-kenlm-2024.5.6/lm/common/joint_order.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/model_buffer.hh` & `camel-kenlm-2024.5.6/lm/common/model_buffer.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/print.hh` & `camel-kenlm-2024.5.6/lm/common/print.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/CMakeLists.txt` & `camel-kenlm-2024.5.6/lm/common/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/special.hh` & `camel-kenlm-2024.5.6/lm/common/special.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/compare.hh` & `camel-kenlm-2024.5.6/lm/common/compare.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/renumber.hh` & `camel-kenlm-2024.5.6/lm/common/renumber.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/model_buffer.cc` & `camel-kenlm-2024.5.6/lm/common/model_buffer.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/size_option.cc` & `camel-kenlm-2024.5.6/lm/common/size_option.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/print.cc` & `camel-kenlm-2024.5.6/lm/common/print.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/ngram.hh` & `camel-kenlm-2024.5.6/lm/common/ngram.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/ngram_stream.hh` & `camel-kenlm-2024.5.6/lm/common/ngram_stream.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/common/model_buffer_test.cc` & `camel-kenlm-2024.5.6/lm/common/model_buffer_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/universal_vocab.hh` & `camel-kenlm-2024.5.6/lm/interpolate/universal_vocab.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.cc` & `camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/pipeline.hh` & `camel-kenlm-2024.5.6/lm/interpolate/pipeline.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.cc` & `camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/CMakeLists.txt` & `camel-kenlm-2024.5.6/lm/interpolate/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_matrix.hh` & `camel-kenlm-2024.5.6/lm/interpolate/tune_matrix.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_instances_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/tune_instances_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/split_worker.hh` & `camel-kenlm-2024.5.6/lm/interpolate/split_worker.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_weights.cc` & `camel-kenlm-2024.5.6/lm/interpolate/tune_weights.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/interpolate_main.cc` & `camel-kenlm-2024.5.6/lm/interpolate/interpolate_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/interpolate_info.hh` & `camel-kenlm-2024.5.6/lm/interpolate/interpolate_info.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/split_worker.cc` & `camel-kenlm-2024.5.6/lm/interpolate/split_worker.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/merge_vocab.hh` & `camel-kenlm-2024.5.6/lm/interpolate/merge_vocab.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/normalize_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/normalize_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/pipeline.cc` & `camel-kenlm-2024.5.6/lm/interpolate/pipeline.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification.hh` & `camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/normalize.cc` & `camel-kenlm-2024.5.6/lm/interpolate/normalize.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.hh` & `camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.cc` & `camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/backoff_matrix.hh` & `camel-kenlm-2024.5.6/lm/interpolate/backoff_matrix.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.hh` & `camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_instances.cc` & `camel-kenlm-2024.5.6/lm/interpolate/tune_instances.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/backoff_reunification_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/backoff_reunification_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/streaming_example_main.cc` & `camel-kenlm-2024.5.6/lm/interpolate/streaming_example_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives.cc` & `camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/normalize.hh` & `camel-kenlm-2024.5.6/lm/interpolate/normalize.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_derivatives_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/tune_derivatives_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/merge_probabilities.hh` & `camel-kenlm-2024.5.6/lm/interpolate/merge_probabilities.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/bounded_sequence_encoding.cc` & `camel-kenlm-2024.5.6/lm/interpolate/bounded_sequence_encoding.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/merge_vocab_test.cc` & `camel-kenlm-2024.5.6/lm/interpolate/merge_vocab_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/interpolate/tune_instances.hh` & `camel-kenlm-2024.5.6/lm/interpolate/tune_instances.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/CMakeLists.txt` & `camel-kenlm-2024.5.6/lm/filter/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/phrase_table_vocab_main.cc` & `camel-kenlm-2024.5.6/lm/filter/phrase_table_vocab_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/count_io.hh` & `camel-kenlm-2024.5.6/lm/filter/count_io.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/filter_main.cc` & `camel-kenlm-2024.5.6/lm/filter/filter_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/thread.hh` & `camel-kenlm-2024.5.6/lm/filter/thread.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/vocab.hh` & `camel-kenlm-2024.5.6/lm/filter/vocab.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/arpa_io.cc` & `camel-kenlm-2024.5.6/lm/filter/arpa_io.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/phrase.cc` & `camel-kenlm-2024.5.6/lm/filter/phrase.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/wrapper.hh` & `camel-kenlm-2024.5.6/lm/filter/wrapper.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/phrase.hh` & `camel-kenlm-2024.5.6/lm/filter/phrase.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/arpa_io.hh` & `camel-kenlm-2024.5.6/lm/filter/arpa_io.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/format.hh` & `camel-kenlm-2024.5.6/lm/filter/format.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/filter/vocab.cc` & `camel-kenlm-2024.5.6/lm/filter/vocab.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/interpolate.hh` & `camel-kenlm-2024.5.6/lm/builder/interpolate.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/pipeline.hh` & `camel-kenlm-2024.5.6/lm/builder/pipeline.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/adjust_counts.cc` & `camel-kenlm-2024.5.6/lm/builder/adjust_counts.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/lmplz_main.cc` & `camel-kenlm-2024.5.6/lm/builder/lmplz_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/output.cc` & `camel-kenlm-2024.5.6/lm/builder/output.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/CMakeLists.txt` & `camel-kenlm-2024.5.6/lm/builder/CMakeLists.txt`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/initial_probabilities.hh` & `camel-kenlm-2024.5.6/lm/builder/initial_probabilities.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/payload.hh` & `camel-kenlm-2024.5.6/lm/builder/payload.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/output.hh` & `camel-kenlm-2024.5.6/lm/builder/output.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/combine_counts.hh` & `camel-kenlm-2024.5.6/lm/builder/combine_counts.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/adjust_counts.hh` & `camel-kenlm-2024.5.6/lm/builder/adjust_counts.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/initial_probabilities.cc` & `camel-kenlm-2024.5.6/lm/builder/initial_probabilities.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/header_info.hh` & `camel-kenlm-2024.5.6/lm/builder/header_info.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/interpolate.cc` & `camel-kenlm-2024.5.6/lm/builder/interpolate.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/debug_print.hh` & `camel-kenlm-2024.5.6/lm/builder/debug_print.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/count_ngrams_main.cc` & `camel-kenlm-2024.5.6/lm/builder/count_ngrams_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/pipeline.cc` & `camel-kenlm-2024.5.6/lm/builder/pipeline.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/README.md` & `camel-kenlm-2024.5.6/lm/builder/README.md`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/corpus_count.cc` & `camel-kenlm-2024.5.6/lm/builder/corpus_count.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/corpus_count_test.cc` & `camel-kenlm-2024.5.6/lm/builder/corpus_count_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/dump_counts_main.cc` & `camel-kenlm-2024.5.6/lm/builder/dump_counts_main.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/adjust_counts_test.cc` & `camel-kenlm-2024.5.6/lm/builder/adjust_counts_test.cc`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/lm/builder/corpus_count.hh` & `camel-kenlm-2024.5.6/lm/builder/corpus_count.hh`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/.github/workflows/ubuntu.yml` & `camel-kenlm-2024.5.6/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

## Comparing `camel-kenlm-2024.5.2/.github/workflows/mac.yml` & `camel-kenlm-2024.5.6/.github/workflows/mac.yml`

 * *Files identical despite different names*

