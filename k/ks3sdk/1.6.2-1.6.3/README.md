# Comparing `tmp/ks3sdk-1.6.2.tar.gz` & `tmp/ks3sdk-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ks3sdk-1.6.2.tar", last modified: Sun Apr  7 06:16:12 2024, max compression
+gzip compressed data, was "ks3sdk-1.6.3.tar", last modified: Mon May  6 06:30:12 2024, max compression
```

## Comparing `ks3sdk-1.6.2.tar` & `ks3sdk-1.6.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       74 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2314 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.836873 ks3sdk-1.6.2/examples/
--rw-r--r--   0 root         (0) root         (0)    24554 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/basic.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/billing.py
--rw-r--r--   0 root         (0) root         (0)     9667 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/bucket.py
--rw-r--r--   0 root         (0) root         (0)     5968 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/crc64.py
--rw-r--r--   0 root         (0) root         (0)    10988 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/encryption.py
--rw-r--r--   0 root         (0) root         (0)     3827 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/multi_thread.py
--rw-r--r--   0 root         (0) root         (0)     2620 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/multipart.py
--rw-r--r--   0 root         (0) root         (0)    12419 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/object.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/postProcessTask.py
--rw-r--r--   0 root         (0) root         (0)      868 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.839873 ks3sdk-1.6.2/ks3/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5764 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/acl.py
--rw-r--r--   0 root         (0) root         (0)     5109 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/auth.py
--rw-r--r--   0 root         (0) root         (0)     4326 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/authV4.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/billing.py
--rw-r--r--   0 root         (0) root         (0)    50561 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/bucket.py
--rw-r--r--   0 root         (0) root         (0)     6887 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/bucketlistresultset.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/compat.py
--rw-r--r--   0 root         (0) root         (0)    14200 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/connection.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/conv.py
--rw-r--r--   0 root         (0) root         (0)     4913 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/crc64_combine.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/deletemarker.py
--rw-r--r--   0 root         (0) root         (0)     8597 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/encryptFp.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/encryption.py
--rw-r--r--   0 root         (0) root         (0)     7259 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/exception.py
--rw-r--r--   0 root         (0) root         (0)     2378 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/handler.py
--rw-r--r--   0 root         (0) root         (0)     5898 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/http.py
--rw-r--r--   0 root         (0) root         (0)    55353 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/key.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/keyfile.py
--rw-r--r--   0 root         (0) root         (0)    14015 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/multipart.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/objectTagging.py
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/prefix.py
--rw-r--r--   0 root         (0) root         (0)    22966 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/provider.py
--rw-r--r--   0 root         (0) root         (0)     4698 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/resultset.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/sts.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/user.py
--rw-r--r--   0 root         (0) root         (0)     7079 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/ks3/xmlParsers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2778 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketCors.py
--rw-r--r--   0 root         (0) root         (0)     2480 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketCrossReplicate.py
--rw-r--r--   0 root         (0) root         (0)     8168 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketLifecycle.py
--rw-r--r--   0 root         (0) root         (0)     3256 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketLogging.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketMirror.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketQuota.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketRetention.py
--rw-r--r--   0 root         (0) root         (0)      721 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketVersioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/ks3sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2314 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:30:12.771948 ks3sdk-1.6.3/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-05-06 06:30:12.771948 ks3sdk-1.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:30:12.767946 ks3sdk-1.6.3/examples/
+-rw-r--r--   0 root         (0) root         (0)    26276 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/basic.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/billing.py
+-rw-r--r--   0 root         (0) root         (0)     9667 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/crc64.py
+-rw-r--r--   0 root         (0) root         (0)    10988 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/multi_thread.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/multipart.py
+-rw-r--r--   0 root         (0) root         (0)    12419 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/object.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/postProcessTask.py
+-rw-r--r--   0 root         (0) root         (0)      868 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/examples/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:30:12.769947 ks3sdk-1.6.3/ks3/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/acl.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/auth.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/authV4.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/billing.py
+-rw-r--r--   0 root         (0) root         (0)    52909 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     6887 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/bucketlistresultset.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/compat.py
+-rw-r--r--   0 root         (0) root         (0)    14200 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/connection.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/conv.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/crc64_combine.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/deletemarker.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/encryptFp.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/http.py
+-rw-r--r--   0 root         (0) root         (0)    55674 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/key.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/keyfile.py
+-rw-r--r--   0 root         (0) root         (0)    14632 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/multipart.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/objectTagging.py
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/prefix.py
+-rw-r--r--   0 root         (0) root         (0)    22966 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/provider.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/resultset.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/sts.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/user.py
+-rw-r--r--   0 root         (0) root         (0)     7079 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:30:12.770948 ks3sdk-1.6.3/ks3/xmlParsers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketCors.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketCrossReplicate.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketInventory.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketLifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketLogging.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketMirror.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketQuota.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketRetention.py
+-rw-r--r--   0 root         (0) root         (0)      721 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/ks3/xmlParsers/bucketVersioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:30:12.771948 ks3sdk-1.6.3/ks3sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-05-06 06:30:12.000000 ks3sdk-1.6.3/ks3sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-05-06 06:30:12.000000 ks3sdk-1.6.3/ks3sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 06:30:12.000000 ks3sdk-1.6.3/ks3sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-06 06:30:12.000000 ks3sdk-1.6.3/ks3sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-06 06:30:12.000000 ks3sdk-1.6.3/ks3sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 06:30:12.771948 ks3sdk-1.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-05-06 06:28:56.000000 ks3sdk-1.6.3/setup.py
```

### Comparing `ks3sdk-1.6.2/LICENSE` & `ks3sdk-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/PKG-INFO` & `ks3sdk-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ks3sdk
-Version: 1.6.2
+Version: 1.6.3
 Summary: Ksyun KS3 SDK
 Home-page: https://gitee.com/ks3sdk/ks3-python-sdk
 Author: ksc_ks3
 Author-email: ksc_ks3@kingsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ks3sdk-1.6.2/README.md` & `ks3sdk-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/basic.py` & `ks3sdk-1.6.3/examples/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,1517 +19,1625 @@
 00000120: 6b65 7443 6f72 732c 2043 4f52 5352 756c  ketCors, CORSRul
 00000130: 650a 6672 6f6d 206b 7333 2e78 6d6c 5061  e.from ks3.xmlPa
 00000140: 7273 6572 732e 6275 636b 6574 4372 6f73  rsers.bucketCros
 00000150: 7352 6570 6c69 6361 7465 2069 6d70 6f72  sReplicate impor
 00000160: 7420 4275 636b 6574 4372 6f73 7352 6570  t BucketCrossRep
 00000170: 6c69 6361 7465 0a66 726f 6d20 6b73 332e  licate.from ks3.
 00000180: 786d 6c50 6172 7365 7273 2e62 7563 6b65  xmlParsers.bucke
-00000190: 744c 6966 6563 7963 6c65 2069 6d70 6f72  tLifecycle impor
-000001a0: 7420 4275 636b 6574 4c69 6665 6379 636c  t BucketLifecycl
-000001b0: 652c 2052 756c 6520 6173 204c 6966 6563  e, Rule as Lifec
-000001c0: 7963 6c65 5275 6c65 2c20 4669 6c74 6572  ycleRule, Filter
-000001d0: 2061 7320 4c69 6665 6379 636c 6546 696c   as LifecycleFil
-000001e0: 7465 722c 205c 0a20 2045 7870 6972 6174  ter, \.  Expirat
-000001f0: 696f 6e20 6173 204c 6966 6563 7963 6c65  ion as Lifecycle
-00000200: 4578 7069 7261 7469 6f6e 2c20 5472 616e  Expiration, Tran
-00000210: 7369 7469 6f6e 2061 7320 4c69 6665 6379  sition as Lifecy
-00000220: 636c 6554 7261 6e73 6974 696f 6e2c 2041  cleTransition, A
-00000230: 626f 7274 496e 636f 6d70 6c65 7465 4d75  bortIncompleteMu
-00000240: 6c74 6970 6172 7455 706c 6f61 640a 6672  ltipartUpload.fr
-00000250: 6f6d 206b 7333 2e78 6d6c 5061 7273 6572  om ks3.xmlParser
-00000260: 732e 6275 636b 6574 4c6f 6767 696e 6720  s.bucketLogging 
-00000270: 696d 706f 7274 2042 7563 6b65 744c 6f67  import BucketLog
-00000280: 6769 6e67 0a23 20e9 a696 e585 88e5 889d  ging.# .........
-00000290: e5a7 8be5 8c96 4163 6365 7373 4b65 7949  ......AccessKeyI
-000002a0: 64e3 8081 4163 6365 7373 4b65 7953 6563  d...AccessKeySec
-000002b0: 7265 74e3 8081 456e 6470 6f69 6e74 e7ad  ret...Endpoint..
-000002c0: 89e4 bfa1 e681 afe3 8082 0a23 20e9 809a  ...........# ...
-000002d0: e8bf 87e7 8eaf e5a2 83e5 8f98 e987 8fe8  ................
-000002e0: 8eb7 e58f 96ef bc8c e688 96e8 8085 e68a  ................
-000002f0: 8ae8 afb8 e5a6 82e2 809c 3ce4 bda0 e79a  ..........<.....
-00000300: 8441 6363 6573 734b 6579 4964 3ee2 809d  .AccessKeyId>...
-00000310: e69b bfe6 8da2 e688 90e7 9c9f e5ae 9ee7  ................
-00000320: 9a84 4163 6365 7373 4b65 7949 64e7 ad89  ..AccessKeyId...
-00000330: e380 820a 6672 6f6d 206b 7333 2e78 6d6c  ....from ks3.xml
-00000340: 5061 7273 6572 732e 6275 636b 6574 4d69  Parsers.bucketMi
-00000350: 7272 6f72 2069 6d70 6f72 7420 4275 636b  rror import Buck
-00000360: 6574 4d69 7272 6f72 2c20 4173 796e 634d  etMirror, AsyncM
-00000370: 6972 726f 7252 756c 652c 2053 796e 634d  irrorRule, SyncM
-00000380: 6972 726f 7252 756c 6573 2c20 4d69 7272  irrorRules, Mirr
-00000390: 6f72 5265 7175 6573 7453 6574 7469 6e67  orRequestSetting
-000003a0: 2c20 5c0a 2020 4865 6164 6572 5365 7474  , \.  HeaderSett
-000003b0: 696e 670a 6672 6f6d 206b 7333 2e78 6d6c  ing.from ks3.xml
-000003c0: 5061 7273 6572 732e 6275 636b 6574 5265  Parsers.bucketRe
-000003d0: 7465 6e74 696f 6e20 696d 706f 7274 2042  tention import B
-000003e0: 7563 6b65 7452 6574 656e 7469 6f6e 2c20  ucketRetention, 
-000003f0: 5275 6c65 2061 7320 5265 7465 6e74 696f  Rule as Retentio
-00000400: 6e52 756c 650a 6672 6f6d 2062 6173 6536  nRule.from base6
-00000410: 3420 696d 706f 7274 2075 726c 7361 6665  4 import urlsafe
-00000420: 5f62 3634 656e 636f 6465 0a69 6d70 6f72  _b64encode.impor
-00000430: 7420 6173 796e 6369 6f0a 0a61 6b20 3d20  t asyncio..ak = 
-00000440: 6f73 2e67 6574 656e 7628 274b 5333 5f49  os.getenv('KS3_I
-00000450: 414d 5f41 4343 4553 535f 4b45 595f 4944  AM_ACCESS_KEY_ID
-00000460: 272c 2027 3c59 4f55 525f 4143 4345 5353  ', '<YOUR_ACCESS
-00000470: 5f4b 4559 3e27 290a 736b 203d 206f 732e  _KEY>').sk = os.
-00000480: 6765 7465 6e76 2827 4b53 335f 4941 4d5f  getenv('KS3_IAM_
-00000490: 4143 4345 5353 5f4b 4559 5f53 4543 5245  ACCESS_KEY_SECRE
-000004a0: 5427 2c20 273c 594f 5552 5f53 4543 5245  T', '<YOUR_SECRE
-000004b0: 545f 4b45 593e 2729 0a62 7563 6b65 745f  T_KEY>').bucket_
-000004c0: 6e61 6d65 203d 206f 732e 6765 7465 6e76  name = os.getenv
-000004d0: 2827 4b53 335f 4255 434b 4554 272c 2027  ('KS3_BUCKET', '
-000004e0: 3c4b 5333 5f54 4553 545f 4255 434b 4554  <KS3_TEST_BUCKET
-000004f0: 3e27 290a 656e 6470 6f69 6e74 203d 2027  >').endpoint = '
-00000500: 6b73 332d 636e 2d62 6569 6a69 6e67 2e6b  ks3-cn-beijing.k
-00000510: 7379 756e 6373 2e63 6f6d 2720 236f 732e  syuncs.com' #os.
-00000520: 6765 7465 6e76 2827 4b53 335f 5445 5354  getenv('KS3_TEST
-00000530: 5f45 4e44 504f 494e 5427 2c20 276b 7333  _ENDPOINT', 'ks3
-00000540: 2d63 6e2d 7368 616e 6768 6169 2d69 6e74  -cn-shanghai-int
-00000550: 6572 6e61 6c2e 6b73 7975 6e63 732e 636f  ernal.ksyuncs.co
-00000560: 6d27 290a 0a63 6f6e 6e20 3d20 436f 6e6e  m')..conn = Conn
-00000570: 6563 7469 6f6e 2861 6b2c 2073 6b2c 2068  ection(ak, sk, h
-00000580: 6f73 743d 656e 6470 6f69 6e74 2c20 706f  ost=endpoint, po
-00000590: 7274 3d38 302c 2075 615f 6164 646f 6e3d  rt=80, ua_addon=
-000005a0: 2774 6573 742d 7561 2f31 2729 2023 706f  'test-ua/1') #po
-000005b0: 7274 3d38 3039 312c 0a6b 6579 5f6e 616d  rt=8091,.key_nam
-000005c0: 6520 3d20 2774 6573 745f 6b65 7927 0a0a  e = 'test_key'..
-000005d0: 0a64 6566 2067 6574 416c 6c42 7563 6b65  .def getAllBucke
-000005e0: 7473 2870 726f 6a65 6374 5f69 6473 3d4e  ts(project_ids=N
-000005f0: 6f6e 6529 3a0a 2020 6275 636b 6574 7320  one):.  buckets 
-00000600: 3d20 636f 6e6e 2e67 6574 5f61 6c6c 5f62  = conn.get_all_b
-00000610: 7563 6b65 7473 2870 726f 6a65 6374 5f69  uckets(project_i
-00000620: 6473 3d70 726f 6a65 6374 5f69 6473 2920  ds=project_ids) 
-00000630: 230a 2020 666f 7220 6220 696e 2062 7563  #.  for b in buc
-00000640: 6b65 7473 3a0a 2020 2020 7072 696e 7428  kets:.    print(
-00000650: 622e 6e61 6d65 2c20 622e 7265 6769 6f6e  b.name, b.region
-00000660: 2c20 622e 5265 6769 6f6e 2c20 622e 6372  , b.Region, b.cr
-00000670: 6561 7469 6f6e 5f64 6174 6529 0a0a 6465  eation_date)..de
-00000680: 6620 6865 6164 4275 636b 6574 2862 7563  f headBucket(buc
-00000690: 6b65 745f 6e61 6d65 293a 0a20 2023 20e5  ket_name):.  # .
-000006a0: a682 e69e 9ce6 ada3 e5b8 b8e8 bf94 e59b  ................
-000006b0: 9eef bc8c e588 9942 7563 6b65 74e5 ad98  .......Bucket...
-000006c0: e59c a8ef bc9b e5a6 82e6 9e9c e68a 9be5  ................
-000006d0: 87ba 5333 5265 7370 6f6e 7365 4572 726f  ..S3ResponseErro
-000006e0: 720a 2020 636f 6e6e 2e68 6561 645f 6275  r.  conn.head_bu
-000006f0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00000700: 290a 0a64 6566 2067 6574 4275 636b 6574  )..def getBucket
-00000710: 4c6f 6361 7469 6f6e 2862 7563 6b65 745f  Location(bucket_
-00000720: 6e61 6d65 293a 0a20 2070 7269 6e74 2863  name):.  print(c
-00000730: 6f6e 6e2e 6765 745f 6275 636b 6574 5f6c  onn.get_bucket_l
-00000740: 6f63 6174 696f 6e28 6275 636b 6574 5f6e  ocation(bucket_n
-00000750: 616d 6529 290a 0a64 6566 2063 7265 6174  ame))..def creat
-00000760: 6542 7563 6b65 7428 6275 636b 6574 5f6e  eBucket(bucket_n
-00000770: 616d 652c 206c 6f63 6174 696f 6e3d 2727  ame, location=''
-00000780: 293a 0a20 2063 6f6e 6e2e 6372 6561 7465  ):.  conn.create
-00000790: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-000007a0: 616d 652c 206c 6f63 6174 696f 6e3d 6c6f  ame, location=lo
-000007b0: 6361 7469 6f6e 2c20 6865 6164 6572 733d  cation, headers=
-000007c0: 7b0a 2020 2020 2778 2d6b 7373 2d62 7563  {.    'x-kss-buc
-000007d0: 6b65 742d 7479 7065 273a 2027 4152 4348  ket-type': 'ARCH
-000007e0: 4956 4527 0a20 207d 290a 0a64 6566 2064  IVE'.  })..def d
-000007f0: 656c 6574 6542 7563 6b65 7428 6275 636b  eleteBucket(buck
-00000800: 6574 5f6e 616d 6529 3a0a 2020 7472 793a  et_name):.  try:
-00000810: 0a20 2020 2063 6f6e 6e2e 6465 6c65 7465  .    conn.delete
-00000820: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-00000830: 616d 6529 0a20 2065 7863 6570 7420 5333  ame).  except S3
-00000840: 5265 7370 6f6e 7365 4572 726f 7220 6173  ResponseError as
-00000850: 2065 7272 6f72 3a0a 2020 2020 7072 696e   error:.    prin
-00000860: 7428 2765 7272 6f72 2729 0a20 2020 2070  t('error').    p
-00000870: 7269 6e74 2865 7272 6f72 290a 0a64 6566  rint(error)..def
-00000880: 2067 6574 4275 636b 6574 4163 6c28 6275   getBucketAcl(bu
-00000890: 636b 6574 5f6e 616d 6529 3a0a 2020 6220  cket_name):.  b 
-000008a0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-000008b0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-000008c0: 2070 6f6c 6963 7920 3d20 622e 6765 745f   policy = b.get_
-000008d0: 6163 6c28 290a 2020 2320 7072 696e 7428  acl().  # print(
-000008e0: 706f 6c69 6379 290a 2020 666f 7220 6772  policy).  for gr
-000008f0: 616e 7420 696e 2070 6f6c 6963 792e 6163  ant in policy.ac
-00000900: 6c2e 6772 616e 7473 3a0a 2020 2020 7072  l.grants:.    pr
-00000910: 696e 7428 6772 616e 742e 7065 726d 6973  int(grant.permis
-00000920: 7369 6f6e 2c20 6772 616e 742e 6469 7370  sion, grant.disp
-00000930: 6c61 795f 6e61 6d65 2c20 6772 616e 742e  lay_name, grant.
-00000940: 656d 6169 6c5f 6164 6472 6573 732c 2067  email_address, g
-00000950: 7261 6e74 2e69 6429 0a0a 6465 6620 7365  rant.id)..def se
-00000960: 7442 7563 6b65 7441 636c 2862 7563 6b65  tBucketAcl(bucke
-00000970: 745f 6e61 6d65 293a 0a20 2062 203d 2063  t_name):.  b = c
-00000980: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00000990: 7563 6b65 745f 6e61 6d65 290a 2020 622e  ucket_name).  b.
-000009a0: 7365 745f 6163 6c28 2270 7269 7661 7465  set_acl("private
-000009b0: 2229 0a0a 6465 6620 6d61 6e61 6765 4275  ")..def manageBu
-000009c0: 636b 6574 506f 6c69 6379 2862 7563 6b65  cketPolicy(bucke
-000009d0: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
-000009e0: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
-000009f0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-00000a00: 0a20 2062 7563 6b65 742e 7365 745f 6275  .  bucket.set_bu
-00000a10: 636b 6574 5f70 6f6c 6963 7928 0a20 2020  cket_policy(.   
-00000a20: 2070 6f6c 6963 793d 277b 2253 7461 7465   policy='{"State
-00000a30: 6d65 6e74 223a 5b7b 2252 6573 6f75 7263  ment":[{"Resourc
-00000a40: 6522 3a5b 226b 726e 3a6b 7363 3a6b 7333  e":["krn:ksc:ks3
-00000a50: 3a3a 3a6a 6961 6e67 7261 6e31 3233 222c  :::jiangran123",
-00000a60: 226b 726e 3a6b 7363 3a6b 7333 3a3a 3a6a  "krn:ksc:ks3:::j
-00000a70: 6961 6e67 7261 6e31 3233 2f2a 225d 2c22  iangran123/*"],"
-00000a80: 5072 696e 6369 7061 6c22 3a7b 224b 5343  Principal":{"KSC
-00000a90: 223a 5b22 6b72 6e3a 6b73 633a 6961 6d3a  ":["krn:ksc:iam:
-00000aa0: 3a33 3234 3332 3432 333a 726f 6f74 225d  :32432423:root"]
-00000ab0: 7d2c 2241 6374 696f 6e22 3a5b 226b 7333  },"Action":["ks3
-00000ac0: 3a2a 225d 2c22 4566 6665 6374 223a 2241  :*"],"Effect":"A
-00000ad0: 6c6c 6f77 227d 5d7d 2729 0a20 2023 2070  llow"}]}').  # p
-00000ae0: 6f6c 6963 7920 3d20 6275 636b 6574 2e67  olicy = bucket.g
-00000af0: 6574 5f62 7563 6b65 745f 706f 6c69 6379  et_bucket_policy
-00000b00: 2829 0a20 2023 2062 7563 6b65 742e 6465  ().  # bucket.de
-00000b10: 6c65 7465 5f62 7563 6b65 745f 706f 6c69  lete_bucket_poli
-00000b20: 6379 2829 0a0a 6465 6620 6d61 6e61 6765  cy()..def manage
-00000b30: 4275 636b 6574 5265 706c 6963 6174 696f  BucketReplicatio
-00000b40: 6e28 6275 636b 6574 5f6e 616d 6529 3a0a  n(bucket_name):.
-00000b50: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00000b60: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00000b70: 745f 6e61 6d65 290a 2020 7472 793a 0a20  t_name).  try:. 
-00000b80: 2020 2070 7269 6e74 2862 7563 6b65 742e     print(bucket.
-00000b90: 6765 745f 6275 636b 6574 5f63 7272 2829  get_bucket_crr()
-00000ba0: 2e74 6f5f 786d 6c28 2929 0a20 2065 7863  .to_xml()).  exc
-00000bb0: 6570 743a 0a20 2020 2062 7563 6b65 742e  ept:.    bucket.
-00000bc0: 7365 745f 6275 636b 6574 5f63 7272 2827  set_bucket_crr('
-00000bd0: 7465 7374 2d62 7563 6b65 742d 7072 6f6a  test-bucket-proj
-00000be0: 6563 7427 2c20 6465 6c65 7465 4d61 726b  ect', deleteMark
-00000bf0: 6572 5374 6174 7573 3d27 4469 7361 626c  erStatus='Disabl
-00000c00: 6564 272c 2070 7265 6669 785f 6c69 7374  ed', prefix_list
-00000c10: 3d5b 2768 656c 6c6f 275d 290a 0a64 6566  =['hello'])..def
-00000c20: 2067 6574 4275 636b 6574 4c69 6665 4379   getBucketLifeCy
-00000c30: 636c 6528 6275 636b 6574 5f6e 616d 6529  cle(bucket_name)
-00000c40: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
-00000c50: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-00000c60: 6b65 745f 6e61 6d65 290a 2020 6c69 6665  ket_name).  life
-00000c70: 6379 636c 6520 3d20 6275 636b 6574 2e67  cycle = bucket.g
-00000c80: 6574 5f62 7563 6b65 745f 6c69 6665 6379  et_bucket_lifecy
-00000c90: 636c 6528 290a 2020 7072 696e 7428 6c69  cle().  print(li
-00000ca0: 6665 6379 636c 652e 746f 5f78 6d6c 2829  fecycle.to_xml()
-00000cb0: 290a 0a64 6566 2073 6574 4275 636b 6574  )..def setBucket
-00000cc0: 4c69 6665 4379 636c 6528 6275 636b 6574  LifeCycle(bucket
-00000cd0: 5f6e 616d 6529 3a0a 2020 6275 636b 6574  _name):.  bucket
-00000ce0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-00000cf0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00000d00: 2020 6c69 6665 6379 636c 6520 3d20 4275    lifecycle = Bu
-00000d10: 636b 6574 4c69 6665 6379 636c 6528 290a  cketLifecycle().
-00000d20: 2020 2320 6964 20e5 928c 2073 7461 7475    # id ... statu
-00000d30: 7320 e5bf 85e9 a1bb 0a20 2072 756c 6520  s .......  rule 
-00000d40: 3d20 4c69 6665 6379 636c 6552 756c 6528  = LifecycleRule(
-00000d50: 6964 3d27 7275 6c65 3127 2c20 7374 6174  id='rule1', stat
-00000d60: 7573 3d27 456e 6162 6c65 6427 290a 2020  us='Enabled').  
-00000d70: 6461 7465 203d 2064 6174 6574 696d 6528  date = datetime(
-00000d80: 3230 3231 2c20 392c 2031 3229 2e73 7472  2021, 9, 12).str
-00000d90: 6674 696d 6528 2725 592d 256d 2d25 6454  ftime('%Y-%m-%dT
-00000da0: 2548 3a25 4d3a 2553 2729 202b 2027 2b30  %H:%M:%S') + '+0
-00000db0: 383a 3030 270a 2020 7275 6c65 2e65 7870  8:00'.  rule.exp
-00000dc0: 6972 6174 696f 6e20 3d20 4c69 6665 6379  iration = Lifecy
-00000dd0: 636c 6545 7870 6972 6174 696f 6e28 6461  cleExpiration(da
-00000de0: 7465 3d64 6174 6529 0a20 206c 6966 6563  te=date).  lifec
-00000df0: 7963 6c65 2e72 756c 6520 3d20 5b72 756c  ycle.rule = [rul
-00000e00: 655d 0a20 2062 7563 6b65 742e 7365 745f  e].  bucket.set_
-00000e10: 6275 636b 6574 5f6c 6966 6563 7963 6c65  bucket_lifecycle
-00000e20: 286c 6966 6563 7963 6c65 290a 0a0a 6465  (lifecycle)...de
-00000e30: 6620 7365 7442 7563 6b65 744c 6966 6543  f setBucketLifeC
-00000e40: 7963 6c65 3228 6275 636b 6574 5f6e 616d  ycle2(bucket_nam
-00000e50: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
-00000e60: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00000e70: 7563 6b65 745f 6e61 6d65 290a 2020 7461  ucket_name).  ta
-00000e80: 6720 3d20 5461 6728 6b65 793d 2274 6167  g = Tag(key="tag
-00000e90: 3122 2c20 7661 6c75 653d 2274 6573 7431  1", value="test1
-00000ea0: 2229 0a20 2023 20e7 ad9b e980 89e5 898d  ").  # .........
-00000eb0: e7bc 80e4 b8ba 2070 7265 6669 7831 e380  ...... prefix1..
-00000ec0: 81e6 a087 e7ad bee4 b8ba 2074 6167 313a  .......... tag1:
-00000ed0: 7465 7374 3120 e79a 8420 6f62 6a65 6374  test1 ... object
-00000ee0: 73ef bc8c e8ae bee7 bdae e8bf 87e6 9c9f  s...............
-00000ef0: e8a7 84e5 8899 efbc 8ce5 9ca8 e585 b6e6  ................
-00000f00: 9c80 e590 8ee4 bfae e694 b9e6 97b6 e997  ................
-00000f10: b433 e5a4 a9e5 908e e8bf 87e6 9c9f e380  .3..............
-00000f20: 820a 2020 7275 6c65 3120 3d20 4c69 6665  ..  rule1 = Life
-00000f30: 6379 636c 6552 756c 6528 2772 756c 6531  cycleRule('rule1
-00000f40: 272c 204c 6966 6563 7963 6c65 4669 6c74  ', LifecycleFilt
-00000f50: 6572 2827 7072 6566 6978 3127 2c20 7461  er('prefix1', ta
-00000f60: 6773 3d5b 7461 675d 292c 0a20 2020 2020  gs=[tag]),.     
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2073 7461 7475 733d 2745 6e61 626c     status='Enabl
-00000f90: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
-00000fa0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00000fb0: 6972 6174 696f 6e3d 4c69 6665 6379 636c  iration=Lifecycl
-00000fc0: 6545 7870 6972 6174 696f 6e28 6461 7973  eExpiration(days
-00000fd0: 3d33 2929 0a0a 2020 2320 e8ae bee7 bdae  =3))..  # ......
-00000fe0: e8bf 87e6 9c9f e8a7 84e5 8899 efbc 8ce7  ................
-00000ff0: ad9b e980 89e6 a087 e7ad bee4 b8ba 2074  .............. t
-00001000: 6167 313a 7465 7374 3120 e79a 8420 6f62  ag1:test1 ... ob
-00001010: 6a65 6374 73ef bc8c e69c 80e5 908e e4bf  jects...........
-00001020: aee6 94b9 e697 b6e9 97b4 e59c a8e6 8c87  ................
-00001030: e5ae 9ae6 97a5 e69c 9fe4 b98b e589 8de7  ................
-00001040: 9a84 efbc 8ce8 bf87 e69c 9f0a 2020 7275  ............  ru
-00001050: 6c65 3220 3d20 4c69 6665 6379 636c 6552  le2 = LifecycleR
-00001060: 756c 6528 2772 756c 6532 272c 204c 6966  ule('rule2', Lif
-00001070: 6563 7963 6c65 4669 6c74 6572 2874 6167  ecycleFilter(tag
-00001080: 733d 5b74 6167 5d29 2c0a 2020 2020 2020  s=[tag]),.      
-00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010a0: 2020 7374 6174 7573 3d27 456e 6162 6c65    status='Enable
-000010b0: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-000010c0: 2020 2020 2020 2020 2020 2020 6578 7069              expi
-000010d0: 7261 7469 6f6e 3d4c 6966 6563 7963 6c65  ration=Lifecycle
-000010e0: 4578 7069 7261 7469 6f6e 280a 2020 2020  Expiration(.    
-000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001100: 2020 2020 2020 6461 7465 3d64 6174 6574        date=datet
-00001110: 696d 6528 3230 3231 2c20 3132 2c20 3132  ime(2021, 12, 12
-00001120: 292e 6973 6f66 6f72 6d61 7428 7469 6d65  ).isoformat(time
-00001130: 7370 6563 3d27 7365 636f 6e64 7327 2920  spec='seconds') 
-00001140: 2b20 272b 3038 3a30 3027 2929 0a0a 2020  + '+08:00'))..  
-00001150: 2320 e8ae bee7 bdae e5ad 98e5 82a8 e7b1  # ..............
-00001160: bbe5 9e8b e8bd ace6 8da2 e8a7 84e5 8899  ................
-00001170: efbc 8ce7 ad9b e980 89e5 898d e7bc 80e4  ................
-00001180: b8ba 2070 7265 6669 7833 20e7 9a84 206f  .. prefix3 ... o
-00001190: 626a 6563 7473 efbc 8ce5 9ca8 e585 b6e6  bjects..........
-000011a0: 9c80 e590 8ee4 bfae e694 b9e6 97b6 e997  ................
-000011b0: b432 30e5 a4a9 e4b9 8be5 908e e8bd ace4  .20.............
-000011c0: b8ba e4bd 8ee9 a291 e8ae bfe9 97ae e7b1  ................
-000011d0: bbe5 9e8b efbc 8ce5 9ca8 e585 b6e6 9c80  ................
-000011e0: e590 8ee4 bfae e694 b9e6 97b6 e997 b433  ...............3
-000011f0: 30e5 a4a9 e4b9 8be5 908e e8bd ace4 b8ba  0...............
-00001200: e5bd 92e6 a1a3 e7b1 bbe5 9e8b e380 820a  ................
-00001210: 2020 7275 6c65 3320 3d20 4c69 6665 6379    rule3 = Lifecy
-00001220: 636c 6552 756c 6528 2772 756c 6533 272c  cleRule('rule3',
-00001230: 204c 6966 6563 7963 6c65 4669 6c74 6572   LifecycleFilter
-00001240: 2827 7072 6566 6978 3327 292c 0a20 2020  ('prefix3'),.   
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 2020 2073 7461 7475 733d 2745 6e61       status='Ena
-00001270: 626c 6564 272c 0a20 2020 2020 2020 2020  bled',.         
-00001280: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001290: 7261 6e73 6974 696f 6e73 3d5b 4c69 6665  ransitions=[Life
-000012a0: 6379 636c 6554 7261 6e73 6974 696f 6e28  cycleTransition(
-000012b0: 6461 7973 3d32 302c 2073 746f 7261 6765  days=20, storage
-000012c0: 5f63 6c61 7373 3d27 5354 414e 4441 5244  _class='STANDARD
-000012d0: 5f49 4127 292c 0a20 2020 2020 2020 2020  _IA'),.         
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 2020 2020 2020 2020 4c69 6665              Life
-00001300: 6379 636c 6554 7261 6e73 6974 696f 6e28  cycleTransition(
-00001310: 6461 7973 3d36 302c 2073 746f 7261 6765  days=60, storage
-00001320: 5f63 6c61 7373 3d27 4152 4348 4956 4527  _class='ARCHIVE'
-00001330: 295d 290a 0a20 2023 20e8 aebe e7bd aee5  )])..  # .......
-00001340: ad98 e582 a8e7 b1bb e59e 8be8 bdac e68d  ................
-00001350: a2e8 a784 e588 99ef bc8c e7ad 9be9 8089  ................
-00001360: e589 8de7 bc80 e4b8 ba20 7072 6566 6978  ......... prefix
-00001370: 3320 e79a 8420 6f62 6a65 6374 73ef bc8c  3 ... objects...
-00001380: e69c 80e5 908e e4bf aee6 94b9 e697 b6e9  ................
-00001390: 97b4 e59c a8e6 8c87 e5ae 9ae6 97a5 e69c  ................
-000013a0: 9fe4 b98b e589 8de7 9a84 efbc 8ce8 bdac  ................
-000013b0: e4b8 bae4 bd8e e9a2 91e8 aebf e997 aee7  ................
-000013c0: b1bb e59e 8b0a 2020 7275 6c65 3420 3d20  ......  rule4 = 
-000013d0: 4c69 6665 6379 636c 6552 756c 6528 2772  LifecycleRule('r
-000013e0: 756c 6534 272c 204c 6966 6563 7963 6c65  ule4', Lifecycle
-000013f0: 4669 6c74 6572 2827 7072 6566 6978 3427  Filter('prefix4'
-00001400: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001410: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00001420: 733d 2745 6e61 626c 6564 272c 0a20 2020  s='Enabled',.   
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2020 2074 7261 6e73 6974 696f 6e73       transitions
-00001450: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
-00001460: 2020 2020 2020 2020 2020 2020 204c 6966               Lif
-00001470: 6563 7963 6c65 5472 616e 7369 7469 6f6e  ecycleTransition
-00001480: 2864 6174 653d 6461 7465 7469 6d65 2832  (date=datetime(2
-00001490: 3032 312c 2031 322c 2031 3229 2e69 736f  021, 12, 12).iso
-000014a0: 666f 726d 6174 2874 696d 6573 7065 633d  format(timespec=
-000014b0: 2773 6563 6f6e 6473 2729 202b 2027 2b30  'seconds') + '+0
-000014c0: 383a 3030 272c 0a20 2020 2020 2020 2020  8:00',.         
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2073 746f 7261 6765 5f63 6c61       storage_cla
-00001500: 7373 3d27 5354 414e 4441 5244 5f49 4127  ss='STANDARD_IA'
-00001510: 295d 290a 2020 2320 e8ae bee7 bdae e588  )]).  # ........
-00001520: 86e7 8987 e4b8 8ae4 bca0 e7a2 8ee7 8987  ................
-00001530: e6b8 85e7 9086 e8a7 84e5 8899 efbc 8ce7  ................
-00001540: ad9b e980 89e5 898d e7bc 80e4 b8ba 2070  .............. p
-00001550: 7265 6669 7835 20e7 9a84 2070 6172 74ef  refix5 ... part.
-00001560: bc8c e59c a8e6 9c80 e590 8ee4 bfae e694  ................
-00001570: b9e6 97b6 e997 b437 e5a4 a9e5 908e e588  .......7........
-00001580: a0e9 99a4 0a20 2072 756c 6535 203d 204c  .....  rule5 = L
-00001590: 6966 6563 7963 6c65 5275 6c65 2827 7275  ifecycleRule('ru
-000015a0: 6c65 3527 2c20 4c69 6665 6379 636c 6546  le5', LifecycleF
-000015b0: 696c 7465 7228 2770 7265 6669 7835 2729  ilter('prefix5')
-000015c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000015d0: 2020 2020 2020 2020 2020 7374 6174 7573            status
-000015e0: 3d27 456e 6162 6c65 6427 2c0a 2020 2020  ='Enabled',.    
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 6162 6f72 745f 696e 636f 6d70      abort_incomp
-00001610: 6c65 7465 5f6d 756c 7469 7061 7274 5f75  lete_multipart_u
-00001620: 706c 6f61 643d 4162 6f72 7449 6e63 6f6d  pload=AbortIncom
-00001630: 706c 6574 654d 756c 7469 7061 7274 5570  pleteMultipartUp
-00001640: 6c6f 6164 2864 6179 735f 6166 7465 725f  load(days_after_
-00001650: 696e 6974 6961 7469 6f6e 3d37 2929 0a0a  initiation=7))..
-00001660: 2020 2320 7072 696e 7428 7275 6c65 312e    # print(rule1.
-00001670: 746f 5f78 6d6c 2829 290a 2020 2320 7072  to_xml()).  # pr
-00001680: 696e 7428 7275 6c65 322e 746f 5f78 6d6c  int(rule2.to_xml
-00001690: 2829 290a 2020 2320 7072 696e 7428 7275  ()).  # print(ru
-000016a0: 6c65 332e 746f 5f78 6d6c 2829 290a 2020  le3.to_xml()).  
-000016b0: 2320 7072 696e 7428 7275 6c65 342e 746f  # print(rule4.to
-000016c0: 5f78 6d6c 2829 290a 2020 2320 7072 696e  _xml()).  # prin
-000016d0: 7428 7275 6c65 352e 746f 5f78 6d6c 2829  t(rule5.to_xml()
-000016e0: 290a 2020 6c69 6665 6379 636c 6520 3d20  ).  lifecycle = 
-000016f0: 4275 636b 6574 4c69 6665 6379 636c 6528  BucketLifecycle(
-00001700: 5b72 756c 6531 2c20 7275 6c65 322c 2072  [rule1, rule2, r
-00001710: 756c 6533 2c20 7275 6c65 342c 2072 756c  ule3, rule4, rul
-00001720: 6535 5d29 0a20 2062 7563 6b65 742e 7365  e5]).  bucket.se
-00001730: 745f 6275 636b 6574 5f6c 6966 6563 7963  t_bucket_lifecyc
-00001740: 6c65 286c 6966 6563 7963 6c65 290a 0a64  le(lifecycle)..d
-00001750: 6566 2064 656c 6574 6542 7563 6b65 744c  ef deleteBucketL
-00001760: 6966 6543 7963 6c65 2862 7563 6b65 745f  ifeCycle(bucket_
-00001770: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
-00001780: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-00001790: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-000017a0: 2062 7563 6b65 742e 6465 6c65 7465 5f62   bucket.delete_b
-000017b0: 7563 6b65 745f 6c69 6665 6379 636c 6528  ucket_lifecycle(
-000017c0: 290a 0a64 6566 2067 6574 4275 636b 6574  )..def getBucket
-000017d0: 4c6f 6767 696e 6728 6275 636b 6574 5f6e  Logging(bucket_n
-000017e0: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
-000017f0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-00001800: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00001810: 7072 696e 7428 6275 636b 6574 2e67 6574  print(bucket.get
-00001820: 5f62 7563 6b65 745f 6c6f 6767 696e 6728  _bucket_logging(
-00001830: 292e 746f 5f78 6d6c 2829 290a 0a64 6566  ).to_xml())..def
-00001840: 2073 6574 4275 636b 6574 4c6f 6767 696e   setBucketLoggin
-00001850: 6728 6275 636b 6574 5f6e 616d 6529 3a0a  g(bucket_name):.
-00001860: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00001870: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00001880: 745f 6e61 6d65 290a 2020 626c 6f67 6769  t_name).  bloggi
-00001890: 6e67 203d 2042 7563 6b65 744c 6f67 6769  ng = BucketLoggi
-000018a0: 6e67 2874 6172 6765 743d 6275 636b 6574  ng(target=bucket
-000018b0: 5f6e 616d 652c 2074 6172 6765 745f 7072  _name, target_pr
-000018c0: 6566 6978 3d27 7465 7374 5f6c 6f67 2729  efix='test_log')
-000018d0: 0a20 2070 7269 6e74 2862 7563 6b65 742e  .  print(bucket.
-000018e0: 7365 745f 6275 636b 6574 5f6c 6f67 6769  set_bucket_loggi
-000018f0: 6e67 2862 6c6f 6767 696e 672e 746f 5f78  ng(blogging.to_x
-00001900: 6d6c 2829 2929 0a0a 6465 6620 656e 6162  ml()))..def enab
-00001910: 6c65 4275 636b 6574 4c6f 6767 696e 6728  leBucketLogging(
-00001920: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
-00001930: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00001940: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00001950: 6e61 6d65 290a 2020 7072 696e 7428 6275  name).  print(bu
-00001960: 636b 6574 2e65 6e61 626c 655f 6c6f 6767  cket.enable_logg
-00001970: 696e 6728 6275 636b 6574 2c20 7461 7267  ing(bucket, targ
-00001980: 6574 5f70 7265 6669 783d 2768 6568 6568  et_prefix='heheh
-00001990: 6568 6527 2929 0a0a 6465 6620 6469 7361  ehe'))..def disa
-000019a0: 626c 6542 7563 6b65 744c 6f67 6769 6e67  bleBucketLogging
-000019b0: 2862 7563 6b65 745f 6e61 6d65 293a 0a20  (bucket_name):. 
-000019c0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-000019d0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-000019e0: 5f6e 616d 6529 0a20 2070 7269 6e74 2862  _name).  print(b
-000019f0: 7563 6b65 742e 6469 7361 626c 655f 6c6f  ucket.disable_lo
-00001a00: 6767 696e 6728 2929 0a0a 6465 6620 6765  gging())..def ge
-00001a10: 7442 7563 6b65 7443 6f72 7328 6275 636b  tBucketCors(buck
-00001a20: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-00001a30: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00001a40: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00001a50: 290a 2020 7072 696e 7428 6275 636b 6574  ).  print(bucket
-00001a60: 2e67 6574 5f62 7563 6b65 745f 636f 7273  .get_bucket_cors
-00001a70: 2829 2e74 6f5f 786d 6c28 2929 0a0a 6465  ().to_xml())..de
-00001a80: 6620 7075 7442 7563 6b65 7443 6f72 7328  f putBucketCors(
-00001a90: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
-00001aa0: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00001ab0: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00001ac0: 6e61 6d65 290a 2020 636f 7273 203d 2042  name).  cors = B
-00001ad0: 7563 6b65 7443 6f72 7328 5b43 4f52 5352  ucketCors([CORSR
-00001ae0: 756c 6528 6f72 6967 696e 733d 5b22 6874  ule(origins=["ht
-00001af0: 7470 3a2f 2f64 6576 2e6b 7379 756e 2e63  tp://dev.ksyun.c
-00001b00: 6f6d 225d 2c20 6d65 7468 6f64 733d 5b22  om"], methods=["
-00001b10: 4745 5422 2c20 2248 4541 4422 5d2c 206d  GET", "HEAD"], m
-00001b20: 6178 5f61 6765 3d22 3230 3022 2c20 6865  ax_age="200", he
-00001b30: 6164 6572 733d 5b22 636f 6e74 656e 742d  aders=["content-
-00001b40: 7479 7065 225d 2c20 6578 706f 7365 645f  type"], exposed_
-00001b50: 6865 6164 6572 733d 5b22 636f 6e74 656e  headers=["conten
-00001b60: 742d 7479 7065 222c 2022 782d 6b73 732d  t-type", "x-kss-
-00001b70: 6163 6c22 5d29 5d29 0a20 2070 7269 6e74  acl"])]).  print
-00001b80: 2827 636f 7273 3a20 272c 2063 6f72 732e  ('cors: ', cors.
-00001b90: 746f 5f78 6d6c 2829 290a 2020 7072 696e  to_xml()).  prin
-00001ba0: 7428 6275 636b 6574 2e73 6574 5f62 7563  t(bucket.set_buc
-00001bb0: 6b65 745f 636f 7273 2863 6f72 7329 290a  ket_cors(cors)).
-00001bc0: 0a64 6566 2064 656c 6574 6542 7563 6b65  .def deleteBucke
-00001bd0: 7443 6f72 7328 6275 636b 6574 5f6e 616d  tCors(bucket_nam
-00001be0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
-00001bf0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00001c00: 7563 6b65 745f 6e61 6d65 290a 2020 7072  ucket_name).  pr
-00001c10: 696e 7428 6275 636b 6574 2e64 656c 6574  int(bucket.delet
-00001c20: 655f 6275 636b 6574 5f63 6f72 7328 2929  e_bucket_cors())
-00001c30: 0a0a 6465 6620 6765 7442 7563 6b65 7443  ..def getBucketC
-00001c40: 7272 2862 7563 6b65 745f 6e61 6d65 293a  rr(bucket_name):
+00000190: 7449 6e76 656e 746f 7279 2069 6d70 6f72  tInventory impor
+000001a0: 7420 4275 636b 6574 496e 7665 6e74 6f72  t BucketInventor
+000001b0: 792c 2044 6573 7469 6e61 7469 6f6e 2c20  y, Destination, 
+000001c0: 5363 6865 6475 6c65 2c20 4669 6c74 6572  Schedule, Filter
+000001d0: 2061 7320 496e 7665 6e74 6f72 7946 696c   as InventoryFil
+000001e0: 7465 720a 6672 6f6d 206b 7333 2e78 6d6c  ter.from ks3.xml
+000001f0: 5061 7273 6572 732e 6275 636b 6574 4c69  Parsers.bucketLi
+00000200: 6665 6379 636c 6520 696d 706f 7274 2042  fecycle import B
+00000210: 7563 6b65 744c 6966 6563 7963 6c65 2c20  ucketLifecycle, 
+00000220: 5275 6c65 2061 7320 4c69 6665 6379 636c  Rule as Lifecycl
+00000230: 6552 756c 652c 2046 696c 7465 7220 6173  eRule, Filter as
+00000240: 204c 6966 6563 7963 6c65 4669 6c74 6572   LifecycleFilter
+00000250: 2c20 5c0a 2020 4578 7069 7261 7469 6f6e  , \.  Expiration
+00000260: 2061 7320 4c69 6665 6379 636c 6545 7870   as LifecycleExp
+00000270: 6972 6174 696f 6e2c 2054 7261 6e73 6974  iration, Transit
+00000280: 696f 6e20 6173 204c 6966 6563 7963 6c65  ion as Lifecycle
+00000290: 5472 616e 7369 7469 6f6e 2c20 4162 6f72  Transition, Abor
+000002a0: 7449 6e63 6f6d 706c 6574 654d 756c 7469  tIncompleteMulti
+000002b0: 7061 7274 5570 6c6f 6164 0a66 726f 6d20  partUpload.from 
+000002c0: 6b73 332e 786d 6c50 6172 7365 7273 2e62  ks3.xmlParsers.b
+000002d0: 7563 6b65 744c 6f67 6769 6e67 2069 6d70  ucketLogging imp
+000002e0: 6f72 7420 4275 636b 6574 4c6f 6767 696e  ort BucketLoggin
+000002f0: 670a 2320 e9a6 96e5 8588 e588 9de5 a78b  g.# ............
+00000300: e58c 9641 6363 6573 734b 6579 4964 e380  ...AccessKeyId..
+00000310: 8141 6363 6573 734b 6579 5365 6372 6574  .AccessKeySecret
+00000320: e380 8145 6e64 706f 696e 74e7 ad89 e4bf  ...Endpoint.....
+00000330: a1e6 81af e380 820a 2320 e980 9ae8 bf87  ........# ......
+00000340: e78e afe5 a283 e58f 98e9 878f e88e b7e5  ................
+00000350: 8f96 efbc 8ce6 8896 e880 85e6 8a8a e8af  ................
+00000360: b8e5 a682 e280 9c3c e4bd a0e7 9a84 4163  .......<......Ac
+00000370: 6365 7373 4b65 7949 643e e280 9de6 9bbf  cessKeyId>......
+00000380: e68d a2e6 8890 e79c 9fe5 ae9e e79a 8441  ...............A
+00000390: 6363 6573 734b 6579 4964 e7ad 89e3 8082  ccessKeyId......
+000003a0: 0a66 726f 6d20 6b73 332e 786d 6c50 6172  .from ks3.xmlPar
+000003b0: 7365 7273 2e62 7563 6b65 744d 6972 726f  sers.bucketMirro
+000003c0: 7220 696d 706f 7274 2042 7563 6b65 744d  r import BucketM
+000003d0: 6972 726f 722c 2041 7379 6e63 4d69 7272  irror, AsyncMirr
+000003e0: 6f72 5275 6c65 2c20 5379 6e63 4d69 7272  orRule, SyncMirr
+000003f0: 6f72 5275 6c65 732c 204d 6972 726f 7252  orRules, MirrorR
+00000400: 6571 7565 7374 5365 7474 696e 672c 205c  equestSetting, \
+00000410: 0a20 2048 6561 6465 7253 6574 7469 6e67  .  HeaderSetting
+00000420: 0a66 726f 6d20 6b73 332e 786d 6c50 6172  .from ks3.xmlPar
+00000430: 7365 7273 2e62 7563 6b65 7452 6574 656e  sers.bucketReten
+00000440: 7469 6f6e 2069 6d70 6f72 7420 4275 636b  tion import Buck
+00000450: 6574 5265 7465 6e74 696f 6e2c 2052 756c  etRetention, Rul
+00000460: 6520 6173 2052 6574 656e 7469 6f6e 5275  e as RetentionRu
+00000470: 6c65 0a66 726f 6d20 6261 7365 3634 2069  le.from base64 i
+00000480: 6d70 6f72 7420 7572 6c73 6166 655f 6236  mport urlsafe_b6
+00000490: 3465 6e63 6f64 650a 696d 706f 7274 2061  4encode.import a
+000004a0: 7379 6e63 696f 0a0a 616b 203d 206f 732e  syncio..ak = os.
+000004b0: 6765 7465 6e76 2827 4b53 335f 4941 4d5f  getenv('KS3_IAM_
+000004c0: 4143 4345 5353 5f4b 4559 5f49 4427 2c20  ACCESS_KEY_ID', 
+000004d0: 273c 594f 5552 5f41 4343 4553 535f 4b45  '<YOUR_ACCESS_KE
+000004e0: 593e 2729 0a73 6b20 3d20 6f73 2e67 6574  Y>').sk = os.get
+000004f0: 656e 7628 274b 5333 5f49 414d 5f41 4343  env('KS3_IAM_ACC
+00000500: 4553 535f 4b45 595f 5345 4352 4554 272c  ESS_KEY_SECRET',
+00000510: 2027 3c59 4f55 525f 5345 4352 4554 5f4b   '<YOUR_SECRET_K
+00000520: 4559 3e27 290a 6275 636b 6574 5f6e 616d  EY>').bucket_nam
+00000530: 6520 3d20 6f73 2e67 6574 656e 7628 274b  e = os.getenv('K
+00000540: 5333 5f42 5543 4b45 5427 2c20 273c 4b53  S3_BUCKET', '<KS
+00000550: 335f 5445 5354 5f42 5543 4b45 543e 2729  3_TEST_BUCKET>')
+00000560: 0a65 6e64 706f 696e 7420 3d20 276b 7333  .endpoint = 'ks3
+00000570: 2d63 6e2d 6265 696a 696e 672e 6b73 7975  -cn-beijing.ksyu
+00000580: 6e63 732e 636f 6d27 2023 6f73 2e67 6574  ncs.com' #os.get
+00000590: 656e 7628 274b 5333 5f54 4553 545f 454e  env('KS3_TEST_EN
+000005a0: 4450 4f49 4e54 272c 2027 6b73 332d 636e  DPOINT', 'ks3-cn
+000005b0: 2d73 6861 6e67 6861 692d 696e 7465 726e  -shanghai-intern
+000005c0: 616c 2e6b 7379 756e 6373 2e63 6f6d 2729  al.ksyuncs.com')
+000005d0: 0a0a 636f 6e6e 203d 2043 6f6e 6e65 6374  ..conn = Connect
+000005e0: 696f 6e28 616b 2c20 736b 2c20 686f 7374  ion(ak, sk, host
+000005f0: 3d65 6e64 706f 696e 742c 2070 6f72 743d  =endpoint, port=
+00000600: 3830 2c20 7561 5f61 6464 6f6e 3d27 7465  80, ua_addon='te
+00000610: 7374 2d75 612f 3127 2920 2370 6f72 743d  st-ua/1') #port=
+00000620: 3830 3931 2c0a 6b65 795f 6e61 6d65 203d  8091,.key_name =
+00000630: 2027 7465 7374 5f6b 6579 270a 0a0a 6465   'test_key'...de
+00000640: 6620 6765 7441 6c6c 4275 636b 6574 7328  f getAllBuckets(
+00000650: 7072 6f6a 6563 745f 6964 733d 4e6f 6e65  project_ids=None
+00000660: 293a 0a20 2062 7563 6b65 7473 203d 2063  ):.  buckets = c
+00000670: 6f6e 6e2e 6765 745f 616c 6c5f 6275 636b  onn.get_all_buck
+00000680: 6574 7328 7072 6f6a 6563 745f 6964 733d  ets(project_ids=
+00000690: 7072 6f6a 6563 745f 6964 7329 2023 0a20  project_ids) #. 
+000006a0: 2066 6f72 2062 2069 6e20 6275 636b 6574   for b in bucket
+000006b0: 733a 0a20 2020 2070 7269 6e74 2862 2e6e  s:.    print(b.n
+000006c0: 616d 652c 2062 2e72 6567 696f 6e2c 2062  ame, b.region, b
+000006d0: 2e52 6567 696f 6e2c 2062 2e63 7265 6174  .Region, b.creat
+000006e0: 696f 6e5f 6461 7465 290a 0a64 6566 2068  ion_date)..def h
+000006f0: 6561 6442 7563 6b65 7428 6275 636b 6574  eadBucket(bucket
+00000700: 5f6e 616d 6529 3a0a 2020 2320 e5a6 82e6  _name):.  # ....
+00000710: 9e9c e6ad a3e5 b8b8 e8bf 94e5 9b9e efbc  ................
+00000720: 8ce5 8899 4275 636b 6574 e5ad 98e5 9ca8  ....Bucket......
+00000730: efbc 9be5 a682 e69e 9ce6 8a9b e587 ba53  ...............S
+00000740: 3352 6573 706f 6e73 6545 7272 6f72 0a20  3ResponseError. 
+00000750: 2063 6f6e 6e2e 6865 6164 5f62 7563 6b65   conn.head_bucke
+00000760: 7428 6275 636b 6574 5f6e 616d 6529 0a0a  t(bucket_name)..
+00000770: 6465 6620 6765 7442 7563 6b65 744c 6f63  def getBucketLoc
+00000780: 6174 696f 6e28 6275 636b 6574 5f6e 616d  ation(bucket_nam
+00000790: 6529 3a0a 2020 7072 696e 7428 636f 6e6e  e):.  print(conn
+000007a0: 2e67 6574 5f62 7563 6b65 745f 6c6f 6361  .get_bucket_loca
+000007b0: 7469 6f6e 2862 7563 6b65 745f 6e61 6d65  tion(bucket_name
+000007c0: 2929 0a0a 6465 6620 6372 6561 7465 4275  ))..def createBu
+000007d0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+000007e0: 2c20 6c6f 6361 7469 6f6e 3d27 2729 3a0a  , location=''):.
+000007f0: 2020 636f 6e6e 2e63 7265 6174 655f 6275    conn.create_bu
+00000800: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00000810: 2c20 6c6f 6361 7469 6f6e 3d6c 6f63 6174  , location=locat
+00000820: 696f 6e2c 2068 6561 6465 7273 3d7b 0a20  ion, headers={. 
+00000830: 2020 2027 782d 6b73 732d 6275 636b 6574     'x-kss-bucket
+00000840: 2d74 7970 6527 3a20 2741 5243 4849 5645  -type': 'ARCHIVE
+00000850: 270a 2020 7d29 0a0a 6465 6620 6465 6c65  '.  })..def dele
+00000860: 7465 4275 636b 6574 2862 7563 6b65 745f  teBucket(bucket_
+00000870: 6e61 6d65 293a 0a20 2074 7279 3a0a 2020  name):.  try:.  
+00000880: 2020 636f 6e6e 2e64 656c 6574 655f 6275    conn.delete_bu
+00000890: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+000008a0: 290a 2020 6578 6365 7074 2053 3352 6573  ).  except S3Res
+000008b0: 706f 6e73 6545 7272 6f72 2061 7320 6572  ponseError as er
+000008c0: 726f 723a 0a20 2020 2070 7269 6e74 2827  ror:.    print('
+000008d0: 6572 726f 7227 290a 2020 2020 7072 696e  error').    prin
+000008e0: 7428 6572 726f 7229 0a0a 6465 6620 6765  t(error)..def ge
+000008f0: 7442 7563 6b65 7441 636c 2862 7563 6b65  tBucketAcl(bucke
+00000900: 745f 6e61 6d65 293a 0a20 2062 203d 2063  t_name):.  b = c
+00000910: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00000920: 7563 6b65 745f 6e61 6d65 290a 2020 706f  ucket_name).  po
+00000930: 6c69 6379 203d 2062 2e67 6574 5f61 636c  licy = b.get_acl
+00000940: 2829 0a20 2023 2070 7269 6e74 2870 6f6c  ().  # print(pol
+00000950: 6963 7929 0a20 2066 6f72 2067 7261 6e74  icy).  for grant
+00000960: 2069 6e20 706f 6c69 6379 2e61 636c 2e67   in policy.acl.g
+00000970: 7261 6e74 733a 0a20 2020 2070 7269 6e74  rants:.    print
+00000980: 2867 7261 6e74 2e70 6572 6d69 7373 696f  (grant.permissio
+00000990: 6e2c 2067 7261 6e74 2e64 6973 706c 6179  n, grant.display
+000009a0: 5f6e 616d 652c 2067 7261 6e74 2e65 6d61  _name, grant.ema
+000009b0: 696c 5f61 6464 7265 7373 2c20 6772 616e  il_address, gran
+000009c0: 742e 6964 290a 0a64 6566 2073 6574 4275  t.id)..def setBu
+000009d0: 636b 6574 4163 6c28 6275 636b 6574 5f6e  cketAcl(bucket_n
+000009e0: 616d 6529 3a0a 2020 6220 3d20 636f 6e6e  ame):.  b = conn
+000009f0: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00000a00: 6574 5f6e 616d 6529 0a20 2062 2e73 6574  et_name).  b.set
+00000a10: 5f61 636c 2822 7072 6976 6174 6522 290a  _acl("private").
+00000a20: 0a64 6566 206d 616e 6167 6542 7563 6b65  .def manageBucke
+00000a30: 7450 6f6c 6963 7928 6275 636b 6574 5f6e  tPolicy(bucket_n
+00000a40: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
+00000a50: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00000a60: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00000a70: 6275 636b 6574 2e73 6574 5f62 7563 6b65  bucket.set_bucke
+00000a80: 745f 706f 6c69 6379 280a 2020 2020 706f  t_policy(.    po
+00000a90: 6c69 6379 3d27 7b22 5374 6174 656d 656e  licy='{"Statemen
+00000aa0: 7422 3a5b 7b22 5265 736f 7572 6365 223a  t":[{"Resource":
+00000ab0: 5b22 6b72 6e3a 6b73 633a 6b73 333a 3a3a  ["krn:ksc:ks3:::
+00000ac0: 6a69 616e 6772 616e 3132 3322 2c22 6b72  jiangran123","kr
+00000ad0: 6e3a 6b73 633a 6b73 333a 3a3a 6a69 616e  n:ksc:ks3:::jian
+00000ae0: 6772 616e 3132 332f 2a22 5d2c 2250 7269  gran123/*"],"Pri
+00000af0: 6e63 6970 616c 223a 7b22 4b53 4322 3a5b  ncipal":{"KSC":[
+00000b00: 226b 726e 3a6b 7363 3a69 616d 3a3a 3332  "krn:ksc:iam::32
+00000b10: 3433 3234 3233 3a72 6f6f 7422 5d7d 2c22  432423:root"]},"
+00000b20: 4163 7469 6f6e 223a 5b22 6b73 333a 2a22  Action":["ks3:*"
+00000b30: 5d2c 2245 6666 6563 7422 3a22 416c 6c6f  ],"Effect":"Allo
+00000b40: 7722 7d5d 7d27 290a 2020 2320 706f 6c69  w"}]}').  # poli
+00000b50: 6379 203d 2062 7563 6b65 742e 6765 745f  cy = bucket.get_
+00000b60: 6275 636b 6574 5f70 6f6c 6963 7928 290a  bucket_policy().
+00000b70: 2020 2320 6275 636b 6574 2e64 656c 6574    # bucket.delet
+00000b80: 655f 6275 636b 6574 5f70 6f6c 6963 7928  e_bucket_policy(
+00000b90: 290a 0a64 6566 206d 616e 6167 6542 7563  )..def manageBuc
+00000ba0: 6b65 7452 6570 6c69 6361 7469 6f6e 2862  ketReplication(b
+00000bb0: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
+00000bc0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+00000bd0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00000be0: 616d 6529 0a20 2074 7279 3a0a 2020 2020  ame).  try:.    
+00000bf0: 7072 696e 7428 6275 636b 6574 2e67 6574  print(bucket.get
+00000c00: 5f62 7563 6b65 745f 6372 7228 292e 746f  _bucket_crr().to
+00000c10: 5f78 6d6c 2829 290a 2020 6578 6365 7074  _xml()).  except
+00000c20: 3a0a 2020 2020 6275 636b 6574 2e73 6574  :.    bucket.set
+00000c30: 5f62 7563 6b65 745f 6372 7228 2774 6573  _bucket_crr('tes
+00000c40: 742d 6275 636b 6574 2d70 726f 6a65 6374  t-bucket-project
+00000c50: 272c 2064 656c 6574 654d 6172 6b65 7253  ', deleteMarkerS
+00000c60: 7461 7475 733d 2744 6973 6162 6c65 6427  tatus='Disabled'
+00000c70: 2c20 7072 6566 6978 5f6c 6973 743d 5b27  , prefix_list=['
+00000c80: 6865 6c6c 6f27 5d29 0a0a 6465 6620 6765  hello'])..def ge
+00000c90: 7442 7563 6b65 744c 6966 6543 7963 6c65  tBucketLifeCycle
+00000ca0: 2862 7563 6b65 745f 6e61 6d65 293a 0a20  (bucket_name):. 
+00000cb0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
+00000cc0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
+00000cd0: 5f6e 616d 6529 0a20 206c 6966 6563 7963  _name).  lifecyc
+00000ce0: 6c65 203d 2062 7563 6b65 742e 6765 745f  le = bucket.get_
+00000cf0: 6275 636b 6574 5f6c 6966 6563 7963 6c65  bucket_lifecycle
+00000d00: 2829 0a20 2070 7269 6e74 286c 6966 6563  ().  print(lifec
+00000d10: 7963 6c65 2e74 6f5f 786d 6c28 2929 0a0a  ycle.to_xml())..
+00000d20: 6465 6620 7365 7442 7563 6b65 744c 6966  def setBucketLif
+00000d30: 6543 7963 6c65 2862 7563 6b65 745f 6e61  eCycle(bucket_na
+00000d40: 6d65 293a 0a20 2062 7563 6b65 7420 3d20  me):.  bucket = 
+00000d50: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+00000d60: 6275 636b 6574 5f6e 616d 6529 0a20 206c  bucket_name).  l
+00000d70: 6966 6563 7963 6c65 203d 2042 7563 6b65  ifecycle = Bucke
+00000d80: 744c 6966 6563 7963 6c65 2829 0a20 2023  tLifecycle().  #
+00000d90: 2069 6420 e592 8c20 7374 6174 7573 20e5   id ... status .
+00000da0: bf85 e9a1 bb0a 2020 7275 6c65 203d 204c  ......  rule = L
+00000db0: 6966 6563 7963 6c65 5275 6c65 2869 643d  ifecycleRule(id=
+00000dc0: 2772 756c 6531 272c 2073 7461 7475 733d  'rule1', status=
+00000dd0: 2745 6e61 626c 6564 2729 0a20 2064 6174  'Enabled').  dat
+00000de0: 6520 3d20 6461 7465 7469 6d65 2832 3032  e = datetime(202
+00000df0: 312c 2039 2c20 3132 292e 7374 7266 7469  1, 9, 12).strfti
+00000e00: 6d65 2827 2559 2d25 6d2d 2564 5425 483a  me('%Y-%m-%dT%H:
+00000e10: 254d 3a25 5327 2920 2b20 272b 3038 3a30  %M:%S') + '+08:0
+00000e20: 3027 0a20 2072 756c 652e 6578 7069 7261  0'.  rule.expira
+00000e30: 7469 6f6e 203d 204c 6966 6563 7963 6c65  tion = Lifecycle
+00000e40: 4578 7069 7261 7469 6f6e 2864 6174 653d  Expiration(date=
+00000e50: 6461 7465 290a 2020 6c69 6665 6379 636c  date).  lifecycl
+00000e60: 652e 7275 6c65 203d 205b 7275 6c65 5d0a  e.rule = [rule].
+00000e70: 2020 6275 636b 6574 2e73 6574 5f62 7563    bucket.set_buc
+00000e80: 6b65 745f 6c69 6665 6379 636c 6528 6c69  ket_lifecycle(li
+00000e90: 6665 6379 636c 6529 0a0a 0a64 6566 2073  fecycle)...def s
+00000ea0: 6574 4275 636b 6574 4c69 6665 4379 636c  etBucketLifeCycl
+00000eb0: 6532 2862 7563 6b65 745f 6e61 6d65 293a  e2(bucket_name):
+00000ec0: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
+00000ed0: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00000ee0: 6574 5f6e 616d 6529 0a20 2074 6167 203d  et_name).  tag =
+00000ef0: 2054 6167 286b 6579 3d22 7461 6731 222c   Tag(key="tag1",
+00000f00: 2076 616c 7565 3d22 7465 7374 3122 290a   value="test1").
+00000f10: 2020 2320 e7ad 9be9 8089 e589 8de7 bc80    # ............
+00000f20: e4b8 ba20 7072 6566 6978 31e3 8081 e6a0  ... prefix1.....
+00000f30: 87e7 adbe e4b8 ba20 7461 6731 3a74 6573  ....... tag1:tes
+00000f40: 7431 20e7 9a84 206f 626a 6563 7473 efbc  t1 ... objects..
+00000f50: 8ce8 aebe e7bd aee8 bf87 e69c 9fe8 a784  ................
+00000f60: e588 99ef bc8c e59c a8e5 85b6 e69c 80e5  ................
+00000f70: 908e e4bf aee6 94b9 e697 b6e9 97b4 33e5  ..............3.
+00000f80: a4a9 e590 8ee8 bf87 e69c 9fe3 8082 0a20  ............... 
+00000f90: 2072 756c 6531 203d 204c 6966 6563 7963   rule1 = Lifecyc
+00000fa0: 6c65 5275 6c65 2827 7275 6c65 3127 2c20  leRule('rule1', 
+00000fb0: 4c69 6665 6379 636c 6546 696c 7465 7228  LifecycleFilter(
+00000fc0: 2770 7265 6669 7831 272c 2074 6167 733d  'prefix1', tags=
+00000fd0: 5b74 6167 5d29 2c0a 2020 2020 2020 2020  [tag]),.        
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 7374 6174 7573 3d27 456e 6162 6c65 6427  status='Enabled'
+00001000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001010: 2020 2020 2020 2020 2020 6578 7069 7261            expira
+00001020: 7469 6f6e 3d4c 6966 6563 7963 6c65 4578  tion=LifecycleEx
+00001030: 7069 7261 7469 6f6e 2864 6179 733d 3329  piration(days=3)
+00001040: 290a 0a20 2023 20e8 aebe e7bd aee8 bf87  )..  # .........
+00001050: e69c 9fe8 a784 e588 99ef bc8c e7ad 9be9  ................
+00001060: 8089 e6a0 87e7 adbe e4b8 ba20 7461 6731  ........... tag1
+00001070: 3a74 6573 7431 20e7 9a84 206f 626a 6563  :test1 ... objec
+00001080: 7473 efbc 8ce6 9c80 e590 8ee4 bfae e694  ts..............
+00001090: b9e6 97b6 e997 b4e5 9ca8 e68c 87e5 ae9a  ................
+000010a0: e697 a5e6 9c9f e4b9 8be5 898d e79a 84ef  ................
+000010b0: bc8c e8bf 87e6 9c9f 0a20 2072 756c 6532  .........  rule2
+000010c0: 203d 204c 6966 6563 7963 6c65 5275 6c65   = LifecycleRule
+000010d0: 2827 7275 6c65 3227 2c20 4c69 6665 6379  ('rule2', Lifecy
+000010e0: 636c 6546 696c 7465 7228 7461 6773 3d5b  cleFilter(tags=[
+000010f0: 7461 675d 292c 0a20 2020 2020 2020 2020  tag]),.         
+00001100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001110: 7461 7475 733d 2745 6e61 626c 6564 272c  tatus='Enabled',
+00001120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001130: 2020 2020 2020 2020 2065 7870 6972 6174           expirat
+00001140: 696f 6e3d 4c69 6665 6379 636c 6545 7870  ion=LifecycleExp
+00001150: 6972 6174 696f 6e28 0a20 2020 2020 2020  iration(.       
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2064 6174 653d 6461 7465 7469 6d65     date=datetime
+00001180: 2832 3032 312c 2031 322c 2031 3229 2e69  (2021, 12, 12).i
+00001190: 736f 666f 726d 6174 2874 696d 6573 7065  soformat(timespe
+000011a0: 633d 2773 6563 6f6e 6473 2729 202b 2027  c='seconds') + '
+000011b0: 2b30 383a 3030 2729 290a 0a20 2023 20e8  +08:00'))..  # .
+000011c0: aebe e7bd aee5 ad98 e582 a8e7 b1bb e59e  ................
+000011d0: 8be8 bdac e68d a2e8 a784 e588 99ef bc8c  ................
+000011e0: e7ad 9be9 8089 e589 8de7 bc80 e4b8 ba20  ............... 
+000011f0: 7072 6566 6978 3320 e79a 8420 6f62 6a65  prefix3 ... obje
+00001200: 6374 73ef bc8c e59c a8e5 85b6 e69c 80e5  cts.............
+00001210: 908e e4bf aee6 94b9 e697 b6e9 97b4 3230  ..............20
+00001220: e5a4 a9e4 b98b e590 8ee8 bdac e4b8 bae4  ................
+00001230: bd8e e9a2 91e8 aebf e997 aee7 b1bb e59e  ................
+00001240: 8bef bc8c e59c a8e5 85b6 e69c 80e5 908e  ................
+00001250: e4bf aee6 94b9 e697 b6e9 97b4 3330 e5a4  ............30..
+00001260: a9e4 b98b e590 8ee8 bdac e4b8 bae5 bd92  ................
+00001270: e6a1 a3e7 b1bb e59e 8be3 8082 0a20 2072  .............  r
+00001280: 756c 6533 203d 204c 6966 6563 7963 6c65  ule3 = Lifecycle
+00001290: 5275 6c65 2827 7275 6c65 3327 2c20 4c69  Rule('rule3', Li
+000012a0: 6665 6379 636c 6546 696c 7465 7228 2770  fecycleFilter('p
+000012b0: 7265 6669 7833 2729 2c0a 2020 2020 2020  refix3'),.      
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012d0: 2020 7374 6174 7573 3d27 456e 6162 6c65    status='Enable
+000012e0: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+000012f0: 2020 2020 2020 2020 2020 2020 7472 616e              tran
+00001300: 7369 7469 6f6e 733d 5b4c 6966 6563 7963  sitions=[Lifecyc
+00001310: 6c65 5472 616e 7369 7469 6f6e 2864 6179  leTransition(day
+00001320: 733d 3230 2c20 7374 6f72 6167 655f 636c  s=20, storage_cl
+00001330: 6173 733d 2753 5441 4e44 4152 445f 4941  ass='STANDARD_IA
+00001340: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001360: 2020 2020 2020 2020 204c 6966 6563 7963           Lifecyc
+00001370: 6c65 5472 616e 7369 7469 6f6e 2864 6179  leTransition(day
+00001380: 733d 3630 2c20 7374 6f72 6167 655f 636c  s=60, storage_cl
+00001390: 6173 733d 2741 5243 4849 5645 2729 5d29  ass='ARCHIVE')])
+000013a0: 0a0a 2020 2320 e8ae bee7 bdae e5ad 98e5  ..  # ..........
+000013b0: 82a8 e7b1 bbe5 9e8b e8bd ace6 8da2 e8a7  ................
+000013c0: 84e5 8899 efbc 8ce7 ad9b e980 89e5 898d  ................
+000013d0: e7bc 80e4 b8ba 2070 7265 6669 7833 20e7  ...... prefix3 .
+000013e0: 9a84 206f 626a 6563 7473 efbc 8ce6 9c80  .. objects......
+000013f0: e590 8ee4 bfae e694 b9e6 97b6 e997 b4e5  ................
+00001400: 9ca8 e68c 87e5 ae9a e697 a5e6 9c9f e4b9  ................
+00001410: 8be5 898d e79a 84ef bc8c e8bd ace4 b8ba  ................
+00001420: e4bd 8ee9 a291 e8ae bfe9 97ae e7b1 bbe5  ................
+00001430: 9e8b 0a20 2072 756c 6534 203d 204c 6966  ...  rule4 = Lif
+00001440: 6563 7963 6c65 5275 6c65 2827 7275 6c65  ecycleRule('rule
+00001450: 3427 2c20 4c69 6665 6379 636c 6546 696c  4', LifecycleFil
+00001460: 7465 7228 2770 7265 6669 7834 2729 2c0a  ter('prefix4'),.
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 2020 2020 7374 6174 7573 3d27          status='
+00001490: 456e 6162 6c65 6427 2c0a 2020 2020 2020  Enabled',.      
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2020 7472 616e 7369 7469 6f6e 733d 5b0a    transitions=[.
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 2020 2020 2020 2020 4c69 6665 6379            Lifecy
+000014e0: 636c 6554 7261 6e73 6974 696f 6e28 6461  cleTransition(da
+000014f0: 7465 3d64 6174 6574 696d 6528 3230 3231  te=datetime(2021
+00001500: 2c20 3132 2c20 3132 292e 6973 6f66 6f72  , 12, 12).isofor
+00001510: 6d61 7428 7469 6d65 7370 6563 3d27 7365  mat(timespec='se
+00001520: 636f 6e64 7327 2920 2b20 272b 3038 3a30  conds') + '+08:0
+00001530: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001560: 2020 7374 6f72 6167 655f 636c 6173 733d    storage_class=
+00001570: 2753 5441 4e44 4152 445f 4941 2729 5d29  'STANDARD_IA')])
+00001580: 0a20 2023 20e8 aebe e7bd aee5 8886 e789  .  # ...........
+00001590: 87e4 b88a e4bc a0e7 a28e e789 87e6 b885  ................
+000015a0: e790 86e8 a784 e588 99ef bc8c e7ad 9be9  ................
+000015b0: 8089 e589 8de7 bc80 e4b8 ba20 7072 6566  ........... pref
+000015c0: 6978 3520 e79a 8420 7061 7274 efbc 8ce5  ix5 ... part....
+000015d0: 9ca8 e69c 80e5 908e e4bf aee6 94b9 e697  ................
+000015e0: b6e9 97b4 37e5 a4a9 e590 8ee5 88a0 e999  ....7...........
+000015f0: a40a 2020 7275 6c65 3520 3d20 4c69 6665  ..  rule5 = Life
+00001600: 6379 636c 6552 756c 6528 2772 756c 6535  cycleRule('rule5
+00001610: 272c 204c 6966 6563 7963 6c65 4669 6c74  ', LifecycleFilt
+00001620: 6572 2827 7072 6566 6978 3527 292c 0a20  er('prefix5'),. 
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2020 2020 2073 7461 7475 733d 2745         status='E
+00001650: 6e61 626c 6564 272c 0a20 2020 2020 2020  nabled',.       
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2061 626f 7274 5f69 6e63 6f6d 706c 6574   abort_incomplet
+00001680: 655f 6d75 6c74 6970 6172 745f 7570 6c6f  e_multipart_uplo
+00001690: 6164 3d41 626f 7274 496e 636f 6d70 6c65  ad=AbortIncomple
+000016a0: 7465 4d75 6c74 6970 6172 7455 706c 6f61  teMultipartUploa
+000016b0: 6428 6461 7973 5f61 6674 6572 5f69 6e69  d(days_after_ini
+000016c0: 7469 6174 696f 6e3d 3729 290a 0a20 2023  tiation=7))..  #
+000016d0: 2070 7269 6e74 2872 756c 6531 2e74 6f5f   print(rule1.to_
+000016e0: 786d 6c28 2929 0a20 2023 2070 7269 6e74  xml()).  # print
+000016f0: 2872 756c 6532 2e74 6f5f 786d 6c28 2929  (rule2.to_xml())
+00001700: 0a20 2023 2070 7269 6e74 2872 756c 6533  .  # print(rule3
+00001710: 2e74 6f5f 786d 6c28 2929 0a20 2023 2070  .to_xml()).  # p
+00001720: 7269 6e74 2872 756c 6534 2e74 6f5f 786d  rint(rule4.to_xm
+00001730: 6c28 2929 0a20 2023 2070 7269 6e74 2872  l()).  # print(r
+00001740: 756c 6535 2e74 6f5f 786d 6c28 2929 0a20  ule5.to_xml()). 
+00001750: 206c 6966 6563 7963 6c65 203d 2042 7563   lifecycle = Buc
+00001760: 6b65 744c 6966 6563 7963 6c65 285b 7275  ketLifecycle([ru
+00001770: 6c65 312c 2072 756c 6532 2c20 7275 6c65  le1, rule2, rule
+00001780: 332c 2072 756c 6534 2c20 7275 6c65 355d  3, rule4, rule5]
+00001790: 290a 2020 6275 636b 6574 2e73 6574 5f62  ).  bucket.set_b
+000017a0: 7563 6b65 745f 6c69 6665 6379 636c 6528  ucket_lifecycle(
+000017b0: 6c69 6665 6379 636c 6529 0a0a 6465 6620  lifecycle)..def 
+000017c0: 6465 6c65 7465 4275 636b 6574 4c69 6665  deleteBucketLife
+000017d0: 4379 636c 6528 6275 636b 6574 5f6e 616d  Cycle(bucket_nam
+000017e0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+000017f0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00001800: 7563 6b65 745f 6e61 6d65 290a 2020 6275  ucket_name).  bu
+00001810: 636b 6574 2e64 656c 6574 655f 6275 636b  cket.delete_buck
+00001820: 6574 5f6c 6966 6563 7963 6c65 2829 0a0a  et_lifecycle()..
+00001830: 6465 6620 6765 7442 7563 6b65 744c 6f67  def getBucketLog
+00001840: 6769 6e67 2862 7563 6b65 745f 6e61 6d65  ging(bucket_name
+00001850: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
+00001860: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
+00001870: 636b 6574 5f6e 616d 6529 0a20 2070 7269  cket_name).  pri
+00001880: 6e74 2862 7563 6b65 742e 6765 745f 6275  nt(bucket.get_bu
+00001890: 636b 6574 5f6c 6f67 6769 6e67 2829 2e74  cket_logging().t
+000018a0: 6f5f 786d 6c28 2929 0a0a 6465 6620 7365  o_xml())..def se
+000018b0: 7442 7563 6b65 744c 6f67 6769 6e67 2862  tBucketLogging(b
+000018c0: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
+000018d0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+000018e0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+000018f0: 616d 6529 0a20 2062 6c6f 6767 696e 6720  ame).  blogging 
+00001900: 3d20 4275 636b 6574 4c6f 6767 696e 6728  = BucketLogging(
+00001910: 7461 7267 6574 3d62 7563 6b65 745f 6e61  target=bucket_na
+00001920: 6d65 2c20 7461 7267 6574 5f70 7265 6669  me, target_prefi
+00001930: 783d 2774 6573 745f 6c6f 6727 290a 2020  x='test_log').  
+00001940: 7072 696e 7428 6275 636b 6574 2e73 6574  print(bucket.set
+00001950: 5f62 7563 6b65 745f 6c6f 6767 696e 6728  _bucket_logging(
+00001960: 626c 6f67 6769 6e67 2e74 6f5f 786d 6c28  blogging.to_xml(
+00001970: 2929 290a 0a64 6566 2065 6e61 626c 6542  )))..def enableB
+00001980: 7563 6b65 744c 6f67 6769 6e67 2862 7563  ucketLogging(buc
+00001990: 6b65 745f 6e61 6d65 293a 0a20 2062 7563  ket_name):.  buc
+000019a0: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
+000019b0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+000019c0: 6529 0a20 2070 7269 6e74 2862 7563 6b65  e).  print(bucke
+000019d0: 742e 656e 6162 6c65 5f6c 6f67 6769 6e67  t.enable_logging
+000019e0: 2862 7563 6b65 742c 2074 6172 6765 745f  (bucket, target_
+000019f0: 7072 6566 6978 3d27 6865 6865 6865 6865  prefix='hehehehe
+00001a00: 2729 290a 0a64 6566 2064 6973 6162 6c65  '))..def disable
+00001a10: 4275 636b 6574 4c6f 6767 696e 6728 6275  BucketLogging(bu
+00001a20: 636b 6574 5f6e 616d 6529 3a0a 2020 6275  cket_name):.  bu
+00001a30: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
+00001a40: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
+00001a50: 6d65 290a 2020 7072 696e 7428 6275 636b  me).  print(buck
+00001a60: 6574 2e64 6973 6162 6c65 5f6c 6f67 6769  et.disable_loggi
+00001a70: 6e67 2829 290a 0a64 6566 2067 6574 4275  ng())..def getBu
+00001a80: 636b 6574 436f 7273 2862 7563 6b65 745f  cketCors(bucket_
+00001a90: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00001aa0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00001ab0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00001ac0: 2070 7269 6e74 2862 7563 6b65 742e 6765   print(bucket.ge
+00001ad0: 745f 6275 636b 6574 5f63 6f72 7328 292e  t_bucket_cors().
+00001ae0: 746f 5f78 6d6c 2829 290a 0a64 6566 2070  to_xml())..def p
+00001af0: 7574 4275 636b 6574 436f 7273 2862 7563  utBucketCors(buc
+00001b00: 6b65 745f 6e61 6d65 293a 0a20 2062 7563  ket_name):.  buc
+00001b10: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
+00001b20: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+00001b30: 6529 0a20 2063 6f72 7320 3d20 4275 636b  e).  cors = Buck
+00001b40: 6574 436f 7273 285b 434f 5253 5275 6c65  etCors([CORSRule
+00001b50: 286f 7269 6769 6e73 3d5b 2268 7474 703a  (origins=["http:
+00001b60: 2f2f 6465 762e 6b73 7975 6e2e 636f 6d22  //dev.ksyun.com"
+00001b70: 5d2c 206d 6574 686f 6473 3d5b 2247 4554  ], methods=["GET
+00001b80: 222c 2022 4845 4144 225d 2c20 6d61 785f  ", "HEAD"], max_
+00001b90: 6167 653d 2232 3030 222c 2068 6561 6465  age="200", heade
+00001ba0: 7273 3d5b 2263 6f6e 7465 6e74 2d74 7970  rs=["content-typ
+00001bb0: 6522 5d2c 2065 7870 6f73 6564 5f68 6561  e"], exposed_hea
+00001bc0: 6465 7273 3d5b 2263 6f6e 7465 6e74 2d74  ders=["content-t
+00001bd0: 7970 6522 2c20 2278 2d6b 7373 2d61 636c  ype", "x-kss-acl
+00001be0: 225d 295d 290a 2020 7072 696e 7428 2763  "])]).  print('c
+00001bf0: 6f72 733a 2027 2c20 636f 7273 2e74 6f5f  ors: ', cors.to_
+00001c00: 786d 6c28 2929 0a20 2070 7269 6e74 2862  xml()).  print(b
+00001c10: 7563 6b65 742e 7365 745f 6275 636b 6574  ucket.set_bucket
+00001c20: 5f63 6f72 7328 636f 7273 2929 0a0a 6465  _cors(cors))..de
+00001c30: 6620 6465 6c65 7465 4275 636b 6574 436f  f deleteBucketCo
+00001c40: 7273 2862 7563 6b65 745f 6e61 6d65 293a  rs(bucket_name):
 00001c50: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
 00001c60: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
 00001c70: 6574 5f6e 616d 6529 0a20 2070 7269 6e74  et_name).  print
-00001c80: 2862 7563 6b65 742e 6765 745f 6275 636b  (bucket.get_buck
-00001c90: 6574 5f63 7272 2829 2e74 6f5f 786d 6c28  et_crr().to_xml(
-00001ca0: 2929 0a0a 6465 6620 7365 7442 7563 6b65  ))..def setBucke
-00001cb0: 7443 7272 2862 7563 6b65 745f 6e61 6d65  tCrr(bucket_name
-00001cc0: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-00001cd0: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00001ce0: 636b 6574 5f6e 616d 6529 0a20 2023 2064  cket_name).  # d
-00001cf0: 656c 6574 654d 6172 6b65 7253 7461 7475  eleteMarkerStatu
-00001d00: 7320 e79a 84e5 80bc e4b8 ba20 456e 6162  s ......... Enab
-00001d10: 6c65 6420 e592 8c20 4469 7361 626c 6564  led ... Disabled
-00001d20: 0a20 2023 2068 6973 746f 7269 6361 6c4f  .  # historicalO
-00001d30: 626a 6563 7452 6570 6c69 6361 7469 6f6e  bjectReplication
-00001d40: 20e8 a1a8 e7a4 bae6 98af e590 a6e5 bc80   ...............
-00001d50: e590 afe5 ad98 e987 8fe5 a48d e588 b6ef  ................
-00001d60: bc8c e580 bce4 b8ba 2045 6e61 626c 6564  ........ Enabled
-00001d70: 20e5 928c 2044 6973 6162 6c65 640a 2020   ... Disabled.  
-00001d80: 7072 696e 7428 6275 636b 6574 2e73 6574  print(bucket.set
-00001d90: 5f62 7563 6b65 745f 6372 7228 2774 6573  _bucket_crr('tes
-00001da0: 742d 6275 636b 6574 2d72 6570 6c69 272c  t-bucket-repli',
-00001db0: 2064 656c 6574 654d 6172 6b65 7253 7461   deleteMarkerSta
-00001dc0: 7475 733d 4275 636b 6574 4372 6f73 7352  tus=BucketCrossR
-00001dd0: 6570 6c69 6361 7465 2e45 4e41 424c 4544  eplicate.ENABLED
-00001de0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 6869 7374 6f72 6963 616c 4f62 6a65 6374  historicalObject
-00001e10: 5265 706c 6963 6174 696f 6e3d 4275 636b  Replication=Buck
-00001e20: 6574 4372 6f73 7352 6570 6c69 6361 7465  etCrossReplicate
-00001e30: 2e45 4e41 424c 4544 2c20 7072 6566 6978  .ENABLED, prefix
-00001e40: 3d5b 2768 656c 6c6f 275d 2929 0a0a 6465  =['hello']))..de
-00001e50: 6620 6465 6c65 7465 4275 636b 6574 4372  f deleteBucketCr
-00001e60: 7228 6275 636b 6574 5f6e 616d 6529 3a0a  r(bucket_name):.
-00001e70: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00001e80: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00001e90: 745f 6e61 6d65 290a 2020 7072 696e 7428  t_name).  print(
-00001ea0: 6275 636b 6574 2e64 656c 6574 655f 6275  bucket.delete_bu
-00001eb0: 636b 6574 5f63 7272 2829 290a 0a64 6566  cket_crr())..def
-00001ec0: 2067 6574 4275 636b 6574 4c6f 6767 696e   getBucketLoggin
-00001ed0: 6728 6275 636b 6574 5f6e 616d 6529 3a0a  g(bucket_name):.
-00001ee0: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00001ef0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00001f00: 745f 6e61 6d65 290a 2020 7072 696e 7428  t_name).  print(
-00001f10: 6275 636b 6574 2e67 6574 5f62 7563 6b65  bucket.get_bucke
-00001f20: 745f 6c6f 6767 696e 6728 292e 746f 5f78  t_logging().to_x
-00001f30: 6d6c 2829 290a 0a64 6566 2073 6574 4275  ml())..def setBu
-00001f40: 636b 6574 4c6f 6767 696e 6728 6275 636b  cketLogging(buck
-00001f50: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-00001f60: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00001f70: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00001f80: 290a 2020 626c 6f67 6769 6e67 203d 2042  ).  blogging = B
-00001f90: 7563 6b65 744c 6f67 6769 6e67 2874 6172  ucketLogging(tar
-00001fa0: 6765 743d 6275 636b 6574 5f6e 616d 6529  get=bucket_name)
-00001fb0: 0a20 2070 7269 6e74 2862 7563 6b65 742e  .  print(bucket.
-00001fc0: 7365 745f 6275 636b 6574 5f6c 6f67 6769  set_bucket_loggi
-00001fd0: 6e67 2862 6c6f 6767 696e 672e 746f 5f78  ng(blogging.to_x
-00001fe0: 6d6c 2829 2929 0a0a 6465 6620 6765 7442  ml()))..def getB
-00001ff0: 7563 6b65 744d 6972 726f 7228 6275 636b  ucketMirror(buck
-00002000: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-00002010: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00002020: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00002030: 290a 2020 7072 696e 7428 6275 636b 6574  ).  print(bucket
-00002040: 2e67 6574 5f62 7563 6b65 745f 6d69 7272  .get_bucket_mirr
-00002050: 6f72 2829 290a 0a64 6566 2073 6574 4275  or())..def setBu
-00002060: 636b 6574 4d69 7272 6f72 2862 7563 6b65  cketMirror(bucke
-00002070: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
-00002080: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
-00002090: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-000020a0: 0a20 2073 6574 5f68 6561 6465 7273 203d  .  set_headers =
-000020b0: 205b 7b0a 2020 2020 2020 226b 6579 223a   [{.      "key":
-000020c0: 2022 6422 2c0a 2020 2020 2020 2276 616c   "d",.      "val
-000020d0: 7565 223a 2022 6222 0a20 207d 5d0a 2020  ue": "b".  }].  
-000020e0: 7265 6d6f 7665 5f68 6561 6465 7273 203d  remove_headers =
-000020f0: 205b 7b0a 2020 2020 2020 226b 6579 223a   [{.      "key":
-00002100: 2022 6422 0a20 207d 5d0a 2020 7061 7373   "d".  }].  pass
-00002110: 5f68 6561 6465 7273 203d 205b 7b0a 2020  _headers = [{.  
-00002120: 2020 2020 226b 6579 223a 2022 6162 6322      "key": "abc"
-00002130: 0a20 207d 5d0a 2020 6865 6164 6572 5f73  .  }].  header_s
-00002140: 6574 7469 6e67 203d 2048 6561 6465 7253  etting = HeaderS
-00002150: 6574 7469 6e67 2873 6574 5f68 6561 6465  etting(set_heade
-00002160: 7273 3d73 6574 5f68 6561 6465 7273 2c20  rs=set_headers, 
-00002170: 7265 6d6f 7665 5f68 6561 6465 7273 3d72  remove_headers=r
-00002180: 656d 6f76 655f 6865 6164 6572 732c 2070  emove_headers, p
-00002190: 6173 735f 616c 6c3d 4661 6c73 652c 2070  ass_all=False, p
-000021a0: 6173 735f 6865 6164 6572 733d 7061 7373  ass_headers=pass
-000021b0: 5f68 6561 6465 7273 290a 2020 6d69 7272  _headers).  mirr
-000021c0: 6f72 5f72 6571 7565 7374 5f73 6574 7469  or_request_setti
-000021d0: 6e67 203d 204d 6972 726f 7252 6571 7565  ng = MirrorReque
-000021e0: 7374 5365 7474 696e 6728 7061 7373 5f71  stSetting(pass_q
-000021f0: 7565 7279 5f73 7472 696e 673d 4661 6c73  uery_string=Fals
-00002200: 652c 2066 6f6c 6c6f 7733 7878 3d46 616c  e, follow3xx=Fal
-00002210: 7365 2c20 6865 6164 6572 5f73 6574 7469  se, header_setti
-00002220: 6e67 3d68 6561 6465 725f 7365 7474 696e  ng=header_settin
-00002230: 6729 0a20 2061 7379 6e63 5f6d 6972 726f  g).  async_mirro
-00002240: 725f 7275 6c65 203d 2041 7379 6e63 4d69  r_rule = AsyncMi
-00002250: 7272 6f72 5275 6c65 2e72 756c 655f 7769  rrorRule.rule_wi
-00002260: 7468 5f61 636c 286d 6972 726f 725f 7572  th_acl(mirror_ur
-00002270: 6c73 3d5b 2268 7474 703a 2f2f 6162 632e  ls=["http://abc.
-00002280: 6f6d 222c 2022 6874 7470 3a2f 2f77 7777  om", "http://www
-00002290: 2e77 7073 2e63 6e22 5d2c 2073 6176 696e  .wps.cn"], savin
-000022a0: 675f 7365 7474 696e 675f 6163 6c3d 2270  g_setting_acl="p
-000022b0: 7269 7661 7465 2229 0a20 2073 796e 635f  rivate").  sync_
-000022c0: 6d69 7272 6f72 5f72 756c 6573 203d 2053  mirror_rules = S
-000022d0: 796e 634d 6972 726f 7252 756c 6573 2e72  yncMirrorRules.r
-000022e0: 756c 6573 5f77 6974 685f 7072 6566 6978  ules_with_prefix
-000022f0: 5f61 636c 286b 6579 5f70 7265 6669 7865  _acl(key_prefixe
-00002300: 733d 5b22 6162 6322 5d2c 206d 6972 726f  s=["abc"], mirro
-00002310: 725f 7572 6c3d 2268 7474 703a 2f2f 762d  r_url="http://v-
-00002320: 6b73 2d61 2d69 2e6f 7269 6769 6e61 6c76  ks-a-i.originalv
-00002330: 6f64 2e63 6f6d 222c 206d 6972 726f 725f  od.com", mirror_
-00002340: 7265 7175 6573 745f 7365 7474 696e 673d  request_setting=
-00002350: 6d69 7272 6f72 5f72 6571 7565 7374 5f73  mirror_request_s
-00002360: 6574 7469 6e67 2c20 7361 7669 6e67 5f73  etting, saving_s
-00002370: 6574 7469 6e67 5f61 636c 3d22 7072 6976  etting_acl="priv
-00002380: 6174 6522 290a 2020 6d69 7272 6f72 203d  ate").  mirror =
-00002390: 2042 7563 6b65 744d 6972 726f 7228 7573   BucketMirror(us
-000023a0: 655f 6465 6661 756c 745f 726f 626f 7473  e_default_robots
-000023b0: 3d46 616c 7365 2c20 6173 796e 635f 6d69  =False, async_mi
-000023c0: 7272 6f72 5f72 756c 653d 6173 796e 635f  rror_rule=async_
-000023d0: 6d69 7272 6f72 5f72 756c 652c 2073 796e  mirror_rule, syn
-000023e0: 635f 6d69 7272 6f72 5f72 756c 6573 3d5b  c_mirror_rules=[
-000023f0: 7379 6e63 5f6d 6972 726f 725f 7275 6c65  sync_mirror_rule
-00002400: 735d 290a 2020 7072 696e 7428 6275 636b  s]).  print(buck
-00002410: 6574 2e73 6574 5f62 7563 6b65 745f 6d69  et.set_bucket_mi
-00002420: 7272 6f72 286d 6972 726f 7229 290a 0a64  rror(mirror))..d
-00002430: 6566 2064 656c 6574 6542 7563 6b65 744d  ef deleteBucketM
-00002440: 6972 726f 7228 6275 636b 6574 5f6e 616d  irror(bucket_nam
-00002450: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
-00002460: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00002470: 7563 6b65 745f 6e61 6d65 290a 2020 7072  ucket_name).  pr
-00002480: 696e 7428 6275 636b 6574 2e64 656c 6574  int(bucket.delet
-00002490: 655f 6275 636b 6574 5f6d 6972 726f 7228  e_bucket_mirror(
-000024a0: 2929 0a0a 0a64 6566 2073 6574 4275 636b  ))...def setBuck
-000024b0: 6574 5265 7465 6e74 696f 6e28 6275 636b  etRetention(buck
-000024c0: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-000024d0: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-000024e0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-000024f0: 290a 2020 6275 636b 6574 5f72 6574 656e  ).  bucket_reten
-00002500: 7469 6f6e 203d 2042 7563 6b65 7452 6574  tion = BucketRet
-00002510: 656e 7469 6f6e 2829 0a20 2023 20e8 aebe  ention().  # ...
-00002520: e7bd aee5 9b9e e694 b6e7 ab99 e8a7 84e5  ................
-00002530: 8899 efbc 9ae5 90af e794 a82f e7a6 81e7  .........../....
-00002540: 94a8 e380 81e6 9687 e4bb b6e4 bf9d e795  ................
-00002550: 99e5 a4a9 e695 b00a 2020 7275 6c65 203d  ........  rule =
-00002560: 2052 6574 656e 7469 6f6e 5275 6c65 2852   RetentionRule(R
-00002570: 6574 656e 7469 6f6e 5275 6c65 2e45 4e41  etentionRule.ENA
-00002580: 424c 4544 2c20 3229 0a20 2023 2072 756c  BLED, 2).  # rul
-00002590: 6520 3d20 5265 7465 6e74 696f 6e52 756c  e = RetentionRul
-000025a0: 6528 5265 7465 6e74 696f 6e52 756c 652e  e(RetentionRule.
-000025b0: 4449 5341 424c 4544 2c20 3229 0a20 2062  DISABLED, 2).  b
-000025c0: 7563 6b65 745f 7265 7465 6e74 696f 6e2e  ucket_retention.
-000025d0: 7275 6c65 203d 2072 756c 650a 2020 6275  rule = rule.  bu
-000025e0: 636b 6574 2e73 6574 5f62 7563 6b65 745f  cket.set_bucket_
-000025f0: 7265 7465 6e74 696f 6e28 6275 636b 6574  retention(bucket
-00002600: 5f72 6574 656e 7469 6f6e 290a 0a0a 6465  _retention)...de
-00002610: 6620 6765 7442 7563 6b65 7452 6574 656e  f getBucketReten
-00002620: 7469 6f6e 2862 7563 6b65 745f 6e61 6d65  tion(bucket_name
-00002630: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-00002640: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00002650: 636b 6574 5f6e 616d 6529 0a20 2072 6574  cket_name).  ret
-00002660: 203d 2062 7563 6b65 742e 6765 745f 6275   = bucket.get_bu
-00002670: 636b 6574 5f72 6574 656e 7469 6f6e 2829  cket_retention()
-00002680: 0a20 2070 7269 6e74 2872 6574 2e74 6f5f  .  print(ret.to_
-00002690: 786d 6c28 2929 0a0a 0a64 6566 206c 6973  xml())...def lis
-000026a0: 7452 6574 656e 7469 6f6e 2862 7563 6b65  tRetention(bucke
-000026b0: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
-000026c0: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
-000026d0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-000026e0: 0a20 206b 6579 7320 3d20 6275 636b 6574  .  keys = bucket
-000026f0: 2e6c 6973 745f 7265 7465 6e74 696f 6e28  .list_retention(
-00002700: 290a 2020 666f 7220 6b20 696e 206b 6579  ).  for k in key
-00002710: 733a 0a20 2020 2070 7269 6e74 286b 2e6e  s:.    print(k.n
-00002720: 616d 6529 0a20 2020 2070 7269 6e74 286b  ame).    print(k
-00002730: 2e72 6574 656e 7469 6f6e 5f69 6429 0a20  .retention_id). 
-00002740: 2020 2070 7269 6e74 286b 2e73 746f 7261     print(k.stora
-00002750: 6765 5f63 6c61 7373 290a 0a0a 6465 6620  ge_class)...def 
-00002760: 636c 6561 724f 626a 6563 7428 6275 636b  clearObject(buck
-00002770: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-00002780: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00002790: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-000027a0: 290a 2020 6b20 3d20 6275 636b 6574 2e6e  ).  k = bucket.n
-000027b0: 6577 5f6b 6579 2827 636c 6561 725f 6b65  ew_key('clear_ke
-000027c0: 795f 6e61 6d65 2729 0a20 206b 2e63 6c65  y_name').  k.cle
-000027d0: 6172 5f6f 626a 6563 7428 273c 7265 7465  ar_object('<rete
-000027e0: 6e74 696f 6e5f 6964 3e27 290a 0a0a 6465  ntion_id>')...de
-000027f0: 6620 7265 636f 7665 724f 626a 6563 7428  f recoverObject(
-00002800: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
-00002810: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00002820: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00002830: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
-00002840: 6574 2e6e 6577 5f6b 6579 2827 7265 636f  et.new_key('reco
-00002850: 7665 725f 6b65 795f 6e61 6d65 2729 0a20  ver_key_name'). 
-00002860: 2023 20e5 a682 e69e 9c72 6574 656e 7469   # ......retenti
-00002870: 6f6e 5f69 64e4 b8ba e7a9 baef bc8c e9bb  on_id...........
-00002880: 98e8 aea4 e681 a2e5 a48d e59b 9ee6 94b6  ................
-00002890: e7ab 99e4 b8ad e68c 87e5 ae9a 6b65 79e7  ............key.
-000028a0: 9a84 e69c 80e6 96b0 e789 88e6 9cac 0a20  ............... 
-000028b0: 206b 2e72 6563 6f76 6572 5f6f 626a 6563   k.recover_objec
-000028c0: 7428 6f76 6572 7772 6974 653d 5472 7565  t(overwrite=True
-000028d0: 2c20 7265 7465 6e74 696f 6e5f 6964 3d27  , retention_id='
-000028e0: 3c72 6574 656e 7469 6f6e 5f69 643e 2729  <retention_id>')
-000028f0: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
-00002900: 2323 2323 2323 2323 2020 6b73 332e 6269  ########  ks3.bi
-00002910: 6c6c 696e 6720 2023 2323 2323 2323 2323  lling  #########
-00002920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002930: 2323 0a66 726f 6d20 6b73 332e 6269 6c6c  ##.from ks3.bill
-00002940: 696e 6720 696d 706f 7274 2067 6574 5f62  ing import get_b
-00002950: 7563 6b65 7473 5f64 6174 610a 0a64 6566  uckets_data..def
-00002960: 2067 6574 4275 636b 6574 7344 6174 6128   getBucketsData(
-00002970: 6275 636b 6574 5f6e 616d 6573 3d4e 6f6e  bucket_names=Non
-00002980: 6529 3a0a 2020 6461 7461 203d 2067 6574  e):.  data = get
-00002990: 5f62 7563 6b65 7473 5f64 6174 6128 616b  _buckets_data(ak
-000029a0: 2c20 736b 2c20 7374 6172 745f 7469 6d65  , sk, start_time
-000029b0: 3d22 3230 3231 3131 3139 3233 3030 222c  ="202111192300",
-000029c0: 2065 6e64 5f74 696d 653d 2232 3032 3131   end_time="20211
-000029d0: 3131 3932 3335 3922 2c20 6275 636b 6574  1192359", bucket
-000029e0: 5f6e 616d 6573 3d62 7563 6b65 745f 6e61  _names=bucket_na
-000029f0: 6d65 732c 2070 726f 6475 6374 733d 2244  mes, products="D
-00002a00: 6174 6153 697a 652c 5265 7175 6573 7473  ataSize,Requests
-00002a10: 4765 7422 290a 2020 7072 696e 7428 6461  Get").  print(da
-00002a20: 7461 290a 0a23 2323 2323 2323 2323 2323  ta)..###########
-00002a30: 2323 2323 2323 2323 2323 2020 6b73 332e  ##########  ks3.
-00002a40: 6f62 6a65 6374 2020 2323 2323 2323 2323  object  ########
-00002a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002a60: 2323 230a 6465 6620 6765 744f 626a 6563  ###.def getObjec
-00002a70: 744d 6574 6128 6275 636b 6574 5f6e 616d  tMeta(bucket_nam
-00002a80: 652c 206f 626a 6563 745f 6b65 795f 6e61  e, object_key_na
-00002a90: 6d65 2c20 6865 6164 6572 733d 4e6f 6e65  me, headers=None
-00002aa0: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-00002ab0: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00002ac0: 636b 6574 5f6e 616d 6529 0a20 2072 6573  cket_name).  res
-00002ad0: 7020 3d20 6275 636b 6574 2e67 6574 5f6b  p = bucket.get_k
-00002ae0: 6579 5f6d 6574 6128 6f62 6a65 6374 5f6b  ey_meta(object_k
-00002af0: 6579 5f6e 616d 652c 2068 6561 6465 7273  ey_name, headers
-00002b00: 3d68 6561 6465 7273 290a 2020 6966 2072  =headers).  if r
-00002b10: 6573 703a 0a20 2020 2070 7269 6e74 2822  esp:.    print("
-00002b20: e88e b7e5 8f96 e696 87e4 bbb6 6865 6164  ............head
-00002b30: 6572 e688 90e5 8a9f 3a20 222c 2072 6573  er......: ", res
-00002b40: 702e 6865 6164 6572 7329 0a0a 6465 6620  p.headers)..def 
-00002b50: 7570 6c6f 6164 4f62 6a65 6374 4672 6f6d  uploadObjectFrom
-00002b60: 4669 6c65 2866 696c 656e 616d 6529 3a0a  File(filename):.
-00002b70: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00002b80: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00002b90: 745f 6e61 6d65 290a 2020 6b20 3d20 6275  t_name).  k = bu
-00002ba0: 636b 6574 2e6e 6577 5f6b 6579 2866 696c  cket.new_key(fil
-00002bb0: 656e 616d 6529 0a20 2072 6574 203d 206b  ename).  ret = k
-00002bc0: 2e73 6574 5f63 6f6e 7465 6e74 735f 6672  .set_contents_fr
-00002bd0: 6f6d 5f66 696c 656e 616d 6528 6f73 2e70  om_filename(os.p
-00002be0: 6174 682e 6578 7061 6e64 7573 6572 2822  ath.expanduser("
-00002bf0: 7e22 2920 2b20 272f 446f 776e 6c6f 6164  ~") + '/Download
-00002c00: 732f 2720 2b20 6669 6c65 6e61 6d65 290a  s/' + filename).
-00002c10: 2020 6966 2072 6574 2061 6e64 2072 6574    if ret and ret
-00002c20: 2e73 7461 7475 7320 3d3d 2032 3030 3a0a  .status == 200:.
-00002c30: 2020 2020 7072 696e 7428 22e4 b88a e4bc      print(".....
-00002c40: a0e6 8890 e58a 9f22 290a 0a64 6566 2075  .......")..def u
-00002c50: 706c 6f61 645f 6173 796e 6328 6669 6c65  pload_async(file
-00002c60: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
-00002c70: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-00002c80: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-00002c90: 206b 203d 2062 7563 6b65 742e 6e65 775f   k = bucket.new_
-00002ca0: 6b65 7928 6669 6c65 6e61 6d65 290a 2020  key(filename).  
-00002cb0: 7265 7420 3d20 6173 796e 6369 6f2e 7275  ret = asyncio.ru
-00002cc0: 6e28 6b2e 7570 6c6f 6164 5f66 696c 655f  n(k.upload_file_
-00002cd0: 6173 796e 6328 6f73 2e70 6174 682e 6578  async(os.path.ex
-00002ce0: 7061 6e64 7573 6572 2822 7e22 2920 2b20  panduser("~") + 
-00002cf0: 272f 446f 776e 6c6f 6164 732f 2720 2b20  '/Downloads/' + 
-00002d00: 6669 6c65 6e61 6d65 2929 0a20 2069 6620  filename)).  if 
-00002d10: 7265 7420 616e 6420 7265 742e 7374 6174  ret and ret.stat
-00002d20: 7573 203d 3d20 3230 303a 0a20 2020 2070  us == 200:.    p
-00002d30: 7269 6e74 2822 e4b8 8ae4 bca0 e688 90e5  rint("..........
-00002d40: 8a9f 2229 0a0a 6465 6620 7570 6c6f 6164  ..")..def upload
-00002d50: 4f62 6a65 6374 4672 6f6d 5374 7269 6e67  ObjectFromString
-00002d60: 2829 3a0a 2020 6275 636b 6574 203d 2063  ():.  bucket = c
-00002d70: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00002d80: 7563 6b65 745f 6e61 6d65 290a 2020 6b20  ucket_name).  k 
-00002d90: 3d20 6275 636b 6574 2e6e 6577 5f6b 6579  = bucket.new_key
-00002da0: 2827 e5a4 a7e5 aeb6 e5a5 bd27 290a 2020  ('.........').  
-00002db0: 2320 2320 6b65 7920 e592 8c20 7661 6c75  # # key ... valu
-00002dc0: 6520 e99c 80e8 a681 2075 726c 20e7 bc96  e ...... url ...
-00002dd0: e7a0 810a 2020 2320 7461 6767 696e 6753  ....  # taggingS
-00002de0: 7472 203d 2027 6e61 6d65 3d6a 6827 0a20  tr = 'name=jh'. 
-00002df0: 2023 2068 6561 6465 7273 203d 207b 2778   # headers = {'x
-00002e00: 2d6b 7373 2d74 6167 6769 6e67 273a 2074  -kss-tagging': t
-00002e10: 6167 6769 6e67 5374 727d 0a20 2072 6574  aggingStr}.  ret
-00002e20: 203d 206b 2e73 6574 5f63 6f6e 7465 6e74   = k.set_content
-00002e30: 735f 6672 6f6d 5f73 7472 696e 6728 2720  s_from_string(' 
-00002e40: 776f 726c 6427 290a 2020 2320 2320 e8af  world').  # # ..
-00002e50: b7e6 b182 4944 e380 82e8 afb7 e6b1 8249  ....ID.........I
-00002e60: 44e6 98af e69c ace6 aca1 e8af b7e6 b182  D...............
-00002e70: e79a 84e5 94af e4b8 80e6 a087 e8af 86ef  ................
-00002e80: bc8c e5bc bae7 8388 e5bb bae8 aeae e59c  ................
-00002e90: a8e7 a88b e5ba 8fe6 97a5 e5bf 97e4 b8ad  ................
-00002ea0: e6b7 bbe5 8aa0 e6ad a4e5 8f82 e695 b0e3  ................
-00002eb0: 8082 0a20 2023 2070 7269 6e74 2872 6574  ...  # print(ret
-00002ec0: 2e68 6561 6465 7273 5b27 782d 6b73 732d  .headers['x-kss-
-00002ed0: 7265 7175 6573 742d 6964 275d 290a 2020  request-id']).  
-00002ee0: 2320 2320 4554 6167 e698 af70 7574 5f6f  # # ETag...put_o
-00002ef0: 626a 6563 74e6 96b9 e6b3 95e8 bf94 e59b  bject...........
-00002f00: 9ee5 80bc e789 b9e6 9c89 e79a 84e5 b19e  ................
-00002f10: e680 a7ef bc8c e794 a8e4 ba8e e6a0 87e8  ................
-00002f20: af86 e4b8 80e4 b8aa 4f62 6a65 6374 e79a  ........Object..
-00002f30: 84e5 8685 e5ae b9e3 8082 0a20 2023 2070  ...........  # p
-00002f40: 7269 6e74 2872 6574 2e68 6561 6465 7273  rint(ret.headers
-00002f50: 290a 2020 2320 4854 5450 e8bf 94e5 9b9e  ).  # HTTP......
-00002f60: e7a0 81e3 8082 0a20 2069 6620 7265 7420  .......  if ret 
-00002f70: 616e 6420 7265 742e 7374 6174 7573 203d  and ret.status =
-00002f80: 3d20 3230 303a 0a20 2020 2070 7269 6e74  = 200:.    print
-00002f90: 2822 e4b8 8ae4 bca0 e688 90e5 8a9f 2229  ("............")
-00002fa0: 0a0a 6465 6620 6865 6164 4f62 6a65 6374  ..def headObject
-00002fb0: 2829 3a0a 2020 6275 636b 6574 203d 2063  ():.  bucket = c
-00002fc0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00002fd0: 7563 6b65 745f 6e61 6d65 290a 2020 6b20  ucket_name).  k 
-00002fe0: 3d20 6275 636b 6574 2e67 6574 5f6b 6579  = bucket.get_key
-00002ff0: 2827 7465 7374 5f65 6e63 7279 7074 696f  ('test_encryptio
-00003000: 6e27 290a 2020 6966 206b 3a0a 2020 2020  n').  if k:.    
-00003010: 7072 696e 7428 6b2e 6e61 6d65 2c20 6b2e  print(k.name, k.
-00003020: 7369 7a65 2c20 6b2e 6c61 7374 5f6d 6f64  size, k.last_mod
-00003030: 6966 6965 642c 206b 2e6f 626a 6563 745f  ified, k.object_
-00003040: 7479 7065 2c20 6b2e 7461 6767 696e 675f  type, k.tagging_
-00003050: 636f 756e 7429 0a0a 6465 6620 646f 776e  count)..def down
-00003060: 6c6f 6164 4f62 6a65 6374 416e 6450 7269  loadObjectAndPri
-00003070: 6e74 286b 6579 6e61 6d65 2c20 6279 7465  nt(keyname, byte
-00003080: 5f72 616e 6765 3d28 302c 2031 292c 2068  _range=(0, 1), h
-00003090: 6561 6465 7273 3d4e 6f6e 6529 3a0a 2020  eaders=None):.  
-000030a0: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-000030b0: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-000030c0: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
-000030d0: 6574 2e67 6574 5f6b 6579 286b 6579 6e61  et.get_key(keyna
-000030e0: 6d65 290a 2020 7320 3d20 6b2e 6765 745f  me).  s = k.get_
-000030f0: 636f 6e74 656e 7473 5f61 735f 7374 7269  contents_as_stri
-00003100: 6e67 2862 7974 655f 7261 6e67 653d 6279  ng(byte_range=by
-00003110: 7465 5f72 616e 6765 2c20 6865 6164 6572  te_range, header
-00003120: 733d 6865 6164 6572 7329 2e64 6563 6f64  s=headers).decod
-00003130: 6528 290a 2020 7072 696e 7428 7329 0a0a  e().  print(s)..
-00003140: 6465 6620 646f 776e 6c6f 6164 5f61 7379  def download_asy
-00003150: 6e63 286b 6579 6e61 6d65 2c20 6865 6164  nc(keyname, head
-00003160: 6572 733d 4e6f 6e65 293a 0a20 2062 7563  ers=None):.  buc
-00003170: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00003180: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-00003190: 6529 0a20 206b 203d 2062 7563 6b65 742e  e).  k = bucket.
-000031a0: 6765 745f 6b65 7928 6b65 796e 616d 6529  get_key(keyname)
-000031b0: 0a20 2074 7279 3a0a 2020 2020 6173 796e  .  try:.    asyn
-000031c0: 6369 6f2e 7275 6e28 6b2e 646f 776e 6c6f  cio.run(k.downlo
-000031d0: 6164 5f66 696c 655f 6173 796e 6328 6f73  ad_file_async(os
-000031e0: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
-000031f0: 2822 7e22 2920 2b20 272f 446f 776e 6c6f  ("~") + '/Downlo
-00003200: 6164 732f 2720 2b20 6b65 796e 616d 6529  ads/' + keyname)
-00003210: 290a 2020 2020 7072 696e 7428 27e4 b88b  ).    print('...
-00003220: e8bd bde6 8890 e58a 9f27 290a 2020 6578  .........').  ex
-00003230: 6365 7074 3a0a 2020 2020 7072 696e 7428  cept:.    print(
-00003240: 27e4 b88b e8bd bde5 a4b1 e8b4 a527 290a  '............').
-00003250: 0a64 6566 2064 6f77 6e6c 6f61 644f 626a  .def downloadObj
-00003260: 6563 7441 7353 7472 6561 6d41 6e64 5072  ectAsStreamAndPr
-00003270: 696e 7428 293a 0a20 2062 7563 6b65 7420  int():.  bucket 
-00003280: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-00003290: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-000032a0: 206b 203d 2062 7563 6b65 742e 6765 745f   k = bucket.get_
-000032b0: 6b65 7928 2773 6861 6b65 2e74 7874 2729  key('shake.txt')
-000032c0: 0a20 2062 7974 6573 203d 206b 2e72 6561  .  bytes = k.rea
-000032d0: 6428 3330 3029 0a20 2070 7269 6e74 2827  d(300).  print('
-000032e0: 7374 6172 743a 2027 2c20 6461 7465 7469  start: ', dateti
-000032f0: 6d65 2e6e 6f77 2829 2e73 7472 6674 696d  me.now().strftim
-00003300: 6528 2225 592d 256d 2d25 6420 2548 3a25  e("%Y-%m-%d %H:%
-00003310: 4d3a 2553 2e25 6622 2929 0a20 2077 6869  M:%S.%f")).  whi
-00003320: 6c65 2062 7974 6573 3a0a 2020 2020 7320  le bytes:.    s 
-00003330: 3d20 6279 7465 732e 6465 636f 6465 2829  = bytes.decode()
-00003340: 0a20 2020 2070 7269 6e74 2827 6279 7465  .    print('byte
-00003350: 7320 6465 636f 6465 643a 272c 2073 290a  s decoded:', s).
-00003360: 2020 2020 7469 6d65 2e73 6c65 6570 2835      time.sleep(5
-00003370: 290a 2020 2020 6279 7465 7320 3d20 6b2e  ).    bytes = k.
-00003380: 7265 6164 2833 3030 290a 2020 7072 696e  read(300).  prin
-00003390: 7428 2765 6e64 3a20 272c 2064 6174 6574  t('end: ', datet
-000033a0: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
-000033b0: 6d65 2822 2559 2d25 6d2d 2564 2025 483a  me("%Y-%m-%d %H:
-000033c0: 254d 3a25 532e 2566 2229 290a 0a64 6566  %M:%S.%f"))..def
-000033d0: 2064 6f77 6e6c 6f61 644f 626a 6563 7441   downloadObjectA
-000033e0: 6e64 5361 7665 286b 6579 5f6e 616d 652c  ndSave(key_name,
-000033f0: 2062 7974 655f 7261 6e67 653d 2830 2c20   byte_range=(0, 
-00003400: 3129 2c20 6865 6164 6572 733d 4e6f 6e65  1), headers=None
-00003410: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-00003420: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00003430: 636b 6574 5f6e 616d 6529 0a20 206b 203d  cket_name).  k =
-00003440: 2062 7563 6b65 742e 6765 745f 6b65 7928   bucket.get_key(
-00003450: 6b65 795f 6e61 6d65 290a 2020 6b2e 6765  key_name).  k.ge
-00003460: 745f 636f 6e74 656e 7473 5f74 6f5f 6669  t_contents_to_fi
-00003470: 6c65 6e61 6d65 2827 2f55 7365 7273 2f6a  lename('/Users/j
-00003480: 6162 6261 722f 446f 776e 6c6f 6164 732f  abbar/Downloads/
-00003490: 4453 4330 3333 3830 2e65 6e63 7279 7074  DSC03380.encrypt
-000034a0: 2ee9 9d9e e588 86e5 9d97 2e6a 7067 2e64  ...........jpg.d
-000034b0: 6f77 6e6c 6f61 6427 2c20 6865 6164 6572  ownload', header
-000034c0: 733d 6865 6164 6572 7329 0a0a 6465 6620  s=headers)..def 
-000034d0: 6465 6c65 7465 4f62 6a65 6374 286b 6579  deleteObject(key
-000034e0: 5f6e 616d 6529 3a0a 2020 6275 636b 6574  _name):.  bucket
-000034f0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-00003500: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00003510: 2020 7472 793a 0a20 2020 2062 7563 6b65    try:.    bucke
-00003520: 742e 6465 6c65 7465 5f6b 6579 286b 6579  t.delete_key(key
-00003530: 5f6e 616d 6529 0a20 2020 2070 7269 6e74  _name).    print
-00003540: 2822 e588 a0e9 99a4 e688 90e5 8a9f 2229  ("............")
-00003550: 0a20 2065 7863 6570 7420 4578 6365 7074  .  except Except
-00003560: 696f 6e20 6173 2065 3a0a 2020 2020 7072  ion as e:.    pr
-00003570: 696e 7428 22e5 88a0 e999 a4e5 a4b1 e8b4  int("...........
-00003580: a522 290a 2020 2020 7072 696e 7428 6529  .").    print(e)
-00003590: 0a20 2020 2070 6173 730a 0a64 6566 2067  .    pass..def g
-000035a0: 6574 4f62 6a65 6374 4163 6c28 293a 0a20  etObjectAcl():. 
-000035b0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-000035c0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-000035d0: 5f6e 616d 6529 0a20 2070 6f6c 6963 7920  _name).  policy 
-000035e0: 3d20 6275 636b 6574 2e67 6574 5f61 636c  = bucket.get_acl
-000035f0: 2827 6172 7469 636c 652e 7478 7427 290a  ('article.txt').
-00003600: 2020 7072 696e 7428 706f 6c69 6379 2e74    print(policy.t
-00003610: 6f5f 786d 6c28 2929 0a0a 6465 6620 7365  o_xml())..def se
-00003620: 744f 626a 6563 7441 636c 2829 3a0a 2020  tObjectAcl():.  
-00003630: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00003640: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00003650: 6e61 6d65 290a 2020 2320 6f62 6a65 6374  name).  # object
-00003660: 2070 6f6c 6963 7920 3a20 7072 6976 6174   policy : privat
-00003670: 6520 7c20 7075 626c 6963 2d72 6561 6420  e | public-read 
-00003680: 7c20 7075 626c 6963 2d72 6561 642d 7772  | public-read-wr
-00003690: 6974 650a 2020 6275 636b 6574 2e73 6574  ite.  bucket.set
-000036a0: 5f61 636c 2822 7075 626c 6963 2d72 6561  _acl("public-rea
-000036b0: 6422 2c20 273c 594f 5552 5f4b 4559 5f4e  d", '<YOUR_KEY_N
-000036c0: 414d 453e 2729 0a0a 6465 6620 7365 744f  AME>')..def setO
-000036d0: 626a 6563 744d 6574 6128 293a 0a20 2062  bjectMeta():.  b
-000036e0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-000036f0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00003700: 2020 622e 636f 7079 5f6b 6579 2827 3c79    b.copy_key('<y
-00003710: 6f75 724b 6579 4e61 6d65 3e27 2c20 273c  ourKeyName>', '<
-00003720: 796f 7572 4275 636b 6574 4e61 6d65 3e27  yourBucketName>'
-00003730: 2c20 273c 796f 7572 4b65 794e 616d 653e  , '<yourKeyName>
-00003740: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00003750: 6865 6164 6572 733d 7b27 636f 6e74 656e  headers={'conten
-00003760: 742d 7479 7065 273a 2027 7465 7874 2f70  t-type': 'text/p
-00003770: 6c61 696e 272c 2027 782d 6b73 732d 6d65  lain', 'x-kss-me
-00003780: 7461 6461 7461 2d64 6972 6563 7469 7665  tadata-directive
-00003790: 273a 2027 5245 504c 4143 4527 7d29 0a0a  ': 'REPLACE'})..
-000037a0: 6465 6620 7365 744f 626a 6563 7453 746f  def setObjectSto
-000037b0: 7261 6765 436c 6173 7328 293a 0a20 2062  rageClass():.  b
-000037c0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-000037d0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-000037e0: 2020 622e 636f 7079 5f6b 6579 2827 3c79    b.copy_key('<y
-000037f0: 6f75 724b 6579 4e61 6d65 3e27 2c20 273c  ourKeyName>', '<
-00003800: 796f 7572 4275 636b 6574 4e61 6d65 3e27  yourBucketName>'
-00003810: 2c20 273c 796f 7572 4b65 794e 616d 653e  , '<yourKeyName>
-00003820: 272c 2068 6561 6465 7273 3d7b 2778 2d6b  ', headers={'x-k
-00003830: 7373 2d73 746f 7261 6765 2d63 6c61 7373  ss-storage-class
-00003840: 273a 2027 5354 414e 4441 5244 5f49 4127  ': 'STANDARD_IA'
-00003850: 7d29 0a0a 6465 6620 636f 7079 2864 7374  })..def copy(dst
-00003860: 4b65 792c 2073 7263 4b65 792c 2064 7374  Key, srcKey, dst
-00003870: 5f62 7563 6b65 745f 6e61 6d65 3d4e 6f6e  _bucket_name=Non
-00003880: 652c 2068 6561 6465 7273 3d4e 6f6e 6529  e, headers=None)
-00003890: 3a0a 2020 2320 6275 636b 6574 5f6e 616d  :.  # bucket_nam
-000038a0: 6520 3d20 2768 6170 7079 686f 7572 270a  e = 'happyhour'.
-000038b0: 2020 6220 3d20 636f 6e6e 2e67 6574 5f62    b = conn.get_b
-000038c0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-000038d0: 6529 0a20 2072 6574 7572 6e20 622e 636f  e).  return b.co
-000038e0: 7079 5f6b 6579 2864 7374 4b65 792c 2064  py_key(dstKey, d
-000038f0: 7374 5f62 7563 6b65 745f 6e61 6d65 2c20  st_bucket_name, 
-00003900: 7372 634b 6579 2c20 6865 6164 6572 733d  srcKey, headers=
-00003910: 6865 6164 6572 7329 0a0a 6465 6620 636f  headers)..def co
-00003920: 7079 5f65 6e63 7279 7074 696f 6e28 6473  py_encryption(ds
-00003930: 744b 6579 2c20 7372 634b 6579 2c20 656e  tKey, srcKey, en
-00003940: 6372 7970 745f 6b65 793d 4e6f 6e65 293a  crypt_key=None):
-00003950: 0a20 2062 203d 2063 6f6e 6e2e 6765 745f  .  b = conn.get_
-00003960: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
-00003970: 6d65 290a 2020 622e 636f 7079 5f6b 6579  me).  b.copy_key
-00003980: 2864 7374 4b65 792c 2062 7563 6b65 745f  (dstKey, bucket_
-00003990: 6e61 6d65 2c20 7372 634b 6579 2c20 656e  name, srcKey, en
-000039a0: 6372 7970 745f 6b65 793d 656e 6372 7970  crypt_key=encryp
-000039b0: 745f 6b65 7929 0a0a 6465 6620 6c69 7374  t_key)..def list
-000039c0: 5f6f 626a 6563 7473 2829 3a0a 2020 6275  _objects():.  bu
-000039d0: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-000039e0: 6275 636b 6574 2827 7465 7374 2d62 7563  bucket('test-buc
-000039f0: 6b65 7427 290a 2020 6b65 7973 203d 2062  ket').  keys = b
-00003a00: 7563 6b65 742e 6c69 7374 2870 7265 6669  ucket.list(prefi
-00003a10: 783d 2731 3627 290a 2020 7265 7331 203d  x='16').  res1 =
-00003a20: 205b 6b2e 6e61 6d65 2066 6f72 206b 2069   [k.name for k i
-00003a30: 6e20 6b65 7973 5d0a 2020 7072 696e 7428  n keys].  print(
-00003a40: 2772 6573 3120 3a20 272c 2072 6573 3129  'res1 : ', res1)
-00003a50: 0a0a 2020 6b65 7973 3220 3d20 6275 636b  ..  keys2 = buck
-00003a60: 6574 2e6c 6973 744f 626a 6563 7473 2870  et.listObjects(p
-00003a70: 7265 6669 783d 2731 3627 290a 2020 2320  refix='16').  # 
-00003a80: 7265 7332 203d 205b 6b2e 6e61 6d65 2066  res2 = [k.name f
-00003a90: 6f72 206b 2069 6e20 6b65 7973 325d 0a20  or k in keys2]. 
-00003aa0: 2070 7269 6e74 2827 6b65 7973 3220 3a20   print('keys2 : 
-00003ab0: 272c 206b 6579 7332 290a 2020 2320 666f  ', keys2).  # fo
-00003ac0: 7220 6b20 696e 206b 6579 733a 0a20 2023  r k in keys:.  #
-00003ad0: 2020 2070 7269 6e74 2827 6f62 6a65 6374     print('object
-00003ae0: 3a27 2c20 6b2e 6e61 6d65 290a 0a64 6566  :', k.name)..def
-00003af0: 206c 6973 745f 6f62 6a65 6374 735f 7632   list_objects_v2
-00003b00: 2864 656c 696d 6974 6572 3d27 2327 2c20  (delimiter='#', 
-00003b10: 7072 6566 6978 3d4e 6f6e 652c 206d 6178  prefix=None, max
-00003b20: 5f6b 6579 733d 4e6f 6e65 2c20 6d61 726b  _keys=None, mark
-00003b30: 6572 3d4e 6f6e 652c 2065 6e63 6f64 696e  er=None, encodin
-00003b40: 675f 7479 7065 3d27 272c 2066 6574 6368  g_type='', fetch
-00003b50: 5f6f 776e 6572 3d54 7275 6529 3a0a 2020  _owner=True):.  
-00003b60: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00003b70: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00003b80: 6e61 6d65 290a 2020 6b65 7973 203d 2062  name).  keys = b
-00003b90: 7563 6b65 742e 6c69 7374 5f76 3228 6465  ucket.list_v2(de
-00003ba0: 6c69 6d69 7465 723d 6465 6c69 6d69 7465  limiter=delimite
-00003bb0: 722c 2070 7265 6669 783d 7072 6566 6978  r, prefix=prefix
-00003bc0: 2c20 6d61 785f 6b65 7973 3d6d 6178 5f6b  , max_keys=max_k
-00003bd0: 6579 732c 206d 6172 6b65 723d 6d61 726b  eys, marker=mark
-00003be0: 6572 2c20 656e 636f 6469 6e67 5f74 7970  er, encoding_typ
-00003bf0: 653d 656e 636f 6469 6e67 5f74 7970 652c  e=encoding_type,
-00003c00: 2066 6574 6368 5f6f 776e 6572 3d66 6574   fetch_owner=fet
-00003c10: 6368 5f6f 776e 6572 290a 2020 666f 7220  ch_owner).  for 
-00003c20: 6b20 696e 206b 6579 733a 0a20 2020 2070  k in keys:.    p
-00003c30: 7269 6e74 2827 6f62 6a65 6374 3a27 2c20  rint('object:', 
-00003c40: 6b2e 6e61 6d65 290a 0a64 6566 206c 6973  k.name)..def lis
-00003c50: 744f 626a 6563 7473 4d6f 7265 2862 7563  tObjectsMore(buc
-00003c60: 6b65 745f 6e61 6d65 2c20 6465 6c69 6d69  ket_name, delimi
-00003c70: 7465 723d 4e6f 6e65 2c20 7072 6566 6978  ter=None, prefix
-00003c80: 3d4e 6f6e 652c 206d 6178 5f6b 6579 733d  =None, max_keys=
-00003c90: 4e6f 6e65 2c20 6d61 726b 6572 3d4e 6f6e  None, marker=Non
-00003ca0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
-00003cb0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-00003cc0: 7563 6b65 745f 6e61 6d65 290a 2020 6b65  ucket_name).  ke
-00003cd0: 7973 203d 2062 7563 6b65 742e 6c69 7374  ys = bucket.list
-00003ce0: 2864 656c 696d 6974 6572 3d64 656c 696d  (delimiter=delim
-00003cf0: 6974 6572 2c20 7072 6566 6978 3d70 7265  iter, prefix=pre
-00003d00: 6669 782c 206d 6178 5f6b 6579 733d 6d61  fix, max_keys=ma
-00003d10: 785f 6b65 7973 2c20 6d61 726b 6572 3d6d  x_keys, marker=m
-00003d20: 6172 6b65 7229 0a20 2023 2070 7269 6e74  arker).  # print
-00003d30: 286c 656e 286b 6579 7329 290a 2020 7265  (len(keys)).  re
-00003d40: 7320 3d20 5b6b 2e6e 616d 6520 666f 7220  s = [k.name for 
-00003d50: 6b20 696e 206b 6579 735d 0a20 2070 7269  k in keys].  pri
-00003d60: 6e74 2827 7265 733a 2027 2c20 7265 7329  nt('res: ', res)
-00003d70: 0a20 2023 2070 7269 6e74 2827 6974 656d  .  # print('item
-00003d80: 3a27 2c20 6b2e 6e61 6d65 2c20 7479 7065  :', k.name, type
-00003d90: 286b 2929 0a0a 6465 6620 6c69 7374 416e  (k))..def listAn
-00003da0: 6444 656c 6574 6528 293a 0a20 2062 7563  dDelete():.  buc
-00003db0: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00003dc0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-00003dd0: 6529 0a20 206b 6579 7320 3d20 6275 636b  e).  keys = buck
-00003de0: 6574 2e6c 6973 7428 6465 6c69 6d69 7465  et.list(delimite
-00003df0: 723d 272f 272c 206d 6178 5f6b 6579 733d  r='/', max_keys=
-00003e00: 3130 2c20 7072 6566 6978 3d27 3135 2729  10, prefix='15')
-00003e10: 0a20 2070 7269 6e74 286b 6579 732e 6d61  .  print(keys.ma
-00003e20: 726b 6572 290a 2020 666f 7220 6b20 696e  rker).  for k in
-00003e30: 206b 6579 733a 0a20 2020 2070 7269 6e74   keys:.    print
-00003e40: 2827 6f62 6a65 6374 3a27 2c20 6b2e 6e61  ('object:', k.na
-00003e50: 6d65 290a 2020 2020 6465 6c65 7465 4f62  me).    deleteOb
-00003e60: 6a65 6374 286b 2e6e 616d 6529 0a0a 6465  ject(k.name)..de
-00003e70: 6620 6c69 7374 4f62 6a65 6374 7341 6e64  f listObjectsAnd
-00003e80: 4669 6c74 6572 2865 6e64 5469 6d65 3d4e  Filter(endTime=N
-00003e90: 6f6e 6529 3a0a 2020 6275 636b 6574 203d  one):.  bucket =
-00003ea0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-00003eb0: 2827 6175 746f 2d74 6573 742d 6275 636b  ('auto-test-buck
-00003ec0: 6574 2729 0a20 206b 6579 7320 3d20 6275  et').  keys = bu
-00003ed0: 636b 6574 2e6c 6973 744f 626a 6563 7473  cket.listObjects
-00003ee0: 2864 656c 696d 6974 6572 3d27 2f27 2c20  (delimiter='/', 
-00003ef0: 6d61 785f 6b65 7973 3d32 2920 2320 7374  max_keys=2) # st
-00003f00: 6172 745f 7469 6d65 3d31 3634 3033 3331  art_time=1640331
-00003f10: 3434 362c 2065 6e64 5f74 696d 653d 3136  446, end_time=16
-00003f20: 3431 3839 3530 3936 0a20 2066 6f72 206b  41895096.  for k
-00003f30: 2069 6e20 6b65 7973 3a0a 2020 2020 7072   in keys:.    pr
-00003f40: 696e 7428 6b29 0a0a 6465 6620 6765 744f  int(k)..def getO
-00003f50: 626a 6563 7454 6167 6769 6e67 2829 3a0a  bjectTagging():.
-00003f60: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00003f70: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00003f80: 745f 6e61 6d65 290a 2020 6b65 7920 3d20  t_name).  key = 
-00003f90: 6275 636b 6574 2e67 6574 5f6b 6579 2827  bucket.get_key('
-00003fa0: 7465 7374 5461 6767 696e 6727 290a 2020  testTagging').  
-00003fb0: 7461 6767 696e 6720 3d20 6b65 792e 6765  tagging = key.ge
-00003fc0: 745f 6f62 6a65 6374 5f74 6167 6769 6e67  t_object_tagging
-00003fd0: 2829 0a20 2070 7269 6e74 2874 6167 6769  ().  print(taggi
-00003fe0: 6e67 2e74 6f5f 786d 6c28 2929 0a0a 6465  ng.to_xml())..de
-00003ff0: 6620 7365 744f 626a 6563 7454 6167 6769  f setObjectTaggi
-00004000: 6e67 2829 3a0a 2020 6275 636b 6574 203d  ng():.  bucket =
+00001c80: 2862 7563 6b65 742e 6465 6c65 7465 5f62  (bucket.delete_b
+00001c90: 7563 6b65 745f 636f 7273 2829 290a 0a64  ucket_cors())..d
+00001ca0: 6566 2067 6574 4275 636b 6574 4372 7228  ef getBucketCrr(
+00001cb0: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
+00001cc0: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00001cd0: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00001ce0: 6e61 6d65 290a 2020 7072 696e 7428 6275  name).  print(bu
+00001cf0: 636b 6574 2e67 6574 5f62 7563 6b65 745f  cket.get_bucket_
+00001d00: 6372 7228 292e 746f 5f78 6d6c 2829 290a  crr().to_xml()).
+00001d10: 0a64 6566 2073 6574 4275 636b 6574 4372  .def setBucketCr
+00001d20: 7228 6275 636b 6574 5f6e 616d 6529 3a0a  r(bucket_name):.
+00001d30: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00001d40: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00001d50: 745f 6e61 6d65 290a 2020 2320 6465 6c65  t_name).  # dele
+00001d60: 7465 4d61 726b 6572 5374 6174 7573 20e7  teMarkerStatus .
+00001d70: 9a84 e580 bce4 b8ba 2045 6e61 626c 6564  ........ Enabled
+00001d80: 20e5 928c 2044 6973 6162 6c65 640a 2020   ... Disabled.  
+00001d90: 2320 6869 7374 6f72 6963 616c 4f62 6a65  # historicalObje
+00001da0: 6374 5265 706c 6963 6174 696f 6e20 e8a1  ctReplication ..
+00001db0: a8e7 a4ba e698 afe5 90a6 e5bc 80e5 90af  ................
+00001dc0: e5ad 98e9 878f e5a4 8de5 88b6 efbc 8ce5  ................
+00001dd0: 80bc e4b8 ba20 456e 6162 6c65 6420 e592  ..... Enabled ..
+00001de0: 8c20 4469 7361 626c 6564 0a20 2070 7269  . Disabled.  pri
+00001df0: 6e74 2862 7563 6b65 742e 7365 745f 6275  nt(bucket.set_bu
+00001e00: 636b 6574 5f63 7272 2827 7465 7374 2d62  cket_crr('test-b
+00001e10: 7563 6b65 742d 7265 706c 6927 2c20 6465  ucket-repli', de
+00001e20: 6c65 7465 4d61 726b 6572 5374 6174 7573  leteMarkerStatus
+00001e30: 3d42 7563 6b65 7443 726f 7373 5265 706c  =BucketCrossRepl
+00001e40: 6963 6174 652e 454e 4142 4c45 442c 0a20  icate.ENABLED,. 
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2020 2020 2020 2020 2020 2020 2068 6973               his
+00001e70: 746f 7269 6361 6c4f 626a 6563 7452 6570  toricalObjectRep
+00001e80: 6c69 6361 7469 6f6e 3d42 7563 6b65 7443  lication=BucketC
+00001e90: 726f 7373 5265 706c 6963 6174 652e 454e  rossReplicate.EN
+00001ea0: 4142 4c45 442c 2070 7265 6669 783d 5b27  ABLED, prefix=['
+00001eb0: 6865 6c6c 6f27 5d29 290a 0a64 6566 2064  hello']))..def d
+00001ec0: 656c 6574 6542 7563 6b65 7443 7272 2862  eleteBucketCrr(b
+00001ed0: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
+00001ee0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+00001ef0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00001f00: 616d 6529 0a20 2070 7269 6e74 2862 7563  ame).  print(buc
+00001f10: 6b65 742e 6465 6c65 7465 5f62 7563 6b65  ket.delete_bucke
+00001f20: 745f 6372 7228 2929 0a0a 6465 6620 6765  t_crr())..def ge
+00001f30: 7442 7563 6b65 744c 6f67 6769 6e67 2862  tBucketLogging(b
+00001f40: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
+00001f50: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+00001f60: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00001f70: 616d 6529 0a20 2070 7269 6e74 2862 7563  ame).  print(buc
+00001f80: 6b65 742e 6765 745f 6275 636b 6574 5f6c  ket.get_bucket_l
+00001f90: 6f67 6769 6e67 2829 2e74 6f5f 786d 6c28  ogging().to_xml(
+00001fa0: 2929 0a0a 6465 6620 7365 7442 7563 6b65  ))..def setBucke
+00001fb0: 744c 6f67 6769 6e67 2862 7563 6b65 745f  tLogging(bucket_
+00001fc0: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00001fd0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00001fe0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00001ff0: 2062 6c6f 6767 696e 6720 3d20 4275 636b   blogging = Buck
+00002000: 6574 4c6f 6767 696e 6728 7461 7267 6574  etLogging(target
+00002010: 3d62 7563 6b65 745f 6e61 6d65 290a 2020  =bucket_name).  
+00002020: 7072 696e 7428 6275 636b 6574 2e73 6574  print(bucket.set
+00002030: 5f62 7563 6b65 745f 6c6f 6767 696e 6728  _bucket_logging(
+00002040: 626c 6f67 6769 6e67 2e74 6f5f 786d 6c28  blogging.to_xml(
+00002050: 2929 290a 0a64 6566 2067 6574 4275 636b  )))..def getBuck
+00002060: 6574 4d69 7272 6f72 2862 7563 6b65 745f  etMirror(bucket_
+00002070: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00002080: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00002090: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+000020a0: 2070 7269 6e74 2862 7563 6b65 742e 6765   print(bucket.ge
+000020b0: 745f 6275 636b 6574 5f6d 6972 726f 7228  t_bucket_mirror(
+000020c0: 2929 0a0a 6465 6620 7365 7442 7563 6b65  ))..def setBucke
+000020d0: 744d 6972 726f 7228 6275 636b 6574 5f6e  tMirror(bucket_n
+000020e0: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
+000020f0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00002100: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00002110: 7365 745f 6865 6164 6572 7320 3d20 5b7b  set_headers = [{
+00002120: 0a20 2020 2020 2022 6b65 7922 3a20 2264  .      "key": "d
+00002130: 222c 0a20 2020 2020 2022 7661 6c75 6522  ",.      "value"
+00002140: 3a20 2262 220a 2020 7d5d 0a20 2072 656d  : "b".  }].  rem
+00002150: 6f76 655f 6865 6164 6572 7320 3d20 5b7b  ove_headers = [{
+00002160: 0a20 2020 2020 2022 6b65 7922 3a20 2264  .      "key": "d
+00002170: 220a 2020 7d5d 0a20 2070 6173 735f 6865  ".  }].  pass_he
+00002180: 6164 6572 7320 3d20 5b7b 0a20 2020 2020  aders = [{.     
+00002190: 2022 6b65 7922 3a20 2261 6263 220a 2020   "key": "abc".  
+000021a0: 7d5d 0a20 2068 6561 6465 725f 7365 7474  }].  header_sett
+000021b0: 696e 6720 3d20 4865 6164 6572 5365 7474  ing = HeaderSett
+000021c0: 696e 6728 7365 745f 6865 6164 6572 733d  ing(set_headers=
+000021d0: 7365 745f 6865 6164 6572 732c 2072 656d  set_headers, rem
+000021e0: 6f76 655f 6865 6164 6572 733d 7265 6d6f  ove_headers=remo
+000021f0: 7665 5f68 6561 6465 7273 2c20 7061 7373  ve_headers, pass
+00002200: 5f61 6c6c 3d46 616c 7365 2c20 7061 7373  _all=False, pass
+00002210: 5f68 6561 6465 7273 3d70 6173 735f 6865  _headers=pass_he
+00002220: 6164 6572 7329 0a20 206d 6972 726f 725f  aders).  mirror_
+00002230: 7265 7175 6573 745f 7365 7474 696e 6720  request_setting 
+00002240: 3d20 4d69 7272 6f72 5265 7175 6573 7453  = MirrorRequestS
+00002250: 6574 7469 6e67 2870 6173 735f 7175 6572  etting(pass_quer
+00002260: 795f 7374 7269 6e67 3d46 616c 7365 2c20  y_string=False, 
+00002270: 666f 6c6c 6f77 3378 783d 4661 6c73 652c  follow3xx=False,
+00002280: 2068 6561 6465 725f 7365 7474 696e 673d   header_setting=
+00002290: 6865 6164 6572 5f73 6574 7469 6e67 290a  header_setting).
+000022a0: 2020 6173 796e 635f 6d69 7272 6f72 5f72    async_mirror_r
+000022b0: 756c 6520 3d20 4173 796e 634d 6972 726f  ule = AsyncMirro
+000022c0: 7252 756c 652e 7275 6c65 5f77 6974 685f  rRule.rule_with_
+000022d0: 6163 6c28 6d69 7272 6f72 5f75 726c 733d  acl(mirror_urls=
+000022e0: 5b22 6874 7470 3a2f 2f61 6263 2e6f 6d22  ["http://abc.om"
+000022f0: 2c20 2268 7474 703a 2f2f 7777 772e 7770  , "http://www.wp
+00002300: 732e 636e 225d 2c20 7361 7669 6e67 5f73  s.cn"], saving_s
+00002310: 6574 7469 6e67 5f61 636c 3d22 7072 6976  etting_acl="priv
+00002320: 6174 6522 290a 2020 7379 6e63 5f6d 6972  ate").  sync_mir
+00002330: 726f 725f 7275 6c65 7320 3d20 5379 6e63  ror_rules = Sync
+00002340: 4d69 7272 6f72 5275 6c65 732e 7275 6c65  MirrorRules.rule
+00002350: 735f 7769 7468 5f70 7265 6669 785f 6163  s_with_prefix_ac
+00002360: 6c28 6b65 795f 7072 6566 6978 6573 3d5b  l(key_prefixes=[
+00002370: 2261 6263 225d 2c20 6d69 7272 6f72 5f75  "abc"], mirror_u
+00002380: 726c 3d22 6874 7470 3a2f 2f76 2d6b 732d  rl="http://v-ks-
+00002390: 612d 692e 6f72 6967 696e 616c 766f 642e  a-i.originalvod.
+000023a0: 636f 6d22 2c20 6d69 7272 6f72 5f72 6571  com", mirror_req
+000023b0: 7565 7374 5f73 6574 7469 6e67 3d6d 6972  uest_setting=mir
+000023c0: 726f 725f 7265 7175 6573 745f 7365 7474  ror_request_sett
+000023d0: 696e 672c 2073 6176 696e 675f 7365 7474  ing, saving_sett
+000023e0: 696e 675f 6163 6c3d 2270 7269 7661 7465  ing_acl="private
+000023f0: 2229 0a20 206d 6972 726f 7220 3d20 4275  ").  mirror = Bu
+00002400: 636b 6574 4d69 7272 6f72 2875 7365 5f64  cketMirror(use_d
+00002410: 6566 6175 6c74 5f72 6f62 6f74 733d 4661  efault_robots=Fa
+00002420: 6c73 652c 2061 7379 6e63 5f6d 6972 726f  lse, async_mirro
+00002430: 725f 7275 6c65 3d61 7379 6e63 5f6d 6972  r_rule=async_mir
+00002440: 726f 725f 7275 6c65 2c20 7379 6e63 5f6d  ror_rule, sync_m
+00002450: 6972 726f 725f 7275 6c65 733d 5b73 796e  irror_rules=[syn
+00002460: 635f 6d69 7272 6f72 5f72 756c 6573 5d29  c_mirror_rules])
+00002470: 0a20 2070 7269 6e74 2862 7563 6b65 742e  .  print(bucket.
+00002480: 7365 745f 6275 636b 6574 5f6d 6972 726f  set_bucket_mirro
+00002490: 7228 6d69 7272 6f72 2929 0a0a 6465 6620  r(mirror))..def 
+000024a0: 6465 6c65 7465 4275 636b 6574 4d69 7272  deleteBucketMirr
+000024b0: 6f72 2862 7563 6b65 745f 6e61 6d65 293a  or(bucket_name):
+000024c0: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
+000024d0: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+000024e0: 6574 5f6e 616d 6529 0a20 2070 7269 6e74  et_name).  print
+000024f0: 2862 7563 6b65 742e 6465 6c65 7465 5f62  (bucket.delete_b
+00002500: 7563 6b65 745f 6d69 7272 6f72 2829 290a  ucket_mirror()).
+00002510: 0a0a 6465 6620 7365 7442 7563 6b65 7452  ..def setBucketR
+00002520: 6574 656e 7469 6f6e 2862 7563 6b65 745f  etention(bucket_
+00002530: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00002540: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00002550: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00002560: 2062 7563 6b65 745f 7265 7465 6e74 696f   bucket_retentio
+00002570: 6e20 3d20 4275 636b 6574 5265 7465 6e74  n = BucketRetent
+00002580: 696f 6e28 290a 2020 2320 e8ae bee7 bdae  ion().  # ......
+00002590: e59b 9ee6 94b6 e7ab 99e8 a784 e588 99ef  ................
+000025a0: bc9a e590 afe7 94a8 2fe7 a681 e794 a8e3  ......../.......
+000025b0: 8081 e696 87e4 bbb6 e4bf 9de7 9599 e5a4  ................
+000025c0: a9e6 95b0 0a20 2072 756c 6520 3d20 5265  .....  rule = Re
+000025d0: 7465 6e74 696f 6e52 756c 6528 5265 7465  tentionRule(Rete
+000025e0: 6e74 696f 6e52 756c 652e 454e 4142 4c45  ntionRule.ENABLE
+000025f0: 442c 2032 290a 2020 2320 7275 6c65 203d  D, 2).  # rule =
+00002600: 2052 6574 656e 7469 6f6e 5275 6c65 2852   RetentionRule(R
+00002610: 6574 656e 7469 6f6e 5275 6c65 2e44 4953  etentionRule.DIS
+00002620: 4142 4c45 442c 2032 290a 2020 6275 636b  ABLED, 2).  buck
+00002630: 6574 5f72 6574 656e 7469 6f6e 2e72 756c  et_retention.rul
+00002640: 6520 3d20 7275 6c65 0a20 2062 7563 6b65  e = rule.  bucke
+00002650: 742e 7365 745f 6275 636b 6574 5f72 6574  t.set_bucket_ret
+00002660: 656e 7469 6f6e 2862 7563 6b65 745f 7265  ention(bucket_re
+00002670: 7465 6e74 696f 6e29 0a0a 0a64 6566 2067  tention)...def g
+00002680: 6574 4275 636b 6574 5265 7465 6e74 696f  etBucketRetentio
+00002690: 6e28 6275 636b 6574 5f6e 616d 6529 3a0a  n(bucket_name):.
+000026a0: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+000026b0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+000026c0: 745f 6e61 6d65 290a 2020 7265 7420 3d20  t_name).  ret = 
+000026d0: 6275 636b 6574 2e67 6574 5f62 7563 6b65  bucket.get_bucke
+000026e0: 745f 7265 7465 6e74 696f 6e28 290a 2020  t_retention().  
+000026f0: 7072 696e 7428 7265 742e 746f 5f78 6d6c  print(ret.to_xml
+00002700: 2829 290a 0a0a 6465 6620 6c69 7374 5265  ())...def listRe
+00002710: 7465 6e74 696f 6e28 6275 636b 6574 5f6e  tention(bucket_n
+00002720: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
+00002730: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00002740: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00002750: 6b65 7973 203d 2062 7563 6b65 742e 6c69  keys = bucket.li
+00002760: 7374 5f72 6574 656e 7469 6f6e 2829 0a20  st_retention(). 
+00002770: 2066 6f72 206b 2069 6e20 6b65 7973 3a0a   for k in keys:.
+00002780: 2020 2020 7072 696e 7428 6b2e 6e61 6d65      print(k.name
+00002790: 290a 2020 2020 7072 696e 7428 6b2e 7265  ).    print(k.re
+000027a0: 7465 6e74 696f 6e5f 6964 290a 2020 2020  tention_id).    
+000027b0: 7072 696e 7428 6b2e 7374 6f72 6167 655f  print(k.storage_
+000027c0: 636c 6173 7329 0a0a 0a64 6566 2063 6c65  class)...def cle
+000027d0: 6172 4f62 6a65 6374 2862 7563 6b65 745f  arObject(bucket_
+000027e0: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+000027f0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00002800: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00002810: 206b 203d 2062 7563 6b65 742e 6e65 775f   k = bucket.new_
+00002820: 6b65 7928 2763 6c65 6172 5f6b 6579 5f6e  key('clear_key_n
+00002830: 616d 6527 290a 2020 6b2e 636c 6561 725f  ame').  k.clear_
+00002840: 6f62 6a65 6374 2827 3c72 6574 656e 7469  object('<retenti
+00002850: 6f6e 5f69 643e 2729 0a0a 0a64 6566 2072  on_id>')...def r
+00002860: 6563 6f76 6572 4f62 6a65 6374 2862 7563  ecoverObject(buc
+00002870: 6b65 745f 6e61 6d65 293a 0a20 2062 7563  ket_name):.  buc
+00002880: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
+00002890: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+000028a0: 6529 0a20 206b 203d 2062 7563 6b65 742e  e).  k = bucket.
+000028b0: 6e65 775f 6b65 7928 2772 6563 6f76 6572  new_key('recover
+000028c0: 5f6b 6579 5f6e 616d 6527 290a 2020 2320  _key_name').  # 
+000028d0: e5a6 82e6 9e9c 7265 7465 6e74 696f 6e5f  ......retention_
+000028e0: 6964 e4b8 bae7 a9ba efbc 8ce9 bb98 e8ae  id..............
+000028f0: a4e6 81a2 e5a4 8de5 9b9e e694 b6e7 ab99  ................
+00002900: e4b8 ade6 8c87 e5ae 9a6b 6579 e79a 84e6  .........key....
+00002910: 9c80 e696 b0e7 8988 e69c ac0a 2020 6b2e  ............  k.
+00002920: 7265 636f 7665 725f 6f62 6a65 6374 286f  recover_object(o
+00002930: 7665 7277 7269 7465 3d54 7275 652c 2072  verwrite=True, r
+00002940: 6574 656e 7469 6f6e 5f69 643d 273c 7265  etention_id='<re
+00002950: 7465 6e74 696f 6e5f 6964 3e27 290a 0a0a  tention_id>')...
+00002960: 6465 6620 7365 7442 7563 6b65 7449 6e76  def setBucketInv
+00002970: 656e 746f 7279 2862 7563 6b65 745f 6e61  entory(bucket_na
+00002980: 6d65 293a 0a20 2062 7563 6b65 7420 3d20  me):.  bucket = 
+00002990: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+000029a0: 6275 636b 6574 5f6e 616d 6529 0a20 2023  bucket_name).  #
+000029b0: 20e6 b7bb e58a a0e6 b885 e58d 95e8 a784   ...............
+000029c0: e588 99ef bc8c e8a7 84e5 8899 e590 8de4  ................
+000029d0: b8ba 696e 7665 6e74 6f72 7931 efbc 8ce7  ..inventory1....
+000029e0: 8ab6 e680 81e4 b8ba e5bc 80e5 90af 0a20  ............... 
+000029f0: 2023 20e6 b885 e58d 95e6 8aa5 e591 8ae4   # .............
+00002a00: bba5 4353 56e7 9a84 e6a0 bce5 bc8f e5ad  ..CSV...........
+00002a10: 98e5 82a8 efbc 8ce5 ad98 e582 a8e8 b7af  ................
+00002a20: e5be 84e4 b8ba 7461 7267 6574 5f61 6363  ......target_acc
+00002a30: 6f75 6e74 e8b4 a6e5 8fb7 e4b8 8be7 9a84  ount............
+00002a40: 7461 7267 6574 5f62 7563 6b65 74e6 a1b6  target_bucket...
+00002a50: efbc 8ce5 898d e7bc 80e4 b8ba 696e 7665  ............inve
+00002a60: 6e74 6f72 7931 5fe7 9a84 e696 87e4 bbb6  ntory1_.........
+00002a70: 0a20 2023 20e6 8aa5 e591 8ae7 949f e688  .  # ...........
+00002a80: 90e9 a291 e78e 87e4 b8ba e6af 8fe5 91a8  ................
+00002a90: e4b8 80e6 aca1 0a20 2023 20e6 89ab e68f  .......  # .....
+00002aa0: 8fe6 8c87 e5ae 9ae5 898d e7bc 80e5 928c  ................
+00002ab0: e69c 80e5 908e e4bf aee6 94b9 e697 b6e9  ................
+00002ac0: 97b4 e88c 83e5 9bb4 e79a 84e5 afb9 e8b1  ................
+00002ad0: a10a 2020 2320 e6b8 85e5 8d95 e7bb 93e6  ..  # ..........
+00002ae0: 9e9c e4b8 ade5 8c85 e590 ab20 e696 87e4  ........... ....
+00002af0: bbb6 e5a4 a7e5 b08f 20e5 928c 20e6 9c80  ........ ... ...
+00002b00: e590 8ee4 bfae e694 b9e6 97b6 e997 b420  ............... 
+00002b10: e79a 84e4 bfa1 e681 af0a 2020 696e 7665  ..........  inve
+00002b20: 6e74 6f72 7920 3d20 4275 636b 6574 496e  ntory = BucketIn
+00002b30: 7665 6e74 6f72 7928 6964 3d27 696e 7665  ventory(id='inve
+00002b40: 6e74 6f72 7931 272c 2069 735f 656e 6162  ntory1', is_enab
+00002b50: 6c65 643d 5472 7565 2c0a 2020 2020 2020  led=True,.      
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00002b80: 696f 6e3d 4465 7374 696e 6174 696f 6e28  ion=Destination(
+00002b90: 4465 7374 696e 6174 696f 6e2e 464f 524d  Destination.FORM
+00002ba0: 4154 5f43 5356 2c20 6163 636f 756e 745f  AT_CSV, account_
+00002bb0: 6964 3d27 7461 7267 6574 5f61 6363 6f75  id='target_accou
+00002bc0: 6e74 272c 0a20 2020 2020 2020 2020 2020  nt',.           
+00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 2020 2020 2062 7563 6b65             bucke
+00002c00: 743d 2774 6172 6765 745f 6275 636b 6574  t='target_bucket
+00002c10: 272c 2070 7265 6669 783d 2769 6e76 656e  ', prefix='inven
+00002c20: 746f 7279 315f 2729 2c0a 2020 2020 2020  tory1_'),.      
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+00002c50: 3d53 6368 6564 756c 6528 5363 6865 6475  =Schedule(Schedu
+00002c60: 6c65 2e57 4545 4b4c 5929 2c0a 2020 2020  le.WEEKLY),.    
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00002c90: 3d49 6e76 656e 746f 7279 4669 6c74 6572  =InventoryFilter
+00002ca0: 2870 7265 6669 783d 2761 272c 206c 6173  (prefix='a', las
+00002cb0: 745f 6d6f 6469 6679 5f62 6567 696e 5f74  t_modify_begin_t
+00002cc0: 696d 655f 7374 616d 703d 696e 7428 7469  ime_stamp=int(ti
+00002cd0: 6d65 2e74 696d 6528 2929 292c 0a20 2020  me.time())),.   
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00002d00: 6e61 6c5f 6669 656c 6473 3d5b 4275 636b  nal_fields=[Buck
+00002d10: 6574 496e 7665 6e74 6f72 792e 4f50 5449  etInventory.OPTI
+00002d20: 4f4e 414c 5f46 4945 4c44 5f53 495a 452c  ONAL_FIELD_SIZE,
+00002d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 4275 636b 6574 496e 7665 6e74 6f72 792e  BucketInventory.
+00002d70: 4f50 5449 4f4e 414c 5f46 4945 4c44 5f4c  OPTIONAL_FIELD_L
+00002d80: 4153 545f 4d4f 4449 4649 4544 5f44 4154  AST_MODIFIED_DAT
+00002d90: 455d 290a 0a20 2062 7563 6b65 742e 7365  E])..  bucket.se
+00002da0: 745f 6275 636b 6574 5f69 6e76 656e 746f  t_bucket_invento
+00002db0: 7279 2869 6e76 656e 746f 7279 290a 0a64  ry(inventory)..d
+00002dc0: 6566 2067 6574 4275 636b 6574 496e 7665  ef getBucketInve
+00002dd0: 6e74 6f72 7928 6275 636b 6574 5f6e 616d  ntory(bucket_nam
+00002de0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00002df0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00002e00: 7563 6b65 745f 6e61 6d65 290a 2020 696e  ucket_name).  in
+00002e10: 7665 6e74 6f72 7920 3d20 6275 636b 6574  ventory = bucket
+00002e20: 2e67 6574 5f62 7563 6b65 745f 696e 7665  .get_bucket_inve
+00002e30: 6e74 6f72 7928 2769 6e76 656e 746f 7279  ntory('inventory
+00002e40: 3127 290a 2020 7072 696e 7428 696e 7665  1').  print(inve
+00002e50: 6e74 6f72 792e 746f 5f78 6d6c 2829 290a  ntory.to_xml()).
+00002e60: 0a64 6566 206c 6973 7442 7563 6b65 7449  .def listBucketI
+00002e70: 6e76 656e 746f 7279 2862 7563 6b65 745f  nventory(bucket_
+00002e80: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00002e90: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00002ea0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00002eb0: 2072 6573 756c 7420 3d20 6275 636b 6574   result = bucket
+00002ec0: 2e6c 6973 745f 6275 636b 6574 5f69 6e76  .list_bucket_inv
+00002ed0: 656e 746f 7279 2829 0a20 2066 6f72 2069  entory().  for i
+00002ee0: 6e76 656e 746f 7279 2069 6e20 7265 7375  nventory in resu
+00002ef0: 6c74 2e69 6e76 656e 746f 7279 5f63 6f6e  lt.inventory_con
+00002f00: 6669 6775 7261 7469 6f6e 733a 0a20 2020  figurations:.   
+00002f10: 2070 7269 6e74 2869 6e76 656e 746f 7279   print(inventory
+00002f20: 2e74 6f5f 786d 6c28 2929 0a0a 6465 6620  .to_xml())..def 
+00002f30: 6465 6c65 7465 4275 636b 6574 496e 7665  deleteBucketInve
+00002f40: 6e74 6f72 7928 6275 636b 6574 5f6e 616d  ntory(bucket_nam
+00002f50: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00002f60: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00002f70: 7563 6b65 745f 6e61 6d65 290a 2020 6275  ucket_name).  bu
+00002f80: 636b 6574 2e64 656c 6574 655f 6275 636b  cket.delete_buck
+00002f90: 6574 5f69 6e76 656e 746f 7279 2827 696e  et_inventory('in
+00002fa0: 7665 6e74 6f72 7931 2729 0a0a 0a23 2323  ventory1')...###
+00002fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002fc0: 2323 2020 6b73 332e 6269 6c6c 696e 6720  ##  ks3.billing 
+00002fd0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00002fe0: 2323 2323 2323 2323 2323 2323 0a66 726f  ############.fro
+00002ff0: 6d20 6b73 332e 6269 6c6c 696e 6720 696d  m ks3.billing im
+00003000: 706f 7274 2067 6574 5f62 7563 6b65 7473  port get_buckets
+00003010: 5f64 6174 610a 0a64 6566 2067 6574 4275  _data..def getBu
+00003020: 636b 6574 7344 6174 6128 6275 636b 6574  cketsData(bucket
+00003030: 5f6e 616d 6573 3d4e 6f6e 6529 3a0a 2020  _names=None):.  
+00003040: 6461 7461 203d 2067 6574 5f62 7563 6b65  data = get_bucke
+00003050: 7473 5f64 6174 6128 616b 2c20 736b 2c20  ts_data(ak, sk, 
+00003060: 7374 6172 745f 7469 6d65 3d22 3230 3231  start_time="2021
+00003070: 3131 3139 3233 3030 222c 2065 6e64 5f74  11192300", end_t
+00003080: 696d 653d 2232 3032 3131 3131 3932 3335  ime="20211119235
+00003090: 3922 2c20 6275 636b 6574 5f6e 616d 6573  9", bucket_names
+000030a0: 3d62 7563 6b65 745f 6e61 6d65 732c 2070  =bucket_names, p
+000030b0: 726f 6475 6374 733d 2244 6174 6153 697a  roducts="DataSiz
+000030c0: 652c 5265 7175 6573 7473 4765 7422 290a  e,RequestsGet").
+000030d0: 2020 7072 696e 7428 6461 7461 290a 0a23    print(data)..#
+000030e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000030f0: 2323 2323 2020 6b73 332e 6f62 6a65 6374  ####  ks3.object
+00003100: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+00003110: 2323 2323 2323 2323 2323 2323 230a 6465  #############.de
+00003120: 6620 6765 744f 626a 6563 744d 6574 6128  f getObjectMeta(
+00003130: 6275 636b 6574 5f6e 616d 652c 206f 626a  bucket_name, obj
+00003140: 6563 745f 6b65 795f 6e61 6d65 2c20 6865  ect_key_name, he
+00003150: 6164 6572 733d 4e6f 6e65 293a 0a20 2062  aders=None):.  b
+00003160: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+00003170: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00003180: 616d 6529 0a20 2072 6573 7020 3d20 6275  ame).  resp = bu
+00003190: 636b 6574 2e67 6574 5f6b 6579 5f6d 6574  cket.get_key_met
+000031a0: 6128 6f62 6a65 6374 5f6b 6579 5f6e 616d  a(object_key_nam
+000031b0: 652c 2068 6561 6465 7273 3d68 6561 6465  e, headers=heade
+000031c0: 7273 290a 2020 6966 2072 6573 703a 0a20  rs).  if resp:. 
+000031d0: 2020 2070 7269 6e74 2822 e88e b7e5 8f96     print("......
+000031e0: e696 87e4 bbb6 6865 6164 6572 e688 90e5  ......header....
+000031f0: 8a9f 3a20 222c 2072 6573 702e 6865 6164  ..: ", resp.head
+00003200: 6572 7329 0a0a 6465 6620 7570 6c6f 6164  ers)..def upload
+00003210: 4f62 6a65 6374 4672 6f6d 4669 6c65 2866  ObjectFromFile(f
+00003220: 696c 656e 616d 6529 3a0a 2020 6275 636b  ilename):.  buck
+00003230: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00003240: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00003250: 290a 2020 6b20 3d20 6275 636b 6574 2e6e  ).  k = bucket.n
+00003260: 6577 5f6b 6579 2866 696c 656e 616d 6529  ew_key(filename)
+00003270: 0a20 2072 6574 203d 206b 2e73 6574 5f63  .  ret = k.set_c
+00003280: 6f6e 7465 6e74 735f 6672 6f6d 5f66 696c  ontents_from_fil
+00003290: 656e 616d 6528 6f73 2e70 6174 682e 6578  ename(os.path.ex
+000032a0: 7061 6e64 7573 6572 2822 7e22 2920 2b20  panduser("~") + 
+000032b0: 272f 446f 776e 6c6f 6164 732f 2720 2b20  '/Downloads/' + 
+000032c0: 6669 6c65 6e61 6d65 290a 2020 6966 2072  filename).  if r
+000032d0: 6574 2061 6e64 2072 6574 2e73 7461 7475  et and ret.statu
+000032e0: 7320 3d3d 2032 3030 3a0a 2020 2020 7072  s == 200:.    pr
+000032f0: 696e 7428 22e4 b88a e4bc a0e6 8890 e58a  int("...........
+00003300: 9f22 290a 0a64 6566 2075 706c 6f61 645f  .")..def upload_
+00003310: 6173 796e 6328 6669 6c65 6e61 6d65 293a  async(filename):
+00003320: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
+00003330: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00003340: 6574 5f6e 616d 6529 0a20 206b 203d 2062  et_name).  k = b
+00003350: 7563 6b65 742e 6e65 775f 6b65 7928 6669  ucket.new_key(fi
+00003360: 6c65 6e61 6d65 290a 2020 7265 7420 3d20  lename).  ret = 
+00003370: 6173 796e 6369 6f2e 7275 6e28 6b2e 7570  asyncio.run(k.up
+00003380: 6c6f 6164 5f66 696c 655f 6173 796e 6328  load_file_async(
+00003390: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
+000033a0: 6572 2822 7e22 2920 2b20 272f 446f 776e  er("~") + '/Down
+000033b0: 6c6f 6164 732f 2720 2b20 6669 6c65 6e61  loads/' + filena
+000033c0: 6d65 2929 0a20 2069 6620 7265 7420 616e  me)).  if ret an
+000033d0: 6420 7265 742e 7374 6174 7573 203d 3d20  d ret.status == 
+000033e0: 3230 303a 0a20 2020 2070 7269 6e74 2822  200:.    print("
+000033f0: e4b8 8ae4 bca0 e688 90e5 8a9f 2229 0a0a  ............")..
+00003400: 6465 6620 7570 6c6f 6164 4f62 6a65 6374  def uploadObject
+00003410: 4672 6f6d 5374 7269 6e67 2829 3a0a 2020  FromString():.  
+00003420: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00003430: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00003440: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
+00003450: 6574 2e6e 6577 5f6b 6579 2827 e5a4 a7e5  et.new_key('....
+00003460: aeb6 e5a5 bd27 290a 2020 2320 2320 6b65  .....').  # # ke
+00003470: 7920 e592 8c20 7661 6c75 6520 e99c 80e8  y ... value ....
+00003480: a681 2075 726c 20e7 bc96 e7a0 810a 2020  .. url .......  
+00003490: 2320 7461 6767 696e 6753 7472 203d 2027  # taggingStr = '
+000034a0: 6e61 6d65 3d6a 6827 0a20 2023 2068 6561  name=jh'.  # hea
+000034b0: 6465 7273 203d 207b 2778 2d6b 7373 2d74  ders = {'x-kss-t
+000034c0: 6167 6769 6e67 273a 2074 6167 6769 6e67  agging': tagging
+000034d0: 5374 727d 0a20 2072 6574 203d 206b 2e73  Str}.  ret = k.s
+000034e0: 6574 5f63 6f6e 7465 6e74 735f 6672 6f6d  et_contents_from
+000034f0: 5f73 7472 696e 6728 2720 776f 726c 6427  _string(' world'
+00003500: 290a 2020 2320 2320 e8af b7e6 b182 4944  ).  # # ......ID
+00003510: e380 82e8 afb7 e6b1 8249 44e6 98af e69c  .........ID.....
+00003520: ace6 aca1 e8af b7e6 b182 e79a 84e5 94af  ................
+00003530: e4b8 80e6 a087 e8af 86ef bc8c e5bc bae7  ................
+00003540: 8388 e5bb bae8 aeae e59c a8e7 a88b e5ba  ................
+00003550: 8fe6 97a5 e5bf 97e4 b8ad e6b7 bbe5 8aa0  ................
+00003560: e6ad a4e5 8f82 e695 b0e3 8082 0a20 2023  .............  #
+00003570: 2070 7269 6e74 2872 6574 2e68 6561 6465   print(ret.heade
+00003580: 7273 5b27 782d 6b73 732d 7265 7175 6573  rs['x-kss-reques
+00003590: 742d 6964 275d 290a 2020 2320 2320 4554  t-id']).  # # ET
+000035a0: 6167 e698 af70 7574 5f6f 626a 6563 74e6  ag...put_object.
+000035b0: 96b9 e6b3 95e8 bf94 e59b 9ee5 80bc e789  ................
+000035c0: b9e6 9c89 e79a 84e5 b19e e680 a7ef bc8c  ................
+000035d0: e794 a8e4 ba8e e6a0 87e8 af86 e4b8 80e4  ................
+000035e0: b8aa 4f62 6a65 6374 e79a 84e5 8685 e5ae  ..Object........
+000035f0: b9e3 8082 0a20 2023 2070 7269 6e74 2872  .....  # print(r
+00003600: 6574 2e68 6561 6465 7273 290a 2020 2320  et.headers).  # 
+00003610: 4854 5450 e8bf 94e5 9b9e e7a0 81e3 8082  HTTP............
+00003620: 0a20 2069 6620 7265 7420 616e 6420 7265  .  if ret and re
+00003630: 742e 7374 6174 7573 203d 3d20 3230 303a  t.status == 200:
+00003640: 0a20 2020 2070 7269 6e74 2822 e4b8 8ae4  .    print("....
+00003650: bca0 e688 90e5 8a9f 2229 0a0a 6465 6620  ........")..def 
+00003660: 6865 6164 4f62 6a65 6374 2829 3a0a 2020  headObject():.  
+00003670: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00003680: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00003690: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
+000036a0: 6574 2e67 6574 5f6b 6579 2827 7465 7374  et.get_key('test
+000036b0: 5f65 6e63 7279 7074 696f 6e27 290a 2020  _encryption').  
+000036c0: 6966 206b 3a0a 2020 2020 7072 696e 7428  if k:.    print(
+000036d0: 6b2e 6e61 6d65 2c20 6b2e 7369 7a65 2c20  k.name, k.size, 
+000036e0: 6b2e 6c61 7374 5f6d 6f64 6966 6965 642c  k.last_modified,
+000036f0: 206b 2e6f 626a 6563 745f 7479 7065 2c20   k.object_type, 
+00003700: 6b2e 7461 6767 696e 675f 636f 756e 7429  k.tagging_count)
+00003710: 0a0a 6465 6620 646f 776e 6c6f 6164 4f62  ..def downloadOb
+00003720: 6a65 6374 416e 6450 7269 6e74 286b 6579  jectAndPrint(key
+00003730: 6e61 6d65 2c20 6279 7465 5f72 616e 6765  name, byte_range
+00003740: 3d28 302c 2031 292c 2068 6561 6465 7273  =(0, 1), headers
+00003750: 3d4e 6f6e 6529 3a0a 2020 6275 636b 6574  =None):.  bucket
+00003760: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+00003770: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00003780: 2020 6b20 3d20 6275 636b 6574 2e67 6574    k = bucket.get
+00003790: 5f6b 6579 286b 6579 6e61 6d65 290a 2020  _key(keyname).  
+000037a0: 7320 3d20 6b2e 6765 745f 636f 6e74 656e  s = k.get_conten
+000037b0: 7473 5f61 735f 7374 7269 6e67 2862 7974  ts_as_string(byt
+000037c0: 655f 7261 6e67 653d 6279 7465 5f72 616e  e_range=byte_ran
+000037d0: 6765 2c20 6865 6164 6572 733d 6865 6164  ge, headers=head
+000037e0: 6572 7329 2e64 6563 6f64 6528 290a 2020  ers).decode().  
+000037f0: 7072 696e 7428 7329 0a0a 6465 6620 646f  print(s)..def do
+00003800: 776e 6c6f 6164 5f61 7379 6e63 286b 6579  wnload_async(key
+00003810: 6e61 6d65 2c20 6865 6164 6572 733d 4e6f  name, headers=No
+00003820: 6e65 293a 0a20 2062 7563 6b65 7420 3d20  ne):.  bucket = 
+00003830: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+00003840: 6275 636b 6574 5f6e 616d 6529 0a20 206b  bucket_name).  k
+00003850: 203d 2062 7563 6b65 742e 6765 745f 6b65   = bucket.get_ke
+00003860: 7928 6b65 796e 616d 6529 0a20 2074 7279  y(keyname).  try
+00003870: 3a0a 2020 2020 6173 796e 6369 6f2e 7275  :.    asyncio.ru
+00003880: 6e28 6b2e 646f 776e 6c6f 6164 5f66 696c  n(k.download_fil
+00003890: 655f 6173 796e 6328 6f73 2e70 6174 682e  e_async(os.path.
+000038a0: 6578 7061 6e64 7573 6572 2822 7e22 2920  expanduser("~") 
+000038b0: 2b20 272f 446f 776e 6c6f 6164 732f 2720  + '/Downloads/' 
+000038c0: 2b20 6b65 796e 616d 6529 290a 2020 2020  + keyname)).    
+000038d0: 7072 696e 7428 27e4 b88b e8bd bde6 8890  print('.........
+000038e0: e58a 9f27 290a 2020 6578 6365 7074 3a0a  ...').  except:.
+000038f0: 2020 2020 7072 696e 7428 27e4 b88b e8bd      print('.....
+00003900: bde5 a4b1 e8b4 a527 290a 0a64 6566 2064  .......')..def d
+00003910: 6f77 6e6c 6f61 644f 626a 6563 7441 7353  ownloadObjectAsS
+00003920: 7472 6561 6d41 6e64 5072 696e 7428 293a  treamAndPrint():
+00003930: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
+00003940: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00003950: 6574 5f6e 616d 6529 0a20 206b 203d 2062  et_name).  k = b
+00003960: 7563 6b65 742e 6765 745f 6b65 7928 2773  ucket.get_key('s
+00003970: 6861 6b65 2e74 7874 2729 0a20 2062 7974  hake.txt').  byt
+00003980: 6573 203d 206b 2e72 6561 6428 3330 3029  es = k.read(300)
+00003990: 0a20 2070 7269 6e74 2827 7374 6172 743a  .  print('start:
+000039a0: 2027 2c20 6461 7465 7469 6d65 2e6e 6f77   ', datetime.now
+000039b0: 2829 2e73 7472 6674 696d 6528 2225 592d  ().strftime("%Y-
+000039c0: 256d 2d25 6420 2548 3a25 4d3a 2553 2e25  %m-%d %H:%M:%S.%
+000039d0: 6622 2929 0a20 2077 6869 6c65 2062 7974  f")).  while byt
+000039e0: 6573 3a0a 2020 2020 7320 3d20 6279 7465  es:.    s = byte
+000039f0: 732e 6465 636f 6465 2829 0a20 2020 2070  s.decode().    p
+00003a00: 7269 6e74 2827 6279 7465 7320 6465 636f  rint('bytes deco
+00003a10: 6465 643a 272c 2073 290a 2020 2020 7469  ded:', s).    ti
+00003a20: 6d65 2e73 6c65 6570 2835 290a 2020 2020  me.sleep(5).    
+00003a30: 6279 7465 7320 3d20 6b2e 7265 6164 2833  bytes = k.read(3
+00003a40: 3030 290a 2020 7072 696e 7428 2765 6e64  00).  print('end
+00003a50: 3a20 272c 2064 6174 6574 696d 652e 6e6f  : ', datetime.no
+00003a60: 7728 292e 7374 7266 7469 6d65 2822 2559  w().strftime("%Y
+00003a70: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+00003a80: 2566 2229 290a 0a64 6566 2064 6f77 6e6c  %f"))..def downl
+00003a90: 6f61 644f 626a 6563 7441 6e64 5361 7665  oadObjectAndSave
+00003aa0: 286b 6579 5f6e 616d 652c 2062 7974 655f  (key_name, byte_
+00003ab0: 7261 6e67 653d 2830 2c20 3129 2c20 6865  range=(0, 1), he
+00003ac0: 6164 6572 733d 4e6f 6e65 293a 0a20 2062  aders=None):.  b
+00003ad0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
+00003ae0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00003af0: 616d 6529 0a20 206b 203d 2062 7563 6b65  ame).  k = bucke
+00003b00: 742e 6765 745f 6b65 7928 6b65 795f 6e61  t.get_key(key_na
+00003b10: 6d65 290a 2020 6b2e 6765 745f 636f 6e74  me).  k.get_cont
+00003b20: 656e 7473 5f74 6f5f 6669 6c65 6e61 6d65  ents_to_filename
+00003b30: 2827 2f55 7365 7273 2f6a 6162 6261 722f  ('/Users/jabbar/
+00003b40: 446f 776e 6c6f 6164 732f 4453 4330 3333  Downloads/DSC033
+00003b50: 3830 2e65 6e63 7279 7074 2ee9 9d9e e588  80.encrypt......
+00003b60: 86e5 9d97 2e6a 7067 2e64 6f77 6e6c 6f61  .....jpg.downloa
+00003b70: 6427 2c20 6865 6164 6572 733d 6865 6164  d', headers=head
+00003b80: 6572 7329 0a0a 6465 6620 6465 6c65 7465  ers)..def delete
+00003b90: 4f62 6a65 6374 286b 6579 5f6e 616d 6529  Object(key_name)
+00003ba0: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
+00003bb0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00003bc0: 6b65 745f 6e61 6d65 290a 2020 7472 793a  ket_name).  try:
+00003bd0: 0a20 2020 2062 7563 6b65 742e 6465 6c65  .    bucket.dele
+00003be0: 7465 5f6b 6579 286b 6579 5f6e 616d 6529  te_key(key_name)
+00003bf0: 0a20 2020 2070 7269 6e74 2822 e588 a0e9  .    print("....
+00003c00: 99a4 e688 90e5 8a9f 2229 0a20 2065 7863  ........").  exc
+00003c10: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00003c20: 2065 3a0a 2020 2020 7072 696e 7428 22e5   e:.    print(".
+00003c30: 88a0 e999 a4e5 a4b1 e8b4 a522 290a 2020  ...........").  
+00003c40: 2020 7072 696e 7428 6529 0a20 2020 2070    print(e).    p
+00003c50: 6173 730a 0a64 6566 2067 6574 4f62 6a65  ass..def getObje
+00003c60: 6374 4163 6c28 293a 0a20 2062 7563 6b65  ctAcl():.  bucke
+00003c70: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
+00003c80: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+00003c90: 0a20 2070 6f6c 6963 7920 3d20 6275 636b  .  policy = buck
+00003ca0: 6574 2e67 6574 5f61 636c 2827 6172 7469  et.get_acl('arti
+00003cb0: 636c 652e 7478 7427 290a 2020 7072 696e  cle.txt').  prin
+00003cc0: 7428 706f 6c69 6379 2e74 6f5f 786d 6c28  t(policy.to_xml(
+00003cd0: 2929 0a0a 6465 6620 7365 744f 626a 6563  ))..def setObjec
+00003ce0: 7441 636c 2829 3a0a 2020 6275 636b 6574  tAcl():.  bucket
+00003cf0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+00003d00: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00003d10: 2020 2320 6f62 6a65 6374 2070 6f6c 6963    # object polic
+00003d20: 7920 3a20 7072 6976 6174 6520 7c20 7075  y : private | pu
+00003d30: 626c 6963 2d72 6561 6420 7c20 7075 626c  blic-read | publ
+00003d40: 6963 2d72 6561 642d 7772 6974 650a 2020  ic-read-write.  
+00003d50: 6275 636b 6574 2e73 6574 5f61 636c 2822  bucket.set_acl("
+00003d60: 7075 626c 6963 2d72 6561 6422 2c20 273c  public-read", '<
+00003d70: 594f 5552 5f4b 4559 5f4e 414d 453e 2729  YOUR_KEY_NAME>')
+00003d80: 0a0a 6465 6620 7365 744f 626a 6563 744d  ..def setObjectM
+00003d90: 6574 6128 293a 0a20 2062 203d 2063 6f6e  eta():.  b = con
+00003da0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00003db0: 6b65 745f 6e61 6d65 290a 2020 622e 636f  ket_name).  b.co
+00003dc0: 7079 5f6b 6579 2827 3c79 6f75 724b 6579  py_key('<yourKey
+00003dd0: 4e61 6d65 3e27 2c20 273c 796f 7572 4275  Name>', '<yourBu
+00003de0: 636b 6574 4e61 6d65 3e27 2c20 273c 796f  cketName>', '<yo
+00003df0: 7572 4b65 794e 616d 653e 272c 0a20 2020  urKeyName>',.   
+00003e00: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00003e10: 733d 7b27 636f 6e74 656e 742d 7479 7065  s={'content-type
+00003e20: 273a 2027 7465 7874 2f70 6c61 696e 272c  ': 'text/plain',
+00003e30: 2027 782d 6b73 732d 6d65 7461 6461 7461   'x-kss-metadata
+00003e40: 2d64 6972 6563 7469 7665 273a 2027 5245  -directive': 'RE
+00003e50: 504c 4143 4527 7d29 0a0a 6465 6620 7365  PLACE'})..def se
+00003e60: 744f 626a 6563 7453 746f 7261 6765 436c  tObjectStorageCl
+00003e70: 6173 7328 293a 0a20 2062 203d 2063 6f6e  ass():.  b = con
+00003e80: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00003e90: 6b65 745f 6e61 6d65 290a 2020 622e 636f  ket_name).  b.co
+00003ea0: 7079 5f6b 6579 2827 3c79 6f75 724b 6579  py_key('<yourKey
+00003eb0: 4e61 6d65 3e27 2c20 273c 796f 7572 4275  Name>', '<yourBu
+00003ec0: 636b 6574 4e61 6d65 3e27 2c20 273c 796f  cketName>', '<yo
+00003ed0: 7572 4b65 794e 616d 653e 272c 2068 6561  urKeyName>', hea
+00003ee0: 6465 7273 3d7b 2778 2d6b 7373 2d73 746f  ders={'x-kss-sto
+00003ef0: 7261 6765 2d63 6c61 7373 273a 2027 5354  rage-class': 'ST
+00003f00: 414e 4441 5244 5f49 4127 7d29 0a0a 6465  ANDARD_IA'})..de
+00003f10: 6620 636f 7079 2864 7374 4b65 792c 2073  f copy(dstKey, s
+00003f20: 7263 4b65 792c 2064 7374 5f62 7563 6b65  rcKey, dst_bucke
+00003f30: 745f 6e61 6d65 3d4e 6f6e 652c 2068 6561  t_name=None, hea
+00003f40: 6465 7273 3d4e 6f6e 6529 3a0a 2020 2320  ders=None):.  # 
+00003f50: 6275 636b 6574 5f6e 616d 6520 3d20 2768  bucket_name = 'h
+00003f60: 6170 7079 686f 7572 270a 2020 6220 3d20  appyhour'.  b = 
+00003f70: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+00003f80: 6275 636b 6574 5f6e 616d 6529 0a20 2072  bucket_name).  r
+00003f90: 6574 7572 6e20 622e 636f 7079 5f6b 6579  eturn b.copy_key
+00003fa0: 2864 7374 4b65 792c 2064 7374 5f62 7563  (dstKey, dst_buc
+00003fb0: 6b65 745f 6e61 6d65 2c20 7372 634b 6579  ket_name, srcKey
+00003fc0: 2c20 6865 6164 6572 733d 6865 6164 6572  , headers=header
+00003fd0: 7329 0a0a 6465 6620 636f 7079 5f65 6e63  s)..def copy_enc
+00003fe0: 7279 7074 696f 6e28 6473 744b 6579 2c20  ryption(dstKey, 
+00003ff0: 7372 634b 6579 2c20 656e 6372 7970 745f  srcKey, encrypt_
+00004000: 6b65 793d 4e6f 6e65 293a 0a20 2062 203d  key=None):.  b =
 00004010: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
 00004020: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00004030: 6b65 7920 3d20 6275 636b 6574 2e67 6574  key = bucket.get
-00004040: 5f6b 6579 2827 7465 7374 5461 6767 696e  _key('testTaggin
-00004050: 6727 290a 2020 7461 6767 696e 6720 3d20  g').  tagging = 
-00004060: 5b54 6167 2827 3027 292c 2054 6167 2827  [Tag('0'), Tag('
-00004070: 3127 2c20 2731 2729 5d0a 2020 6b65 792e  1', '1')].  key.
-00004080: 7365 745f 6f62 6a65 6374 5f74 6167 6769  set_object_taggi
-00004090: 6e67 2874 6167 6769 6e67 290a 0a64 6566  ng(tagging)..def
-000040a0: 2064 656c 6574 654f 626a 6563 7454 6167   deleteObjectTag
-000040b0: 6769 6e67 2829 3a0a 2020 6275 636b 6574  ging():.  bucket
-000040c0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-000040d0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-000040e0: 2020 6b65 7920 3d20 6275 636b 6574 2e67    key = bucket.g
-000040f0: 6574 5f6b 6579 2827 6865 6865 2729 0a20  et_key('hehe'). 
-00004100: 206b 6579 2e64 656c 6574 655f 6f62 6a65   key.delete_obje
-00004110: 6374 5f74 6167 6769 6e67 2829 0a0a 6465  ct_tagging()..de
-00004120: 6620 6361 6c63 466f 6c64 6572 5369 7a65  f calcFolderSize
-00004130: 2862 7563 6b65 742c 2066 6f6c 6465 7229  (bucket, folder)
-00004140: 3a0a 2020 6c65 6e67 7468 203d 2030 0a20  :.  length = 0. 
-00004150: 206b 6579 7320 3d20 6275 636b 6574 2e6c   keys = bucket.l
-00004160: 6973 7428 7072 6566 6978 3d66 6f6c 6465  ist(prefix=folde
-00004170: 7229 0a20 2066 6f72 206b 2069 6e20 6b65  r).  for k in ke
-00004180: 7973 3a0a 2020 2020 6966 2069 7369 6e73  ys:.    if isins
-00004190: 7461 6e63 6528 6b2c 204b 6579 293a 0a20  tance(k, Key):. 
-000041a0: 2020 2020 206c 656e 6774 6820 2b3d 206b       length += k
-000041b0: 2e73 697a 650a 2020 7265 7475 726e 206c  .size.  return l
-000041c0: 656e 6774 680a 0a66 726f 6d20 6b73 332e  ength..from ks3.
-000041d0: 7072 6566 6978 2069 6d70 6f72 7420 5072  prefix import Pr
-000041e0: 6566 6978 0a0a 2320 e588 97e4 b8be e68c  efix..# ........
-000041f0: 87e5 ae9a e79b aee5 bd95 e4b8 8be7 9a84  ................
-00004200: e696 87e4 bbb6 e5a4 a7e5 b08f 0a64 6566  .............def
-00004210: 2067 6574 466f 6c64 6572 5369 7a65 496e   getFolderSizeIn
-00004220: 4275 636b 6574 2829 3a0a 2020 6275 636b  Bucket():.  buck
-00004230: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00004240: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00004250: 290a 2020 6b65 7973 203d 2062 7563 6b65  ).  keys = bucke
-00004260: 742e 6c69 7374 2864 656c 696d 6974 6572  t.list(delimiter
-00004270: 3d27 2f27 290a 2020 666f 7220 6b20 696e  ='/').  for k in
-00004280: 206b 6579 733a 0a20 2020 2069 6620 6973   keys:.    if is
-00004290: 696e 7374 616e 6365 286b 2c20 5072 6566  instance(k, Pref
-000042a0: 6978 293a 0a20 2020 2020 2070 7269 6e74  ix):.      print
-000042b0: 2827 6469 723a 2027 202b 206b 2e6e 616d  ('dir: ' + k.nam
-000042c0: 6520 2b20 2720 2073 697a 653a 2720 2b20  e + '  size:' + 
-000042d0: 7374 7228 6361 6c63 466f 6c64 6572 5369  str(calcFolderSi
-000042e0: 7a65 2862 7563 6b65 742c 206b 2e6e 616d  ze(bucket, k.nam
-000042f0: 6529 2920 2b20 2242 7974 6522 290a 0a0a  e)) + "Byte")...
-00004300: 6465 6620 7465 7374 5f6d 756c 7469 7061  def test_multipa
-00004310: 7274 5f75 706c 6f61 6428 656e 6372 7970  rt_upload(encryp
-00004320: 745f 6b65 793d 4e6f 6e65 293a 0a20 2069  t_key=None):.  i
-00004330: 6d70 6f72 7420 6d61 7468 2c20 6f73 0a20  mport math, os. 
-00004340: 2066 726f 6d20 6669 6c65 6368 756e 6b69   from filechunki
-00004350: 6f20 696d 706f 7274 2046 696c 6543 6875  o import FileChu
-00004360: 6e6b 494f 0a20 2062 7563 6b65 7420 3d20  nkIO.  bucket = 
-00004370: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-00004380: 6275 636b 6574 5f6e 616d 6529 0a0a 2020  bucket_name)..  
-00004390: 736f 7572 6365 5f70 6174 6820 3d20 272f  source_path = '/
-000043a0: 5573 6572 732f 6a61 6262 6172 2f44 6f77  Users/jabbar/Dow
-000043b0: 6e6c 6f61 6473 2f44 5343 3033 3338 302e  nloads/DSC03380.
-000043c0: 4a50 4727 0a20 2023 20e6 ba90 e696 87e4  JPG'.  # .......
-000043d0: bbb6 e5a4 a7e5 b08f 0a20 2073 6f75 7263  .........  sourc
-000043e0: 655f 7369 7a65 203d 206f 732e 7374 6174  e_size = os.stat
-000043f0: 2873 6f75 7263 655f 7061 7468 292e 7374  (source_path).st
-00004400: 5f73 697a 650a 0a20 206d 7020 3d20 6275  _size..  mp = bu
-00004410: 636b 6574 2e69 6e69 7469 6174 655f 6d75  cket.initiate_mu
-00004420: 6c74 6970 6172 745f 7570 6c6f 6164 2822  ltipart_upload("
-00004430: 4453 4330 3333 3830 2e6d 702e 6a70 6722  DSC03380.mp.jpg"
-00004440: 2c20 656e 6372 7970 745f 6b65 793d 656e  , encrypt_key=en
-00004450: 6372 7970 745f 6b65 7929 0a20 2070 7269  crypt_key).  pri
-00004460: 6e74 286d 7029 0a0a 2020 6368 756e 6b5f  nt(mp)..  chunk_
-00004470: 7369 7a65 203d 2035 3234 3238 3830 0a20  size = 5242880. 
-00004480: 2063 6875 6e6b 5f63 6f75 6e74 203d 2069   chunk_count = i
-00004490: 6e74 286d 6174 682e 6365 696c 2873 6f75  nt(math.ceil(sou
-000044a0: 7263 655f 7369 7a65 202a 2031 2e30 202f  rce_size * 1.0 /
-000044b0: 2063 6875 6e6b 5f73 697a 6520 2a20 312e   chunk_size * 1.
-000044c0: 3029 290a 0a20 2023 20e9 809a e8bf 8720  0))..  # ...... 
-000044d0: 4669 6c65 4368 756e 6b49 4f20 e5b0 86e6  FileChunkIO ....
-000044e0: 9687 e4bb b6e5 8886 e789 870a 2020 666f  ............  fo
-000044f0: 7220 6920 696e 2072 616e 6765 2863 6875  r i in range(chu
-00004500: 6e6b 5f63 6f75 6e74 293a 0a20 2020 206f  nk_count):.    o
-00004510: 6666 7365 7420 3d20 6368 756e 6b5f 7369  ffset = chunk_si
-00004520: 7a65 202a 2069 0a20 2020 2062 7974 6573  ze * i.    bytes
-00004530: 203d 206d 696e 2863 6875 6e6b 5f73 697a   = min(chunk_siz
-00004540: 652c 2073 6f75 7263 655f 7369 7a65 202d  e, source_size -
-00004550: 206f 6666 7365 7429 0a20 2020 2077 6974   offset).    wit
-00004560: 6820 4669 6c65 4368 756e 6b49 4f28 736f  h FileChunkIO(so
-00004570: 7572 6365 5f70 6174 682c 2027 7227 2c20  urce_path, 'r', 
-00004580: 6f66 6673 6574 3d6f 6666 7365 742c 2062  offset=offset, b
-00004590: 7974 6573 3d62 7974 6573 2920 6173 2066  ytes=bytes) as f
-000045a0: 703a 0a20 2020 2020 2023 20e9 8090 e4b8  p:.      # .....
-000045b0: aae4 b88a e4bc a0e5 8886 e789 870a 2020  ..............  
-000045c0: 2020 2020 6d70 2e75 706c 6f61 645f 7061      mp.upload_pa
-000045d0: 7274 5f66 726f 6d5f 6669 6c65 2866 702c  rt_from_file(fp,
-000045e0: 2070 6172 745f 6e75 6d3d 6920 2b20 3129   part_num=i + 1)
-000045f0: 0a20 2070 7269 6e74 286d 702e 746f 5f78  .  print(mp.to_x
-00004600: 6d6c 2829 290a 2020 2320 e58f 91e9 8081  ml()).  # ......
-00004610: e8af b7e6 b182 efbc 8ce5 9088 e5b9 b6e5  ................
-00004620: 8886 e789 87ef bc8c e5ae 8ce6 8890 e588  ................
-00004630: 86e7 8987 e4b8 8ae4 bca0 0a20 2072 6574  ...........  ret
-00004640: 203d 206d 702e 636f 6d70 6c65 7465 5f75   = mp.complete_u
-00004650: 706c 6f61 6428 290a 2020 6966 2072 6574  pload().  if ret
-00004660: 2061 6e64 2072 6574 2e73 7461 7475 7320   and ret.status 
-00004670: 3d3d 2032 3030 3a0a 2020 2020 7072 696e  == 200:.    prin
-00004680: 7428 22e4 b88a e4bc a0e6 8890 e58a 9f22  t("............"
-00004690: 290a 0a64 6566 2074 6573 745f 6665 7463  )..def test_fetc
-000046a0: 685f 6f62 6a65 6374 2829 3a0a 2020 6275  h_object():.  bu
-000046b0: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-000046c0: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
-000046d0: 6d65 290a 2020 6b65 7920 3d20 6275 636b  me).  key = buck
-000046e0: 6574 2e6e 6577 5f6b 6579 2827 7777 772d  et.new_key('www-
-000046f0: 6c6f 676f 2729 0a20 206b 6579 2e66 6574  logo').  key.fet
-00004700: 6368 5f6f 626a 6563 7428 736f 7572 6365  ch_object(source
-00004710: 5f75 726c 3d27 6874 7470 3a2f 2f66 652e  _url='http://fe.
-00004720: 6b73 7975 6e2e 636f 6d2f 7072 6f6a 6563  ksyun.com/projec
-00004730: 742f 7265 736f 7572 6365 2f69 6d67 2f77  t/resource/img/w
-00004740: 7777 2d6c 6f67 6f2e 706e 6727 2c0a 2020  ww-logo.png',.  
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 2020 6865 6164 6572 733d 7b27 782d      headers={'x-
-00004770: 6b73 732d 6163 6c27 3a20 2770 7562 6c69  kss-acl': 'publi
-00004780: 632d 7265 6164 277d 290a 2020 7072 696e  c-read'}).  prin
-00004790: 7428 2766 6574 6368 e688 90e5 8a9f 2729  t('fetch......')
-000047a0: 0a0a 6465 6620 7465 7374 5f67 656e 6572  ..def test_gener
-000047b0: 6174 655f 7572 6c28 6b65 795f 6e61 6d65  ate_url(key_name
-000047c0: 2c20 696d 6167 655f 6174 7472 733d 4e6f  , image_attrs=No
-000047d0: 6e65 293a 0a20 2062 203d 2063 6f6e 6e2e  ne):.  b = conn.
-000047e0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-000047f0: 745f 6e61 6d65 290a 2020 6b20 3d20 622e  t_name).  k = b.
-00004800: 6765 745f 6b65 7928 6b65 795f 6e61 6d65  get_key(key_name
-00004810: 290a 2020 6966 206b 3a0a 2020 2020 7572  ).  if k:.    ur
-00004820: 6c20 3d20 6b2e 6765 6e65 7261 7465 5f75  l = k.generate_u
-00004830: 726c 2836 3030 2c20 696d 6167 655f 6174  rl(600, image_at
-00004840: 7472 733d 696d 6167 655f 6174 7472 7329  trs=image_attrs)
-00004850: 2020 2320 3630 7320 e590 8ee8 afa5 e993    # 60s ........
-00004860: bee6 8ea5 e8bf 87e6 9c9f 0a20 2020 2070  ...........    p
-00004870: 7269 6e74 2875 726c 290a 2020 656c 7365  rint(url).  else
-00004880: 3a0a 2020 2020 7072 696e 7428 276f 626a  :.    print('obj
-00004890: 6563 7420 6e6f 7420 666f 756e 6427 290a  ect not found').
-000048a0: 0a64 6566 2074 6573 745f 6765 745f 7072  .def test_get_pr
-000048b0: 6573 6967 6e65 645f 7572 6c28 6b65 795f  esigned_url(key_
-000048c0: 6e61 6d65 293a 0a20 2062 203d 2063 6f6e  name):.  b = con
-000048d0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-000048e0: 6b65 745f 6e61 6d65 290a 2020 2320 e696  ket_name).  # ..
-000048f0: b0e5 bbba e5af b9e8 b1a1 6b65 790a 2020  ..........key.  
-00004900: 6b20 3d20 622e 6e65 775f 6b65 7928 6b65  k = b.new_key(ke
-00004910: 795f 6e61 6d65 290a 2020 6966 206b 3a0a  y_name).  if k:.
-00004920: 2020 2020 7572 6c20 3d20 6b2e 6765 745f      url = k.get_
-00004930: 7072 6573 6967 6e65 645f 7572 6c28 3630  presigned_url(60
-00004940: 3030 3029 2020 2320 3630 7320 e590 8ee8  000)  # 60s ....
-00004950: afa5 e993 bee6 8ea5 e8bf 87e6 9c9f 0a20  ............... 
-00004960: 2020 2070 7269 6e74 2875 726c 290a 2020     print(url).  
-00004970: 2020 7265 7475 726e 2075 726c 0a0a 6465    return url..de
-00004980: 6620 7265 7374 6f72 654f 626a 6563 7428  f restoreObject(
-00004990: 6b65 795f 6e61 6d65 293a 0a20 2062 203d  key_name):.  b =
-000049a0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-000049b0: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-000049c0: 6b20 3d20 622e 6765 745f 6b65 7928 6b65  k = b.get_key(ke
-000049d0: 795f 6e61 6d65 290a 2020 6b2e 7265 7374  y_name).  k.rest
-000049e0: 6f72 655f 6f62 6a65 6374 2829 0a0a 6465  ore_object()..de
-000049f0: 6620 7465 7374 5f70 7574 5f76 6961 5f70  f test_put_via_p
-00004a00: 7265 7369 676e 6564 5f75 726c 286b 6579  resigned_url(key
-00004a10: 293a 0a20 2075 726c 203d 2074 6573 745f  ):.  url = test_
-00004a20: 6765 745f 7072 6573 6967 6e65 645f 7572  get_presigned_ur
-00004a30: 6c28 6b65 7929 0a20 2077 6974 6820 6f70  l(key).  with op
-00004a40: 656e 2827 2e2f 6172 7469 636c 652e 7478  en('./article.tx
-00004a50: 7427 2c20 2772 6227 2920 6173 2066 703a  t', 'rb') as fp:
-00004a60: 0a20 2020 2072 6573 756c 7420 3d20 7265  .    result = re
-00004a70: 7175 6573 7473 2e70 7574 2875 726c 2c20  quests.put(url, 
-00004a80: 6461 7461 3d66 7029 0a20 2020 2070 7269  data=fp).    pri
-00004a90: 6e74 2872 6573 756c 7429 0a0a 6672 6f6d  nt(result)..from
-00004aa0: 206b 7333 2e73 7473 2069 6d70 6f72 7420   ks3.sts import 
-00004ab0: 6173 7375 6d65 526f 6c65 0a64 6566 2074  assumeRole.def t
-00004ac0: 6573 745f 6173 7375 6d65 526f 6c65 2829  est_assumeRole()
-00004ad0: 3a0a 2020 7072 696e 7428 6173 7375 6d65  :.  print(assume
-00004ae0: 526f 6c65 2861 6b2c 2073 6b2c 2022 6b72  Role(ak, sk, "kr
-00004af0: 6e3a 6b73 633a 6961 6d3a 3a78 7878 3a72  n:ksc:iam::xxx:r
-00004b00: 6f6c 652f 7878 2d74 6573 742d 6275 636b  ole/xx-test-buck
-00004b10: 6574 222c 2022 6b73 3322 2c20 3336 3030  et", "ks3", 3600
-00004b20: 2929 0a0a 0a64 6566 2070 7574 5f6f 626a  ))...def put_obj
-00004b30: 6563 745f 6361 6c6c 6261 636b 286b 6579  ect_callback(key
-00004b40: 5f6e 616d 6529 3a0a 2020 6220 3d20 636f  _name):.  b = co
-00004b50: 6e6e 2e67 6574 5f62 7563 6b65 7428 2768  nn.get_bucket('h
-00004b60: 616e 6a69 6e67 2d74 6573 7430 3030 2729  anjing-test000')
-00004b70: 0a20 2023 20e6 96b0 e5bb bae5 afb9 e8b1  .  # ...........
-00004b80: a16b 6579 0a20 206b 203d 2062 2e6e 6577  .key.  k = b.new
-00004b90: 5f6b 6579 286b 6579 5f6e 616d 6529 0a20  _key(key_name). 
-00004ba0: 2023 20e4 b88a e4bc a0e6 8890 e58a 9fe5   # .............
-00004bb0: 908e efbc 8ce5 9091 e59b 9ee8 b083 e59c  ................
-00004bc0: b0e5 9d80 504f 5354 e695 b0e6 8dae 0a20  ....POST....... 
-00004bd0: 2023 20e9 9c80 e8a6 81e8 aebe e7bd ae60   # ............`
-00004be0: 782d 6b73 732d 6361 6c6c 6261 636b 7572  x-kss-callbackur
-00004bf0: 6c60 e592 8c60 782d 6b73 732d 6361 6c6c  l`...`x-kss-call
-00004c00: 6261 636b 626f 6479 60e8 afb7 e6b1 82e5  backbody`.......
-00004c10: a4b4 efbc 8ce8 afa6 e8a7 81e6 9687 e6a1  ................
-00004c20: a35b e4b8 8ae4 bca0 e59b 9ee8 b083 e5a4  .[..............
-00004c30: 84e7 9086 5d28 6874 7470 733a 2f2f 646f  ....](https://do
-00004c40: 6373 2e6b 7379 756e 2e63 6f6d 2f64 6f63  cs.ksyun.com/doc
-00004c50: 756d 656e 7473 2f39 3536 29e3 8082 0a20  uments/956).... 
-00004c60: 2023 2078 2d6b 7373 2d63 616c 6c62 6163   # x-kss-callbac
-00004c70: 6b75 726c 20e4 b8ba e58f 91e8 b5b7 e59b  kurl ...........
-00004c80: 9ee8 b083 e697 b6e8 afb7 e6b1 82e7 9a84  ................
-00004c90: e69c 8de5 8aa1 e599 a8e5 9cb0 e59d 800a  ................
-00004ca0: 2020 2320 782d 6b73 732d 6361 6c6c 6261    # x-kss-callba
-00004cb0: 636b 626f 6479 20e4 b8ba e58f 91e8 b5b7  ckbody .........
-00004cc0: e59b 9ee8 b083 e697 b6e8 afb7 e6b1 82e7  ................
-00004cd0: 9a84 626f 6479 e79a 84e5 80bc 0a20 2068  ..body.......  h
-00004ce0: 6561 6465 7273 203d 207b 2278 2d6b 7373  eaders = {"x-kss
-00004cf0: 2d63 616c 6c62 6163 6b75 726c 223a 2022  -callbackurl": "
-00004d00: 6874 7470 733a 2f2f 7968 2d73 682e 6b73  https://yh-sh.ks
-00004d10: 332d 636e 2d73 6861 6e67 6861 692e 6b73  3-cn-shanghai.ks
-00004d20: 7975 6e63 732e 636f 6d22 2c20 2278 2d6b  yuncs.com", "x-k
-00004d30: 7373 2d63 616c 6c62 6163 6b62 6f64 7922  ss-callbackbody"
-00004d40: 3a20 226f 626a 6563 744b 6579 3d24 7b6b  : "objectKey=${k
-00004d50: 6579 7d26 6574 6167 3d24 7b65 7461 677d  ey}&etag=${etag}
-00004d60: 2662 7563 6b65 743d 247b 6275 636b 6574  &bucket=${bucket
-00004d70: 7d26 6f62 6a65 6374 5369 7a65 3d24 7b6f  }&objectSize=${o
-00004d80: 626a 6563 7453 697a 657d 266d 696d 6554  bjectSize}&mimeT
-00004d90: 7970 653d 247b 6d69 6d65 5479 7065 7d26  ype=${mimeType}&
-00004da0: 6372 6561 7465 5469 6d65 3d24 7b63 7265  createTime=${cre
-00004db0: 6174 6554 696d 657d 222c 2022 782d 6b73  ateTime}", "x-ks
-00004dc0: 732d 6361 6c6c 6261 636b 6175 7468 223a  s-callbackauth":
-00004dd0: 317d 0a20 2072 6574 203d 206b 2e73 6574  1}.  ret = k.set
-00004de0: 5f63 6f6e 7465 6e74 735f 6672 6f6d 5f73  _contents_from_s
-00004df0: 7472 696e 6728 2274 6573 742d 6361 6c6c  tring("test-call
-00004e00: 6261 636b 222c 2068 6561 6465 7273 3d68  back", headers=h
-00004e10: 6561 6465 7273 290a 2020 6966 2072 6574  eaders).  if ret
-00004e20: 2061 6e64 2072 6574 2e73 7461 7475 7320   and ret.status 
-00004e30: 3d3d 2032 3030 3a0a 2020 2020 7072 696e  == 200:.    prin
-00004e40: 7428 22e4 b88a e4bc a0e6 8890 e58a 9f22  t("............"
-00004e50: 290a 0a23 2067 6574 416c 6c42 7563 6b65  )..# getAllBucke
-00004e60: 7473 2829 0a23 2068 6561 6442 7563 6b65  ts().# headBucke
-00004e70: 7428 2762 6a27 290a 2320 6765 7442 7563  t('bj').# getBuc
-00004e80: 6b65 744c 6f63 6174 696f 6e28 2774 6573  ketLocation('tes
-00004e90: 742d 686f 7374 2d73 7479 6c65 2729 0a23  t-host-style').#
-00004ea0: 2063 7265 6174 6542 7563 6b65 7428 2774   createBucket('t
-00004eb0: 6573 742d 6275 636b 6574 2d61 7263 6869  est-bucket-archi
-00004ec0: 7665 2d74 6573 742d 7368 616e 6768 6169  ve-test-shanghai
-00004ed0: 3227 2c20 6c6f 6361 7469 6f6e 3d27 5348  2', location='SH
-00004ee0: 414e 4748 4149 2729 0a23 2064 656c 6574  ANGHAI').# delet
-00004ef0: 6542 7563 6b65 7428 2774 6573 742d 6275  eBucket('test-bu
-00004f00: 636b 6574 2729 0a23 2067 6574 4275 636b  cket').# getBuck
-00004f10: 6574 4163 6c28 2774 6573 742d 6275 636b  etAcl('test-buck
-00004f20: 6574 2729 0a23 2073 6574 4275 636b 6574  et').# setBucket
-00004f30: 4163 6c28 2774 6573 742d 6275 636b 6574  Acl('test-bucket
-00004f40: 2729 0a23 206d 616e 6167 6542 7563 6b65  ').# manageBucke
-00004f50: 7452 6570 6c69 6361 7469 6f6e 2827 7465  tReplication('te
-00004f60: 7374 2d62 7563 6b65 7427 290a 2320 6765  st-bucket').# ge
-00004f70: 7442 7563 6b65 744c 6966 6543 7963 6c65  tBucketLifeCycle
-00004f80: 2862 7563 6b65 745f 6e61 6d65 290a 2320  (bucket_name).# 
-00004f90: 7365 7442 7563 6b65 744c 6966 6543 7963  setBucketLifeCyc
-00004fa0: 6c65 2862 7563 6b65 745f 6e61 6d65 290a  le(bucket_name).
-00004fb0: 2320 7365 7442 7563 6b65 744c 6966 6543  # setBucketLifeC
-00004fc0: 7963 6c65 3228 6275 636b 6574 5f6e 616d  ycle2(bucket_nam
-00004fd0: 6529 0a23 2064 656c 6574 6542 7563 6b65  e).# deleteBucke
-00004fe0: 744c 6966 6543 7963 6c65 2862 7563 6b65  tLifeCycle(bucke
-00004ff0: 745f 6e61 6d65 290a 2320 6765 7442 7563  t_name).# getBuc
-00005000: 6b65 744c 6f67 6769 6e67 2862 7563 6b65  ketLogging(bucke
-00005010: 745f 6e61 6d65 290a 2320 7365 7442 7563  t_name).# setBuc
-00005020: 6b65 744c 6f67 6769 6e67 2862 7563 6b65  ketLogging(bucke
-00005030: 745f 6e61 6d65 290a 2320 6469 7361 626c  t_name).# disabl
-00005040: 6542 7563 6b65 744c 6f67 6769 6e67 2862  eBucketLogging(b
-00005050: 7563 6b65 745f 6e61 6d65 290a 2320 656e  ucket_name).# en
-00005060: 6162 6c65 4275 636b 6574 4c6f 6767 696e  ableBucketLoggin
-00005070: 6728 6275 636b 6574 5f6e 616d 6529 0a23  g(bucket_name).#
-00005080: 2070 7574 4275 636b 6574 436f 7273 2862   putBucketCors(b
-00005090: 7563 6b65 745f 6e61 6d65 290a 2320 6765  ucket_name).# ge
-000050a0: 7442 7563 6b65 7443 6f72 7328 6275 636b  tBucketCors(buck
-000050b0: 6574 5f6e 616d 6529 0a23 2064 656c 6574  et_name).# delet
-000050c0: 6542 7563 6b65 7443 6f72 7328 6275 636b  eBucketCors(buck
-000050d0: 6574 5f6e 616d 6529 0a23 2064 656c 6574  et_name).# delet
-000050e0: 6542 7563 6b65 7443 7272 2862 7563 6b65  eBucketCrr(bucke
-000050f0: 745f 6e61 6d65 290a 2320 6765 7442 7563  t_name).# getBuc
-00005100: 6b65 7443 7272 2862 7563 6b65 745f 6e61  ketCrr(bucket_na
-00005110: 6d65 290a 2320 7365 7442 7563 6b65 7443  me).# setBucketC
-00005120: 7272 2862 7563 6b65 745f 6e61 6d65 290a  rr(bucket_name).
-00005130: 2320 7365 7442 7563 6b65 744d 6972 726f  # setBucketMirro
-00005140: 7228 6275 636b 6574 5f6e 616d 6529 0a23  r(bucket_name).#
-00005150: 2064 656c 6574 6542 7563 6b65 744d 6972   deleteBucketMir
-00005160: 726f 7228 6275 636b 6574 5f6e 616d 6529  ror(bucket_name)
-00005170: 0a23 2067 6574 4275 636b 6574 4d69 7272  .# getBucketMirr
-00005180: 6f72 2862 7563 6b65 745f 6e61 6d65 290a  or(bucket_name).
-00005190: 2323 2323 2320 6f62 6a65 6374 2023 2323  ##### object ###
-000051a0: 2323 0a23 2067 6574 4f62 6a65 6374 4d65  ##.# getObjectMe
-000051b0: 7461 2862 7563 6b65 745f 6e61 6d65 2c20  ta(bucket_name, 
-000051c0: 2761 7274 6963 6c65 2e74 7874 2729 0a23  'article.txt').#
-000051d0: 206c 6973 745f 6f62 6a65 6374 7328 290a   list_objects().
-000051e0: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
-000051f0: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
-00005200: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
-00005210: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
-00005220: 206d 6172 6b65 723d 2731 3035 3027 290a   marker='1050').
-00005230: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
-00005240: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
-00005250: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
-00005260: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
-00005270: 206d 6172 6b65 723d 2731 3035 2f27 290a   marker='105/').
-00005280: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
-00005290: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
-000052a0: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
-000052b0: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
-000052c0: 206d 6172 6b65 723d 2731 3035 2532 4627   marker='105%2F'
-000052d0: 290a 2320 6c69 7374 4f62 6a65 6374 7341  ).# listObjectsA
-000052e0: 6e64 4669 6c74 6572 2829 0a23 2073 6574  ndFilter().# set
-000052f0: 4f62 6a65 6374 5461 6767 696e 6728 290a  ObjectTagging().
-00005300: 2320 6765 744f 626a 6563 7454 6167 6769  # getObjectTaggi
-00005310: 6e67 2829 0a23 2064 656c 6574 654f 626a  ng().# deleteObj
-00005320: 6563 7454 6167 6769 6e67 2829 0a23 2067  ectTagging().# g
-00005330: 6574 466f 6c64 6572 5369 7a65 496e 4275  etFolderSizeInBu
-00005340: 636b 6574 2829 3b0a 2320 646f 776e 6c6f  cket();.# downlo
-00005350: 6164 4f62 6a65 6374 416e 6450 7269 6e74  adObjectAndPrint
-00005360: 2829 0a23 2064 6f77 6e6c 6f61 644f 626a  ().# downloadObj
-00005370: 6563 7441 7353 7472 6561 6d41 6e64 5072  ectAsStreamAndPr
-00005380: 696e 7428 290a 2320 646f 776e 6c6f 6164  int().# download
-00005390: 4f62 6a65 6374 416e 6453 6176 6528 6275  ObjectAndSave(bu
-000053a0: 636b 6574 5f6e 616d 652c 2027 4453 4330  cket_name, 'DSC0
-000053b0: 3333 3830 2e65 6e63 7279 7074 2ee9 9d9e  3380.encrypt....
-000053c0: e588 86e5 9d97 2e6a 7067 272c 2068 6561  .......jpg', hea
-000053d0: 6465 7273 3d7b 0a23 2020 2027 7261 6e67  ders={.#   'rang
-000053e0: 6527 3a20 2762 7974 6573 3d30 2d35 3234  e': 'bytes=0-524
-000053f0: 3238 3830 270a 2320 7d29 0a23 2063 6f75  2880'.# }).# cou
-00005400: 6e74 203d 2032 300a 2320 7768 696c 6520  nt = 20.# while 
-00005410: 5472 7565 3a0a 2320 7570 6c6f 6164 4f62  True:.# uploadOb
-00005420: 6a65 6374 4672 6f6d 4669 6c65 2827 e6b3  jectFromFile('..
-00005430: 95e6 b2bb 2e6a 7065 6727 290a 7570 6c6f  .....jpeg').uplo
-00005440: 6164 5f61 7379 6e63 2827 e6b3 95e6 b2bb  ad_async('......
-00005450: 2e6a 7065 6727 290a 646f 776e 6c6f 6164  .jpeg').download
-00005460: 5f61 7379 6e63 2827 3136 3539 3638 3438  _async('16596848
-00005470: 3732 2e74 6f72 7265 6e74 2729 0a23 2075  72.torrent').# u
-00005480: 706c 6f61 644f 626a 6563 7446 726f 6d46  ploadObjectFromF
-00005490: 696c 6528 2778 6162 2729 0a23 2075 706c  ile('xab').# upl
-000054a0: 6f61 644f 626a 6563 7446 726f 6d46 696c  oadObjectFromFil
-000054b0: 6528 2778 6163 2729 0a23 2020 2074 696d  e('xac').#   tim
-000054c0: 652e 736c 6565 7028 3529 0a23 2020 2063  e.sleep(5).#   c
-000054d0: 6f75 6e74 203d 2063 6f75 6e74 202d 2031  ount = count - 1
-000054e0: 0a23 2075 706c 6f61 644f 626a 6563 7446  .# uploadObjectF
-000054f0: 726f 6d53 7472 696e 6728 290a 2320 6865  romString().# he
-00005500: 6164 4f62 6a65 6374 2829 0a23 2064 6f77  adObject().# dow
-00005510: 6e6c 6f61 644f 626a 6563 7441 6e64 5072  nloadObjectAndPr
-00005520: 696e 7428 2774 6573 745f 6469 7265 6374  int('test_direct
-00005530: 6f72 792f 2729 0a23 2064 656c 6574 654f  ory/').# deleteO
-00005540: 626a 6563 7428 2274 656c 6c6d 6577 6879  bject("tellmewhy
-00005550: 2229 0a23 2067 6574 4f62 6a65 6374 4163  ").# getObjectAc
-00005560: 6c28 290a 0a23 2074 6573 745f 6d75 6c74  l()..# test_mult
-00005570: 6970 6172 745f 7570 6c6f 6164 2865 6e63  ipart_upload(enc
-00005580: 7279 7074 5f6b 6579 3d54 7275 6529 0a0a  rypt_key=True)..
-00005590: 2320 7465 7374 5f66 6574 6368 5f6f 626a  # test_fetch_obj
-000055a0: 6563 7428 290a 2320 6465 6620 7465 7374  ect().# def test
-000055b0: 5f67 656e 6572 6174 655f 7572 6c28 6b65  _generate_url(ke
-000055c0: 795f 6e61 6d65 2c20 696d 6167 655f 6174  y_name, image_at
-000055d0: 7472 733d 4e6f 6e65 293a 0a23 2020 2062  trs=None):.#   b
-000055e0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-000055f0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00005600: 2320 2020 6b20 3d20 622e 6765 745f 6b65  #   k = b.get_ke
-00005610: 7928 6b65 795f 6e61 6d65 290a 2320 2020  y(key_name).#   
-00005620: 6966 206b 3a0a 2320 2020 2020 7572 6c20  if k:.#     url 
-00005630: 3d20 6b2e 6765 6e65 7261 7465 5f75 726c  = k.generate_url
-00005640: 2836 3030 2c20 696d 6167 655f 6174 7472  (600, image_attr
-00005650: 733d 696d 6167 655f 6174 7472 7329 2020  s=image_attrs)  
-00005660: 2320 3630 7320 e590 8ee8 afa5 e993 bee6  # 60s ..........
-00005670: 8ea5 e8bf 87e6 9c9f 0a23 2020 2020 2070  .........#     p
-00005680: 7269 6e74 2875 726c 290a 2320 2020 656c  rint(url).#   el
-00005690: 7365 3a0a 2320 2020 2020 7072 696e 7428  se:.#     print(
-000056a0: 276f 626a 6563 7420 6e6f 7420 666f 756e  'object not foun
-000056b0: 6427 290a 0a23 2062 7563 6b65 7420 3d20  d')..# bucket = 
-000056c0: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-000056d0: 2774 6573 742d 6275 636b 6574 2729 0a23  'test-bucket').#
-000056e0: 206b 6579 7320 3d20 6275 636b 6574 2e6c   keys = bucket.l
-000056f0: 6973 7428 290a 2320 666f 7220 6b20 696e  ist().# for k in
-00005700: 206b 6579 733a 0a23 2020 2070 7269 6e74   keys:.#   print
-00005710: 286b 290a 2320 2020 6966 2069 7369 6e73  (k).#   if isins
-00005720: 7461 6e63 6528 6b2c 204b 6579 293a 0a23  tance(k, Key):.#
-00005730: 2020 2020 2075 726c 203d 206b 2e67 656e       url = k.gen
-00005740: 6572 6174 655f 7572 6c28 3630 3029 0a23  erate_url(600).#
-00005750: 2020 2020 2072 6573 203d 2072 6571 7565       res = reque
-00005760: 7374 732e 6765 7428 7572 6c29 0a23 2020  sts.get(url).#  
-00005770: 2020 2069 6620 7265 732e 7374 6174 7573     if res.status
-00005780: 5f63 6f64 6520 213d 2032 3030 3a0a 2320  _code != 200:.# 
-00005790: 2020 2020 2020 7072 696e 7428 7572 6c29        print(url)
-000057a0: 0a0a 0a23 2072 6573 203d 2072 6571 7565  ...# res = reque
-000057b0: 7374 732e 6765 7428 7572 6c29 0a23 2061  sts.get(url).# a
-000057c0: 7373 6572 7420 7265 732e 7374 6174 7573  ssert res.status
-000057d0: 5f63 6f64 6520 213d 2034 3033 0a23 2074  _code != 403.# t
-000057e0: 6573 745f 6765 6e65 7261 7465 5f75 726c  est_generate_url
-000057f0: 2827 5c5c 615c 5c5c 5c3a 3c3e 2a3f 7c3a  ('\\a\\\\:<>*?|:
-00005800: 712e 6a70 6567 2729 0a23 2074 6573 745f  q.jpeg').# test_
-00005810: 6765 6e65 7261 7465 5f75 726c 2827 2378  generate_url('#x
-00005820: 323b 2e6a 702e 6373 7627 290a 2320 7465  2;.jp.csv').# te
-00005830: 7374 5f67 656e 6572 6174 655f 7572 6c28  st_generate_url(
-00005840: 2731 3030 3836 2f31 3938 2e31 382d 7265  '10086/198.18-re
-00005850: 7365 742d e585 b1e8 aea1 39e6 9da1 2e74  set-......9....t
-00005860: 7874 2729 0a23 2074 6573 745f 6765 6e65  xt').# test_gene
-00005870: 7261 7465 5f75 726c 2827 3130 3038 362f  rate_url('10086/
-00005880: 6765 7462 7563 6b65 742e 6373 7627 290a  getbucket.csv').
-00005890: 2320 7465 7374 5f67 6574 5f70 7265 7369  # test_get_presi
-000058a0: 676e 6564 5f75 726c 2827 7e2a 632f 6865  gned_url('~*c/he
-000058b0: 636b 4461 7461 2b73 6466 3d25 3246 2e6a  ckData+sdf=%2F.j
-000058c0: 736f 6e27 290a 2320 7465 7374 5f70 7574  son').# test_put
-000058d0: 5f76 6961 5f70 7265 7369 676e 6564 5f75  _via_presigned_u
-000058e0: 726c 2827 696e 6465 782e 6874 6d6c 2729  rl('index.html')
-000058f0: 0a23 206c 6973 745f 6f62 6a65 6374 735f  .# list_objects_
-00005900: 7632 2864 656c 696d 6974 6572 3d27 2f27  v2(delimiter='/'
-00005910: 2c20 656e 636f 6469 6e67 5f74 7970 653d  , encoding_type=
-00005920: 2775 726c 272c 2066 6574 6368 5f6f 776e  'url', fetch_own
-00005930: 6572 3d46 616c 7365 290a 2320 6c69 7374  er=False).# list
-00005940: 5f6f 626a 6563 7473 2829 0a23 206c 6973  _objects().# lis
-00005950: 744f 626a 6563 7473 4d6f 7265 2829 0a23  tObjectsMore().#
-00005960: 2064 656c 6574 654f 626a 6563 7428 290a   deleteObject().
-00005970: 2320 6c69 7374 4f62 6a65 6374 7341 6e64  # listObjectsAnd
-00005980: 4669 6c74 6572 2829 0a23 206c 6973 7441  Filter().# listA
-00005990: 6e64 4465 6c65 7465 2829 0a23 2072 6573  ndDelete().# res
-000059a0: 746f 7265 4f62 6a65 6374 2822 7777 772d  toreObject("www-
-000059b0: 6c6f 676f 2229 0a23 2067 6574 4275 636b  logo").# getBuck
-000059c0: 6574 7344 6174 6128 2274 6573 742d 6275  etsData("test-bu
-000059d0: 636b 6574 2229 0a23 2074 6573 745f 6173  cket").# test_as
-000059e0: 7375 6d65 526f 6c65 2829 0a0a 2320 636f  sumeRole()..# co
-000059f0: 7079 5f65 6e63 7279 7074 696f 6e28 2761  py_encryption('a
-00005a00: 7274 6963 6c65 2e65 6e63 7279 7074 696f  rticle.encryptio
-00005a10: 6e2e 7478 7427 2c20 2761 7274 6963 6c65  n.txt', 'article
-00005a20: 2e74 7874 272c 2065 6e63 7279 7074 5f6b  .txt', encrypt_k
-00005a30: 6579 3d54 7275 6529 0a0a 2320 6669 6c65  ey=True)..# file
-00005a40: 4e61 6d65 203d 2022 5c75 3030 3662 5c75  Name = "\u006b\u
-00005a50: 3030 3733 5c75 3030 3566 5c75 3030 3733  0073\u005f\u0073
-00005a60: 5c75 3030 3633 5c75 3030 3631 5c75 3030  \u0063\u0061\u00
-00005a70: 3665 5c75 3030 3566 5c75 3030 3666 5c75  6e\u005f\u006f\u
-00005a80: 3030 3633 5c75 3030 3732 5c75 3030 3266  0063\u0072\u002f
-00005a90: 5c75 3030 3332 5c75 3030 3330 5c75 3030  \u0032\u0030\u00
-00005aa0: 3331 5c75 3030 3338 5c75 3030 3264 5c75  31\u0038\u002d\u
-00005ab0: 3030 3330 5c75 3030 3333 5c75 3030 3264  0030\u0033\u002d
-00005ac0: 5c75 3030 3331 5c75 3030 3332 5c75 3030  \u0031\u0032\u00
-00005ad0: 3266 5c75 3030 3130 5c75 6666 6664 5c75  2f\u0010\ufffd\u
-00005ae0: 3030 3730 5c75 6666 6664 5c75 6666 6664  0070\ufffd\ufffd
-00005af0: 5c75 6666 6664 5c75 3030 3032 5c75 3030  \ufffd\u0002\u00
-00005b00: 3265 5c75 3030 3537 5c75 3030 3766 5c75  2e\u0057\u007f\u
-00005b10: 3030 3562 5c75 6666 6664 5c75 3030 3038  005b\ufffd\u0008
-00005b20: 5c75 6666 6664 5c75 3030 3261 5c75 6666  \ufffd\u002a\uff
-00005b30: 6664 5c75 3030 3265 5c75 3030 3661 5c75  fd\u002e\u006a\u
-00005b40: 3030 3730 5c75 3030 3637 223b 0a23 2068  0070\u0067";.# h
-00005b50: 6568 6520 3d20 2210 efbf bd70 efbf bdef  ehe = "....p....
-00005b60: bfbd efbf bd02 2e57 7f5b efbf bd2a efbf  .......W.[...*..
-00005b70: bd2e 6a70 6722 0a23 2066 6f72 2063 2069  ..jpg".# for c i
-00005b80: 6e20 6865 6865 3a0a 2320 2020 2020 7072  n hehe:.#     pr
-00005b90: 696e 7428 7265 7072 2863 292c 2063 290a  int(repr(c), c).
-00005ba0: 2320 7572 6c63 6f64 6564 203d 2075 726c  # urlcoded = url
-00005bb0: 6c69 622e 7061 7273 652e 7175 6f74 6528  lib.parse.quote(
-00005bc0: 6669 6c65 4e61 6d65 290a 2320 756e 7175  fileName).# unqu
-00005bd0: 6f74 6564 203d 2075 726c 6c69 622e 7061  oted = urllib.pa
-00005be0: 7273 652e 756e 7175 6f74 6528 2725 4646  rse.unquote('%FF
-00005bf0: 2729 0a23 2071 756f 7465 6420 3d20 7572  ').# quoted = ur
-00005c00: 6c6c 6962 2e70 6172 7365 2e71 756f 7465  llib.parse.quote
-00005c10: 2875 6e71 756f 7465 6429 0a23 2070 7269  (unquoted).# pri
-00005c20: 6e74 2875 6e71 756f 7465 6429 0a23 2070  nt(unquoted).# p
-00005c30: 7269 6e74 2871 756f 7465 6429 0a0a 2320  rint(quoted)..# 
-00005c40: 6765 744f 626a 6563 744d 6574 6128 2774  getObjectMeta('t
-00005c50: 6573 742d 6275 636b 6574 272c 2027 6172  est-bucket', 'ar
-00005c60: 7469 636c 652e 7478 7427 290a 2320 6b65  ticle.txt').# ke
-00005c70: 7920 3d20 636f 7079 2827 6172 7469 636c  y = copy('articl
-00005c80: 652e 7478 7427 2c20 2761 7274 6963 6c65  e.txt', 'article
-00005c90: 2e74 7874 272c 2064 7374 5f62 7563 6b65  .txt', dst_bucke
-00005ca0: 745f 6e61 6d65 3d27 7465 7374 2d62 7563  t_name='test-buc
-00005cb0: 6b65 7427 290a 2320 7072 696e 7428 2761  ket').# print('a
-00005cc0: 6674 6572 2063 6f70 795c 6e5c 6e27 290a  fter copy\n\n').
-00005cd0: 2320 6765 744f 626a 6563 744d 6574 6128  # getObjectMeta(
-00005ce0: 2774 6573 742d 6275 636b 6574 272c 2027  'test-bucket', '
-00005cf0: 6172 7469 636c 652e 7478 7427 290a 2320  article.txt').# 
-00005d00: 6765 744f 626a 6563 744d 6574 6128 2774  getObjectMeta('t
-00005d10: 6573 742d 6275 636b 6574 272c 2027 4453  est-bucket', 'DS
-00005d20: 4330 3333 3830 2e73 7365 632e 6a70 6727  C03380.ssec.jpg'
-00005d30: 290a 2320 7570 6c6f 6164 4f62 6a65 6374  ).# uploadObject
-00005d40: 4672 6f6d 4669 6c65 2827 4453 4330 3333  FromFile('DSC033
-00005d50: 3830 2e65 6e63 7279 7074 2e6a 7067 2729  80.encrypt.jpg')
-00005d60: 0a0a 2320 696d 706f 7274 2062 6173 6536  ..# import base6
-00005d70: 340a 2320 696d 706f 7274 2068 6d61 630a  4.# import hmac.
-00005d80: 2320 696d 706f 7274 2068 6173 686c 6962  # import hashlib
-00005d90: 0a23 2069 6d70 6f72 7420 7572 6c6c 6962  .# import urllib
-00005da0: 0a23 2068 203d 2068 6d61 632e 6e65 7728  .# h = hmac.new(
-00005db0: 2261 6363 6573 736b 6579 222c 0a23 2020  "accesskey",.#  
-00005dc0: 2020 2020 2020 2020 2020 2020 2247 4554              "GET
-00005dd0: 5c6e 5c6e 5c6e 3131 3431 3838 3931 3230  \n\n\n1141889120
-00005de0: 5c6e 2f65 7861 6d70 6c65 6275 636b 6574  \n/examplebucket
-00005df0: 2f6f 7373 2d61 7069 2e70 6466 222c 0a23  /oss-api.pdf",.#
-00005e00: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-00005e10: 7368 6c69 622e 7368 6131 290a 2320 7572  shlib.sha1).# ur
-00005e20: 6c6c 6962 2e71 756f 7465 2028 6261 7365  llib.quote (base
-00005e30: 3634 2e65 6e63 6f64 6573 7472 696e 6728  64.encodestring(
-00005e40: 682e 6469 6765 7374 2829 292e 7374 7269  h.digest()).stri
-00005e50: 7028 2929 0a0a 2320 6220 3d20 636f 6e6e  p())..# b = conn
-00005e60: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
-00005e70: 6574 5f6e 616d 6529 0a23 2023 2066 6f72  et_name).# # for
-00005e80: 2070 2069 6e20 622e 6765 745f 616c 6c5f   p in b.get_all_
-00005e90: 6d75 6c74 6970 6172 745f 7570 6c6f 6164  multipart_upload
-00005ea0: 7328 6b65 795f 6d61 726b 6572 3d27 7465  s(key_marker='te
-00005eb0: 7374 2d6d 756c 7469 272c 2075 706c 6f61  st-multi', uploa
-00005ec0: 645f 6964 5f6d 6172 6b65 723d 2762 6266  d_id_marker='bbf
-00005ed0: 6366 3062 6162 3565 3834 3564 3839 3564  cf0bab5e845d895d
-00005ee0: 3063 6663 6432 3633 3262 6631 3827 293a  0cfcd2632bf18'):
-00005ef0: 2020 2020 2737 6536 6237 6237 3931 3264      '7e6b7b7912d
-00005f00: 3134 6562 3039 3432 3431 3366 3236 3263  14eb0942413f262c
-00005f10: 3438 3865 6327 0a23 2061 6c6c 5f75 706c  488ec'.# all_upl
-00005f20: 6f61 6473 203d 2062 2e67 6574 5f61 6c6c  oads = b.get_all
-00005f30: 5f6d 756c 7469 7061 7274 5f75 706c 6f61  _multipart_uploa
-00005f40: 6473 286b 6579 5f6d 6172 6b65 723d 2744  ds(key_marker='D
-00005f50: 5343 3033 3338 302e 656e 6372 7970 742e  SC03380.encrypt.
-00005f60: 6a70 672d 6464 6464 6464 6464 2729 236d  jpg-dddddddd')#m
-00005f70: 6178 5f75 706c 6f61 6473 3d32 3729 0a23  ax_uploads=27).#
-00005f80: 2070 7269 6e74 286c 656e 2861 6c6c 5f75   print(len(all_u
-00005f90: 706c 6f61 6473 2929 0a23 2066 6f72 2070  ploads)).# for p
-00005fa0: 2069 6e20 616c 6c5f 7570 6c6f 6164 733a   in all_uploads:
-00005fb0: 0a23 2020 2070 7269 6e74 2870 2c20 702e  .#   print(p, p.
-00005fc0: 6964 290a 2320 7075 745f 6f62 6a65 6374  id).# put_object
-00005fd0: 5f63 616c 6c62 6163 6b28 2774 6573 742d  _callback('test-
-00005fe0: 6361 6c6c 6261 636b 2729                 callback')
+00004030: 622e 636f 7079 5f6b 6579 2864 7374 4b65  b.copy_key(dstKe
+00004040: 792c 2062 7563 6b65 745f 6e61 6d65 2c20  y, bucket_name, 
+00004050: 7372 634b 6579 2c20 656e 6372 7970 745f  srcKey, encrypt_
+00004060: 6b65 793d 656e 6372 7970 745f 6b65 7929  key=encrypt_key)
+00004070: 0a0a 6465 6620 6c69 7374 5f6f 626a 6563  ..def list_objec
+00004080: 7473 2829 3a0a 2020 6275 636b 6574 203d  ts():.  bucket =
+00004090: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+000040a0: 2827 7465 7374 2d62 7563 6b65 7427 290a  ('test-bucket').
+000040b0: 2020 6b65 7973 203d 2062 7563 6b65 742e    keys = bucket.
+000040c0: 6c69 7374 2870 7265 6669 783d 2731 3627  list(prefix='16'
+000040d0: 290a 2020 7265 7331 203d 205b 6b2e 6e61  ).  res1 = [k.na
+000040e0: 6d65 2066 6f72 206b 2069 6e20 6b65 7973  me for k in keys
+000040f0: 5d0a 2020 7072 696e 7428 2772 6573 3120  ].  print('res1 
+00004100: 3a20 272c 2072 6573 3129 0a0a 2020 6b65  : ', res1)..  ke
+00004110: 7973 3220 3d20 6275 636b 6574 2e6c 6973  ys2 = bucket.lis
+00004120: 744f 626a 6563 7473 2870 7265 6669 783d  tObjects(prefix=
+00004130: 2731 3627 290a 2020 2320 7265 7332 203d  '16').  # res2 =
+00004140: 205b 6b2e 6e61 6d65 2066 6f72 206b 2069   [k.name for k i
+00004150: 6e20 6b65 7973 325d 0a20 2070 7269 6e74  n keys2].  print
+00004160: 2827 6b65 7973 3220 3a20 272c 206b 6579  ('keys2 : ', key
+00004170: 7332 290a 2020 2320 666f 7220 6b20 696e  s2).  # for k in
+00004180: 206b 6579 733a 0a20 2023 2020 2070 7269   keys:.  #   pri
+00004190: 6e74 2827 6f62 6a65 6374 3a27 2c20 6b2e  nt('object:', k.
+000041a0: 6e61 6d65 290a 0a64 6566 206c 6973 745f  name)..def list_
+000041b0: 6f62 6a65 6374 735f 7632 2864 656c 696d  objects_v2(delim
+000041c0: 6974 6572 3d27 2327 2c20 7072 6566 6978  iter='#', prefix
+000041d0: 3d4e 6f6e 652c 206d 6178 5f6b 6579 733d  =None, max_keys=
+000041e0: 4e6f 6e65 2c20 6d61 726b 6572 3d4e 6f6e  None, marker=Non
+000041f0: 652c 2065 6e63 6f64 696e 675f 7479 7065  e, encoding_type
+00004200: 3d27 272c 2066 6574 6368 5f6f 776e 6572  ='', fetch_owner
+00004210: 3d54 7275 6529 3a0a 2020 6275 636b 6574  =True):.  bucket
+00004220: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+00004230: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00004240: 2020 6b65 7973 203d 2062 7563 6b65 742e    keys = bucket.
+00004250: 6c69 7374 5f76 3228 6465 6c69 6d69 7465  list_v2(delimite
+00004260: 723d 6465 6c69 6d69 7465 722c 2070 7265  r=delimiter, pre
+00004270: 6669 783d 7072 6566 6978 2c20 6d61 785f  fix=prefix, max_
+00004280: 6b65 7973 3d6d 6178 5f6b 6579 732c 206d  keys=max_keys, m
+00004290: 6172 6b65 723d 6d61 726b 6572 2c20 656e  arker=marker, en
+000042a0: 636f 6469 6e67 5f74 7970 653d 656e 636f  coding_type=enco
+000042b0: 6469 6e67 5f74 7970 652c 2066 6574 6368  ding_type, fetch
+000042c0: 5f6f 776e 6572 3d66 6574 6368 5f6f 776e  _owner=fetch_own
+000042d0: 6572 290a 2020 666f 7220 6b20 696e 206b  er).  for k in k
+000042e0: 6579 733a 0a20 2020 2070 7269 6e74 2827  eys:.    print('
+000042f0: 6f62 6a65 6374 3a27 2c20 6b2e 6e61 6d65  object:', k.name
+00004300: 290a 0a64 6566 206c 6973 744f 626a 6563  )..def listObjec
+00004310: 7473 4d6f 7265 2862 7563 6b65 745f 6e61  tsMore(bucket_na
+00004320: 6d65 2c20 6465 6c69 6d69 7465 723d 4e6f  me, delimiter=No
+00004330: 6e65 2c20 7072 6566 6978 3d4e 6f6e 652c  ne, prefix=None,
+00004340: 206d 6178 5f6b 6579 733d 4e6f 6e65 2c20   max_keys=None, 
+00004350: 6d61 726b 6572 3d4e 6f6e 6529 3a0a 2020  marker=None):.  
+00004360: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00004370: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00004380: 6e61 6d65 290a 2020 6b65 7973 203d 2062  name).  keys = b
+00004390: 7563 6b65 742e 6c69 7374 2864 656c 696d  ucket.list(delim
+000043a0: 6974 6572 3d64 656c 696d 6974 6572 2c20  iter=delimiter, 
+000043b0: 7072 6566 6978 3d70 7265 6669 782c 206d  prefix=prefix, m
+000043c0: 6178 5f6b 6579 733d 6d61 785f 6b65 7973  ax_keys=max_keys
+000043d0: 2c20 6d61 726b 6572 3d6d 6172 6b65 7229  , marker=marker)
+000043e0: 0a20 2023 2070 7269 6e74 286c 656e 286b  .  # print(len(k
+000043f0: 6579 7329 290a 2020 7265 7320 3d20 5b6b  eys)).  res = [k
+00004400: 2e6e 616d 6520 666f 7220 6b20 696e 206b  .name for k in k
+00004410: 6579 735d 0a20 2070 7269 6e74 2827 7265  eys].  print('re
+00004420: 733a 2027 2c20 7265 7329 0a20 2023 2070  s: ', res).  # p
+00004430: 7269 6e74 2827 6974 656d 3a27 2c20 6b2e  rint('item:', k.
+00004440: 6e61 6d65 2c20 7479 7065 286b 2929 0a0a  name, type(k))..
+00004450: 6465 6620 6c69 7374 416e 6444 656c 6574  def listAndDelet
+00004460: 6528 293a 0a20 2062 7563 6b65 7420 3d20  e():.  bucket = 
+00004470: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+00004480: 6275 636b 6574 5f6e 616d 6529 0a20 206b  bucket_name).  k
+00004490: 6579 7320 3d20 6275 636b 6574 2e6c 6973  eys = bucket.lis
+000044a0: 7428 6465 6c69 6d69 7465 723d 272f 272c  t(delimiter='/',
+000044b0: 206d 6178 5f6b 6579 733d 3130 2c20 7072   max_keys=10, pr
+000044c0: 6566 6978 3d27 3135 2729 0a20 2070 7269  efix='15').  pri
+000044d0: 6e74 286b 6579 732e 6d61 726b 6572 290a  nt(keys.marker).
+000044e0: 2020 666f 7220 6b20 696e 206b 6579 733a    for k in keys:
+000044f0: 0a20 2020 2070 7269 6e74 2827 6f62 6a65  .    print('obje
+00004500: 6374 3a27 2c20 6b2e 6e61 6d65 290a 2020  ct:', k.name).  
+00004510: 2020 6465 6c65 7465 4f62 6a65 6374 286b    deleteObject(k
+00004520: 2e6e 616d 6529 0a0a 6465 6620 6c69 7374  .name)..def list
+00004530: 4f62 6a65 6374 7341 6e64 4669 6c74 6572  ObjectsAndFilter
+00004540: 2865 6e64 5469 6d65 3d4e 6f6e 6529 3a0a  (endTime=None):.
+00004550: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00004560: 6765 745f 6275 636b 6574 2827 6175 746f  get_bucket('auto
+00004570: 2d74 6573 742d 6275 636b 6574 2729 0a20  -test-bucket'). 
+00004580: 206b 6579 7320 3d20 6275 636b 6574 2e6c   keys = bucket.l
+00004590: 6973 744f 626a 6563 7473 2864 656c 696d  istObjects(delim
+000045a0: 6974 6572 3d27 2f27 2c20 6d61 785f 6b65  iter='/', max_ke
+000045b0: 7973 3d32 2920 2320 7374 6172 745f 7469  ys=2) # start_ti
+000045c0: 6d65 3d31 3634 3033 3331 3434 362c 2065  me=1640331446, e
+000045d0: 6e64 5f74 696d 653d 3136 3431 3839 3530  nd_time=16418950
+000045e0: 3936 0a20 2066 6f72 206b 2069 6e20 6b65  96.  for k in ke
+000045f0: 7973 3a0a 2020 2020 7072 696e 7428 6b29  ys:.    print(k)
+00004600: 0a0a 6465 6620 6765 744f 626a 6563 7454  ..def getObjectT
+00004610: 6167 6769 6e67 2829 3a0a 2020 6275 636b  agging():.  buck
+00004620: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00004630: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00004640: 290a 2020 6b65 7920 3d20 6275 636b 6574  ).  key = bucket
+00004650: 2e67 6574 5f6b 6579 2827 7465 7374 5461  .get_key('testTa
+00004660: 6767 696e 6727 290a 2020 7461 6767 696e  gging').  taggin
+00004670: 6720 3d20 6b65 792e 6765 745f 6f62 6a65  g = key.get_obje
+00004680: 6374 5f74 6167 6769 6e67 2829 0a20 2070  ct_tagging().  p
+00004690: 7269 6e74 2874 6167 6769 6e67 2e74 6f5f  rint(tagging.to_
+000046a0: 786d 6c28 2929 0a0a 6465 6620 7365 744f  xml())..def setO
+000046b0: 626a 6563 7454 6167 6769 6e67 2829 3a0a  bjectTagging():.
+000046c0: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+000046d0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+000046e0: 745f 6e61 6d65 290a 2020 6b65 7920 3d20  t_name).  key = 
+000046f0: 6275 636b 6574 2e67 6574 5f6b 6579 2827  bucket.get_key('
+00004700: 7465 7374 5461 6767 696e 6727 290a 2020  testTagging').  
+00004710: 7461 6767 696e 6720 3d20 5b54 6167 2827  tagging = [Tag('
+00004720: 3027 292c 2054 6167 2827 3127 2c20 2731  0'), Tag('1', '1
+00004730: 2729 5d0a 2020 6b65 792e 7365 745f 6f62  ')].  key.set_ob
+00004740: 6a65 6374 5f74 6167 6769 6e67 2874 6167  ject_tagging(tag
+00004750: 6769 6e67 290a 0a64 6566 2064 656c 6574  ging)..def delet
+00004760: 654f 626a 6563 7454 6167 6769 6e67 2829  eObjectTagging()
+00004770: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
+00004780: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00004790: 6b65 745f 6e61 6d65 290a 2020 6b65 7920  ket_name).  key 
+000047a0: 3d20 6275 636b 6574 2e67 6574 5f6b 6579  = bucket.get_key
+000047b0: 2827 6865 6865 2729 0a20 206b 6579 2e64  ('hehe').  key.d
+000047c0: 656c 6574 655f 6f62 6a65 6374 5f74 6167  elete_object_tag
+000047d0: 6769 6e67 2829 0a0a 6465 6620 6361 6c63  ging()..def calc
+000047e0: 466f 6c64 6572 5369 7a65 2862 7563 6b65  FolderSize(bucke
+000047f0: 742c 2066 6f6c 6465 7229 3a0a 2020 6c65  t, folder):.  le
+00004800: 6e67 7468 203d 2030 0a20 206b 6579 7320  ngth = 0.  keys 
+00004810: 3d20 6275 636b 6574 2e6c 6973 7428 7072  = bucket.list(pr
+00004820: 6566 6978 3d66 6f6c 6465 7229 0a20 2066  efix=folder).  f
+00004830: 6f72 206b 2069 6e20 6b65 7973 3a0a 2020  or k in keys:.  
+00004840: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00004850: 6b2c 204b 6579 293a 0a20 2020 2020 206c  k, Key):.      l
+00004860: 656e 6774 6820 2b3d 206b 2e73 697a 650a  ength += k.size.
+00004870: 2020 7265 7475 726e 206c 656e 6774 680a    return length.
+00004880: 0a66 726f 6d20 6b73 332e 7072 6566 6978  .from ks3.prefix
+00004890: 2069 6d70 6f72 7420 5072 6566 6978 0a0a   import Prefix..
+000048a0: 2320 e588 97e4 b8be e68c 87e5 ae9a e79b  # ..............
+000048b0: aee5 bd95 e4b8 8be7 9a84 e696 87e4 bbb6  ................
+000048c0: e5a4 a7e5 b08f 0a64 6566 2067 6574 466f  .......def getFo
+000048d0: 6c64 6572 5369 7a65 496e 4275 636b 6574  lderSizeInBucket
+000048e0: 2829 3a0a 2020 6275 636b 6574 203d 2063  ():.  bucket = c
+000048f0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00004900: 7563 6b65 745f 6e61 6d65 290a 2020 6b65  ucket_name).  ke
+00004910: 7973 203d 2062 7563 6b65 742e 6c69 7374  ys = bucket.list
+00004920: 2864 656c 696d 6974 6572 3d27 2f27 290a  (delimiter='/').
+00004930: 2020 666f 7220 6b20 696e 206b 6579 733a    for k in keys:
+00004940: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00004950: 6365 286b 2c20 5072 6566 6978 293a 0a20  ce(k, Prefix):. 
+00004960: 2020 2020 2070 7269 6e74 2827 6469 723a       print('dir:
+00004970: 2027 202b 206b 2e6e 616d 6520 2b20 2720   ' + k.name + ' 
+00004980: 2073 697a 653a 2720 2b20 7374 7228 6361   size:' + str(ca
+00004990: 6c63 466f 6c64 6572 5369 7a65 2862 7563  lcFolderSize(buc
+000049a0: 6b65 742c 206b 2e6e 616d 6529 2920 2b20  ket, k.name)) + 
+000049b0: 2242 7974 6522 290a 0a0a 6465 6620 7465  "Byte")...def te
+000049c0: 7374 5f6d 756c 7469 7061 7274 5f75 706c  st_multipart_upl
+000049d0: 6f61 6428 656e 6372 7970 745f 6b65 793d  oad(encrypt_key=
+000049e0: 4e6f 6e65 293a 0a20 2069 6d70 6f72 7420  None):.  import 
+000049f0: 6d61 7468 2c20 6f73 0a20 2066 726f 6d20  math, os.  from 
+00004a00: 6669 6c65 6368 756e 6b69 6f20 696d 706f  filechunkio impo
+00004a10: 7274 2046 696c 6543 6875 6e6b 494f 0a20  rt FileChunkIO. 
+00004a20: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
+00004a30: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
+00004a40: 5f6e 616d 6529 0a0a 2020 736f 7572 6365  _name)..  source
+00004a50: 5f70 6174 6820 3d20 272f 5573 6572 732f  _path = '/Users/
+00004a60: 6a61 6262 6172 2f44 6f77 6e6c 6f61 6473  jabbar/Downloads
+00004a70: 2f44 5343 3033 3338 302e 4a50 4727 0a20  /DSC03380.JPG'. 
+00004a80: 2023 20e6 ba90 e696 87e4 bbb6 e5a4 a7e5   # .............
+00004a90: b08f 0a20 2073 6f75 7263 655f 7369 7a65  ...  source_size
+00004aa0: 203d 206f 732e 7374 6174 2873 6f75 7263   = os.stat(sourc
+00004ab0: 655f 7061 7468 292e 7374 5f73 697a 650a  e_path).st_size.
+00004ac0: 0a20 206d 7020 3d20 6275 636b 6574 2e69  .  mp = bucket.i
+00004ad0: 6e69 7469 6174 655f 6d75 6c74 6970 6172  nitiate_multipar
+00004ae0: 745f 7570 6c6f 6164 2822 4453 4330 3333  t_upload("DSC033
+00004af0: 3830 2e6d 702e 6a70 6722 2c20 656e 6372  80.mp.jpg", encr
+00004b00: 7970 745f 6b65 793d 656e 6372 7970 745f  ypt_key=encrypt_
+00004b10: 6b65 7929 0a20 2070 7269 6e74 286d 7029  key).  print(mp)
+00004b20: 0a0a 2020 6368 756e 6b5f 7369 7a65 203d  ..  chunk_size =
+00004b30: 2035 3234 3238 3830 0a20 2063 6875 6e6b   5242880.  chunk
+00004b40: 5f63 6f75 6e74 203d 2069 6e74 286d 6174  _count = int(mat
+00004b50: 682e 6365 696c 2873 6f75 7263 655f 7369  h.ceil(source_si
+00004b60: 7a65 202a 2031 2e30 202f 2063 6875 6e6b  ze * 1.0 / chunk
+00004b70: 5f73 697a 6520 2a20 312e 3029 290a 0a20  _size * 1.0)).. 
+00004b80: 2023 20e9 809a e8bf 8720 4669 6c65 4368   # ...... FileCh
+00004b90: 756e 6b49 4f20 e5b0 86e6 9687 e4bb b6e5  unkIO ..........
+00004ba0: 8886 e789 870a 2020 666f 7220 6920 696e  ......  for i in
+00004bb0: 2072 616e 6765 2863 6875 6e6b 5f63 6f75   range(chunk_cou
+00004bc0: 6e74 293a 0a20 2020 206f 6666 7365 7420  nt):.    offset 
+00004bd0: 3d20 6368 756e 6b5f 7369 7a65 202a 2069  = chunk_size * i
+00004be0: 0a20 2020 2062 7974 6573 203d 206d 696e  .    bytes = min
+00004bf0: 2863 6875 6e6b 5f73 697a 652c 2073 6f75  (chunk_size, sou
+00004c00: 7263 655f 7369 7a65 202d 206f 6666 7365  rce_size - offse
+00004c10: 7429 0a20 2020 2077 6974 6820 4669 6c65  t).    with File
+00004c20: 4368 756e 6b49 4f28 736f 7572 6365 5f70  ChunkIO(source_p
+00004c30: 6174 682c 2027 7227 2c20 6f66 6673 6574  ath, 'r', offset
+00004c40: 3d6f 6666 7365 742c 2062 7974 6573 3d62  =offset, bytes=b
+00004c50: 7974 6573 2920 6173 2066 703a 0a20 2020  ytes) as fp:.   
+00004c60: 2020 2023 20e9 8090 e4b8 aae4 b88a e4bc     # ...........
+00004c70: a0e5 8886 e789 870a 2020 2020 2020 6d70  ........      mp
+00004c80: 2e75 706c 6f61 645f 7061 7274 5f66 726f  .upload_part_fro
+00004c90: 6d5f 6669 6c65 2866 702c 2070 6172 745f  m_file(fp, part_
+00004ca0: 6e75 6d3d 6920 2b20 3129 0a20 2070 7269  num=i + 1).  pri
+00004cb0: 6e74 286d 702e 746f 5f78 6d6c 2829 290a  nt(mp.to_xml()).
+00004cc0: 2020 2320 e58f 91e9 8081 e8af b7e6 b182    # ............
+00004cd0: efbc 8ce5 9088 e5b9 b6e5 8886 e789 87ef  ................
+00004ce0: bc8c e5ae 8ce6 8890 e588 86e7 8987 e4b8  ................
+00004cf0: 8ae4 bca0 0a20 2072 6574 203d 206d 702e  .....  ret = mp.
+00004d00: 636f 6d70 6c65 7465 5f75 706c 6f61 6428  complete_upload(
+00004d10: 290a 2020 6966 2072 6574 2061 6e64 2072  ).  if ret and r
+00004d20: 6574 2e73 7461 7475 7320 3d3d 2032 3030  et.status == 200
+00004d30: 3a0a 2020 2020 7072 696e 7428 22e4 b88a  :.    print("...
+00004d40: e4bc a0e6 8890 e58a 9f22 290a 0a64 6566  .........")..def
+00004d50: 2074 6573 745f 6665 7463 685f 6f62 6a65   test_fetch_obje
+00004d60: 6374 2829 3a0a 2020 6275 636b 6574 203d  ct():.  bucket =
+00004d70: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00004d80: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00004d90: 6b65 7920 3d20 6275 636b 6574 2e6e 6577  key = bucket.new
+00004da0: 5f6b 6579 2827 7777 772d 6c6f 676f 2729  _key('www-logo')
+00004db0: 0a20 206b 6579 2e66 6574 6368 5f6f 626a  .  key.fetch_obj
+00004dc0: 6563 7428 736f 7572 6365 5f75 726c 3d27  ect(source_url='
+00004dd0: 6874 7470 3a2f 2f66 652e 6b73 7975 6e2e  http://fe.ksyun.
+00004de0: 636f 6d2f 7072 6f6a 6563 742f 7265 736f  com/project/reso
+00004df0: 7572 6365 2f69 6d67 2f77 7777 2d6c 6f67  urce/img/www-log
+00004e00: 6f2e 706e 6727 2c0a 2020 2020 2020 2020  o.png',.        
+00004e10: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00004e20: 6164 6572 733d 7b27 782d 6b73 732d 6163  aders={'x-kss-ac
+00004e30: 6c27 3a20 2770 7562 6c69 632d 7265 6164  l': 'public-read
+00004e40: 277d 290a 2020 7072 696e 7428 2766 6574  '}).  print('fet
+00004e50: 6368 e688 90e5 8a9f 2729 0a0a 6465 6620  ch......')..def 
+00004e60: 7465 7374 5f67 656e 6572 6174 655f 7572  test_generate_ur
+00004e70: 6c28 6b65 795f 6e61 6d65 2c20 696d 6167  l(key_name, imag
+00004e80: 655f 6174 7472 733d 4e6f 6e65 293a 0a20  e_attrs=None):. 
+00004e90: 2062 203d 2063 6f6e 6e2e 6765 745f 6275   b = conn.get_bu
+00004ea0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00004eb0: 290a 2020 6b20 3d20 622e 6765 745f 6b65  ).  k = b.get_ke
+00004ec0: 7928 6b65 795f 6e61 6d65 290a 2020 6966  y(key_name).  if
+00004ed0: 206b 3a0a 2020 2020 7572 6c20 3d20 6b2e   k:.    url = k.
+00004ee0: 6765 6e65 7261 7465 5f75 726c 2836 3030  generate_url(600
+00004ef0: 2c20 696d 6167 655f 6174 7472 733d 696d  , image_attrs=im
+00004f00: 6167 655f 6174 7472 7329 2020 2320 3630  age_attrs)  # 60
+00004f10: 7320 e590 8ee8 afa5 e993 bee6 8ea5 e8bf  s ..............
+00004f20: 87e6 9c9f 0a20 2020 2070 7269 6e74 2875  .....    print(u
+00004f30: 726c 290a 2020 656c 7365 3a0a 2020 2020  rl).  else:.    
+00004f40: 7072 696e 7428 276f 626a 6563 7420 6e6f  print('object no
+00004f50: 7420 666f 756e 6427 290a 0a64 6566 2074  t found')..def t
+00004f60: 6573 745f 6765 745f 7072 6573 6967 6e65  est_get_presigne
+00004f70: 645f 7572 6c28 6b65 795f 6e61 6d65 293a  d_url(key_name):
+00004f80: 0a20 2062 203d 2063 6f6e 6e2e 6765 745f  .  b = conn.get_
+00004f90: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
+00004fa0: 6d65 290a 2020 2320 e696 b0e5 bbba e5af  me).  # ........
+00004fb0: b9e8 b1a1 6b65 790a 2020 6b20 3d20 622e  ....key.  k = b.
+00004fc0: 6e65 775f 6b65 7928 6b65 795f 6e61 6d65  new_key(key_name
+00004fd0: 290a 2020 6966 206b 3a0a 2020 2020 7572  ).  if k:.    ur
+00004fe0: 6c20 3d20 6b2e 6765 745f 7072 6573 6967  l = k.get_presig
+00004ff0: 6e65 645f 7572 6c28 3630 3030 3029 2020  ned_url(60000)  
+00005000: 2320 3630 7320 e590 8ee8 afa5 e993 bee6  # 60s ..........
+00005010: 8ea5 e8bf 87e6 9c9f 0a20 2020 2070 7269  .........    pri
+00005020: 6e74 2875 726c 290a 2020 2020 7265 7475  nt(url).    retu
+00005030: 726e 2075 726c 0a0a 6465 6620 7265 7374  rn url..def rest
+00005040: 6f72 654f 626a 6563 7428 6b65 795f 6e61  oreObject(key_na
+00005050: 6d65 293a 0a20 2062 203d 2063 6f6e 6e2e  me):.  b = conn.
+00005060: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00005070: 745f 6e61 6d65 290a 2020 6b20 3d20 622e  t_name).  k = b.
+00005080: 6765 745f 6b65 7928 6b65 795f 6e61 6d65  get_key(key_name
+00005090: 290a 2020 6b2e 7265 7374 6f72 655f 6f62  ).  k.restore_ob
+000050a0: 6a65 6374 2829 0a0a 6465 6620 7465 7374  ject()..def test
+000050b0: 5f70 7574 5f76 6961 5f70 7265 7369 676e  _put_via_presign
+000050c0: 6564 5f75 726c 286b 6579 293a 0a20 2075  ed_url(key):.  u
+000050d0: 726c 203d 2074 6573 745f 6765 745f 7072  rl = test_get_pr
+000050e0: 6573 6967 6e65 645f 7572 6c28 6b65 7929  esigned_url(key)
+000050f0: 0a20 2077 6974 6820 6f70 656e 2827 2e2f  .  with open('./
+00005100: 6172 7469 636c 652e 7478 7427 2c20 2772  article.txt', 'r
+00005110: 6227 2920 6173 2066 703a 0a20 2020 2072  b') as fp:.    r
+00005120: 6573 756c 7420 3d20 7265 7175 6573 7473  esult = requests
+00005130: 2e70 7574 2875 726c 2c20 6461 7461 3d66  .put(url, data=f
+00005140: 7029 0a20 2020 2070 7269 6e74 2872 6573  p).    print(res
+00005150: 756c 7429 0a0a 6672 6f6d 206b 7333 2e73  ult)..from ks3.s
+00005160: 7473 2069 6d70 6f72 7420 6173 7375 6d65  ts import assume
+00005170: 526f 6c65 0a64 6566 2074 6573 745f 6173  Role.def test_as
+00005180: 7375 6d65 526f 6c65 2829 3a0a 2020 7072  sumeRole():.  pr
+00005190: 696e 7428 6173 7375 6d65 526f 6c65 2861  int(assumeRole(a
+000051a0: 6b2c 2073 6b2c 2022 6b72 6e3a 6b73 633a  k, sk, "krn:ksc:
+000051b0: 6961 6d3a 3a78 7878 3a72 6f6c 652f 7878  iam::xxx:role/xx
+000051c0: 2d74 6573 742d 6275 636b 6574 222c 2022  -test-bucket", "
+000051d0: 6b73 3322 2c20 3336 3030 2929 0a0a 0a64  ks3", 3600))...d
+000051e0: 6566 2070 7574 5f6f 626a 6563 745f 6361  ef put_object_ca
+000051f0: 6c6c 6261 636b 286b 6579 5f6e 616d 6529  llback(key_name)
+00005200: 3a0a 2020 6220 3d20 636f 6e6e 2e67 6574  :.  b = conn.get
+00005210: 5f62 7563 6b65 7428 2768 616e 6a69 6e67  _bucket('hanjing
+00005220: 2d74 6573 7430 3030 2729 0a20 2023 20e6  -test000').  # .
+00005230: 96b0 e5bb bae5 afb9 e8b1 a16b 6579 0a20  ...........key. 
+00005240: 206b 203d 2062 2e6e 6577 5f6b 6579 286b   k = b.new_key(k
+00005250: 6579 5f6e 616d 6529 0a20 2023 20e4 b88a  ey_name).  # ...
+00005260: e4bc a0e6 8890 e58a 9fe5 908e efbc 8ce5  ................
+00005270: 9091 e59b 9ee8 b083 e59c b0e5 9d80 504f  ..............PO
+00005280: 5354 e695 b0e6 8dae 0a20 2023 20e9 9c80  ST.......  # ...
+00005290: e8a6 81e8 aebe e7bd ae60 782d 6b73 732d  .........`x-kss-
+000052a0: 6361 6c6c 6261 636b 7572 6c60 e592 8c60  callbackurl`...`
+000052b0: 782d 6b73 732d 6361 6c6c 6261 636b 626f  x-kss-callbackbo
+000052c0: 6479 60e8 afb7 e6b1 82e5 a4b4 efbc 8ce8  dy`.............
+000052d0: afa6 e8a7 81e6 9687 e6a1 a35b e4b8 8ae4  ...........[....
+000052e0: bca0 e59b 9ee8 b083 e5a4 84e7 9086 5d28  ..............](
+000052f0: 6874 7470 733a 2f2f 646f 6373 2e6b 7379  https://docs.ksy
+00005300: 756e 2e63 6f6d 2f64 6f63 756d 656e 7473  un.com/documents
+00005310: 2f39 3536 29e3 8082 0a20 2023 2078 2d6b  /956)....  # x-k
+00005320: 7373 2d63 616c 6c62 6163 6b75 726c 20e4  ss-callbackurl .
+00005330: b8ba e58f 91e8 b5b7 e59b 9ee8 b083 e697  ................
+00005340: b6e8 afb7 e6b1 82e7 9a84 e69c 8de5 8aa1  ................
+00005350: e599 a8e5 9cb0 e59d 800a 2020 2320 782d  ..........  # x-
+00005360: 6b73 732d 6361 6c6c 6261 636b 626f 6479  kss-callbackbody
+00005370: 20e4 b8ba e58f 91e8 b5b7 e59b 9ee8 b083   ...............
+00005380: e697 b6e8 afb7 e6b1 82e7 9a84 626f 6479  ............body
+00005390: e79a 84e5 80bc 0a20 2068 6561 6465 7273  .......  headers
+000053a0: 203d 207b 2278 2d6b 7373 2d63 616c 6c62   = {"x-kss-callb
+000053b0: 6163 6b75 726c 223a 2022 6874 7470 733a  ackurl": "https:
+000053c0: 2f2f 7968 2d73 682e 6b73 332d 636e 2d73  //yh-sh.ks3-cn-s
+000053d0: 6861 6e67 6861 692e 6b73 7975 6e63 732e  hanghai.ksyuncs.
+000053e0: 636f 6d22 2c20 2278 2d6b 7373 2d63 616c  com", "x-kss-cal
+000053f0: 6c62 6163 6b62 6f64 7922 3a20 226f 626a  lbackbody": "obj
+00005400: 6563 744b 6579 3d24 7b6b 6579 7d26 6574  ectKey=${key}&et
+00005410: 6167 3d24 7b65 7461 677d 2662 7563 6b65  ag=${etag}&bucke
+00005420: 743d 247b 6275 636b 6574 7d26 6f62 6a65  t=${bucket}&obje
+00005430: 6374 5369 7a65 3d24 7b6f 626a 6563 7453  ctSize=${objectS
+00005440: 697a 657d 266d 696d 6554 7970 653d 247b  ize}&mimeType=${
+00005450: 6d69 6d65 5479 7065 7d26 6372 6561 7465  mimeType}&create
+00005460: 5469 6d65 3d24 7b63 7265 6174 6554 696d  Time=${createTim
+00005470: 657d 222c 2022 782d 6b73 732d 6361 6c6c  e}", "x-kss-call
+00005480: 6261 636b 6175 7468 223a 317d 0a20 2072  backauth":1}.  r
+00005490: 6574 203d 206b 2e73 6574 5f63 6f6e 7465  et = k.set_conte
+000054a0: 6e74 735f 6672 6f6d 5f73 7472 696e 6728  nts_from_string(
+000054b0: 2274 6573 742d 6361 6c6c 6261 636b 222c  "test-callback",
+000054c0: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
+000054d0: 290a 2020 6966 2072 6574 2061 6e64 2072  ).  if ret and r
+000054e0: 6574 2e73 7461 7475 7320 3d3d 2032 3030  et.status == 200
+000054f0: 3a0a 2020 2020 7072 696e 7428 22e4 b88a  :.    print("...
+00005500: e4bc a0e6 8890 e58a 9f22 290a 0a23 2067  .........")..# g
+00005510: 6574 416c 6c42 7563 6b65 7473 2829 0a23  etAllBuckets().#
+00005520: 2068 6561 6442 7563 6b65 7428 2762 6a27   headBucket('bj'
+00005530: 290a 2320 6765 7442 7563 6b65 744c 6f63  ).# getBucketLoc
+00005540: 6174 696f 6e28 2774 6573 742d 686f 7374  ation('test-host
+00005550: 2d73 7479 6c65 2729 0a23 2063 7265 6174  -style').# creat
+00005560: 6542 7563 6b65 7428 2774 6573 742d 6275  eBucket('test-bu
+00005570: 636b 6574 2d61 7263 6869 7665 2d74 6573  cket-archive-tes
+00005580: 742d 7368 616e 6768 6169 3227 2c20 6c6f  t-shanghai2', lo
+00005590: 6361 7469 6f6e 3d27 5348 414e 4748 4149  cation='SHANGHAI
+000055a0: 2729 0a23 2064 656c 6574 6542 7563 6b65  ').# deleteBucke
+000055b0: 7428 2774 6573 742d 6275 636b 6574 2729  t('test-bucket')
+000055c0: 0a23 2067 6574 4275 636b 6574 4163 6c28  .# getBucketAcl(
+000055d0: 2774 6573 742d 6275 636b 6574 2729 0a23  'test-bucket').#
+000055e0: 2073 6574 4275 636b 6574 4163 6c28 2774   setBucketAcl('t
+000055f0: 6573 742d 6275 636b 6574 2729 0a23 206d  est-bucket').# m
+00005600: 616e 6167 6542 7563 6b65 7452 6570 6c69  anageBucketRepli
+00005610: 6361 7469 6f6e 2827 7465 7374 2d62 7563  cation('test-buc
+00005620: 6b65 7427 290a 2320 6765 7442 7563 6b65  ket').# getBucke
+00005630: 744c 6966 6543 7963 6c65 2862 7563 6b65  tLifeCycle(bucke
+00005640: 745f 6e61 6d65 290a 2320 7365 7442 7563  t_name).# setBuc
+00005650: 6b65 744c 6966 6543 7963 6c65 2862 7563  ketLifeCycle(buc
+00005660: 6b65 745f 6e61 6d65 290a 2320 7365 7442  ket_name).# setB
+00005670: 7563 6b65 744c 6966 6543 7963 6c65 3228  ucketLifeCycle2(
+00005680: 6275 636b 6574 5f6e 616d 6529 0a23 2064  bucket_name).# d
+00005690: 656c 6574 6542 7563 6b65 744c 6966 6543  eleteBucketLifeC
+000056a0: 7963 6c65 2862 7563 6b65 745f 6e61 6d65  ycle(bucket_name
+000056b0: 290a 2320 6765 7442 7563 6b65 744c 6f67  ).# getBucketLog
+000056c0: 6769 6e67 2862 7563 6b65 745f 6e61 6d65  ging(bucket_name
+000056d0: 290a 2320 7365 7442 7563 6b65 744c 6f67  ).# setBucketLog
+000056e0: 6769 6e67 2862 7563 6b65 745f 6e61 6d65  ging(bucket_name
+000056f0: 290a 2320 6469 7361 626c 6542 7563 6b65  ).# disableBucke
+00005700: 744c 6f67 6769 6e67 2862 7563 6b65 745f  tLogging(bucket_
+00005710: 6e61 6d65 290a 2320 656e 6162 6c65 4275  name).# enableBu
+00005720: 636b 6574 4c6f 6767 696e 6728 6275 636b  cketLogging(buck
+00005730: 6574 5f6e 616d 6529 0a23 2070 7574 4275  et_name).# putBu
+00005740: 636b 6574 436f 7273 2862 7563 6b65 745f  cketCors(bucket_
+00005750: 6e61 6d65 290a 2320 6765 7442 7563 6b65  name).# getBucke
+00005760: 7443 6f72 7328 6275 636b 6574 5f6e 616d  tCors(bucket_nam
+00005770: 6529 0a23 2064 656c 6574 6542 7563 6b65  e).# deleteBucke
+00005780: 7443 6f72 7328 6275 636b 6574 5f6e 616d  tCors(bucket_nam
+00005790: 6529 0a23 2064 656c 6574 6542 7563 6b65  e).# deleteBucke
+000057a0: 7443 7272 2862 7563 6b65 745f 6e61 6d65  tCrr(bucket_name
+000057b0: 290a 2320 6765 7442 7563 6b65 7443 7272  ).# getBucketCrr
+000057c0: 2862 7563 6b65 745f 6e61 6d65 290a 2320  (bucket_name).# 
+000057d0: 7365 7442 7563 6b65 7443 7272 2862 7563  setBucketCrr(buc
+000057e0: 6b65 745f 6e61 6d65 290a 2320 7365 7442  ket_name).# setB
+000057f0: 7563 6b65 744d 6972 726f 7228 6275 636b  ucketMirror(buck
+00005800: 6574 5f6e 616d 6529 0a23 2064 656c 6574  et_name).# delet
+00005810: 6542 7563 6b65 744d 6972 726f 7228 6275  eBucketMirror(bu
+00005820: 636b 6574 5f6e 616d 6529 0a23 2067 6574  cket_name).# get
+00005830: 4275 636b 6574 4d69 7272 6f72 2862 7563  BucketMirror(buc
+00005840: 6b65 745f 6e61 6d65 290a 2323 2323 2320  ket_name).##### 
+00005850: 6f62 6a65 6374 2023 2323 2323 0a23 2067  object #####.# g
+00005860: 6574 4f62 6a65 6374 4d65 7461 2862 7563  etObjectMeta(buc
+00005870: 6b65 745f 6e61 6d65 2c20 2761 7274 6963  ket_name, 'artic
+00005880: 6c65 2e74 7874 2729 0a23 206c 6973 745f  le.txt').# list_
+00005890: 6f62 6a65 6374 7328 290a 2320 6c69 7374  objects().# list
+000058a0: 4f62 6a65 6374 734d 6f72 6528 2261 7574  ObjectsMore("aut
+000058b0: 6f2d 7465 7374 2d62 7563 6b65 7422 2c20  o-test-bucket", 
+000058c0: 6465 6c69 6d69 7465 723d 272f 272c 206d  delimiter='/', m
+000058d0: 6178 5f6b 6579 733d 322c 206d 6172 6b65  ax_keys=2, marke
+000058e0: 723d 2731 3035 3027 290a 2320 6c69 7374  r='1050').# list
+000058f0: 4f62 6a65 6374 734d 6f72 6528 2261 7574  ObjectsMore("aut
+00005900: 6f2d 7465 7374 2d62 7563 6b65 7422 2c20  o-test-bucket", 
+00005910: 6465 6c69 6d69 7465 723d 272f 272c 206d  delimiter='/', m
+00005920: 6178 5f6b 6579 733d 322c 206d 6172 6b65  ax_keys=2, marke
+00005930: 723d 2731 3035 2f27 290a 2320 6c69 7374  r='105/').# list
+00005940: 4f62 6a65 6374 734d 6f72 6528 2261 7574  ObjectsMore("aut
+00005950: 6f2d 7465 7374 2d62 7563 6b65 7422 2c20  o-test-bucket", 
+00005960: 6465 6c69 6d69 7465 723d 272f 272c 206d  delimiter='/', m
+00005970: 6178 5f6b 6579 733d 322c 206d 6172 6b65  ax_keys=2, marke
+00005980: 723d 2731 3035 2532 4627 290a 2320 6c69  r='105%2F').# li
+00005990: 7374 4f62 6a65 6374 7341 6e64 4669 6c74  stObjectsAndFilt
+000059a0: 6572 2829 0a23 2073 6574 4f62 6a65 6374  er().# setObject
+000059b0: 5461 6767 696e 6728 290a 2320 6765 744f  Tagging().# getO
+000059c0: 626a 6563 7454 6167 6769 6e67 2829 0a23  bjectTagging().#
+000059d0: 2064 656c 6574 654f 626a 6563 7454 6167   deleteObjectTag
+000059e0: 6769 6e67 2829 0a23 2067 6574 466f 6c64  ging().# getFold
+000059f0: 6572 5369 7a65 496e 4275 636b 6574 2829  erSizeInBucket()
+00005a00: 3b0a 2320 646f 776e 6c6f 6164 4f62 6a65  ;.# downloadObje
+00005a10: 6374 416e 6450 7269 6e74 2829 0a23 2064  ctAndPrint().# d
+00005a20: 6f77 6e6c 6f61 644f 626a 6563 7441 7353  ownloadObjectAsS
+00005a30: 7472 6561 6d41 6e64 5072 696e 7428 290a  treamAndPrint().
+00005a40: 2320 646f 776e 6c6f 6164 4f62 6a65 6374  # downloadObject
+00005a50: 416e 6453 6176 6528 6275 636b 6574 5f6e  AndSave(bucket_n
+00005a60: 616d 652c 2027 4453 4330 3333 3830 2e65  ame, 'DSC03380.e
+00005a70: 6e63 7279 7074 2ee9 9d9e e588 86e5 9d97  ncrypt..........
+00005a80: 2e6a 7067 272c 2068 6561 6465 7273 3d7b  .jpg', headers={
+00005a90: 0a23 2020 2027 7261 6e67 6527 3a20 2762  .#   'range': 'b
+00005aa0: 7974 6573 3d30 2d35 3234 3238 3830 270a  ytes=0-5242880'.
+00005ab0: 2320 7d29 0a23 2063 6f75 6e74 203d 2032  # }).# count = 2
+00005ac0: 300a 2320 7768 696c 6520 5472 7565 3a0a  0.# while True:.
+00005ad0: 2320 7570 6c6f 6164 4f62 6a65 6374 4672  # uploadObjectFr
+00005ae0: 6f6d 4669 6c65 2827 e6b3 95e6 b2bb 2e6a  omFile('.......j
+00005af0: 7065 6727 290a 7570 6c6f 6164 5f61 7379  peg').upload_asy
+00005b00: 6e63 2827 e6b3 95e6 b2bb 2e6a 7065 6727  nc('.......jpeg'
+00005b10: 290a 646f 776e 6c6f 6164 5f61 7379 6e63  ).download_async
+00005b20: 2827 3136 3539 3638 3438 3732 2e74 6f72  ('1659684872.tor
+00005b30: 7265 6e74 2729 0a23 2075 706c 6f61 644f  rent').# uploadO
+00005b40: 626a 6563 7446 726f 6d46 696c 6528 2778  bjectFromFile('x
+00005b50: 6162 2729 0a23 2075 706c 6f61 644f 626a  ab').# uploadObj
+00005b60: 6563 7446 726f 6d46 696c 6528 2778 6163  ectFromFile('xac
+00005b70: 2729 0a23 2020 2074 696d 652e 736c 6565  ').#   time.slee
+00005b80: 7028 3529 0a23 2020 2063 6f75 6e74 203d  p(5).#   count =
+00005b90: 2063 6f75 6e74 202d 2031 0a23 2075 706c   count - 1.# upl
+00005ba0: 6f61 644f 626a 6563 7446 726f 6d53 7472  oadObjectFromStr
+00005bb0: 696e 6728 290a 2320 6865 6164 4f62 6a65  ing().# headObje
+00005bc0: 6374 2829 0a23 2064 6f77 6e6c 6f61 644f  ct().# downloadO
+00005bd0: 626a 6563 7441 6e64 5072 696e 7428 2774  bjectAndPrint('t
+00005be0: 6573 745f 6469 7265 6374 6f72 792f 2729  est_directory/')
+00005bf0: 0a23 2064 656c 6574 654f 626a 6563 7428  .# deleteObject(
+00005c00: 2274 656c 6c6d 6577 6879 2229 0a23 2067  "tellmewhy").# g
+00005c10: 6574 4f62 6a65 6374 4163 6c28 290a 0a23  etObjectAcl()..#
+00005c20: 2074 6573 745f 6d75 6c74 6970 6172 745f   test_multipart_
+00005c30: 7570 6c6f 6164 2865 6e63 7279 7074 5f6b  upload(encrypt_k
+00005c40: 6579 3d54 7275 6529 0a0a 2320 7465 7374  ey=True)..# test
+00005c50: 5f66 6574 6368 5f6f 626a 6563 7428 290a  _fetch_object().
+00005c60: 2320 6465 6620 7465 7374 5f67 656e 6572  # def test_gener
+00005c70: 6174 655f 7572 6c28 6b65 795f 6e61 6d65  ate_url(key_name
+00005c80: 2c20 696d 6167 655f 6174 7472 733d 4e6f  , image_attrs=No
+00005c90: 6e65 293a 0a23 2020 2062 203d 2063 6f6e  ne):.#   b = con
+00005ca0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00005cb0: 6b65 745f 6e61 6d65 290a 2320 2020 6b20  ket_name).#   k 
+00005cc0: 3d20 622e 6765 745f 6b65 7928 6b65 795f  = b.get_key(key_
+00005cd0: 6e61 6d65 290a 2320 2020 6966 206b 3a0a  name).#   if k:.
+00005ce0: 2320 2020 2020 7572 6c20 3d20 6b2e 6765  #     url = k.ge
+00005cf0: 6e65 7261 7465 5f75 726c 2836 3030 2c20  nerate_url(600, 
+00005d00: 696d 6167 655f 6174 7472 733d 696d 6167  image_attrs=imag
+00005d10: 655f 6174 7472 7329 2020 2320 3630 7320  e_attrs)  # 60s 
+00005d20: e590 8ee8 afa5 e993 bee6 8ea5 e8bf 87e6  ................
+00005d30: 9c9f 0a23 2020 2020 2070 7269 6e74 2875  ...#     print(u
+00005d40: 726c 290a 2320 2020 656c 7365 3a0a 2320  rl).#   else:.# 
+00005d50: 2020 2020 7072 696e 7428 276f 626a 6563      print('objec
+00005d60: 7420 6e6f 7420 666f 756e 6427 290a 0a23  t not found')..#
+00005d70: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
+00005d80: 6574 5f62 7563 6b65 7428 2774 6573 742d  et_bucket('test-
+00005d90: 6275 636b 6574 2729 0a23 206b 6579 7320  bucket').# keys 
+00005da0: 3d20 6275 636b 6574 2e6c 6973 7428 290a  = bucket.list().
+00005db0: 2320 666f 7220 6b20 696e 206b 6579 733a  # for k in keys:
+00005dc0: 0a23 2020 2070 7269 6e74 286b 290a 2320  .#   print(k).# 
+00005dd0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00005de0: 6b2c 204b 6579 293a 0a23 2020 2020 2075  k, Key):.#     u
+00005df0: 726c 203d 206b 2e67 656e 6572 6174 655f  rl = k.generate_
+00005e00: 7572 6c28 3630 3029 0a23 2020 2020 2072  url(600).#     r
+00005e10: 6573 203d 2072 6571 7565 7374 732e 6765  es = requests.ge
+00005e20: 7428 7572 6c29 0a23 2020 2020 2069 6620  t(url).#     if 
+00005e30: 7265 732e 7374 6174 7573 5f63 6f64 6520  res.status_code 
+00005e40: 213d 2032 3030 3a0a 2320 2020 2020 2020  != 200:.#       
+00005e50: 7072 696e 7428 7572 6c29 0a0a 0a23 2072  print(url)...# r
+00005e60: 6573 203d 2072 6571 7565 7374 732e 6765  es = requests.ge
+00005e70: 7428 7572 6c29 0a23 2061 7373 6572 7420  t(url).# assert 
+00005e80: 7265 732e 7374 6174 7573 5f63 6f64 6520  res.status_code 
+00005e90: 213d 2034 3033 0a23 2074 6573 745f 6765  != 403.# test_ge
+00005ea0: 6e65 7261 7465 5f75 726c 2827 5c5c 615c  nerate_url('\\a\
+00005eb0: 5c5c 5c3a 3c3e 2a3f 7c3a 712e 6a70 6567  \\\:<>*?|:q.jpeg
+00005ec0: 2729 0a23 2074 6573 745f 6765 6e65 7261  ').# test_genera
+00005ed0: 7465 5f75 726c 2827 2378 323b 2e6a 702e  te_url('#x2;.jp.
+00005ee0: 6373 7627 290a 2320 7465 7374 5f67 656e  csv').# test_gen
+00005ef0: 6572 6174 655f 7572 6c28 2731 3030 3836  erate_url('10086
+00005f00: 2f31 3938 2e31 382d 7265 7365 742d e585  /198.18-reset-..
+00005f10: b1e8 aea1 39e6 9da1 2e74 7874 2729 0a23  ....9....txt').#
+00005f20: 2074 6573 745f 6765 6e65 7261 7465 5f75   test_generate_u
+00005f30: 726c 2827 3130 3038 362f 6765 7462 7563  rl('10086/getbuc
+00005f40: 6b65 742e 6373 7627 290a 2320 7465 7374  ket.csv').# test
+00005f50: 5f67 6574 5f70 7265 7369 676e 6564 5f75  _get_presigned_u
+00005f60: 726c 2827 7e2a 632f 6865 636b 4461 7461  rl('~*c/heckData
+00005f70: 2b73 6466 3d25 3246 2e6a 736f 6e27 290a  +sdf=%2F.json').
+00005f80: 2320 7465 7374 5f70 7574 5f76 6961 5f70  # test_put_via_p
+00005f90: 7265 7369 676e 6564 5f75 726c 2827 696e  resigned_url('in
+00005fa0: 6465 782e 6874 6d6c 2729 0a23 206c 6973  dex.html').# lis
+00005fb0: 745f 6f62 6a65 6374 735f 7632 2864 656c  t_objects_v2(del
+00005fc0: 696d 6974 6572 3d27 2f27 2c20 656e 636f  imiter='/', enco
+00005fd0: 6469 6e67 5f74 7970 653d 2775 726c 272c  ding_type='url',
+00005fe0: 2066 6574 6368 5f6f 776e 6572 3d46 616c   fetch_owner=Fal
+00005ff0: 7365 290a 2320 6c69 7374 5f6f 626a 6563  se).# list_objec
+00006000: 7473 2829 0a23 206c 6973 744f 626a 6563  ts().# listObjec
+00006010: 7473 4d6f 7265 2829 0a23 2064 656c 6574  tsMore().# delet
+00006020: 654f 626a 6563 7428 290a 2320 6c69 7374  eObject().# list
+00006030: 4f62 6a65 6374 7341 6e64 4669 6c74 6572  ObjectsAndFilter
+00006040: 2829 0a23 206c 6973 7441 6e64 4465 6c65  ().# listAndDele
+00006050: 7465 2829 0a23 2072 6573 746f 7265 4f62  te().# restoreOb
+00006060: 6a65 6374 2822 7777 772d 6c6f 676f 2229  ject("www-logo")
+00006070: 0a23 2067 6574 4275 636b 6574 7344 6174  .# getBucketsDat
+00006080: 6128 2274 6573 742d 6275 636b 6574 2229  a("test-bucket")
+00006090: 0a23 2074 6573 745f 6173 7375 6d65 526f  .# test_assumeRo
+000060a0: 6c65 2829 0a0a 2320 636f 7079 5f65 6e63  le()..# copy_enc
+000060b0: 7279 7074 696f 6e28 2761 7274 6963 6c65  ryption('article
+000060c0: 2e65 6e63 7279 7074 696f 6e2e 7478 7427  .encryption.txt'
+000060d0: 2c20 2761 7274 6963 6c65 2e74 7874 272c  , 'article.txt',
+000060e0: 2065 6e63 7279 7074 5f6b 6579 3d54 7275   encrypt_key=Tru
+000060f0: 6529 0a0a 2320 6669 6c65 4e61 6d65 203d  e)..# fileName =
+00006100: 2022 5c75 3030 3662 5c75 3030 3733 5c75   "\u006b\u0073\u
+00006110: 3030 3566 5c75 3030 3733 5c75 3030 3633  005f\u0073\u0063
+00006120: 5c75 3030 3631 5c75 3030 3665 5c75 3030  \u0061\u006e\u00
+00006130: 3566 5c75 3030 3666 5c75 3030 3633 5c75  5f\u006f\u0063\u
+00006140: 3030 3732 5c75 3030 3266 5c75 3030 3332  0072\u002f\u0032
+00006150: 5c75 3030 3330 5c75 3030 3331 5c75 3030  \u0030\u0031\u00
+00006160: 3338 5c75 3030 3264 5c75 3030 3330 5c75  38\u002d\u0030\u
+00006170: 3030 3333 5c75 3030 3264 5c75 3030 3331  0033\u002d\u0031
+00006180: 5c75 3030 3332 5c75 3030 3266 5c75 3030  \u0032\u002f\u00
+00006190: 3130 5c75 6666 6664 5c75 3030 3730 5c75  10\ufffd\u0070\u
+000061a0: 6666 6664 5c75 6666 6664 5c75 6666 6664  fffd\ufffd\ufffd
+000061b0: 5c75 3030 3032 5c75 3030 3265 5c75 3030  \u0002\u002e\u00
+000061c0: 3537 5c75 3030 3766 5c75 3030 3562 5c75  57\u007f\u005b\u
+000061d0: 6666 6664 5c75 3030 3038 5c75 6666 6664  fffd\u0008\ufffd
+000061e0: 5c75 3030 3261 5c75 6666 6664 5c75 3030  \u002a\ufffd\u00
+000061f0: 3265 5c75 3030 3661 5c75 3030 3730 5c75  2e\u006a\u0070\u
+00006200: 3030 3637 223b 0a23 2068 6568 6520 3d20  0067";.# hehe = 
+00006210: 2210 efbf bd70 efbf bdef bfbd efbf bd02  "....p..........
+00006220: 2e57 7f5b efbf bd2a efbf bd2e 6a70 6722  .W.[...*....jpg"
+00006230: 0a23 2066 6f72 2063 2069 6e20 6865 6865  .# for c in hehe
+00006240: 3a0a 2320 2020 2020 7072 696e 7428 7265  :.#     print(re
+00006250: 7072 2863 292c 2063 290a 2320 7572 6c63  pr(c), c).# urlc
+00006260: 6f64 6564 203d 2075 726c 6c69 622e 7061  oded = urllib.pa
+00006270: 7273 652e 7175 6f74 6528 6669 6c65 4e61  rse.quote(fileNa
+00006280: 6d65 290a 2320 756e 7175 6f74 6564 203d  me).# unquoted =
+00006290: 2075 726c 6c69 622e 7061 7273 652e 756e   urllib.parse.un
+000062a0: 7175 6f74 6528 2725 4646 2729 0a23 2071  quote('%FF').# q
+000062b0: 756f 7465 6420 3d20 7572 6c6c 6962 2e70  uoted = urllib.p
+000062c0: 6172 7365 2e71 756f 7465 2875 6e71 756f  arse.quote(unquo
+000062d0: 7465 6429 0a23 2070 7269 6e74 2875 6e71  ted).# print(unq
+000062e0: 756f 7465 6429 0a23 2070 7269 6e74 2871  uoted).# print(q
+000062f0: 756f 7465 6429 0a0a 2320 6765 744f 626a  uoted)..# getObj
+00006300: 6563 744d 6574 6128 2774 6573 742d 6275  ectMeta('test-bu
+00006310: 636b 6574 272c 2027 6172 7469 636c 652e  cket', 'article.
+00006320: 7478 7427 290a 2320 6b65 7920 3d20 636f  txt').# key = co
+00006330: 7079 2827 6172 7469 636c 652e 7478 7427  py('article.txt'
+00006340: 2c20 2761 7274 6963 6c65 2e74 7874 272c  , 'article.txt',
+00006350: 2064 7374 5f62 7563 6b65 745f 6e61 6d65   dst_bucket_name
+00006360: 3d27 7465 7374 2d62 7563 6b65 7427 290a  ='test-bucket').
+00006370: 2320 7072 696e 7428 2761 6674 6572 2063  # print('after c
+00006380: 6f70 795c 6e5c 6e27 290a 2320 6765 744f  opy\n\n').# getO
+00006390: 626a 6563 744d 6574 6128 2774 6573 742d  bjectMeta('test-
+000063a0: 6275 636b 6574 272c 2027 6172 7469 636c  bucket', 'articl
+000063b0: 652e 7478 7427 290a 2320 6765 744f 626a  e.txt').# getObj
+000063c0: 6563 744d 6574 6128 2774 6573 742d 6275  ectMeta('test-bu
+000063d0: 636b 6574 272c 2027 4453 4330 3333 3830  cket', 'DSC03380
+000063e0: 2e73 7365 632e 6a70 6727 290a 2320 7570  .ssec.jpg').# up
+000063f0: 6c6f 6164 4f62 6a65 6374 4672 6f6d 4669  loadObjectFromFi
+00006400: 6c65 2827 4453 4330 3333 3830 2e65 6e63  le('DSC03380.enc
+00006410: 7279 7074 2e6a 7067 2729 0a0a 2320 696d  rypt.jpg')..# im
+00006420: 706f 7274 2062 6173 6536 340a 2320 696d  port base64.# im
+00006430: 706f 7274 2068 6d61 630a 2320 696d 706f  port hmac.# impo
+00006440: 7274 2068 6173 686c 6962 0a23 2069 6d70  rt hashlib.# imp
+00006450: 6f72 7420 7572 6c6c 6962 0a23 2068 203d  ort urllib.# h =
+00006460: 2068 6d61 632e 6e65 7728 2261 6363 6573   hmac.new("acces
+00006470: 736b 6579 222c 0a23 2020 2020 2020 2020  skey",.#        
+00006480: 2020 2020 2020 2247 4554 5c6e 5c6e 5c6e        "GET\n\n\n
+00006490: 3131 3431 3838 3931 3230 5c6e 2f65 7861  1141889120\n/exa
+000064a0: 6d70 6c65 6275 636b 6574 2f6f 7373 2d61  mplebucket/oss-a
+000064b0: 7069 2e70 6466 222c 0a23 2020 2020 2020  pi.pdf",.#      
+000064c0: 2020 2020 2020 2020 6861 7368 6c69 622e          hashlib.
+000064d0: 7368 6131 290a 2320 7572 6c6c 6962 2e71  sha1).# urllib.q
+000064e0: 756f 7465 2028 6261 7365 3634 2e65 6e63  uote (base64.enc
+000064f0: 6f64 6573 7472 696e 6728 682e 6469 6765  odestring(h.dige
+00006500: 7374 2829 292e 7374 7269 7028 2929 0a0a  st()).strip())..
+00006510: 2320 6220 3d20 636f 6e6e 2e67 6574 5f62  # b = conn.get_b
+00006520: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+00006530: 6529 0a23 2023 2066 6f72 2070 2069 6e20  e).# # for p in 
+00006540: 622e 6765 745f 616c 6c5f 6d75 6c74 6970  b.get_all_multip
+00006550: 6172 745f 7570 6c6f 6164 7328 6b65 795f  art_uploads(key_
+00006560: 6d61 726b 6572 3d27 7465 7374 2d6d 756c  marker='test-mul
+00006570: 7469 272c 2075 706c 6f61 645f 6964 5f6d  ti', upload_id_m
+00006580: 6172 6b65 723d 2762 6266 6366 3062 6162  arker='bbfcf0bab
+00006590: 3565 3834 3564 3839 3564 3063 6663 6432  5e845d895d0cfcd2
+000065a0: 3633 3262 6631 3827 293a 2020 2020 2737  632bf18'):    '7
+000065b0: 6536 6237 6237 3931 3264 3134 6562 3039  e6b7b7912d14eb09
+000065c0: 3432 3431 3366 3236 3263 3438 3865 6327  42413f262c488ec'
+000065d0: 0a23 2061 6c6c 5f75 706c 6f61 6473 203d  .# all_uploads =
+000065e0: 2062 2e67 6574 5f61 6c6c 5f6d 756c 7469   b.get_all_multi
+000065f0: 7061 7274 5f75 706c 6f61 6473 286b 6579  part_uploads(key
+00006600: 5f6d 6172 6b65 723d 2744 5343 3033 3338  _marker='DSC0338
+00006610: 302e 656e 6372 7970 742e 6a70 672d 6464  0.encrypt.jpg-dd
+00006620: 6464 6464 6464 2729 236d 6178 5f75 706c  dddddd')#max_upl
+00006630: 6f61 6473 3d32 3729 0a23 2070 7269 6e74  oads=27).# print
+00006640: 286c 656e 2861 6c6c 5f75 706c 6f61 6473  (len(all_uploads
+00006650: 2929 0a23 2066 6f72 2070 2069 6e20 616c  )).# for p in al
+00006660: 6c5f 7570 6c6f 6164 733a 0a23 2020 2070  l_uploads:.#   p
+00006670: 7269 6e74 2870 2c20 702e 6964 290a 2320  rint(p, p.id).# 
+00006680: 7075 745f 6f62 6a65 6374 5f63 616c 6c62  put_object_callb
+00006690: 6163 6b28 2774 6573 742d 6361 6c6c 6261  ack('test-callba
+000066a0: 636b 2729                                ck')
```

### Comparing `ks3sdk-1.6.2/examples/billing.py` & `ks3sdk-1.6.3/examples/billing.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/bucket.py` & `ks3sdk-1.6.3/examples/bucket.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/crc64.py` & `ks3sdk-1.6.3/examples/crc64.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/encryption.py` & `ks3sdk-1.6.3/examples/encryption.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/multi_thread.py` & `ks3sdk-1.6.3/examples/multi_thread.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/multipart.py` & `ks3sdk-1.6.3/examples/multipart.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/object.py` & `ks3sdk-1.6.3/examples/object.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/postProcessTask.py` & `ks3sdk-1.6.3/examples/postProcessTask.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/examples/sts.py` & `ks3sdk-1.6.3/examples/sts.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/acl.py` & `ks3sdk-1.6.3/ks3/acl.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/auth.py` & `ks3sdk-1.6.3/ks3/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
                    'response-cache-control', 'response-content-disposition',
                    'response-content-encoding', 'delete', 'lifecycle',
                    'tagging', 'restore', 'notification', 'thumbnail', 'queryadp',
                    'adp', 'asyntask', 'querytask', 'domain',
                    'storageClass',
                    'websiteConfig',
                    'compose', 'quota', 'policy', 'crr', 'fetch', 'append', 'position',
-                   'mirror', 'retention', 'recycle', 'recover', 'clear']
+                   'mirror', 'retention', 'recycle', 'recover', 'clear', 'inventory',
+                   'id']
 
 
 def url_encode(key):
     if not key:
         return ""
     encode_key = parse.quote(utils.get_utf8_value(key))
     # if '%20' in encode_key:
```

### Comparing `ks3sdk-1.6.2/ks3/authV4.py` & `ks3sdk-1.6.3/ks3/authV4.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/billing.py` & `ks3sdk-1.6.3/ks3/billing.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/bucket.py` & `ks3sdk-1.6.3/ks3/bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from ks3.multipart import MultiPartUpload, CompleteMultiPartUpload
 from ks3.prefix import Prefix
 from ks3.resultset import ResultSet
 from ks3.xmlParsers.bucketQuota import BucketQuota
 from ks3.xmlParsers.bucketVersioning import BucketVersioningConfig
 from ks3.deletemarker import DeleteMarker
 from ks3.xmlParsers.bucketRetention import BucketRetention
+from ks3.xmlParsers.bucketInventory import BucketInventory, ListInventoryConfigurationsResult
 
 try:
     from ks3.encryption import Crypts
 except:
     pass
 
 
@@ -1155,14 +1156,64 @@
             if not isinstance(body, bytes):
                 body = body.encode('utf-8')
             xml.sax.parseString(body, h)
             return retention
         else:
             raise S3ResponseError(response.status, response.reason, body)
 
+    def set_bucket_inventory(self, bucket_inventory):
+        headers = {'content-type': 'application/xml'}
+        inventory_xml = bucket_inventory.to_xml()
+        if not isinstance(inventory_xml, bytes):
+            inventory_xml = inventory_xml.encode('utf-8')
+        md5 = ks3.utils.compute_base64_md5_digest(inventory_xml)
+        headers['Content-MD5'] = md5
+        response = self.connection.make_request('PUT', self.name, data=inventory_xml,
+                                                query_args='inventory&id=%s' % bucket_inventory.id,
+                                                headers=headers)
+        body = response.read()
+        if response.status == 200:
+            return None
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
+    def get_bucket_inventory(self, inventory_id):
+        response = self.connection.make_request('GET', self.name, query_args='inventory&id=%s' % inventory_id)
+        body = response.read()
+        if response.status == 200:
+            inventory = BucketInventory()
+            h = handler.XmlHandler(inventory, self)
+            if not isinstance(body, bytes):
+                body = body.encode('utf-8')
+            xml.sax.parseString(body, h)
+            return inventory
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
+    def list_bucket_inventory(self):
+        response = self.connection.make_request('GET', self.name, query_args='inventory')
+        body = response.read()
+        if response.status == 200:
+            result = ListInventoryConfigurationsResult()
+            h = handler.XmlHandler(result, self)
+            if not isinstance(body, bytes):
+                body = body.encode('utf-8')
+            xml.sax.parseString(body, h)
+            return result
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
+    def delete_bucket_inventory(self, inventory_id):
+        response = self.connection.make_request('DELETE', self.name, query_args='inventory&id=%s' % inventory_id)
+        body = response.read()
+        if response.status == 204:
+            return None
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
 
 class BucketLocation(object):
     def __init__(self):
         self.location = ''
 
     def startElement(self, name, attrs, connection):
         pass
```

### Comparing `ks3sdk-1.6.2/ks3/bucketlistresultset.py` & `ks3sdk-1.6.3/ks3/bucketlistresultset.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/compat.py` & `ks3sdk-1.6.3/ks3/compat.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/connection.py` & `ks3sdk-1.6.3/ks3/connection.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/crc64_combine.py` & `ks3sdk-1.6.3/ks3/crc64_combine.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/deletemarker.py` & `ks3sdk-1.6.3/ks3/deletemarker.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/encryptFp.py` & `ks3sdk-1.6.3/ks3/encryptFp.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/encryption.py` & `ks3sdk-1.6.3/ks3/encryption.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/exception.py` & `ks3sdk-1.6.3/ks3/exception.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/handler.py` & `ks3sdk-1.6.3/ks3/handler.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/http.py` & `ks3sdk-1.6.3/ks3/http.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/key.py` & `ks3sdk-1.6.3/ks3/key.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,39 +421,49 @@
                 fp.block_count = 0
                 fp.calc_iv = ""
             if chunked_transfer:
                 headers['Transfer-Encoding'] = 'chunked'
             else:
                 headers['Content-Length'] = str(len(fp))
             headers["x-kss-meta-unencrypted-content-length"] = str(self.size)
+            if self.bucket.connection.enable_crc and not isinstance(fp, utils.FpAdapter):
+                fp = utils.FpAdapter(fp)
             resp = self.bucket.connection.make_request(
                 method,
                 self.bucket.name,
                 self.name,
                 data=fp,
                 headers=headers,
                 query_args=query_args,
             )
             if resp and resp.status > 299:
                 raise provider.storage_response_error(resp.status, resp.reason, resp.read())
             self.handle_version_headers(resp, force=True)
             self.handle_addl_headers(resp.getheaders())
+            if self.bucket.connection.enable_crc:
+                self.client_crc = str(fp.crc)
+                utils.check_crc(self.client_crc, resp.getheader(self.provider.checksum_crc64ecma_header))
             return resp
+        if self.bucket.connection.enable_crc and not isinstance(fp, utils.FpAdapter):
+            fp = utils.FpAdapter(fp)
         resp = self.bucket.connection.make_request(
             method,
             self.bucket.name,
             self.name,
             data=fp,
             headers=headers,
             query_args=query_args
         )
         if resp and resp.status > 299:
             raise provider.storage_response_error(resp.status, resp.reason, resp.read())
         self.handle_version_headers(resp, force=True)
         self.handle_addl_headers(resp.getheaders())
+        if self.bucket.connection.enable_crc:
+            self.client_crc = str(fp.crc)
+            utils.check_crc(self.client_crc, resp.getheader(self.provider.checksum_crc64ecma_header))
         return resp
 
     def set_contents_from_file(self, fp, method="PUT", headers=None, replace=True,
                                cb=None, num_cb=10, policy=None, md5=None,
                                reduced_redundancy=False, query_args=None,
                                encrypt_key=False, size=None, rewind=False,
                                crypt_context=None, calc_encrypt_md5=True):
@@ -522,16 +532,14 @@
             be rewound to the start before any bytes are read from
             it. The default behaviour is False which reads from the
             current position of the file pointer (fp).
 
         :rtype: int
         :return: The number of bytes written to the key.
         """
-        if self.bucket.connection.enable_crc and not isinstance(fp, utils.FpAdapter):
-            fp = utils.FpAdapter(fp)
         provider = self.bucket.connection.provider
         headers = headers or {}
         if policy:
             headers[provider.acl_header] = policy
         if encrypt_key:
             headers[provider.server_side_encryption_header] = 'AES256'
 
@@ -633,17 +641,14 @@
                                       chunked_transfer=chunked_transfer, size=size,
                                       crypt_context=crypt_context)
             else:
                 resp = self.send_file(fp, method=method, headers=headers, cb=cb, num_cb=num_cb,
                                       query_args=query_args,
                                       chunked_transfer=chunked_transfer, size=size)
 
-            if self.bucket.connection.enable_crc:
-                self.client_crc = str(fp.crc)
-                utils.check_crc(self.client_crc, resp.getheader(self.provider.checksum_crc64ecma_header))
 
             return resp
             # return number of bytes written.
             # return self.size
 
     def set_contents_from_filename(self, filename, method="PUT", headers=None, replace=True,
                                    cb=None, num_cb=10, policy=None, md5=None,
```

### Comparing `ks3sdk-1.6.2/ks3/keyfile.py` & `ks3sdk-1.6.3/ks3/keyfile.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/multipart.py` & `ks3sdk-1.6.3/ks3/multipart.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,15 +286,24 @@
             self.size_accumulator[part_num] = part_size
         else:
             response = key.set_contents_from_file(fp, headers=headers, replace=replace,
                                        cb=cb, num_cb=num_cb, md5=md5,
                                        reduced_redundancy=False,
                                        query_args=query_args, size=size)
         if self.bucket.connection.enable_crc:
-            part_info = PartInfo(fp.tell(), response.getheader(self.bucket.connection.provider.checksum_crc64ecma_header))
+            part_size = fp.tell()
+            if self.bucket.connection.local_encrypt and self.crypt_context:
+                if is_last_part is True:
+                    # After local encryption, the size of the last part is filled to a multiple of 16
+                    pad = 16 - part_size % 16
+                    part_size += pad
+                elif part_num == 1:
+                    # Local encryption sets the key ciphertext with a size of 16 bytes in the first part of the file
+                    part_size += 16
+            part_info = PartInfo(part_size, response.getheader(self.bucket.connection.provider.checksum_crc64ecma_header))
             self.part_crc_infos[part_num] = part_info
         return response
     def add_all_part(self, part_num):
         sum = 0
         for i in range(1,part_num):
             if self.size_accumulator.get(i):
                 sum += self.size_accumulator[i]
@@ -347,15 +356,16 @@
 
         :rtype: :class:`boto.s3.multipart.CompletedMultiPartUpload`
         :returns: An object representing the completed upload.
         """
         xml = self.to_xml()
         resp = self.bucket.complete_multipart_upload(self.key_name,
                                                      self.id, xml)
-        if self.bucket.connection.enable_crc and self.part_crc_infos:
+        if self.bucket.connection.enable_crc and len(self.part_crc_infos) > 0:
+            # Iterating from 0 is equivalent to iterating from the first crc value
             parts_crc = 0
             crc_obj = ks3.utils.Crc64(0)
 
             part_tuples = sorted(self.part_crc_infos.items(), key=lambda i: i[0])
             for t in part_tuples:
                 p = t[1]
                 parts_crc = crc_obj.combine(parts_crc, int(p.part_crc), p.size)
```

### Comparing `ks3sdk-1.6.2/ks3/objectTagging.py` & `ks3sdk-1.6.3/ks3/objectTagging.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/prefix.py` & `ks3sdk-1.6.3/ks3/prefix.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/provider.py` & `ks3sdk-1.6.3/ks3/provider.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/resultset.py` & `ks3sdk-1.6.3/ks3/resultset.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/sts.py` & `ks3sdk-1.6.3/ks3/sts.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/user.py` & `ks3sdk-1.6.3/ks3/user.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/utils.py` & `ks3sdk-1.6.3/ks3/utils.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketCors.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketCors.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketCrossReplicate.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketCrossReplicate.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketLifecycle.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketLifecycle.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketLogging.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketLogging.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketMirror.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketMirror.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketQuota.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketQuota.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketRetention.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketRetention.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3/xmlParsers/bucketVersioning.py` & `ks3sdk-1.6.3/ks3/xmlParsers/bucketVersioning.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.2/ks3sdk.egg-info/PKG-INFO` & `ks3sdk-1.6.3/ks3sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ks3sdk
-Version: 1.6.2
+Version: 1.6.3
 Summary: Ksyun KS3 SDK
 Home-page: https://gitee.com/ks3sdk/ks3-python-sdk
 Author: ksc_ks3
 Author-email: ksc_ks3@kingsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ks3sdk-1.6.2/ks3sdk.egg-info/SOURCES.txt` & `ks3sdk-1.6.3/ks3sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 ks3/resultset.py
 ks3/sts.py
 ks3/user.py
 ks3/utils.py
 ks3/xmlParsers/__init__.py
 ks3/xmlParsers/bucketCors.py
 ks3/xmlParsers/bucketCrossReplicate.py
+ks3/xmlParsers/bucketInventory.py
 ks3/xmlParsers/bucketLifecycle.py
 ks3/xmlParsers/bucketLogging.py
 ks3/xmlParsers/bucketMirror.py
 ks3/xmlParsers/bucketQuota.py
 ks3/xmlParsers/bucketRetention.py
 ks3/xmlParsers/bucketVersioning.py
 ks3sdk.egg-info/PKG-INFO
```

### Comparing `ks3sdk-1.6.2/setup.py` & `ks3sdk-1.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     description='Ksyun KS3 SDK',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['ks3', 'ks3.xmlParsers'],
     install_requires=[
         'six', 'python-dateutil',
         'aiofiles~=23.2.1',
-        'crcmod~=1.7'
+        'crcmod~=1.7',
+        'pycryptodome~=3.20.0'
     ],
     include_package_data=True,
     url='https://gitee.com/ks3sdk/ks3-python-sdk',
     author='ksc_ks3',
     author_email='ksc_ks3@kingsoft.com',
     license='MIT',
     classifiers=[
```

