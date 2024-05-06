# Comparing `tmp/ReverseBox-0.8.9.tar.gz` & `tmp/ReverseBox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.8.9.tar", last modified: Sat May  4 18:19:32 2024, max compression
+gzip compressed data, was "ReverseBox-0.9.0.tar", last modified: Mon May  6 13:03:41 2024, max compression
```

## Comparing `ReverseBox-0.8.9.tar` & `ReverseBox-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.444450 ReverseBox-0.8.9/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.8.9/LICENSE
--rw-rw-rw-   0        0        0     6982 2024-05-04 18:19:32.443453 ReverseBox-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     5581 2024-05-03 23:01:57.000000 ReverseBox-0.8.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.383663 ReverseBox-0.8.9/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     6982 2024-05-04 18:19:32.000000 ReverseBox-0.8.9/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2024-05-04 18:19:32.000000 ReverseBox-0.8.9/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 18:19:32.000000 ReverseBox-0.8.9/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-04 18:19:32.000000 ReverseBox-0.8.9/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 18:19:32.000000 ReverseBox-0.8.9/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.384637 ReverseBox-0.8.9/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.8.9/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.389624 ReverseBox-0.8.9/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.9/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.8.9/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.8.9/reversebox/checksum/checksum_bsd16.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.8.9/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.8.9/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.391619 ReverseBox-0.8.9/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.8.9/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.8.9/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.8.9/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.396605 ReverseBox-0.8.9/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.9/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.8.9/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.8.9/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0     1065 2024-05-04 18:17:46.000000 ReverseBox-0.8.9/reversebox/compression/compression_refpack.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.8.9/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.406551 ReverseBox-0.8.9/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.8.9/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.8.9/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.8.9/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.8.9/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.8.9/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.8.9/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.8.9/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.8.9/reversebox/crc/crc32_asobo.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.8.9/reversebox/crc/crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.8.9/reversebox/crc/crc64_asobo.py
--rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.8.9/reversebox/crc/crc8.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.411567 ReverseBox-0.8.9/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.9/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.8.9/reversebox/encryption/encryption_rot13.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.8.9/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.8.9/reversebox/encryption/encryption_xor_basic_key_guesser.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.8.9/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.8.9/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.417550 ReverseBox-0.8.9/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.9/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.8.9/reversebox/hash/hash_fnv.py
--rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.8.9/reversebox/hash/hash_md2.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.8.9/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.8.9/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.8.9/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.422532 ReverseBox-0.8.9/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.8.9/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.8.9/reversebox/image/image_dds.py
--rw-rw-rw-   0        0        0    12186 2024-05-04 18:17:45.000000 ReverseBox-0.8.9/reversebox/image/image_decoder.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.8.9/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.8.9/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0      641 2024-05-04 18:17:38.000000 ReverseBox-0.8.9/reversebox/image/image_formats.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.430519 ReverseBox-0.8.9/reversebox/image/swizzling/
--rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.8.9/reversebox/image/swizzling/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_3ds.py
--rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_cmpr.py
--rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_ps2.py
--rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_psp.py
--rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_psvita.py
--rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_switch.py
--rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_xbox.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.438493 ReverseBox-0.8.9/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.9/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.8.9/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0      989 2024-05-04 18:17:46.000000 ReverseBox-0.8.9/reversebox/io_files/bytes_helper_functions.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.8.9/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.8.9/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.8.9/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.8.9/reversebox/io_files/translation_text_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:19:32.440461 ReverseBox-0.8.9/reversebox/libs/
--rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.8.9/reversebox/libs/__init__.py
--rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.8.9/reversebox/libs/refpack.dll
--rw-rw-rw-   0        0        0       42 2024-05-04 18:19:32.444450 ReverseBox-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-04 18:19:31.000000 ReverseBox-0.8.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.649448 ReverseBox-0.9.0/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     6982 2024-05-06 13:03:41.649448 ReverseBox-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5581 2024-05-03 23:01:57.000000 ReverseBox-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.552707 ReverseBox-0.9.0/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     6982 2024-05-06 13:03:41.000000 ReverseBox-0.9.0/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2024-05-06 13:03:41.000000 ReverseBox-0.9.0/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:03:41.000000 ReverseBox-0.9.0/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-06 13:03:41.000000 ReverseBox-0.9.0/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 13:03:41.000000 ReverseBox-0.9.0/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.553704 ReverseBox-0.9.0/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.9.0/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.559688 ReverseBox-0.9.0/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.0/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.9.0/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.9.0/reversebox/checksum/checksum_bsd16.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.9.0/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.9.0/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.563677 ReverseBox-0.9.0/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.9.0/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.9.0/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.9.0/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.571656 ReverseBox-0.9.0/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.0/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.9.0/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.9.0/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0     1154 2024-05-04 22:26:48.000000 ReverseBox-0.9.0/reversebox/compression/compression_refpack.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.9.0/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.588612 ReverseBox-0.9.0/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.9.0/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.9.0/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.9.0/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.9.0/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.9.0/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.9.0/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.9.0/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.9.0/reversebox/crc/crc32_asobo.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.9.0/reversebox/crc/crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.9.0/reversebox/crc/crc64_asobo.py
+-rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.9.0/reversebox/crc/crc8.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.597587 ReverseBox-0.9.0/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.0/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.9.0/reversebox/encryption/encryption_rot13.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.9.0/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.9.0/reversebox/encryption/encryption_xor_basic_key_guesser.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.9.0/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.9.0/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.606563 ReverseBox-0.9.0/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.0/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.9.0/reversebox/hash/hash_fnv.py
+-rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.9.0/reversebox/hash/hash_md2.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.9.0/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.9.0/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.9.0/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.616537 ReverseBox-0.9.0/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.9.0/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.9.0/reversebox/image/image_dds.py
+-rw-rw-rw-   0        0        0    12631 2024-05-06 13:03:40.000000 ReverseBox-0.9.0/reversebox/image/image_decoder.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.9.0/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.9.0/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0      641 2024-05-06 13:01:53.000000 ReverseBox-0.9.0/reversebox/image/image_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.629503 ReverseBox-0.9.0/reversebox/image/swizzling/
+-rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.9.0/reversebox/image/swizzling/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_3ds.py
+-rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_cmpr.py
+-rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_ps2.py
+-rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_psp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_psvita.py
+-rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_switch.py
+-rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_xbox.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.641471 ReverseBox-0.9.0/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.0/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.9.0/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 13:01:53.000000 ReverseBox-0.9.0/reversebox/io_files/bytes_helper_functions.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.9.0/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.9.0/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.9.0/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.9.0/reversebox/io_files/translation_text_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:03:41.643465 ReverseBox-0.9.0/reversebox/libs/
+-rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.9.0/reversebox/libs/__init__.py
+-rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.9.0/reversebox/libs/refpack.dll
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:03:41.650446 ReverseBox-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-06 12:53:33.000000 ReverseBox-0.9.0/setup.py
```

### Comparing `ReverseBox-0.8.9/LICENSE` & `ReverseBox-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/PKG-INFO` & `ReverseBox-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.9
+Version: 0.9.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.8.9/README.md` & `ReverseBox-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.9.0/ReverseBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.9
+Version: 0.9.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.8.9/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.9.0/ReverseBox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/common/logger.py` & `ReverseBox-0.9.0/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/compression/compression_refpack.py` & `ReverseBox-0.9.0/reversebox/compression/compression_refpack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Copyright © 2024  Bartłomiej Duda
 License: GPL-3.0 License
 """
 import ctypes
-from ctypes import c_char
+from ctypes import byref, c_char
 from pathlib import Path
 
 
 class RefpackHandler:
     def compress_data(self, input_data: bytes) -> bytes:
         return input_data  # TODO - fix this
 
     def decompress_data(self, compressed_data: bytes) -> bytes:
         if compressed_data[:2] != b"\x10\xFB":
             raise Exception("Wrong refpack compression header!")
         temp_buffer = (c_char * len(compressed_data) * 100)()
-        refpack_dll_path: str = str(
-            Path(__file__).parents[1].resolve().joinpath("libs").joinpath("refpack.dll")
-        )
         try:
-            refpack_dll_file = ctypes.cdll.LoadLibrary(refpack_dll_path)
+            refpack_dll_path: str = str(
+                Path(__file__)
+                .parents[1]
+                .resolve()
+                .joinpath("libs")
+                .joinpath("refpack.dll")
+            )
+            refpack_dll_file = ctypes.CDLL(refpack_dll_path)
             uncompressed_data_size = refpack_dll_file.unrefpack(
-                compressed_data, temp_buffer
+                compressed_data, byref(temp_buffer), 1
             )
         except Exception as error:
             raise Exception(f"Error while decompressing refpack data! Error: {error}")
         return bytes(bytearray(temp_buffer)[:uncompressed_data_size])
```

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_arc.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc16_sick.py` & `ReverseBox-0.9.0/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc32_asobo.py` & `ReverseBox-0.9.0/reversebox/crc/crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.9.0/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc64_asobo.py` & `ReverseBox-0.9.0/reversebox/crc/crc64_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/crc/crc8.py` & `ReverseBox-0.9.0/reversebox/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/encryption/encryption_rot13.py` & `ReverseBox-0.9.0/reversebox/encryption/encryption_rot13.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.9.0/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/encryption/encryption_xor_basic_key_guesser.py` & `ReverseBox-0.9.0/reversebox/encryption/encryption_xor_basic_key_guesser.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.9.0/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.9.0/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/hash/hash_fnv.py` & `ReverseBox-0.9.0/reversebox/hash/hash_fnv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/image_dds.py` & `ReverseBox-0.9.0/reversebox/image/image_dds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/image_decoder.py` & `ReverseBox-0.9.0/reversebox/image/image_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,37 +6,35 @@
 
 from PIL import Image
 
 from reversebox.common.logger import get_logger
 from reversebox.image.image_formats import ImageFormats
 from reversebox.io_files.bytes_handler import BytesHandler
 from reversebox.io_files.bytes_helper_functions import (
-    get_bits,
-    get_uint8,
     get_uint16,
     get_uint24,
-    get_uint32,
+    get_uint32, get_uint8, get_bits,
 )
 
 logger = get_logger(__name__)
 
 # fmt: off
 # mypy: ignore-errors
 
 
 class ImageDecoder:
     def __init__(self):
         pass
 
     def _decode_rgba2222_pixel(self, pixel_int: int) -> bytes:
         p = bytearray(4)
-        p[0] = get_bits(pixel_int, 0, 2, 8)
-        p[1] = get_bits(pixel_int, 2, 4, 8)
-        p[2] = get_bits(pixel_int, 4, 6, 8)
-        p[3] = get_bits(pixel_int, 6, 8, 8)
+        p[0] = get_bits(pixel_int, 2, 0)
+        p[1] = get_bits(pixel_int, 2, 2)
+        p[2] = get_bits(pixel_int, 2, 4)
+        p[3] = get_bits(pixel_int, 2, 6)
         return p
 
     def _decode_rgbx5551_pixel(self, pixel_int: int) -> bytes:
         p = bytearray(4)
         r = pixel_int & 0x1F
         g = (pixel_int >> 5) & 0x1F
         b = (pixel_int >> 10) & 0x1F
@@ -144,15 +142,15 @@
         p[1] = (g << 4) | (g >> 0)
         p[2] = (r << 4) | (r >> 0)
         p[3] = (a << 4) | (a >> 0)
         return p
 
     generic_data_formats = {
         # image_format: (decode_function, bits_per_pixel, image_entry_read_function)
-        ImageFormats.RGBA2222: (_decode_rgba2222_pixel, 8, get_uint8),
+        ImageFormats.RGBA2222: (_decode_rgba2222_pixel, 8, 1, get_uint8),
         ImageFormats.RGB565: (_decode_rgb565_pixel, 16, get_uint16),
         ImageFormats.RGB888: (_decode_rgb888_pixel, 24, get_uint24),
         ImageFormats.BGR888: (_decode_bgr888_pixel, 24, get_uint24),
         ImageFormats.ARGB4444: (_decode_argb4444_pixel, 16, get_uint16),
         ImageFormats.RGBA4444: (_decode_rgba4444_pixel, 16, get_uint16),
         ImageFormats.XRGB1555: (_decode_xrgb1555_pixel, 16, get_uint16),
         ImageFormats.ABGR1555: (_decode_abgr1555_pixel, 16, get_uint16),
@@ -188,15 +186,22 @@
     def _decode_generic(self, image_data: bytes, img_width: int, img_height: int, image_format: tuple, image_endianess: str) -> bytes:
         decode_function, bits_per_pixel, image_entry_read_function = image_format
         image_handler = BytesHandler(image_data)
         texture_data = bytearray(img_width * img_height * 4)
         read_offset = 0
         image_endianess_format: str = self._get_endianess_format(image_endianess)
 
-        if bits_per_pixel == 16:
+        if bits_per_pixel == 8:
+            bytes_per_pixel = 1
+            for i in range(len(image_data) // bytes_per_pixel):
+                image_pixel: bytes = image_handler.get_bytes(read_offset, bytes_per_pixel)
+                pixel_int: int = image_entry_read_function(image_pixel, image_endianess_format)
+                read_offset += bytes_per_pixel
+                texture_data[i * 4 : (i + 1) * 4] = decode_function(self, pixel_int)  # noqa
+        elif bits_per_pixel == 16:
             bytes_per_pixel = 2
             for i in range(len(image_data) // bytes_per_pixel):
                 image_pixel: bytes = image_handler.get_bytes(read_offset, bytes_per_pixel)
                 pixel_int: int = image_entry_read_function(image_pixel, image_endianess_format)
                 read_offset += bytes_per_pixel
                 texture_data[i * 4 : (i + 1) * 4] = decode_function(self, pixel_int)  # noqa
         elif bits_per_pixel == 24:
```

### Comparing `ReverseBox-0.8.9/reversebox/image/image_finder_gui.py` & `ReverseBox-0.9.0/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/image_finder_main.py` & `ReverseBox-0.9.0/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/image_formats.py` & `ReverseBox-0.9.0/reversebox/image/image_formats.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_3ds.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_3ds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_cmpr.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_cmpr.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_ps2.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_ps2.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_psp.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_psp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_psvita.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_psvita.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/image/swizzling/swizzle_switch.py` & `ReverseBox-0.9.0/reversebox/image/swizzling/swizzle_switch.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.9.0/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/io_files/bytes_helper_functions.py` & `ReverseBox-0.9.0/reversebox/io_files/bytes_helper_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import struct
 
 
-def get_bits(num: int, start: int, end: int, length: int = 64) -> int:
-    mask = 2 ** (end - start) - 1
-    shift = length - (end - start) - start
-    return (num & (mask << shift)) >> shift
+def get_bits(number: int, number_of_bits: int, position: int) -> int:
+    shifted_number = number >> (position - 1)
+    mask = (1 << number_of_bits) - 1
+    extracted_bits = shifted_number & mask
+    extracted_number = bin(extracted_bits)[2:]
+    return int(extracted_number, 2)
 
 
 def get_uint8(input_bytes: bytes, endianess: str) -> int:
     result = struct.unpack(endianess + "B", input_bytes)[0]
     return result
```

### Comparing `ReverseBox-0.8.9/reversebox/io_files/check_file.py` & `ReverseBox-0.9.0/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/io_files/file_handler.py` & `ReverseBox-0.9.0/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/io_files/mod_handler.py` & `ReverseBox-0.9.0/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.9.0/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/reversebox/libs/refpack.dll` & `ReverseBox-0.9.0/reversebox/libs/refpack.dll`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.9/setup.py` & `ReverseBox-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.8.9"
+VERSION_NUM = "0.9.0"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

