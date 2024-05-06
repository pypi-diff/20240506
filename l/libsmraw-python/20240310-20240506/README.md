# Comparing `tmp/libsmraw-python-20240310.tar.gz` & `tmp/libsmraw-python-20240506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsmraw-python-20240310.tar", last modified: Sun Mar 10 05:38:28 2024, max compression
+gzip compressed data, was "libsmraw-python-20240506.tar", last modified: Mon May  6 04:00:58 2024, max compression
```

## Comparing `libsmraw-python-20240310.tar` & `libsmraw-python-20240506.tar`

### file list

```diff
@@ -1,832 +1,832 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33134 2024-03-10 05:19:37.000000 libsmraw-20240310/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-10 05:19:19.000000 libsmraw-20240310/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-10 05:06:09.000000 libsmraw-20240310/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-10 05:19:37.000000 libsmraw-20240310/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:06:09.000000 libsmraw-20240310/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-10 05:19:38.000000 libsmraw-20240310/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11673 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9554 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31438 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8411 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17322 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7562 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11295 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-10 05:19:30.000000 libsmraw-20240310/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-10 05:19:30.000000 libsmraw-20240310/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15720 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-10 05:19:30.000000 libsmraw-20240310/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5819 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11864 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8491 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-10 05:19:30.000000 libsmraw-20240310/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-10 05:19:30.000000 libsmraw-20240310/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19969 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:28.000000 libsmraw-20240310/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7503 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-10 05:06:12.000000 libsmraw-20240310/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-03-10 05:06:09.000000 libsmraw-20240310/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23825 2024-03-10 05:19:49.000000 libsmraw-20240310/include/libsmraw.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/include/libsmraw/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2330 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-03-10 05:19:49.000000 libsmraw-20240310/include/libsmraw/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-03-10 05:19:49.000000 libsmraw-20240310/include/libsmraw/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-03-10 05:19:49.000000 libsmraw-20240310/include/libsmraw/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27895 2024-03-10 05:19:37.000000 libsmraw-20240310/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23825 2024-03-10 05:06:11.000000 libsmraw-20240310/include/libsmraw.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/smraw.net/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-03-10 05:06:11.000000 libsmraw-20240310/smraw.net/smraw.net.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      195 2023-12-03 09:14:28.000000 libsmraw-20240310/smraw.net/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-03-10 05:06:11.000000 libsmraw-20240310/smraw.net/smraw.net.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2024-03-10 05:06:11.000000 libsmraw-20240310/smraw.net/smraw.net_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-03-10 05:19:49.000000 libsmraw-20240310/smraw.net/smraw.net.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1223 2024-03-10 05:06:11.000000 libsmraw-20240310/smraw.net/smraw.net.cpp
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22241 2024-03-10 05:19:37.000000 libsmraw-20240310/smraw.net/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16867 2024-03-10 05:06:11.000000 libsmraw-20240310/smraw.net/smraw.net_handle.cpp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-10 05:06:11.000000 libsmraw-20240310/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-10 05:06:11.000000 libsmraw-20240310/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-10 05:06:11.000000 libsmraw-20240310/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-10 05:06:11.000000 libsmraw-20240310/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-10 05:06:11.000000 libsmraw-20240310/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-10 05:06:11.000000 libsmraw-20240310/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-10 05:06:11.000000 libsmraw-20240310/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-10 05:06:09.000000 libsmraw-20240310/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-10 05:06:11.000000 libsmraw-20240310/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-03-10 05:19:49.000000 libsmraw-20240310/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18120 2024-03-10 05:19:36.000000 libsmraw-20240310/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19180 2024-03-10 05:19:49.000000 libsmraw-20240310/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-10 05:06:11.000000 libsmraw-20240310/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-10 05:06:11.000000 libsmraw-20240310/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-10 05:06:11.000000 libsmraw-20240310/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24902 2024-03-10 05:19:37.000000 libsmraw-20240310/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-03-10 05:06:09.000000 libsmraw-20240310/libsmraw.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29905 2024-03-10 05:19:37.000000 libsmraw-20240310/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-10 05:19:12.000000 libsmraw-20240310/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30378 2024-03-10 05:19:37.000000 libsmraw-20240310/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-10 05:19:18.000000 libsmraw-20240310/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2246 2023-12-03 09:14:22.000000 libsmraw-20240310/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33364 2024-03-10 05:19:37.000000 libsmraw-20240310/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-10 05:19:08.000000 libsmraw-20240310/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:14:22.000000 libsmraw-20240310/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-10 05:19:37.000000 libsmraw-20240310/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      682 2024-03-10 05:06:09.000000 libsmraw-20240310/libsmraw.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-03-10 05:06:12.000000 libsmraw-20240310/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/libsmraw-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-03-10 05:19:49.000000 libsmraw-20240310/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/libsmraw-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/libsmraw-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-10 05:06:09.000000 libsmraw-20240310/dpkg/libsmraw.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-03-10 05:19:49.000000 libsmraw-20240310/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-10 05:06:09.000000 libsmraw-20240310/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1985774 2024-03-10 05:19:35.000000 libsmraw-20240310/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-10 05:19:37.000000 libsmraw-20240310/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-10 05:19:37.000000 libsmraw-20240310/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_tools_signal/smraw_test_tools_signal.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26907 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/libsmraw.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_filename/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5818 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_filename/smraw_test_filename.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_write/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5647 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_write/smraw_test_write.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw.net/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4594 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/smraw.net/smraw.net.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smrawverify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8066 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/smrawverify/smrawverify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_glob/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5479 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_glob/smraw_test_glob.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smrawmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7841 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/smrawmount/smrawmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1251 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5563 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_error/smraw_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6475 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_handle/smraw_test_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_tools_output/smraw_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_information_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6258 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_information_file/smraw_test_information_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libsmraw/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7472 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libsmraw/libsmraw.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5815 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_support/smraw_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/pysmraw/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6401 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/pysmraw/pysmraw.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_io_handle/smraw_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23121 2024-03-10 05:19:37.000000 libsmraw-20240310/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7854 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-10 05:06:32.000000 libsmraw-20240310/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/msvscpp/smraw_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5650 2024-03-10 05:06:43.000000 libsmraw-20240310/msvscpp/smraw_test_notify/smraw_test_notify.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      176 2024-03-10 05:06:10.000000 libsmraw-20240310/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30669 2024-03-10 05:19:37.000000 libsmraw-20240310/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-10 05:19:11.000000 libsmraw-20240310/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-03-10 05:06:09.000000 libsmraw-20240310/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-10 05:19:37.000000 libsmraw-20240310/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32353 2024-03-10 05:19:37.000000 libsmraw-20240310/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 05:19:09.000000 libsmraw-20240310/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-10 05:06:09.000000 libsmraw-20240310/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-03-10 05:06:09.000000 libsmraw-20240310/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-10 05:19:37.000000 libsmraw-20240310/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-10 05:06:09.000000 libsmraw-20240310/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4324 2024-03-10 05:07:12.000000 libsmraw-20240310/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:14:22.000000 libsmraw-20240310/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/libsmraw/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2679 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_information_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1503 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1324 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_filename.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21622 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_information_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_filename.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1866 2023-12-03 09:14:27.000000 libsmraw-20240310/libsmraw/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13206 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   147172 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56308 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2024-03-10 05:19:49.000000 libsmraw-20240310/libsmraw/libsmraw_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3646 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39358 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3268 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2024-03-10 05:19:49.000000 libsmraw-20240310/libsmraw/libsmraw.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-03-10 05:06:11.000000 libsmraw-20240310/libsmraw/libsmraw_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33765 2024-03-10 05:19:37.000000 libsmraw-20240310/libsmraw/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32759 2024-03-10 05:19:37.000000 libsmraw-20240310/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-10 05:19:17.000000 libsmraw-20240310/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-10 05:19:38.000000 libsmraw-20240310/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/smrawtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6328 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/storage_media_buffer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2995 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3246 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_find.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3367 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18984 2024-03-10 05:07:04.000000 libsmraw-20240310/smrawtools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16509 2024-03-10 05:07:04.000000 libsmraw-20240310/smrawtools/smrawmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10555 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2719 2023-12-03 09:14:26.000000 libsmraw-20240310/smrawtools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_glob.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20772 2024-03-10 05:07:04.000000 libsmraw-20240310/smrawtools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11862 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawverify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3625 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20791 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/process_status.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40796 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/verification_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5348 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/verification_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5938 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2295 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2847 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_system_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3685 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/process_status.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libsmraw.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13969 2024-03-10 05:07:04.000000 libsmraw-20240310/smrawtools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35746 2024-03-10 05:19:37.000000 libsmraw-20240310/smrawtools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13489 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_glob.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4366 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/smrawtools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1875 2024-03-10 05:06:11.000000 libsmraw-20240310/smrawtools/storage_media_buffer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2478 2024-03-10 05:19:49.000000 libsmraw-20240310/libsmraw.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29947 2024-03-10 05:19:37.000000 libsmraw-20240310/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-10 05:19:15.000000 libsmraw-20240310/libcpath/libcpath_path.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/pysmraw/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_file_objects_io_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2023-12-03 09:14:28.000000 libsmraw-20240310/pysmraw/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16022 2024-03-10 05:07:04.000000 libsmraw-20240310/pysmraw/pysmraw.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3076 2024-03-10 05:07:04.000000 libsmraw-20240310/pysmraw/pysmraw_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1278 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2281 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4969 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_file_objects_io_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_libsmraw.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2024-03-10 05:07:04.000000 libsmraw-20240310/pysmraw/pysmraw.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-03-10 05:06:11.000000 libsmraw-20240310/pysmraw/pysmraw_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42537 2024-03-10 05:19:37.000000 libsmraw-20240310/pysmraw/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38622 2024-03-10 05:07:04.000000 libsmraw-20240310/pysmraw/pysmraw_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2023-12-03 09:14:23.000000 libsmraw-20240310/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11380 2024-03-10 05:06:12.000000 libsmraw-20240310/manuals/libsmraw.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      160 2023-12-03 09:14:28.000000 libsmraw-20240310/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 05:06:12.000000 libsmraw-20240310/manuals/smrawmount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26874 2024-03-10 05:19:37.000000 libsmraw-20240310/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libsmraw.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_write_functions.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11240 2024-03-10 05:07:04.000000 libsmraw-20240310/tests/pysmraw_test_handle.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4056 2024-03-10 05:07:04.000000 libsmraw-20240310/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2024-03-10 05:07:04.000000 libsmraw-20240310/tests/smraw_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5259 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_filename.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11452 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_write.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3970 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/smraw_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3305 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_glob.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9191 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/smraw_test_information_file.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4078 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libuna.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3340 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_smrawverify.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15315 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/smraw_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/pysmraw_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    12283 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_glob.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69597 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/smraw_test_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57455 2024-03-10 05:19:38.000000 libsmraw-20240310/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10720 2024-03-10 05:06:43.000000 libsmraw-20240310/tests/smraw_test_functions.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4103 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-03-10 05:06:12.000000 libsmraw-20240310/tests/smraw_test_libhmac.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-03-10 05:06:11.000000 libsmraw-20240310/ossfuzz/ossfuzz_libsmraw.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3039 2024-03-10 05:06:11.000000 libsmraw-20240310/ossfuzz/handle_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2023-12-03 09:14:30.000000 libsmraw-20240310/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-10 05:06:11.000000 libsmraw-20240310/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32157 2024-03-10 05:19:37.000000 libsmraw-20240310/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-10 05:19:30.000000 libsmraw-20240310/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32479 2024-03-10 05:19:37.000000 libsmraw-20240310/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-03-10 05:19:22.000000 libsmraw-20240310/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30727 2024-03-10 05:19:37.000000 libsmraw-20240310/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-10 05:19:16.000000 libsmraw-20240310/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:27.000000 libsmraw-20240310/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:28.000000 libsmraw-20240310/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:28.000000 libsmraw-20240310/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:28.000000 libsmraw-20240310/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:28.000000 libsmraw-20240310/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:28.000000 libsmraw-20240310/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:28.000000 libsmraw-20240310/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:28.000000 libsmraw-20240310/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:28.000000 libsmraw-20240310/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:28.000000 libsmraw-20240310/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-03-10 05:19:49.000000 libsmraw-20240310/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:28.000000 libsmraw-20240310/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:28.000000 libsmraw-20240310/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53471 2024-03-10 05:19:37.000000 libsmraw-20240310/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-10 05:19:25.000000 libsmraw-20240310/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40920 2024-03-10 05:19:37.000000 libsmraw-20240310/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1634 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35080 2024-03-10 05:19:37.000000 libsmraw-20240310/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-10 05:19:21.000000 libsmraw-20240310/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:26.000000 libsmraw-20240310/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29781 2024-03-10 05:19:37.000000 libsmraw-20240310/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-10 05:19:14.000000 libsmraw-20240310/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-10 05:38:25.000000 libsmraw-20240310/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-10 05:19:10.000000 libsmraw-20240310/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29294 2024-03-10 05:19:37.000000 libsmraw-20240310/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56852 2024-03-10 05:19:33.000000 libsmraw-20240310/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8036 2024-03-10 05:06:09.000000 libsmraw-20240310/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-03-10 05:38:28.490536 libsmraw-20240310/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33754 2024-05-06 03:41:21.000000 libsmraw-20240506/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-06 03:41:02.000000 libsmraw-20240506/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-05 12:42:17.000000 libsmraw-20240506/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-06 03:41:20.000000 libsmraw-20240506/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 12:42:17.000000 libsmraw-20240506/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-06 03:41:21.000000 libsmraw-20240506/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-10 05:06:12.000000 libsmraw-20240506/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-06 03:41:15.000000 libsmraw-20240506/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-06 03:41:14.000000 libsmraw-20240506/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-06 03:41:14.000000 libsmraw-20240506/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-06 03:41:15.000000 libsmraw-20240506/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-06 03:41:14.000000 libsmraw-20240506/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-03-10 05:06:12.000000 libsmraw-20240506/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:28.000000 libsmraw-20240506/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-05 12:42:23.000000 libsmraw-20240506/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-10 05:06:12.000000 libsmraw-20240506/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-05 12:47:03.000000 libsmraw-20240506/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23825 2024-05-06 03:41:40.000000 libsmraw-20240506/include/libsmraw.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/include/libsmraw/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2330 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-05-06 03:41:40.000000 libsmraw-20240506/include/libsmraw/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-05-06 03:41:40.000000 libsmraw-20240506/include/libsmraw/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-06 03:41:40.000000 libsmraw-20240506/include/libsmraw/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27931 2024-05-06 03:41:20.000000 libsmraw-20240506/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23825 2024-05-05 12:42:19.000000 libsmraw-20240506/include/libsmraw.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/smraw.net/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1077 2024-05-05 12:42:20.000000 libsmraw-20240506/smraw.net/smraw.net.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      166 2024-05-05 12:47:14.000000 libsmraw-20240506/smraw.net/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-05-05 12:42:20.000000 libsmraw-20240506/smraw.net/smraw.net.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2024-05-05 12:42:20.000000 libsmraw-20240506/smraw.net/smraw.net_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1075 2024-05-06 03:41:41.000000 libsmraw-20240506/smraw.net/smraw.net.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1223 2024-05-05 12:42:20.000000 libsmraw-20240506/smraw.net/smraw.net.cpp
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22297 2024-05-06 03:41:21.000000 libsmraw-20240506/smraw.net/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16867 2024-05-05 12:42:20.000000 libsmraw-20240506/smraw.net/smraw.net_handle.cpp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-05 12:42:19.000000 libsmraw-20240506/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-05 12:42:19.000000 libsmraw-20240506/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-05 12:42:19.000000 libsmraw-20240506/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-05 12:42:19.000000 libsmraw-20240506/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-05 12:42:19.000000 libsmraw-20240506/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-05 12:42:19.000000 libsmraw-20240506/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-05 12:42:19.000000 libsmraw-20240506/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-05 12:47:03.000000 libsmraw-20240506/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-05 12:42:19.000000 libsmraw-20240506/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-06 03:41:40.000000 libsmraw-20240506/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18203 2024-05-06 03:41:20.000000 libsmraw-20240506/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19269 2024-05-06 03:41:41.000000 libsmraw-20240506/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-05 12:42:19.000000 libsmraw-20240506/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-05 12:42:19.000000 libsmraw-20240506/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-05 12:42:19.000000 libsmraw-20240506/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24965 2024-05-06 03:41:20.000000 libsmraw-20240506/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3457 2024-05-05 12:42:17.000000 libsmraw-20240506/libsmraw.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30163 2024-05-06 03:41:21.000000 libsmraw-20240506/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-06 03:40:51.000000 libsmraw-20240506/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30672 2024-05-06 03:41:21.000000 libsmraw-20240506/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-06 03:41:01.000000 libsmraw-20240506/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-05 12:48:56.000000 libsmraw-20240506/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34015 2024-05-06 03:41:20.000000 libsmraw-20240506/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-06 03:40:43.000000 libsmraw-20240506/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:14:22.000000 libsmraw-20240506/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-06 03:41:20.000000 libsmraw-20240506/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      682 2024-05-05 12:42:17.000000 libsmraw-20240506/libsmraw.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-05 12:42:22.000000 libsmraw-20240506/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/libsmraw-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-06 03:41:40.000000 libsmraw-20240506/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/libsmraw-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/libsmraw-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-05 12:42:17.000000 libsmraw-20240506/dpkg/libsmraw.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-05-06 03:41:41.000000 libsmraw-20240506/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-05 12:42:17.000000 libsmraw-20240506/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1991632 2024-05-06 03:41:19.000000 libsmraw-20240506/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-06 03:41:20.000000 libsmraw-20240506/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-06 03:41:20.000000 libsmraw-20240506/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_tools_signal/smraw_test_tools_signal.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26907 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/libsmraw.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_filename/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5818 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_filename/smraw_test_filename.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_write/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5647 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_write/smraw_test_write.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw.net/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4594 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/smraw.net/smraw.net.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smrawverify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8066 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/smrawverify/smrawverify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_glob/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5479 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_glob/smraw_test_glob.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smrawmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7841 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/smrawmount/smrawmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1222 2024-05-05 12:47:22.000000 libsmraw-20240506/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5563 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_error/smraw_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6475 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_handle/smraw_test_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_tools_output/smraw_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_information_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6258 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_information_file/smraw_test_information_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libsmraw/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7472 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libsmraw/libsmraw.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5815 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_support/smraw_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/pysmraw/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6401 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/pysmraw/pysmraw.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_io_handle/smraw_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23177 2024-05-06 03:41:21.000000 libsmraw-20240506/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7854 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-05 12:43:19.000000 libsmraw-20240506/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/msvscpp/smraw_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5650 2024-05-05 12:43:52.000000 libsmraw-20240506/msvscpp/smraw_test_notify/smraw_test_notify.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      176 2024-05-05 12:42:19.000000 libsmraw-20240506/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30996 2024-05-06 03:41:21.000000 libsmraw-20240506/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-06 03:40:49.000000 libsmraw-20240506/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-05-05 12:42:17.000000 libsmraw-20240506/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-06 03:41:20.000000 libsmraw-20240506/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32909 2024-05-06 03:41:21.000000 libsmraw-20240506/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-06 03:40:45.000000 libsmraw-20240506/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-05 12:42:17.000000 libsmraw-20240506/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-05-05 12:42:17.000000 libsmraw-20240506/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-06 03:41:20.000000 libsmraw-20240506/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-05 12:42:17.000000 libsmraw-20240506/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4324 2024-05-05 12:44:09.000000 libsmraw-20240506/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:14:22.000000 libsmraw-20240506/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/libsmraw/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2679 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_information_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1503 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1324 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_filename.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21622 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_information_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5288 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_filename.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-05-05 12:47:34.000000 libsmraw-20240506/libsmraw/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13206 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   147172 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56308 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2024-05-06 03:41:40.000000 libsmraw-20240506/libsmraw/libsmraw_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3646 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39358 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3268 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2024-05-06 03:41:40.000000 libsmraw-20240506/libsmraw/libsmraw.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-05-05 12:42:20.000000 libsmraw-20240506/libsmraw/libsmraw_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34165 2024-05-06 03:41:21.000000 libsmraw-20240506/libsmraw/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33348 2024-05-06 03:41:21.000000 libsmraw-20240506/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-06 03:40:59.000000 libsmraw-20240506/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-06 03:41:21.000000 libsmraw-20240506/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/smrawtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6328 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/storage_media_buffer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2995 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3246 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_find.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3367 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18984 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16509 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/smrawmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10555 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2715 2024-05-05 12:48:27.000000 libsmraw-20240506/smrawtools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_glob.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20772 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11862 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawverify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3625 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20791 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/process_status.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40796 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/verification_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5348 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/verification_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5938 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2295 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2847 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_system_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3685 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/process_status.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libsmraw.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13969 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36479 2024-05-06 03:41:21.000000 libsmraw-20240506/smrawtools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13489 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_glob.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4366 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/smrawtools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-05 12:42:21.000000 libsmraw-20240506/smrawtools/smrawtools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-05-05 12:44:02.000000 libsmraw-20240506/smrawtools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1875 2024-05-05 12:42:22.000000 libsmraw-20240506/smrawtools/storage_media_buffer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2480 2024-05-06 03:41:41.000000 libsmraw-20240506/libsmraw.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30194 2024-05-06 03:41:21.000000 libsmraw-20240506/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-06 03:40:56.000000 libsmraw-20240506/libcpath/libcpath_path.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/pysmraw/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_file_objects_io_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2024-05-05 12:48:20.000000 libsmraw-20240506/pysmraw/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16022 2024-05-05 12:44:02.000000 libsmraw-20240506/pysmraw/pysmraw.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3076 2024-05-05 12:44:02.000000 libsmraw-20240506/pysmraw/pysmraw_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1278 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2281 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4969 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_file_objects_io_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_libsmraw.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2024-05-05 12:44:02.000000 libsmraw-20240506/pysmraw/pysmraw.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-05-05 12:42:21.000000 libsmraw-20240506/pysmraw/pysmraw_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42993 2024-05-06 03:41:21.000000 libsmraw-20240506/pysmraw/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38622 2024-05-05 12:44:02.000000 libsmraw-20240506/pysmraw/pysmraw_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1385 2023-12-03 09:14:23.000000 libsmraw-20240506/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11380 2024-05-05 12:42:22.000000 libsmraw-20240506/manuals/libsmraw.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      131 2024-05-05 12:48:08.000000 libsmraw-20240506/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 12:42:22.000000 libsmraw-20240506/manuals/smrawmount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26930 2024-05-06 03:41:21.000000 libsmraw-20240506/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libsmraw.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1488 2024-05-05 13:08:41.000000 libsmraw-20240506/tests/test_write_functions.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11240 2024-05-05 12:44:02.000000 libsmraw-20240506/tests/pysmraw_test_handle.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4025 2024-05-05 12:44:46.000000 libsmraw-20240506/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2024-05-05 12:44:19.000000 libsmraw-20240506/tests/smraw_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5259 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_filename.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11452 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_write.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5021 2024-05-05 12:48:00.000000 libsmraw-20240506/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3970 2024-05-05 12:43:52.000000 libsmraw-20240506/tests/smraw_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3305 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_glob.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9191 2024-05-05 12:43:52.000000 libsmraw-20240506/tests/smraw_test_information_file.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4407 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libuna.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3309 2024-05-05 12:45:14.000000 libsmraw-20240506/tests/test_smrawverify.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15315 2024-05-05 12:43:52.000000 libsmraw-20240506/tests/smraw_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/pysmraw_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    12252 2024-05-05 13:08:08.000000 libsmraw-20240506/tests/test_glob.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69597 2024-05-05 12:43:52.000000 libsmraw-20240506/tests/smraw_test_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58265 2024-05-06 03:41:21.000000 libsmraw-20240506/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10720 2024-05-05 12:43:52.000000 libsmraw-20240506/tests/smraw_test_functions.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4072 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-05 12:42:22.000000 libsmraw-20240506/tests/smraw_test_libhmac.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:58.000000 libsmraw-20240506/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-05-05 12:42:20.000000 libsmraw-20240506/ossfuzz/ossfuzz_libsmraw.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3039 2024-05-05 12:42:20.000000 libsmraw-20240506/ossfuzz/handle_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      900 2024-05-05 12:47:42.000000 libsmraw-20240506/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-05 12:42:20.000000 libsmraw-20240506/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32276 2024-05-06 03:41:21.000000 libsmraw-20240506/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-06 03:41:14.000000 libsmraw-20240506/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33059 2024-05-06 03:41:21.000000 libsmraw-20240506/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-06 03:41:06.000000 libsmraw-20240506/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31091 2024-05-06 03:41:21.000000 libsmraw-20240506/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-06 03:40:57.000000 libsmraw-20240506/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:28.000000 libsmraw-20240506/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:28.000000 libsmraw-20240506/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:28.000000 libsmraw-20240506/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:28.000000 libsmraw-20240506/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:28.000000 libsmraw-20240506/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:28.000000 libsmraw-20240506/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:28.000000 libsmraw-20240506/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:28.000000 libsmraw-20240506/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:28.000000 libsmraw-20240506/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-06 03:41:40.000000 libsmraw-20240506/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:28.000000 libsmraw-20240506/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:28.000000 libsmraw-20240506/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56675 2024-05-06 03:41:21.000000 libsmraw-20240506/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-06 03:41:09.000000 libsmraw-20240506/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40858 2024-05-06 03:41:20.000000 libsmraw-20240506/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:57.000000 libsmraw-20240506/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35880 2024-05-06 03:41:21.000000 libsmraw-20240506/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-06 03:41:04.000000 libsmraw-20240506/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:56.000000 libsmraw-20240506/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30032 2024-05-06 03:41:21.000000 libsmraw-20240506/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-06 03:40:54.000000 libsmraw-20240506/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-06 04:00:55.000000 libsmraw-20240506/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-06 03:40:47.000000 libsmraw-20240506/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29499 2024-05-06 03:41:21.000000 libsmraw-20240506/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56852 2024-05-06 03:41:17.000000 libsmraw-20240506/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8036 2024-05-06 03:26:20.000000 libsmraw-20240506/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-05-06 04:00:58.934686 libsmraw-20240506/PKG-INFO
```

### Comparing `libsmraw-20240310/libfdata/libfdata_error.h` & `libsmraw-20240506/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_area.c` & `libsmraw-20240506/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_stream.h` & `libsmraw-20240506/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_cache.h` & `libsmraw-20240506/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_range_list.c` & `libsmraw-20240506/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_mapped_range.c` & `libsmraw-20240506/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_libcerror.h` & `libsmraw-20240506/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_definitions.h` & `libsmraw-20240506/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libsmraw-20240310/libfdata/libfdata_list.c` & `libsmraw-20240506/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_libcdata.h` & `libsmraw-20240506/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_list.h` & `libsmraw-20240506/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_list_element.h` & `libsmraw-20240506/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/Makefile.am` & `libsmraw-20240506/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libsmraw-20240310/libfdata/libfdata_libcnotify.h` & `libsmraw-20240506/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_extern.h` & `libsmraw-20240506/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_notify.c` & `libsmraw-20240506/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_cache.c` & `libsmraw-20240506/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_stream.c` & `libsmraw-20240506/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_unused.h` & `libsmraw-20240506/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_range.h` & `libsmraw-20240506/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_area.h` & `libsmraw-20240506/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_error.c` & `libsmraw-20240506/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_support.h` & `libsmraw-20240506/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_range.c` & `libsmraw-20240506/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_mapped_range.h` & `libsmraw-20240506/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_support.c` & `libsmraw-20240506/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_list_element.c` & `libsmraw-20240506/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_segments_array.c` & `libsmraw-20240506/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_types.h` & `libsmraw-20240506/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_notify.h` & `libsmraw-20240506/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_range_list.h` & `libsmraw-20240506/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_segments_array.h` & `libsmraw-20240506/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/Makefile.in` & `libsmraw-20240506/libfdata/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -544,16 +546,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -577,15 +579,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -797,24 +800,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -910,17 +928,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libfdata/libfdata_vector.c` & `libsmraw-20240506/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_libfcache.h` & `libsmraw-20240506/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfdata/libfdata_vector.h` & `libsmraw-20240506/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/COPYING` & `libsmraw-20240506/COPYING`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/install-sh` & `libsmraw-20240506/install-sh`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/depcomp` & `libsmraw-20240506/depcomp`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libcfile.m4` & `libsmraw-20240506/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
@@ -203,15 +203,15 @@
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -357,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/tests.m4` & `libsmraw-20240506/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libcpath.m4` & `libsmraw-20240506/m4/libcpath.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
@@ -152,15 +152,15 @@
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -272,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/lib-prefix.m4` & `libsmraw-20240506/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/progtest.m4` & `libsmraw-20240506/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libuna.m4` & `libsmraw-20240506/m4/libuna.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -942,15 +942,15 @@
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -972,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/gettext.m4` & `libsmraw-20240506/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/lib-ld.m4` & `libsmraw-20240506/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libclocale.m4` & `libsmraw-20240506/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
@@ -126,15 +126,15 @@
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -219,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/libcdata.m4` & `libsmraw-20240506/m4/libcdata.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
@@ -497,15 +497,15 @@
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -527,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/libcsplit.m4` & `libsmraw-20240506/m4/libcsplit.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
@@ -147,15 +147,15 @@
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -177,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/common.m4` & `libsmraw-20240506/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libcthreads.m4` & `libsmraw-20240506/m4/libcthreads.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
@@ -246,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -288,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libsmraw-20240310/m4/ltversion.m4` & `libsmraw-20240506/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/ltsugar.m4` & `libsmraw-20240506/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libfdata.m4` & `libsmraw-20240506/m4/libfdata.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
@@ -454,15 +454,15 @@
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -484,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/host-cpu-c-abi.m4` & `libsmraw-20240506/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libfuse.m4` & `libsmraw-20240506/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libsmraw-20240310/m4/libtool.m4` & `libsmraw-20240506/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/po.m4` & `libsmraw-20240506/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libcerror.m4` & `libsmraw-20240506/m4/libcerror.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
@@ -99,15 +99,15 @@
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/libcnotify.m4` & `libsmraw-20240506/m4/libcnotify.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
@@ -96,15 +96,15 @@
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -137,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/libbfio.m4` & `libsmraw-20240506/m4/libbfio.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
@@ -320,15 +320,15 @@
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -350,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/libhmac.m4` & `libsmraw-20240506/m4/libhmac.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libhmac required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libhmac is available
 dnl ac_libhmac_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBHMAC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno],
     [ac_cv_libhmac=no],
@@ -165,15 +165,15 @@
           [ac_cv_libhmac_dummy=yes],
           [ac_cv_libhmac=no])
 
         ac_cv_libhmac_LIBADD="-lhmac"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
+      [test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libhmac in directory: $ac_cv_with_libhmac],
         [1])
       ])
     ])
 
   AS_IF(
@@ -243,15 +243,15 @@
     [ac_cv_libhmac_sha256=$ac_cv_libcrypto_sha256])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno],
     [ac_cv_libhmac_sha512=local],
     [ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512])
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
   ])
 
 dnl Function to detect how to enable libhmac
 AC_DEFUN([AX_LIBHMAC_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/intlmacosx.m4` & `libsmraw-20240506/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/lt~obsolete.m4` & `libsmraw-20240506/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/lib-link.m4` & `libsmraw-20240506/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/iconv.m4` & `libsmraw-20240506/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/ltoptions.m4` & `libsmraw-20240506/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/nls.m4` & `libsmraw-20240506/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/python.m4` & `libsmraw-20240506/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libsmraw-20240310/m4/libcrypto.m4` & `libsmraw-20240506/m4/libcrypto.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libfvalue.m4` & `libsmraw-20240506/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
@@ -589,15 +589,15 @@
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -619,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/types.m4` & `libsmraw-20240506/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/m4/libfcache.m4` & `libsmraw-20240506/m4/libfcache.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
@@ -151,15 +151,15 @@
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -195,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libsmraw-20240310/m4/pthread.m4` & `libsmraw-20240506/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw.h` & `libsmraw-20240506/include/libsmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/definitions.h.in` & `libsmraw-20240506/include/libsmraw/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/definitions.h` & `libsmraw-20240506/include/libsmraw/definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBSMRAW_DEFINIONS_H )
 #define _LIBSMRAW_DEFINIONS_H
 
 #include <libsmraw/types.h>
 
-#define LIBSMRAW_VERSION			20240310
+#define LIBSMRAW_VERSION			20240506
 
 /* The version string
  */
-#define LIBSMRAW_VERSION_STRING			"20240310"
+#define LIBSMRAW_VERSION_STRING			"20240506"
 
 /* The access flags definitions
  * bit 1					set to 1 for read access
  * bit 2					set to 1 for write access
  * bit 3        set to 1 to truncate an existing file on write
  * bit 4-8					not used
  */
```

### Comparing `libsmraw-20240310/include/libsmraw/types.h.in` & `libsmraw-20240506/include/libsmraw/types.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/types.h` & `libsmraw-20240506/include/libsmraw/types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/features.h.in` & `libsmraw-20240506/include/libsmraw/features.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/error.h` & `libsmraw-20240506/include/libsmraw/error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/extern.h` & `libsmraw-20240506/include/libsmraw/extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/features.h` & `libsmraw-20240506/include/libsmraw/features.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/libsmraw/codepage.h` & `libsmraw-20240506/include/libsmraw/codepage.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/include/Makefile.in` & `libsmraw-20240506/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -526,15 +528,20 @@
 
 EXTRA_DIST = \
 	libsmraw.h.in \
 	libsmraw/definitions.h.in \
 	libsmraw/features.h.in \
 	libsmraw/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmraw.h \
+	libsmraw/definitions.h \
+	libsmraw/features.h \
+	libsmraw/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -731,23 +738,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -829,17 +838,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsmraw.h
-	-rm -f libsmraw/definitions.h
-	-rm -f libsmraw/features.h
-	-rm -f libsmraw/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/include/libsmraw.h.in` & `libsmraw-20240506/include/libsmraw.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smraw.net/smraw.net.rc.in` & `libsmraw-20240506/smraw.net/smraw.net.rc.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smraw.net/smraw.net.h` & `libsmraw-20240506/smraw.net/smraw.net.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smraw.net/smraw.net_handle.h` & `libsmraw-20240506/smraw.net/smraw.net_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smraw.net/smraw.net.rc` & `libsmraw-20240506/smraw.net/smraw.net.rc`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Managed .Net wrapper library for libsmraw\0"
-      VALUE "FileVersion",		"20240310" "\0"
+      VALUE "FileVersion",		"20240506" "\0"
       VALUE "InternalName",		"smraw.net.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"smraw.net.dll\0"
       VALUE "ProductName",		"smraw.net\0"
-      VALUE "ProductVersion",		"20240310" "\0"
+      VALUE "ProductVersion",		"20240506" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libsmraw/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libsmraw-20240310/smraw.net/smraw.net.cpp` & `libsmraw-20240506/smraw.net/smraw.net.cpp`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smraw.net/Makefile.in` & `libsmraw-20240506/smraw.net/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -396,14 +396,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -467,15 +469,16 @@
 top_srcdir = @top_srcdir@
 EXTRA_DIST = \
 	smraw.net.cpp smraw.net.h \
 	smraw.net_handle.cpp smraw.net_handle.h \
 	smraw.net.rc \
 	smraw.net.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -581,23 +584,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -676,13 +681,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/smraw.net/smraw.net_handle.cpp` & `libsmraw-20240506/smraw.net/smraw.net_handle.cpp`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/config_borlandc.h` & `libsmraw-20240506/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/file_stream.h` & `libsmraw-20240506/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/memory.h` & `libsmraw-20240506/common/memory.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/byte_stream.h` & `libsmraw-20240506/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/common.h` & `libsmraw-20240506/common/common.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/config_winapi.h` & `libsmraw-20240506/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/system_string.h` & `libsmraw-20240506/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/types.h.in` & `libsmraw-20240506/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/types.h` & `libsmraw-20240506/common/types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/config.h.in` & `libsmraw-20240506/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,17 @@
 
 /* Define to 1 if you have the <libfdata.h> header file. */
 #undef HAVE_LIBFDATA_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 #undef HAVE_LIBFVALUE
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 #undef HAVE_LIBFVALUE_H
 
 /* Define to 1 if you have the `hmac' library (-lhmac). */
```

### Comparing `libsmraw-20240310/common/config.h` & `libsmraw-20240506/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,18 @@
 /* Define to 1 if you have the `fdata' library (-lfdata). */
 /* #undef HAVE_LIBFDATA */
 
 /* Define to 1 if you have the <libfdata.h> header file. */
 /* #undef HAVE_LIBFDATA_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 /* #undef HAVE_LIBFVALUE */
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 /* #undef HAVE_LIBFVALUE_H */
 
@@ -601,24 +604,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libsmraw"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libsmraw 20240310"
+#define PACKAGE_STRING "libsmraw 20240506"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libsmraw"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240310"
+#define PACKAGE_VERSION "20240506"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -639,15 +642,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240310"
+#define VERSION "20240506"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libsmraw-20240310/common/wide_string.h` & `libsmraw-20240506/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/narrow_string.h` & `libsmraw-20240506/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/config_msc.h` & `libsmraw-20240506/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/common/Makefile.in` & `libsmraw-20240506/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -414,14 +414,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -479,15 +481,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -495,15 +499,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -671,23 +678,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -767,15 +776,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/libsmraw.spec.in` & `libsmraw-20240506/libsmraw.spec.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_wide_string.c` & `libsmraw-20240506/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_support.h` & `libsmraw-20240506/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/Makefile.am` & `libsmraw-20240506/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libsmraw-20240310/libclocale/libclocale_definitions.h` & `libsmraw-20240506/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libsmraw-20240310/libclocale/libclocale_unused.h` & `libsmraw-20240506/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_libcerror.h` & `libsmraw-20240506/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_locale.h` & `libsmraw-20240506/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_support.c` & `libsmraw-20240506/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_codepage.c` & `libsmraw-20240506/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_locale.c` & `libsmraw-20240506/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/Makefile.in` & `libsmraw-20240506/libclocale/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -458,14 +458,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -525,30 +527,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -751,24 +754,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -855,17 +864,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libclocale/libclocale_extern.h` & `libsmraw-20240506/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_wide_string.h` & `libsmraw-20240506/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libclocale/libclocale_codepage.h` & `libsmraw-20240506/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_libcdata.h` & `libsmraw-20240506/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_types.h` & `libsmraw-20240506/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_cache_value.c` & `libsmraw-20240506/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_unused.h` & `libsmraw-20240506/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/Makefile.am` & `libsmraw-20240506/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libsmraw-20240310/libfcache/libfcache_support.h` & `libsmraw-20240506/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_error.h` & `libsmraw-20240506/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_support.c` & `libsmraw-20240506/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_cache.h` & `libsmraw-20240506/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_error.c` & `libsmraw-20240506/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_libcerror.h` & `libsmraw-20240506/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_date_time.c` & `libsmraw-20240506/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_extern.h` & `libsmraw-20240506/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_cache_value.h` & `libsmraw-20240506/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/Makefile.in` & `libsmraw-20240506/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -527,16 +529,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -548,15 +550,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -760,24 +763,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -865,17 +875,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libfcache/libfcache_date_time.h` & `libsmraw-20240506/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfcache/libfcache_definitions.h` & `libsmraw-20240506/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libsmraw-20240310/libfcache/libfcache_cache.c` & `libsmraw-20240506/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/Makefile.am` & `libsmraw-20240506/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libsmraw.pc \
+	libsmraw.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libsmraw.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -91,19 +98,7 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libsmraw && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libsmraw.pc
-	-rm -f libsmraw.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_range.h` & `libsmraw-20240506/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_range_io_handle.c` & `libsmraw-20240506/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_support.c` & `libsmraw-20240506/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libcpath.h` & `libsmraw-20240506/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_error.h` & `libsmraw-20240506/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libclocale.h` & `libsmraw-20240506/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_error.c` & `libsmraw-20240506/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libuna.h` & `libsmraw-20240506/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_io_handle.h` & `libsmraw-20240506/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_pool.h` & `libsmraw-20240506/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_range.c` & `libsmraw-20240506/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_types.h` & `libsmraw-20240506/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_unused.h` & `libsmraw-20240506/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libcdata.h` & `libsmraw-20240506/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file.h` & `libsmraw-20240506/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/Makefile.am` & `libsmraw-20240506/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libcfile.h` & `libsmraw-20240506/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_definitions.h` & `libsmraw-20240506/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libsmraw-20240310/libbfio/libbfio_codepage.h` & `libsmraw-20240506/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_io_handle.c` & `libsmraw-20240506/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_support.h` & `libsmraw-20240506/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_memory_range.h` & `libsmraw-20240506/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_pool.c` & `libsmraw-20240506/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file_range_io_handle.h` & `libsmraw-20240506/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libcthreads.h` & `libsmraw-20240506/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_system_string.h` & `libsmraw-20240506/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_memory_range_io_handle.c` & `libsmraw-20240506/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_handle.c` & `libsmraw-20240506/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_file.c` & `libsmraw-20240506/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_handle.h` & `libsmraw-20240506/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_memory_range.c` & `libsmraw-20240506/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_pool.c` & `libsmraw-20240506/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_libcerror.h` & `libsmraw-20240506/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/Makefile.in` & `libsmraw-20240506/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -479,14 +479,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -545,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -585,15 +587,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,24 +807,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -890,14 +907,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -908,23 +927,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/libbfio/libbfio_system_string.c` & `libsmraw-20240506/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_memory_range_io_handle.h` & `libsmraw-20240506/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_extern.h` & `libsmraw-20240506/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/libbfio/libbfio_pool.h` & `libsmraw-20240506/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsmraw-20240310/config.guess` & `libsmraw-20240506/config.guess`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw.pc.in` & `libsmraw-20240506/libsmraw.pc.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/dpkg/copyright` & `libsmraw-20240506/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/dpkg/control` & `libsmraw-20240506/dpkg/control`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/dpkg/rules` & `libsmraw-20240506/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/COPYING.LESSER` & `libsmraw-20240506/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/configure` & `libsmraw-20240506/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libsmraw 20240310.
+# Generated by GNU Autoconf 2.71 for libsmraw 20240506.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libsmraw'
 PACKAGE_TARNAME='libsmraw'
-PACKAGE_VERSION='20240310'
-PACKAGE_STRING='libsmraw 20240310'
+PACKAGE_VERSION='20240506'
+PACKAGE_STRING='libsmraw 20240506'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libsmraw.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 ax_libhmac_spec_build_requires
 ax_libhmac_spec_requires
 ax_libhmac_pc_libs_private
 LIBHMAC_LIBADD
 LIBHMAC_CPPFLAGS
 HAVE_LOCAL_LIBHMAC_FALSE
 HAVE_LOCAL_LIBHMAC_TRUE
@@ -1115,14 +1117,16 @@
 libfdata_LIBS
 libfvalue_CFLAGS
 libfvalue_LIBS
 libhmac_CFLAGS
 libhmac_LIBS
 openssl_CFLAGS
 openssl_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1665,15 +1669,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libsmraw 20240310 to adapt to many kinds of systems.
+\`configure' configures libsmraw 20240506 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1736,15 +1740,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libsmraw 20240310:";;
+     short | recursive ) echo "Configuration of libsmraw 20240506:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1927,14 +1931,17 @@
               C compiler flags for libhmac, overriding pkg-config
   libhmac_LIBS
               linker flags for libhmac, overriding pkg-config
   openssl_CFLAGS
               C compiler flags for openssl, overriding pkg-config
   openssl_LIBS
               linker flags for openssl, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1997,15 +2004,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libsmraw configure 20240310
+libsmraw configure 20240506
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2718,15 +2725,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libsmraw $as_me 20240310, which was
+It was created by libsmraw $as_me 20240506, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4207,15 +4214,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libsmraw'
- VERSION='20240310'
+ VERSION='20240506'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -24302,15 +24309,15 @@
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24452,15 +24459,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -26194,15 +26201,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -27114,15 +27121,15 @@
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -30990,15 +30997,15 @@
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31023,15 +31030,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31657,15 +31664,15 @@
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31821,15 +31828,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -32358,15 +32365,15 @@
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32421,15 +32428,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -33223,15 +33230,15 @@
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33256,15 +33263,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -40545,15 +40552,15 @@
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40578,15 +40585,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -41846,15 +41853,15 @@
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42168,15 +42175,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -43052,15 +43059,15 @@
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43250,15 +43257,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -45447,15 +45454,15 @@
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45480,15 +45487,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -46479,15 +46486,15 @@
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46580,15 +46587,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -49947,15 +49954,15 @@
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49980,15 +49987,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -54373,15 +54380,15 @@
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54406,15 +54413,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -54725,16 +54732,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -55904,15 +55915,15 @@
 
 
         ac_cv_libhmac_LIBADD="-lhmac"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
+    if test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libhmac in directory: $ac_cv_with_libhmac
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -60204,15 +60215,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno
 then :
   ac_cv_libhmac_sha512=local
 else $as_nop
   ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512
 fi
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBHMAC 1" >>confdefs.h
@@ -60277,33 +60288,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
+
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
 
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -60371,51 +60456,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -60578,45 +60722,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -60784,29 +60921,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -60837,14 +60994,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -60852,14 +61015,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
   ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -62007,15 +62178,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libsmraw $as_me 20240310, which was
+This file was extended by libsmraw $as_me 20240506, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -62075,15 +62246,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libsmraw config.status 20240310
+libsmraw config.status 20240506
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libsmraw-20240310/compile` & `libsmraw-20240506/compile`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/missing` & `libsmraw-20240506/missing`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libfdata/libfdata.vcproj` & `libsmraw-20240506/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_tools_signal/smraw_test_tools_signal.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_tools_signal/smraw_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libsmraw.sln` & `libsmraw-20240506/msvscpp/libsmraw.sln`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_filename/smraw_test_filename.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_filename/smraw_test_filename.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_write/smraw_test_write.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_write/smraw_test_write.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw.net/smraw.net.vcproj` & `libsmraw-20240506/msvscpp/smraw.net/smraw.net.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smrawverify/smrawverify.vcproj` & `libsmraw-20240506/msvscpp/smrawverify/smrawverify.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_glob/smraw_test_glob.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_glob/smraw_test_glob.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libclocale/libclocale.vcproj` & `libsmraw-20240506/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smrawmount/smrawmount.vcproj` & `libsmraw-20240506/msvscpp/smrawmount/smrawmount.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libfcache/libfcache.vcproj` & `libsmraw-20240506/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/Makefile.am` & `libsmraw-20240506/msvscpp/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -30,13 +30,11 @@
 	smrawmount/smrawmount.vcproj \
 	smrawverify/smrawverify.vcproj \
 	libsmraw.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libsmraw-20240310/msvscpp/libbfio/libbfio.vcproj` & `libsmraw-20240506/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_error/smraw_test_error.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_error/smraw_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_handle/smraw_test_handle.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_handle/smraw_test_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcfile/libcfile.vcproj` & `libsmraw-20240506/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcdata/libcdata.vcproj` & `libsmraw-20240506/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_tools_output/smraw_test_tools_output.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_tools_output/smraw_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_information_file/smraw_test_information_file.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_information_file/smraw_test_information_file.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libsmraw/libsmraw.vcproj` & `libsmraw-20240506/msvscpp/libsmraw/libsmraw.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcthreads/libcthreads.vcproj` & `libsmraw-20240506/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_support/smraw_test_support.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_support/smraw_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcpath/libcpath.vcproj` & `libsmraw-20240506/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/pysmraw/pysmraw.vcproj` & `libsmraw-20240506/msvscpp/pysmraw/pysmraw.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_io_handle/smraw_test_io_handle.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_io_handle/smraw_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libhmac/libhmac.vcproj` & `libsmraw-20240506/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcsplit/libcsplit.vcproj` & `libsmraw-20240506/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libuna/libuna.vcproj` & `libsmraw-20240506/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/Makefile.in` & `libsmraw-20240506/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -497,15 +499,16 @@
 	smrawmount/smrawmount.vcproj \
 	smrawverify/smrawverify.vcproj \
 	libsmraw.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -609,23 +612,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -704,13 +709,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/msvscpp/libfvalue/libfvalue.vcproj` & `libsmraw-20240506/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcnotify/libcnotify.vcproj` & `libsmraw-20240506/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/libcerror/libcerror.vcproj` & `libsmraw-20240506/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/msvscpp/smraw_test_notify/smraw_test_notify.vcproj` & `libsmraw-20240506/msvscpp/smraw_test_notify/smraw_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_extern.h` & `libsmraw-20240506/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_support.h` & `libsmraw-20240506/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_unused.h` & `libsmraw-20240506/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_notify.h` & `libsmraw-20240506/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_support.c` & `libsmraw-20240506/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_types.h` & `libsmraw-20240506/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/Makefile.am` & `libsmraw-20240506/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcfile/libcfile_notify.c` & `libsmraw-20240506/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_system_string.h` & `libsmraw-20240506/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_file.h` & `libsmraw-20240506/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_libcnotify.h` & `libsmraw-20240506/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_system_string.c` & `libsmraw-20240506/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_error.h` & `libsmraw-20240506/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_libcerror.h` & `libsmraw-20240506/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_file.c` & `libsmraw-20240506/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_libclocale.h` & `libsmraw-20240506/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_winapi.h` & `libsmraw-20240506/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/Makefile.in` & `libsmraw-20240506/libcfile/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -527,16 +529,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -551,15 +553,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -764,24 +767,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -870,17 +881,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcfile/libcfile_error.c` & `libsmraw-20240506/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_libuna.h` & `libsmraw-20240506/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_winapi.c` & `libsmraw-20240506/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcfile/libcfile_definitions.h` & `libsmraw-20240506/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libsmraw-20240310/INSTALL` & `libsmraw-20240506/INSTALL`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_list_element.h` & `libsmraw-20240506/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_array.h` & `libsmraw-20240506/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_definitions.h` & `libsmraw-20240506/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libsmraw-20240310/libcdata/libcdata_libcerror.h` & `libsmraw-20240506/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_unused.h` & `libsmraw-20240506/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_btree.h` & `libsmraw-20240506/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_btree.c` & `libsmraw-20240506/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_support.c` & `libsmraw-20240506/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_list.c` & `libsmraw-20240506/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_extern.h` & `libsmraw-20240506/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_list.h` & `libsmraw-20240506/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_btree_values_list.h` & `libsmraw-20240506/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/Makefile.am` & `libsmraw-20240506/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcdata/libcdata_btree_node.h` & `libsmraw-20240506/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_range_list_value.h` & `libsmraw-20240506/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_range_list.h` & `libsmraw-20240506/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_range_list.c` & `libsmraw-20240506/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_array.c` & `libsmraw-20240506/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_list_element.c` & `libsmraw-20240506/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_libcthreads.h` & `libsmraw-20240506/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_tree_node.h` & `libsmraw-20240506/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_error.h` & `libsmraw-20240506/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_types.h` & `libsmraw-20240506/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_btree_node.c` & `libsmraw-20240506/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_tree_node.c` & `libsmraw-20240506/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_support.h` & `libsmraw-20240506/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/Makefile.in` & `libsmraw-20240506/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -475,14 +475,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -541,16 +543,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -567,15 +569,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -785,24 +788,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -896,17 +912,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcdata/libcdata_range_list_value.c` & `libsmraw-20240506/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_btree_values_list.c` & `libsmraw-20240506/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcdata/libcdata_error.c` & `libsmraw-20240506/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/config.sub` & `libsmraw-20240506/config.sub`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/setup.py` & `libsmraw-20240506/setup.py`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/acinclude.m4` & `libsmraw-20240506/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/config.rpath` & `libsmraw-20240506/config.rpath`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_extern.h` & `libsmraw-20240506/libsmraw/libsmraw_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_information_file.h` & `libsmraw-20240506/libsmraw/libsmraw_information_file.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libcnotify.h` & `libsmraw-20240506/libsmraw/libsmraw_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_types.h` & `libsmraw-20240506/libsmraw/libsmraw_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libfvalue.h` & `libsmraw-20240506/libsmraw/libsmraw_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_filename.h` & `libsmraw-20240506/libsmraw/libsmraw_filename.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_error.c` & `libsmraw-20240506/libsmraw/libsmraw_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_information_file.c` & `libsmraw-20240506/libsmraw/libsmraw_information_file.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libbfio.h` & `libsmraw-20240506/libsmraw/libsmraw_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_filename.c` & `libsmraw-20240506/libsmraw/libsmraw_filename.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/Makefile.am` & `libsmraw-20240506/libsmraw/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -61,21 +61,19 @@
 libsmraw_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libsmraw_definitions.h.in \
 	libsmraw.rc \
 	libsmraw.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmraw_definitions.h \
+	libsmraw.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libsmraw_definitions.h
-	-rm -f libsmraw.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsmraw ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsmraw_la_SOURCES)
```

### Comparing `libsmraw-20240310/libsmraw/libsmraw_io_handle.h` & `libsmraw-20240506/libsmraw/libsmraw_io_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libcerror.h` & `libsmraw-20240506/libsmraw/libsmraw_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libcthreads.h` & `libsmraw-20240506/libsmraw/libsmraw_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_unused.h` & `libsmraw-20240506/libsmraw/libsmraw_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_handle.h` & `libsmraw-20240506/libsmraw/libsmraw_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libclocale.h` & `libsmraw-20240506/libsmraw/libsmraw_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_handle.c` & `libsmraw-20240506/libsmraw/libsmraw_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_support.c` & `libsmraw-20240506/libsmraw/libsmraw_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libfdata.h` & `libsmraw-20240506/libsmraw/libsmraw_libfdata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_definitions.h` & `libsmraw-20240506/libsmraw/libsmraw_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 /* Define HAVE_LOCAL_LIBSMRAW for local use of libsmraw
  */
 #if !defined( HAVE_LOCAL_LIBSMRAW )
 #include <libsmraw/definitions.h>
 
 #else
 
-#define LIBSMRAW_VERSION				20240310
+#define LIBSMRAW_VERSION				20240506
 
 /* The version string
  */
-#define LIBSMRAW_VERSION_STRING				"20240310"
+#define LIBSMRAW_VERSION_STRING				"20240506"
 
 /* The access flags definitions
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3        set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libsmraw-20240310/libsmraw/libsmraw_support.h` & `libsmraw-20240506/libsmraw/libsmraw_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_libuna.h` & `libsmraw-20240506/libsmraw/libsmraw_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_io_handle.c` & `libsmraw-20240506/libsmraw/libsmraw_io_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_definitions.h.in` & `libsmraw-20240506/libsmraw/libsmraw_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw.c` & `libsmraw-20240506/libsmraw/libsmraw.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_error.h` & `libsmraw-20240506/libsmraw/libsmraw_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw.rc` & `libsmraw-20240506/libsmraw/libsmraw.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the storage media (SM) (split) RAW format\0"
-      VALUE "FileVersion",		"20240310" "\0"
+      VALUE "FileVersion",		"20240506" "\0"
       VALUE "InternalName",		"libsmraw.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libsmraw.dll\0"
       VALUE "ProductName",		"libsmraw\0"
-      VALUE "ProductVersion",		"20240310" "\0"
+      VALUE "ProductVersion",		"20240506" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libsmraw/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libsmraw-20240310/libsmraw/libsmraw.rc.in` & `libsmraw-20240506/libsmraw/libsmraw.rc.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_notify.c` & `libsmraw-20240506/libsmraw/libsmraw_notify.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_notify.h` & `libsmraw-20240506/libsmraw/libsmraw_notify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/libsmraw_codepage.h` & `libsmraw-20240506/libsmraw/libsmraw_codepage.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw/Makefile.in` & `libsmraw-20240506/libsmraw/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -486,14 +486,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -552,16 +554,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -616,15 +618,18 @@
 
 libsmraw_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libsmraw_definitions.h.in \
 	libsmraw.rc \
 	libsmraw.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmraw_definitions.h \
+	libsmraw.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -862,24 +867,34 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libsmraw.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_error.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_filename.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_handle.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_information_file.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_notify.Plo
+	-rm -f ./$(DEPDIR)/libsmraw_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -970,19 +985,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsmraw_definitions.h
-	-rm -f libsmraw.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsmraw ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsmraw_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread.h` & `libsmraw-20240506/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_read_write_lock.h` & `libsmraw-20240506/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread.c` & `libsmraw-20240506/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread_pool.h` & `libsmraw-20240506/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_support.h` & `libsmraw-20240506/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_lock.h` & `libsmraw-20240506/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_unused.h` & `libsmraw-20240506/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_lock.c` & `libsmraw-20240506/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_condition.h` & `libsmraw-20240506/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_repeating_thread.h` & `libsmraw-20240506/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/Makefile.am` & `libsmraw-20240506/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcthreads/libcthreads_support.c` & `libsmraw-20240506/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_mutex.c` & `libsmraw-20240506/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_queue.c` & `libsmraw-20240506/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_mutex.h` & `libsmraw-20240506/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_types.h` & `libsmraw-20240506/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread_attributes.h` & `libsmraw-20240506/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_condition.c` & `libsmraw-20240506/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_error.c` & `libsmraw-20240506/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_read_write_lock.c` & `libsmraw-20240506/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_libcerror.h` & `libsmraw-20240506/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_definitions.h` & `libsmraw-20240506/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread_pool.c` & `libsmraw-20240506/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_error.h` & `libsmraw-20240506/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_thread_attributes.c` & `libsmraw-20240506/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_extern.h` & `libsmraw-20240506/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/libcthreads_repeating_thread.c` & `libsmraw-20240506/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcthreads/Makefile.in` & `libsmraw-20240506/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -479,14 +479,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -545,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -569,15 +571,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -787,24 +790,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -898,17 +914,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcthreads/libcthreads_queue.h` & `libsmraw-20240506/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/test-driver` & `libsmraw-20240506/test-driver`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/storage_media_buffer.c` & `libsmraw-20240506/smrawtools/storage_media_buffer.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libfvalue.h` & `libsmraw-20240506/smrawtools/smrawtools_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_dokan.c` & `libsmraw-20240506/smrawtools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_file_system.h` & `libsmraw-20240506/smrawtools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_fuse.c` & `libsmraw-20240506/smrawtools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_find.h` & `libsmraw-20240506/smrawtools/smrawtools_find.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_dokan.h` & `libsmraw-20240506/smrawtools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libcnotify.h` & `libsmraw-20240506/smrawtools/smrawtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/digest_hash.c` & `libsmraw-20240506/smrawtools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_file_system.c` & `libsmraw-20240506/smrawtools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawmount.c` & `libsmraw-20240506/smrawtools/smrawmount.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/byte_size_string.c` & `libsmraw-20240506/smrawtools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/Makefile.am` & `libsmraw-20240506/smrawtools/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -90,19 +90,17 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsmraw/libsmraw.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on smrawmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smrawmount_SOURCES)
 	@echo "Running splint on smrawverify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smrawverify_SOURCES)
```

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libuna.h` & `libsmraw-20240506/smrawtools/smrawtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libcpath.h` & `libsmraw-20240506/smrawtools/smrawtools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_glob.h` & `libsmraw-20240506/smrawtools/smrawtools_glob.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_file_entry.c` & `libsmraw-20240506/smrawtools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawverify.c` & `libsmraw-20240506/smrawtools/smrawverify.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libhmac.h` & `libsmraw-20240506/smrawtools/smrawtools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_file_entry.h` & `libsmraw-20240506/smrawtools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libcsplit.h` & `libsmraw-20240506/smrawtools/smrawtools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/process_status.c` & `libsmraw-20240506/smrawtools/process_status.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/verification_handle.c` & `libsmraw-20240506/smrawtools/verification_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_output.h` & `libsmraw-20240506/smrawtools/smrawtools_output.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_unused.h` & `libsmraw-20240506/smrawtools/smrawtools_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/verification_handle.h` & `libsmraw-20240506/smrawtools/verification_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/log_handle.c` & `libsmraw-20240506/smrawtools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_handle.h` & `libsmraw-20240506/smrawtools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_system_split_string.h` & `libsmraw-20240506/smrawtools/smrawtools_system_split_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/process_status.h` & `libsmraw-20240506/smrawtools/process_status.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libcerror.h` & `libsmraw-20240506/smrawtools/smrawtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_getopt.h` & `libsmraw-20240506/smrawtools/smrawtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libclocale.h` & `libsmraw-20240506/smrawtools/smrawtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libsmraw.h` & `libsmraw-20240506/smrawtools/smrawtools_libsmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libbfio.h` & `libsmraw-20240506/smrawtools/smrawtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_libcdata.h` & `libsmraw-20240506/smrawtools/smrawtools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_handle.c` & `libsmraw-20240506/smrawtools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_signal.c` & `libsmraw-20240506/smrawtools/smrawtools_signal.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/Makefile.in` & `libsmraw-20240506/smrawtools/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -535,16 +537,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -625,15 +627,16 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsmraw/libsmraw.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -895,23 +898,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/digest_hash.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/process_status.Po
+	-rm -f ./$(DEPDIR)/smrawmount.Po
+	-rm -f ./$(DEPDIR)/smrawtools_getopt.Po
+	-rm -f ./$(DEPDIR)/smrawtools_glob.Po
+	-rm -f ./$(DEPDIR)/smrawtools_output.Po
+	-rm -f ./$(DEPDIR)/smrawtools_signal.Po
+	-rm -f ./$(DEPDIR)/smrawverify.Po
+	-rm -f ./$(DEPDIR)/storage_media_buffer.Po
+	-rm -f ./$(DEPDIR)/verification_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1011,17 +1033,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on smrawmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smrawmount_SOURCES)
 	@echo "Running splint on smrawverify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smrawverify_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/smrawtools/log_handle.h` & `libsmraw-20240506/smrawtools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_i18n.h` & `libsmraw-20240506/smrawtools/smrawtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_glob.c` & `libsmraw-20240506/smrawtools/smrawtools_glob.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/byte_size_string.h` & `libsmraw-20240506/smrawtools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/digest_hash.h` & `libsmraw-20240506/smrawtools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_output.c` & `libsmraw-20240506/smrawtools/smrawtools_output.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_signal.h` & `libsmraw-20240506/smrawtools/smrawtools_signal.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/smrawtools_getopt.c` & `libsmraw-20240506/smrawtools/smrawtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/mount_fuse.h` & `libsmraw-20240506/smrawtools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/smrawtools/storage_media_buffer.h` & `libsmraw-20240506/smrawtools/storage_media_buffer.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libsmraw.spec` & `libsmraw-20240506/libsmraw.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libsmraw
-Version: 20240310
+Version: 20240506
 Release: 1
 Summary: Library to access the storage media (SM) (split) RAW format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libsmraw
              
@@ -36,16 +36,16 @@
 
 %description -n libsmraw-python3
 Python 3 bindings for libsmraw
 
 %package -n libsmraw-tools
 Summary: Several tools for reading and writing storage media (SM) (split) RAW files
 Group: Applications/System
-Requires: libsmraw = %{version}-%{release} openssl fuse-libs 
-BuildRequires: openssl-devel fuse-devel 
+Requires: libsmraw = %{version}-%{release} openssl fuse3-libs 
+BuildRequires: openssl-devel fuse3-devel 
 
 %description -n libsmraw-tools
 Several tools for reading and writing storage media (SM) (split) RAW files
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libsmraw-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sun Mar 10 2024 Joachim Metz <joachim.metz@gmail.com> 20240310-1
+* Mon May  6 2024 Joachim Metz <joachim.metz@gmail.com> 20240506-1
 - Auto-generated
```

### Comparing `libsmraw-20240310/libcpath/libcpath_support.c` & `libsmraw-20240506/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_libcerror.h` & `libsmraw-20240506/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_definitions.h` & `libsmraw-20240506/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libsmraw-20240310/libcpath/Makefile.am` & `libsmraw-20240506/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcpath/libcpath_error.c` & `libsmraw-20240506/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_extern.h` & `libsmraw-20240506/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_system_string.h` & `libsmraw-20240506/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_support.h` & `libsmraw-20240506/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_libcsplit.h` & `libsmraw-20240506/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_system_string.c` & `libsmraw-20240506/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_libclocale.h` & `libsmraw-20240506/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_error.h` & `libsmraw-20240506/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/Makefile.in` & `libsmraw-20240506/libcpath/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -455,14 +455,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -521,16 +523,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -542,15 +544,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -753,24 +756,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -857,17 +866,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcpath/libcpath_libuna.h` & `libsmraw-20240506/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_unused.h` & `libsmraw-20240506/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_path.c` & `libsmraw-20240506/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcpath/libcpath_path.h` & `libsmraw-20240506/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_file_objects_io_pool.h` & `libsmraw-20240506/pysmraw/pysmraw_file_objects_io_pool.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_error.h` & `libsmraw-20240506/pysmraw/pysmraw_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_error.c` & `libsmraw-20240506/pysmraw/pysmraw_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/Makefile.am` & `libsmraw-20240506/pysmraw/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -41,13 +41,11 @@
 	@LIBBFIO_LIBADD@
 
 pysmraw_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pysmraw_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libsmraw-20240310/pysmraw/pysmraw_unused.h` & `libsmraw-20240506/pysmraw/pysmraw_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_integer.c` & `libsmraw-20240506/pysmraw/pysmraw_integer.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_python.h` & `libsmraw-20240506/pysmraw/pysmraw_python.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw.c` & `libsmraw-20240506/pysmraw/pysmraw.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_integer.h` & `libsmraw-20240506/pysmraw/pysmraw_integer.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_libcerror.h` & `libsmraw-20240506/pysmraw/pysmraw_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_file_object_io_handle.c` & `libsmraw-20240506/pysmraw/pysmraw_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_handle.h` & `libsmraw-20240506/pysmraw/pysmraw_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_metadata.h` & `libsmraw-20240506/pysmraw/pysmraw_metadata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_metadata.c` & `libsmraw-20240506/pysmraw/pysmraw_metadata.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_libbfio.h` & `libsmraw-20240506/pysmraw/pysmraw_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_libclocale.h` & `libsmraw-20240506/pysmraw/pysmraw_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_file_objects_io_pool.c` & `libsmraw-20240506/pysmraw/pysmraw_file_objects_io_pool.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_libsmraw.h` & `libsmraw-20240506/pysmraw/pysmraw_libsmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw.h` & `libsmraw-20240506/pysmraw/pysmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/pysmraw_file_object_io_handle.h` & `libsmraw-20240506/pysmraw/pysmraw_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/pysmraw/Makefile.in` & `libsmraw-20240506/pysmraw/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -496,14 +496,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -562,16 +564,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -603,15 +605,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pysmraw_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pysmraw_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -893,24 +896,33 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_error.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_file_objects_io_pool.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_handle.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_integer.Plo
+	-rm -f ./$(DEPDIR)/pysmraw_la-pysmraw_metadata.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1001,13 +1013,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/pysmraw/pysmraw_handle.c` & `libsmraw-20240506/pysmraw/pysmraw_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/ChangeLog` & `libsmraw-20240506/ChangeLog`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/manuals/libsmraw.3` & `libsmraw-20240506/manuals/libsmraw.3`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/manuals/smrawmount.1` & `libsmraw-20240506/manuals/smrawmount.1`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/manuals/Makefile.in` & `libsmraw-20240506/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -501,15 +503,16 @@
 	libsmraw.3 \
 	smrawmount.1
 
 EXTRA_DIST = \
 	libsmraw.3 \
 	smrawmount.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -702,23 +705,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -800,13 +805,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/tests/smraw_test_libsmraw.h` & `libsmraw-20240506/tests/smraw_test_libsmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_memory.h` & `libsmraw-20240506/tests/smraw_test_memory.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_write_functions.sh` & `libsmraw-20240506/tests/test_write_functions.sh`

 * *Files 5% similar despite different names*

```diff
@@ -59,20 +59,17 @@
 }
 
 if ! test -z ${SKIP_LIBRARY_TESTS};
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmraw-20240310/tests/smraw_test_memory.c` & `libsmraw-20240506/tests/smraw_test_memory.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_libcnotify.h` & `libsmraw-20240506/tests/smraw_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_getopt.c` & `libsmraw-20240506/tests/smraw_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/pysmraw_test_handle.py` & `libsmraw-20240506/tests/pysmraw_test_handle.py`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_tools.sh` & `libsmraw-20240506/tests/test_tools.sh`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmraw-20240310/tests/smraw_test_functions.h` & `libsmraw-20240506/tests/smraw_test_functions.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_libcerror.h` & `libsmraw-20240506/tests/smraw_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_filename.c` & `libsmraw-20240506/tests/smraw_test_filename.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_tools_signal.c` & `libsmraw-20240506/tests/smraw_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_macros.h` & `libsmraw-20240506/tests/smraw_test_macros.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_write.c` & `libsmraw-20240506/tests/smraw_test_write.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/Makefile.am` & `libsmraw-20240506/tests/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -219,13 +219,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	../libsmraw/libsmraw.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@
 	@PTHREAD_LIBADD@
 	@LIBDL_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libsmraw-20240310/tests/smraw_test_support.c` & `libsmraw-20240506/tests/smraw_test_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_glob.c` & `libsmraw-20240506/tests/smraw_test_glob.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_information_file.c` & `libsmraw-20240506/tests/smraw_test_information_file.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_python_module.sh` & `libsmraw-20240506/tests/test_python_module.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="handle";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libsmraw";
+PYTHON_MODULE="pysmraw";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysmraw_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysmraw_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pysmraw");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libsmraw-20240310/tests/smraw_test_getopt.h` & `libsmraw-20240506/tests/smraw_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_libuna.h` & `libsmraw-20240506/tests/smraw_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_smrawverify.sh` & `libsmraw-20240506/tests/test_smrawverify.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Verify tool testing script
 #
-# Version: 20231001
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("smrawverify");
 OPTIONS_PER_PROFILE=("-q");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmraw-20240310/tests/smraw_test_libcpath.h` & `libsmraw-20240506/tests/smraw_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_libclocale.h` & `libsmraw-20240506/tests/smraw_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_unused.h` & `libsmraw-20240506/tests/smraw_test_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_io_handle.c` & `libsmraw-20240506/tests/smraw_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_runner.sh` & `libsmraw-20240506/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_error.c` & `libsmraw-20240506/tests/smraw_test_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/pysmraw_test_support.py` & `libsmraw-20240506/tests/pysmraw_test_support.py`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_glob.sh` & `libsmraw-20240506/tests/test_glob.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Library glob testing script
 #
-# Version: 20230410
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 seq()
 {
@@ -156,20 +156,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmraw-20240310/tests/smraw_test_handle.c` & `libsmraw-20240506/tests/smraw_test_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_notify.c` & `libsmraw-20240506/tests/smraw_test_notify.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_libbfio.h` & `libsmraw-20240506/tests/smraw_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/Makefile.in` & `libsmraw-20240506/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -729,14 +729,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -796,16 +798,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1000,16 +1002,18 @@
 	@LIBCRYPTO_LIBADD@ \
 	@LIBCPATH_LIBADD@ \
 	@LIBCSPLIT_LIBADD@ \
 	../libsmraw/libsmraw.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1483,24 +1487,42 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../smrawtools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../smrawtools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../smrawtools/$(DEPDIR)/smrawtools_output.Po
+	-rm -f ../smrawtools/$(DEPDIR)/smrawtools_signal.Po
+	-rm -f ./$(DEPDIR)/smraw_test_error.Po
+	-rm -f ./$(DEPDIR)/smraw_test_filename.Po
+	-rm -f ./$(DEPDIR)/smraw_test_functions.Po
+	-rm -f ./$(DEPDIR)/smraw_test_getopt.Po
+	-rm -f ./$(DEPDIR)/smraw_test_glob.Po
+	-rm -f ./$(DEPDIR)/smraw_test_handle.Po
+	-rm -f ./$(DEPDIR)/smraw_test_information_file.Po
+	-rm -f ./$(DEPDIR)/smraw_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/smraw_test_memory.Po
+	-rm -f ./$(DEPDIR)/smraw_test_notify.Po
+	-rm -f ./$(DEPDIR)/smraw_test_support.Po
+	-rm -f ./$(DEPDIR)/smraw_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/smraw_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/smraw_test_write.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1602,13 +1624,10 @@
 
 .PRECIOUS: Makefile
 
 	@PTHREAD_LIBADD@
 	@PTHREAD_LIBADD@
 	@LIBDL_LIBADD@
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/tests/smraw_test_tools_output.c` & `libsmraw-20240506/tests/smraw_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/smraw_test_functions.c` & `libsmraw-20240506/tests/smraw_test_functions.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/tests/test_library.sh` & `libsmraw-20240506/tests/test_library.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="error filename information_file io_handle notify support";
 LIBRARY_TESTS_WITH_INPUT="handle";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmraw-20240310/tests/smraw_test_libhmac.h` & `libsmraw-20240506/tests/smraw_test_libhmac.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/ossfuzz/ossfuzz_libsmraw.h` & `libsmraw-20240506/ossfuzz/ossfuzz_libsmraw.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/ossfuzz/handle_fuzzer.cc` & `libsmraw-20240506/ossfuzz/handle_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/ossfuzz/Makefile.am` & `libsmraw-20240506/ossfuzz/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libsmraw/libsmraw.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
```

### Comparing `libsmraw-20240310/ossfuzz/ossfuzz_libbfio.h` & `libsmraw-20240506/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/ossfuzz/Makefile.in` & `libsmraw-20240506/ossfuzz/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -534,16 +536,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -563,15 +565,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libsmraw/libsmraw.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -813,23 +816,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/handle_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -913,17 +919,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on handle_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(handle_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/ltmain.sh` & `libsmraw-20240506/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha1_context.c` & `libsmraw-20240506/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha224.h` & `libsmraw-20240506/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha512_context.c` & `libsmraw-20240506/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_extern.h` & `libsmraw-20240506/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_md5.c` & `libsmraw-20240506/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_md5.h` & `libsmraw-20240506/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_error.h` & `libsmraw-20240506/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_types.h` & `libsmraw-20240506/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_byte_stream.h` & `libsmraw-20240506/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha512.c` & `libsmraw-20240506/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha256_context.c` & `libsmraw-20240506/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha224.c` & `libsmraw-20240506/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_definitions.h` & `libsmraw-20240506/libhmac/libhmac_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libsmraw-20240310/libhmac/libhmac_unused.h` & `libsmraw-20240506/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha1.h` & `libsmraw-20240506/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha256_context.h` & `libsmraw-20240506/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/Makefile.am` & `libsmraw-20240506/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBHMAC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libhmac.la
 
 libhmac_la_SOURCES = \
@@ -25,19 +25,17 @@
 	libhmac_sha512.c libhmac_sha512.h \
 	libhmac_sha512_context.c libhmac_sha512_context.h \
 	libhmac_support.c libhmac_support.h \
 	libhmac_types.h \
 	libhmac_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libsmraw-20240310/libhmac/libhmac_sha224_context.c` & `libsmraw-20240506/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_md5_context.h` & `libsmraw-20240506/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha256.c` & `libsmraw-20240506/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha1_context.h` & `libsmraw-20240506/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_libcerror.h` & `libsmraw-20240506/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_error.c` & `libsmraw-20240506/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_support.h` & `libsmraw-20240506/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/Makefile.in` & `libsmraw-20240506/libhmac/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -478,14 +478,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -544,16 +546,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBHMAC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCRYPTO_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBHMAC_TRUE@noinst_LTLIBRARIES = libhmac.la
 @HAVE_LOCAL_LIBHMAC_TRUE@libhmac_la_SOURCES = \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_byte_stream.h \
@@ -571,15 +573,16 @@
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha256_context.c libhmac_sha256_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512.c libhmac_sha512.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512_context.c libhmac_sha512_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_support.c libhmac_support.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_types.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -790,24 +793,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -902,17 +919,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libhmac/libhmac_sha256.h` & `libsmraw-20240506/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha224_context.h` & `libsmraw-20240506/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha512_context.h` & `libsmraw-20240506/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha512.h` & `libsmraw-20240506/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_support.c` & `libsmraw-20240506/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_sha1.c` & `libsmraw-20240506/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libhmac/libhmac_md5_context.c` & `libsmraw-20240506/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_narrow_string.c` & `libsmraw-20240506/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_definitions.h` & `libsmraw-20240506/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libsmraw-20240310/libcsplit/libcsplit_types.h` & `libsmraw-20240506/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_wide_split_string.c` & `libsmraw-20240506/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_support.h` & `libsmraw-20240506/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/Makefile.am` & `libsmraw-20240506/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcsplit/libcsplit_libcerror.h` & `libsmraw-20240506/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_wide_string.c` & `libsmraw-20240506/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_unused.h` & `libsmraw-20240506/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_wide_split_string.h` & `libsmraw-20240506/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_error.c` & `libsmraw-20240506/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_narrow_split_string.c` & `libsmraw-20240506/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_extern.h` & `libsmraw-20240506/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_error.h` & `libsmraw-20240506/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_support.c` & `libsmraw-20240506/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_wide_string.h` & `libsmraw-20240506/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/Makefile.in` & `libsmraw-20240506/libcsplit/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -465,14 +465,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -531,16 +533,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -549,15 +551,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +765,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -868,17 +879,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcsplit/libcsplit_narrow_split_string.h` & `libsmraw-20240506/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcsplit/libcsplit_narrow_string.h` & `libsmraw-20240506/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/remove-potcdate.sin` & `libsmraw-20240506/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/Makefile.in.in` & `libsmraw-20240506/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/en@quot.header` & `libsmraw-20240506/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/en@boldquot.header` & `libsmraw-20240506/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/insert-header.sin` & `libsmraw-20240506/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/Makevars` & `libsmraw-20240506/po/Makevars`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/Makevars.in` & `libsmraw-20240506/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/po/Rules-quot` & `libsmraw-20240506/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1251.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf16_string.c` & `libsmraw-20240506/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base16_stream.c` & `libsmraw-20240506/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf8_stream.h` & `libsmraw-20240506/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_2.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_932.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_dingbats.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf8_string.c` & `libsmraw-20240506/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base64_stream.c` & `libsmraw-20240506/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_error.h` & `libsmraw-20240506/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_turkish.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_unicode_character.c` & `libsmraw-20240506/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_gaelic.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_arabic.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_thai.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_874.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_15.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf8_string.h` & `libsmraw-20240506/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_16.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1255.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf7_stream.c` & `libsmraw-20240506/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_byte_stream.h` & `libsmraw-20240506/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_koi8_u.c` & `libsmraw-20240506/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_unused.h` & `libsmraw-20240506/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_6.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_14.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base64_stream.h` & `libsmraw-20240506/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_error.c` & `libsmraw-20240506/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_centraleurroman.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_romanian.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_6.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_9.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_russian.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_dingbats.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_15.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_936.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_croatian.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_scsu.h` & `libsmraw-20240506/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/Makefile.am` & `libsmraw-20240506/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libsmraw-20240310/libuna/libuna_utf32_stream.c` & `libsmraw-20240506/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_936.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_10.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_roman.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf7_stream.h` & `libsmraw-20240506/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_3.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_thai.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_farsi.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_ukrainian.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_inuit.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_932.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_874.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_5.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_10.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_definitions.h` & `libsmraw-20240506/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libsmraw-20240310/libuna/libuna_url_stream.h` & `libsmraw-20240506/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_icelandic.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_koi8_u.h` & `libsmraw-20240506/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf16_stream.c` & `libsmraw-20240506/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1253.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_4.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_greek.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_libcerror.h` & `libsmraw-20240506/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_centraleurroman.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1254.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_13.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_7.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1255.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_unicode_character.h` & `libsmraw-20240506/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_8.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_13.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_949.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_cyrillic.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_celtic.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_support.h` & `libsmraw-20240506/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_4.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_949.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf16_stream.h` & `libsmraw-20240506/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_symbol.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_roman.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1257.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1254.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_950.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_extern.h` & `libsmraw-20240506/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1256.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_types.h` & `libsmraw-20240506/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base32_stream.h` & `libsmraw-20240506/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1253.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_16.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf8_stream.c` & `libsmraw-20240506/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1250.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_2.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_support.c` & `libsmraw-20240506/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_koi8_r.c` & `libsmraw-20240506/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_5.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf16_string.h` & `libsmraw-20240506/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf32_string.c` & `libsmraw-20240506/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_icelandic.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1256.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf32_string.h` & `libsmraw-20240506/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_romanian.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_8.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_koi8_r.h` & `libsmraw-20240506/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_cyrillic.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_arabic.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_croatian.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_9.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_greek.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1258.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_7.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/Makefile.in` & `libsmraw-20240506/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -633,14 +633,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -699,16 +701,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -774,15 +776,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1044,24 +1047,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1207,17 +1275,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_3.c` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1250.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_scsu.c` & `libsmraw-20240506/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1252.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_turkish.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_ukrainian.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_russian.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1258.c` & `libsmraw-20240506/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_celtic.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_byte_stream.c` & `libsmraw-20240506/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_gaelic.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_utf32_stream.h` & `libsmraw-20240506/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_symbol.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1257.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_inuit.h` & `libsmraw-20240506/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_mac_farsi.c` & `libsmraw-20240506/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_950.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_url_stream.c` & `libsmraw-20240506/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1251.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_windows_1252.h` & `libsmraw-20240506/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_codepage_iso_8859_14.h` & `libsmraw-20240506/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base16_stream.h` & `libsmraw-20240506/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libuna/libuna_base32_stream.c` & `libsmraw-20240506/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/Makefile.in` & `libsmraw-20240506/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -515,14 +515,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -645,16 +647,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libsmraw.pc \
+	libsmraw.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libsmraw.pc
 
 all: all-recursive
 
@@ -1071,23 +1080,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1197,22 +1209,10 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libsmraw && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libsmraw.pc
-	-rm -f libsmraw.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmraw-20240310/libfvalue/libfvalue_filetime.c` & `libsmraw-20240506/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_utf16_string.c` & `libsmraw-20240506/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libfwnt.h` & `libsmraw-20240506/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value.c` & `libsmraw-20240506/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value.h` & `libsmraw-20240506/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_definitions.h` & `libsmraw-20240506/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libsmraw-20240310/libfvalue/libfvalue_codepage.h` & `libsmraw-20240506/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_split_utf16_string.c` & `libsmraw-20240506/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_error.c` & `libsmraw-20240506/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_utf8_string.c` & `libsmraw-20240506/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_unused.h` & `libsmraw-20240506/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_split_utf16_string.h` & `libsmraw-20240506/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_filetime.h` & `libsmraw-20240506/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_support.c` & `libsmraw-20240506/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_extern.h` & `libsmraw-20240506/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/Makefile.am` & `libsmraw-20240506/libfvalue/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -38,19 +38,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value_type.h` & `libsmraw-20240506/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libcerror.h` & `libsmraw-20240506/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_split_utf8_string.c` & `libsmraw-20240506/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_data_handle.h` & `libsmraw-20240506/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libcnotify.h` & `libsmraw-20240506/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_data_handle.c` & `libsmraw-20240506/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_integer.c` & `libsmraw-20240506/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value_type.c` & `libsmraw-20240506/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_integer.h` & `libsmraw-20240506/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_binary_data.h` & `libsmraw-20240506/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value_entry.h` & `libsmraw-20240506/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_utf16_string.h` & `libsmraw-20240506/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_error.h` & `libsmraw-20240506/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_table.h` & `libsmraw-20240506/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libfguid.h` & `libsmraw-20240506/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_split_utf8_string.h` & `libsmraw-20240506/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_floating_point.h` & `libsmraw-20240506/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libfdatetime.h` & `libsmraw-20240506/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_string.h` & `libsmraw-20240506/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_binary_data.c` & `libsmraw-20240506/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_value_entry.c` & `libsmraw-20240506/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libcdata.h` & `libsmraw-20240506/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_support.h` & `libsmraw-20240506/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_table.c` & `libsmraw-20240506/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/Makefile.in` & `libsmraw-20240506/libfvalue/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -496,14 +496,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -562,16 +564,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -602,15 +604,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -825,24 +828,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -941,17 +962,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libfvalue/libfvalue_utf8_string.h` & `libsmraw-20240506/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_floating_point.c` & `libsmraw-20240506/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_types.h` & `libsmraw-20240506/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_string.c` & `libsmraw-20240506/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libfvalue/libfvalue_libuna.h` & `libsmraw-20240506/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_definitions.h` & `libsmraw-20240506/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libsmraw-20240310/libcnotify/libcnotify_extern.h` & `libsmraw-20240506/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_support.c` & `libsmraw-20240506/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_stream.h` & `libsmraw-20240506/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/Makefile.am` & `libsmraw-20240506/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcnotify/libcnotify_unused.h` & `libsmraw-20240506/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_verbose.h` & `libsmraw-20240506/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_print.h` & `libsmraw-20240506/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_stream.c` & `libsmraw-20240506/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_support.h` & `libsmraw-20240506/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_verbose.c` & `libsmraw-20240506/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/Makefile.in` & `libsmraw-20240506/libcnotify/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -457,14 +457,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -523,30 +525,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -749,24 +752,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -853,17 +862,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/libcnotify/libcnotify_libcerror.h` & `libsmraw-20240506/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcnotify/libcnotify_print.c` & `libsmraw-20240506/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_system.c` & `libsmraw-20240506/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_error.c` & `libsmraw-20240506/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_extern.h` & `libsmraw-20240506/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/Makefile.am` & `libsmraw-20240506/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libsmraw-20240310/libcerror/libcerror_types.h` & `libsmraw-20240506/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_support.h` & `libsmraw-20240506/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_error.h` & `libsmraw-20240506/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_system.h` & `libsmraw-20240506/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_definitions.h` & `libsmraw-20240506/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libsmraw-20240310/libcerror/libcerror_support.c` & `libsmraw-20240506/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/libcerror_unused.h` & `libsmraw-20240506/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/libcerror/Makefile.in` & `libsmraw-20240506/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -520,28 +522,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -743,24 +746,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -846,17 +854,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmraw-20240310/aclocal.m4` & `libsmraw-20240506/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libsmraw-20240310/configure.ac` & `libsmraw-20240506/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libsmraw],
- [20240310],
+ [20240506],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libsmraw.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

