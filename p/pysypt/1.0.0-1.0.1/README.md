# Comparing `tmp/pysypt-1.0.0.tar.gz` & `tmp/pysypt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysypt-1.0.0.tar", last modified: Mon May  6 11:52:29 2024, max compression
+gzip compressed data, was "pysypt-1.0.1.tar", last modified: Mon May  6 12:23:38 2024, max compression
```

## Comparing `pysypt-1.0.0.tar` & `pysypt-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.079297 pysypt-1.0.0/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 12:03:35.000000 pysypt-1.0.0/MANIFEST.in
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1318 2024-05-06 11:52:29.079111 pysypt-1.0.0/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1093 2024-05-06 11:51:55.000000 pysypt-1.0.0/README.md
--rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2024-05-06 11:47:46.000000 pysypt-1.0.0/pyproject.toml
--rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2024-05-06 11:52:29.079335 pysypt-1.0.0/setup.cfg
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072135 pysypt-1.0.0/src/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071777 pysypt-1.0.0/src/java/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071823 pysypt-1.0.0/src/java/encryption-app/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071865 pysypt-1.0.0/src/java/encryption-app/build/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071914 pysypt-1.0.0/src/java/encryption-app/build/distributions/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072021 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072747 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8868 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3221 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078152 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
--rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-12-18 12:41:30.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)     4933 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-12-18 12:43:10.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   124506 2024-05-06 10:11:56.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078383 pysypt-1.0.0/src/pysypt/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       69 2024-05-06 11:47:46.000000 pysypt-1.0.0/src/pysypt/__init__.py
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1564 2024-05-06 11:38:32.000000 pysypt-1.0.0/src/pysypt/encryption.py
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078925 pysypt-1.0.0/src/pysypt.egg-info/
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1318 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1512 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/SOURCES.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/dependency_links.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/top_level.txt
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.474219 pysypt-1.0.1/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 12:03:35.000000 pysypt-1.0.1/MANIFEST.in
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:23:38.474034 pysypt-1.0.1/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1097 2024-05-06 12:18:11.000000 pysypt-1.0.1/README.md
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2024-05-06 12:22:50.000000 pysypt-1.0.1/pyproject.toml
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2024-05-06 12:23:38.474299 pysypt-1.0.1/setup.cfg
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466415 pysypt-1.0.1/src/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466045 pysypt-1.0.1/src/java/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466096 pysypt-1.0.1/src/java/encryption-app/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466145 pysypt-1.0.1/src/java/encryption-app/build/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466194 pysypt-1.0.1/src/java/encryption-app/build/distributions/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466302 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.467149 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8868 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3221 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.472878 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-12-18 12:41:30.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     3339 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-12-18 12:43:10.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   124506 2024-05-06 10:11:56.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.473175 pysypt-1.0.1/src/pysypt/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       69 2024-05-06 12:22:50.000000 pysypt-1.0.1/src/pysypt/__init__.py
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1750 2024-05-06 12:18:11.000000 pysypt-1.0.1/src/pysypt/encryption.py
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.473827 pysypt-1.0.1/src/pysypt.egg-info/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1512 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/SOURCES.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/dependency_links.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/top_level.txt
```

### Comparing `pysypt-1.0.0/PKG-INFO` & `pysypt-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysypt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # pysypt
 
 Python wrapper around [jasypt](http://www.jasypt.org/) for encrypting and decrypting strings using the BouncyCastle
@@ -17,15 +17,15 @@
 
 algorithm = "PBEWITHSHA256AND256BITAES-CBC-BC"
 key = "secret_key"
 message = "my secret message"
 
 enc = StringEncryptor(algorithm=algorithm, key=key)
 
-encrypted = enc.encrypt(enc)
+encrypted = enc.encrypt(message)
 print(encrypted)
 # output
 # pmwLKcnp8KP8jHDUf9r21Pbr8L/jQcKeOlcIrLosYSWpL6DhCY+APpSlPRwGl1EB
 
 print(enc.decrypt(encrypted))
 # output
 # my secret message
```

### Comparing `pysypt-1.0.0/README.md` & `pysypt-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 algorithm = "PBEWITHSHA256AND256BITAES-CBC-BC"
 key = "secret_key"
 message = "my secret message"
 
 enc = StringEncryptor(algorithm=algorithm, key=key)
 
-encrypted = enc.encrypt(enc)
+encrypted = enc.encrypt(message)
 print(encrypted)
 # output
 # pmwLKcnp8KP8jHDUf9r21Pbr8L/jQcKeOlcIrLosYSWpL6DhCY+APpSlPRwGl1EB
 
 print(enc.decrypt(encrypted))
 # output
 # my secret message
```

### Comparing `pysypt-1.0.0/pyproject.toml` & `pysypt-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysypt"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider."
 readme = "README.md"
 requires-python = ">=3.11"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar` & `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.0/src/pysypt/encryption.py` & `pysypt-1.0.1/src/pysypt/encryption.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import subprocess
+import timeit
 from pathlib import Path
 from subprocess import Popen
 
 import pexpect
 from py4j.java_gateway import JavaGateway
 
 src_dir = Path(__file__).parent / "../"
@@ -27,29 +28,37 @@
         shell=True)
 
 
 class StringEncryptor:
     def __init__(self, algorithm: str, key: str):
         logger.info("initializing encryptor...")
 
-        self.child = pexpect.spawn(f'{EXECUTABLE_PATH} --algorithm "{algorithm}" --key "{key}"')
+        self.child = pexpect.spawn(str(EXECUTABLE_PATH))
         self.child.expect('py4j - Gateway Server Started')
 
         gateway = JavaGateway()
         self.encryptor = gateway.entry_point.getEncryptor()
+        self.encryptor.setAlgorithm(algorithm)
+        self.encryptor.setPassword(key)
 
     def __del__(self):
         self.child.kill(2)
 
     def encrypt(self, message: str):
         return self.encryptor.encrypt(message)
 
     def decrypt(self, message: str):
         return self.encryptor.decrypt(message)
 
 
 if __name__ == '__main__':
     enc = StringEncryptor('PBEWITHSHA256AND256BITAES-CBC-BC', 'safsadfsda')
 
-    x = enc.encrypt("hello hasdfdsaf ello")
-    print(x)
-    print(enc.decrypt(x))
+    start = timeit.default_timer()
+
+    for _ in range(10_000):
+        x = enc.encrypt("hello hasdfdsaf ello")
+        dec = enc.decrypt(x)
+
+    end = timeit.default_timer()
+
+    print(f"{end - start:.2f}")
```

### Comparing `pysypt-1.0.0/src/pysypt.egg-info/PKG-INFO` & `pysypt-1.0.1/src/pysypt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysypt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # pysypt
 
 Python wrapper around [jasypt](http://www.jasypt.org/) for encrypting and decrypting strings using the BouncyCastle
@@ -17,15 +17,15 @@
 
 algorithm = "PBEWITHSHA256AND256BITAES-CBC-BC"
 key = "secret_key"
 message = "my secret message"
 
 enc = StringEncryptor(algorithm=algorithm, key=key)
 
-encrypted = enc.encrypt(enc)
+encrypted = enc.encrypt(message)
 print(encrypted)
 # output
 # pmwLKcnp8KP8jHDUf9r21Pbr8L/jQcKeOlcIrLosYSWpL6DhCY+APpSlPRwGl1EB
 
 print(enc.decrypt(encrypted))
 # output
 # my secret message
```

### Comparing `pysypt-1.0.0/src/pysypt.egg-info/SOURCES.txt` & `pysypt-1.0.1/src/pysypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

