# Comparing `tmp/rastervision_aws_s3-0.30.0.tar.gz` & `tmp/rastervision_aws_s3-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_aws_s3-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
+gzip compressed data, was "rastervision_aws_s3-0.30.1.tar", last modified: Mon May  6 21:02:13 2024, max compression
```

## Comparing `rastervision_aws_s3-0.30.0.tar` & `rastervision_aws_s3-0.30.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision/aws_s3/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      421 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.0/rastervision/aws_s3/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10519 2024-04-07 00:38:15.000000 rastervision_aws_s3-0.30.0/rastervision/aws_s3/s3_file_system.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      363 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       40 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       75 2024-04-10 21:55:10.000000 rastervision_aws_s3-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.751693 rastervision_aws_s3-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1717 2024-04-10 21:55:10.000000 rastervision_aws_s3-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.643122 rastervision_aws_s3-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-05-06 21:02:13.643122 rastervision_aws_s3-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.639122 rastervision_aws_s3-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.643122 rastervision_aws_s3-0.30.1/rastervision/aws_s3/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      421 2023-08-24 18:41:21.000000 rastervision_aws_s3-0.30.1/rastervision/aws_s3/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11035 2024-05-03 19:36:28.000000 rastervision_aws_s3-0.30.1/rastervision/aws_s3/s3_file_system.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.643122 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      363 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       40 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:13.000000 rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       75 2024-05-06 20:16:58.000000 rastervision_aws_s3-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:13.643122 rastervision_aws_s3-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1717 2024-05-06 20:16:58.000000 rastervision_aws_s3-0.30.1/setup.py
```

### Comparing `rastervision_aws_s3-0.30.0/PKG-INFO` & `rastervision_aws_s3-0.30.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_aws_s3
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds an AWS S3 file system
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_s3-0.30.0/rastervision/aws_s3/s3_file_system.py` & `rastervision_aws_s3-0.30.1/rastervision/aws_s3/s3_file_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Any, Iterator, Tuple
 import io
 import os
 import subprocess
 from datetime import datetime
 from urllib.parse import urlparse
 
 import boto3
@@ -12,68 +12,75 @@
 from rastervision.pipeline.file_system import (FileSystem, NotReadableError,
                                                NotWritableError)
 
 AWS_S3 = 'aws_s3'
 
 
 # Code from https://alexwlchan.net/2017/07/listing-s3-keys/
-def get_matching_s3_objects(bucket, prefix='', suffix='',
-                            request_payer='None'):
-    """
-    Generate objects in an S3 bucket.
-
-    :param bucket: Name of the S3 bucket.
-    :param prefix: Only fetch objects whose key starts with
-        this prefix (optional).
-    :param suffix: Only fetch objects whose keys end with
-        this suffix (optional).
+def get_matching_s3_objects(
+        bucket: str,
+        prefix: str = '',
+        suffix: str = '',
+        delimiter: str = '/',
+        request_payer: str = 'None') -> Iterator[tuple[str, Any]]:
+    """Generate objects in an S3 bucket.
+
+    Args:
+        bucket: Name of the S3 bucket.
+        prefix: Only fetch objects whose key starts with this prefix.
+        suffix: Only fetch objects whose keys end with this suffix.
     """
     s3 = S3FileSystem.get_client()
-    kwargs = {'Bucket': bucket, 'RequestPayer': request_payer}
-
-    # If the prefix is a single string (not a tuple of strings), we can
-    # do the filtering directly in the S3 API.
-    if isinstance(prefix, str):
-        kwargs['Prefix'] = prefix
-
+    kwargs = dict(
+        Bucket=bucket,
+        RequestPayer=request_payer,
+        Delimiter=delimiter,
+        Prefix=prefix,
+    )
     while True:
-
-        # The S3 API response is a large blob of metadata.
-        # 'Contents' contains information about the listed objects.
-        resp = s3.list_objects_v2(**kwargs)
-
-        try:
-            contents = resp['Contents']
-        except KeyError:
-            return
-
-        for obj in contents:
+        resp: dict = s3.list_objects_v2(**kwargs)
+        dirs: list[dict] = resp.get('CommonPrefixes', {})
+        files: list[dict] = resp.get('Contents', {})
+        for obj in dirs:
+            key = obj['Prefix']
+            if key.startswith(prefix) and key.endswith(suffix):
+                yield key, obj
+        for obj in files:
             key = obj['Key']
             if key.startswith(prefix) and key.endswith(suffix):
-                yield obj
-
+                yield key, obj
         # The S3 API is paginated, returning up to 1000 keys at a time.
         # Pass the continuation token into the next response, until we
         # reach the final page (when this field is missing).
         try:
             kwargs['ContinuationToken'] = resp['NextContinuationToken']
         except KeyError:
             break
 
 
-def get_matching_s3_keys(bucket, prefix='', suffix='', request_payer='None'):
-    """
-    Generate the keys in an S3 bucket.
-
-    :param bucket: Name of the S3 bucket.
-    :param prefix: Only fetch keys that start with this prefix (optional).
-    :param suffix: Only fetch keys that end with this suffix (optional).
+def get_matching_s3_keys(bucket: str,
+                         prefix: str = '',
+                         suffix: str = '',
+                         delimiter: str = '/',
+                         request_payer: str = 'None') -> Iterator[str]:
+    """Generate the keys in an S3 bucket.
+
+    Args:
+        bucket: Name of the S3 bucket.
+        prefix: Only fetch keys that start with this prefix.
+        suffix: Only fetch keys that end with this suffix.
     """
-    for obj in get_matching_s3_objects(bucket, prefix, suffix, request_payer):
-        yield obj['Key']
+    obj_iterator = get_matching_s3_objects(
+        bucket,
+        prefix=prefix,
+        suffix=suffix,
+        delimiter=delimiter,
+        request_payer=request_payer)
+    out = (key for key, _ in obj_iterator)
+    return out
 
 
 def progressbar(total_size: int, desc: str):
     return tqdm(
         total=total_size,
         desc=desc,
         unit='B',
@@ -176,16 +183,17 @@
         import botocore
 
         s3 = S3FileSystem.get_client()
         request_payer = S3FileSystem.get_request_payer()
         bucket, key = S3FileSystem.parse_uri(uri)
         with io.BytesIO() as file_buffer:
             try:
-                file_size = s3.head_object(
-                    Bucket=bucket, Key=key)['ContentLength']
+                obj = s3.head_object(
+                    Bucket=bucket, Key=key, RequestPayer=request_payer)
+                file_size = obj['ContentLength']
                 with progressbar(file_size, desc='Downloading') as bar:
                     s3.download_fileobj(
                         Bucket=bucket,
                         Key=key,
                         Fileobj=file_buffer,
                         Callback=lambda bytes: bar.update(bytes),
                         ExtraArgs={'RequestPayer': request_payer})
@@ -252,15 +260,17 @@
     def copy_from(src_uri: str, dst_path: str) -> None:
         import botocore
 
         s3 = S3FileSystem.get_client()
         request_payer = S3FileSystem.get_request_payer()
         bucket, key = S3FileSystem.parse_uri(src_uri)
         try:
-            file_size = s3.head_object(Bucket=bucket, Key=key)['ContentLength']
+            obj = s3.head_object(
+                Bucket=bucket, Key=key, RequestPayer=request_payer)
+            file_size = obj['ContentLength']
             with progressbar(file_size, desc=f'Downloading') as bar:
                 s3.download_file(
                     Bucket=bucket,
                     Key=key,
                     Filename=dst_path,
                     Callback=lambda bytes: bar.update(bytes),
                     ExtraArgs={'RequestPayer': request_payer})
@@ -280,15 +290,20 @@
         s3 = S3FileSystem.get_client()
         request_payer = S3FileSystem.get_request_payer()
         head_data = s3.head_object(
             Bucket=bucket, Key=key, RequestPayer=request_payer)
         return head_data['LastModified']
 
     @staticmethod
-    def list_paths(uri, ext=''):
+    def list_paths(uri: str, ext: str = '', delimiter: str = '/') -> list[str]:
         request_payer = S3FileSystem.get_request_payer()
         parsed_uri = urlparse(uri)
         bucket = parsed_uri.netloc
         prefix = os.path.join(parsed_uri.path[1:])
         keys = get_matching_s3_keys(
-            bucket, prefix, suffix=ext, request_payer=request_payer)
-        return [os.path.join('s3://', bucket, key) for key in keys]
+            bucket,
+            prefix,
+            suffix=ext,
+            delimiter=delimiter,
+            request_payer=request_payer)
+        paths = [os.path.join('s3://', bucket, key) for key in keys]
+        return paths
```

### Comparing `rastervision_aws_s3-0.30.0/rastervision_aws_s3.egg-info/PKG-INFO` & `rastervision_aws_s3-0.30.1/rastervision_aws_s3.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-aws-s3
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds an AWS S3 file system
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_s3-0.30.0/setup.py` & `rastervision_aws_s3-0.30.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_aws_s3'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds an AWS S3 file system'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

