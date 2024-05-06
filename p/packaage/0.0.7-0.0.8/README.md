# Comparing `tmp/packaage-0.0.7.tar.gz` & `tmp/packaage-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaage-0.0.7.tar", last modified: Thu Aug 31 09:01:36 2023, max compression
+gzip compressed data, was "packaage-0.0.8.tar", last modified: Mon May  6 11:52:25 2024, max compression
```

## Comparing `packaage-0.0.7.tar` & `packaage-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-31 09:01:36.219973 packaage-0.0.7/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1069 2023-08-11 11:54:30.000000 packaage-0.0.7/LICENSE.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2023-08-31 09:01:36.219973 packaage-0.0.7/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1254 2023-08-31 07:48:13.000000 packaage-0.0.7/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-31 09:01:36.219973 packaage-0.0.7/packaage/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-08-31 09:01:06.000000 packaage-0.0.7/packaage/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2873 2023-08-31 06:35:49.000000 packaage-0.0.7/packaage/aws.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      271 2023-08-31 06:35:49.000000 packaage-0.0.7/packaage/life.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      492 2023-08-31 06:36:42.000000 packaage-0.0.7/packaage/nlp.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      398 2023-08-31 07:03:29.000000 packaage-0.0.7/packaage/setup.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      591 2023-08-31 06:37:40.000000 packaage-0.0.7/packaage/test.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-08-31 09:01:36.219973 packaage-0.0.7/packaage.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2023-08-31 09:01:36.000000 packaage-0.0.7/packaage.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      294 2023-08-31 09:01:36.000000 packaage-0.0.7/packaage.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-08-31 09:01:36.000000 packaage-0.0.7/packaage.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       32 2023-08-31 09:01:36.000000 packaage-0.0.7/packaage.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        9 2023-08-31 09:01:36.000000 packaage-0.0.7/packaage.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-08-31 09:01:36.219973 packaage-0.0.7/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-08-11 11:54:30.000000 packaage-0.0.7/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-06 11:52:25.592633 packaage-0.0.8/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1069 2023-08-11 11:54:30.000000 packaage-0.0.8/LICENSE.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2024-05-06 11:52:25.592633 packaage-0.0.8/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1254 2023-08-31 07:48:13.000000 packaage-0.0.8/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-06 11:52:25.582633 packaage-0.0.8/packaage/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2024-05-06 11:43:34.000000 packaage-0.0.8/packaage/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2958 2024-05-06 11:41:36.000000 packaage-0.0.8/packaage/aws.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      271 2023-08-31 06:35:49.000000 packaage-0.0.8/packaage/life.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      492 2023-08-31 06:36:42.000000 packaage-0.0.8/packaage/nlp.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      398 2023-08-31 07:03:29.000000 packaage-0.0.8/packaage/setup.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      591 2023-08-31 06:37:40.000000 packaage-0.0.8/packaage/test.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-05-06 11:52:25.582633 packaage-0.0.8/packaage.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2024-05-06 11:52:25.000000 packaage-0.0.8/packaage.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      294 2024-05-06 11:52:25.000000 packaage-0.0.8/packaage.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-05-06 11:52:25.000000 packaage-0.0.8/packaage.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-05-06 11:52:25.000000 packaage-0.0.8/packaage.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        9 2024-05-06 11:52:25.000000 packaage-0.0.8/packaage.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-05-06 11:52:25.592633 packaage-0.0.8/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      599 2023-08-11 11:54:30.000000 packaage-0.0.8/setup.py
```

### Comparing `packaage-0.0.7/LICENSE.txt` & `packaage-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packaage-0.0.7/PKG-INFO` & `packaage-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Packaage is a Python library with few AI utils
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Packaage
 
 Ever get this feeling that you wrote a bunch of stuff ever and ever and ever and ever and ever ...
```

### Comparing `packaage-0.0.7/README.md` & `packaage-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `packaage-0.0.7/packaage/aws.py` & `packaage-0.0.8/packaage/aws.py`

 * *Files 21% similar despite different names*

```diff
@@ -63,27 +63,30 @@
 
     if commit:
         connector.set_session(autocommit=True)
 
     return connector
 
 
-def s3_to_memory(bucket: str, file_key: str) -> Union[str, bytes]:
+def s3_to_memory(bucket: str, file_key: str, decode_utf: bool = False) -> Union[str, bytes]:
     """Download the content of a file from s3 into memory
 
     Args:
         bucket (str): The bucket name where the file is located
         file_key (str): The complete file key of the file inside the bucket
 
     Returns:
         Union[str, bytes]: The content of the file as a string of a bytes array depending on the
             file.
     """
     s3_client = boto3.client('s3')
 
     response = s3_client.get_object(Bucket=bucket, Key=file_key)
 
-    return response['Body'].read().decode('utf-8')
+    if decode_utf:
+        return response['Body'].read().decode('utf-8')
+
+    return response['Body'].read()
 
 
 def upload_to_s3(bucket: str, file_key: str) -> None:
     pass
```

### Comparing `packaage-0.0.7/packaage/test.py` & `packaage-0.0.8/packaage/test.py`

 * *Files identical despite different names*

### Comparing `packaage-0.0.7/packaage.egg-info/PKG-INFO` & `packaage-0.0.8/packaage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaage
-Version: 0.0.7
+Version: 0.0.8
 Summary: Packaage is a Python library with few AI utils
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Packaage
 
 Ever get this feeling that you wrote a bunch of stuff ever and ever and ever and ever and ever ...
```

### Comparing `packaage-0.0.7/setup.py` & `packaage-0.0.8/setup.py`

 * *Files identical despite different names*

