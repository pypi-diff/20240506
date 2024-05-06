# Comparing `tmp/pysypt-1.0.1.tar.gz` & `tmp/pysypt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysypt-1.0.1.tar", last modified: Mon May  6 12:23:38 2024, max compression
+gzip compressed data, was "pysypt-1.0.2.tar", last modified: Mon May  6 12:46:37 2024, max compression
```

## Comparing `pysypt-1.0.1.tar` & `pysypt-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.474219 pysypt-1.0.1/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 12:03:35.000000 pysypt-1.0.1/MANIFEST.in
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:23:38.474034 pysypt-1.0.1/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1097 2024-05-06 12:18:11.000000 pysypt-1.0.1/README.md
--rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2024-05-06 12:22:50.000000 pysypt-1.0.1/pyproject.toml
--rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2024-05-06 12:23:38.474299 pysypt-1.0.1/setup.cfg
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466415 pysypt-1.0.1/src/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466045 pysypt-1.0.1/src/java/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466096 pysypt-1.0.1/src/java/encryption-app/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466145 pysypt-1.0.1/src/java/encryption-app/build/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466194 pysypt-1.0.1/src/java/encryption-app/build/distributions/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.466302 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.467149 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8868 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3221 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.472878 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
--rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-12-18 12:41:30.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)     3339 2024-05-06 12:23:34.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-12-18 12:43:10.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   124506 2024-05-06 10:11:56.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2024-05-06 09:44:04.000000 pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.473175 pysypt-1.0.1/src/pysypt/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       69 2024-05-06 12:22:50.000000 pysypt-1.0.1/src/pysypt/__init__.py
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1750 2024-05-06 12:18:11.000000 pysypt-1.0.1/src/pysypt/encryption.py
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:23:38.473827 pysypt-1.0.1/src/pysypt.egg-info/
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1512 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/SOURCES.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/dependency_links.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2024-05-06 12:23:38.000000 pysypt-1.0.1/src/pysypt.egg-info/top_level.txt
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.376042 pysypt-1.0.2/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 12:03:35.000000 pysypt-1.0.2/MANIFEST.in
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:46:37.375845 pysypt-1.0.2/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1097 2024-05-06 12:18:11.000000 pysypt-1.0.2/README.md
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2024-05-06 12:45:51.000000 pysypt-1.0.2/pyproject.toml
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2024-05-06 12:46:37.376080 pysypt-1.0.2/setup.cfg
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367844 pysypt-1.0.2/src/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367477 pysypt-1.0.2/src/java/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367530 pysypt-1.0.2/src/java/encryption-app/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367576 pysypt-1.0.2/src/java/encryption-app/build/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367630 pysypt-1.0.2/src/java/encryption-app/build/distributions/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.367735 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.368699 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8868 2024-05-06 12:46:32.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3221 2024-05-06 12:46:32.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.374663 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-12-18 12:41:30.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     3339 2024-05-06 12:46:32.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-12-18 12:43:10.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   124506 2024-05-06 10:11:56.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2024-05-06 09:44:04.000000 pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.374947 pysypt-1.0.2/src/pysypt/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      748 2024-05-06 12:45:51.000000 pysypt-1.0.2/src/pysypt/__init__.py
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      512 2024-05-06 12:41:45.000000 pysypt-1.0.2/src/pysypt/encryption.py
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 12:46:37.375642 pysypt-1.0.2/src/pysypt.egg-info/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1322 2024-05-06 12:46:37.000000 pysypt-1.0.2/src/pysypt.egg-info/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1512 2024-05-06 12:46:37.000000 pysypt-1.0.2/src/pysypt.egg-info/SOURCES.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2024-05-06 12:46:37.000000 pysypt-1.0.2/src/pysypt.egg-info/dependency_links.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2024-05-06 12:46:37.000000 pysypt-1.0.2/src/pysypt.egg-info/top_level.txt
```

### Comparing `pysypt-1.0.1/PKG-INFO` & `pysypt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysypt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # pysypt
 
 Python wrapper around [jasypt](http://www.jasypt.org/) for encrypting and decrypting strings using the BouncyCastle
```

### Comparing `pysypt-1.0.1/README.md` & `pysypt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/pyproject.toml` & `pysypt-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysypt"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider."
 readme = "README.md"
 requires-python = ">=3.11"
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 3339 bytes, number of entries: 6
-drwxr-xr-x  2.0 unx        0 b- defN 24-May-06 14:23 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 24-May-06 14:23 META-INF/MANIFEST.MF
--rw-r--r--  2.0 unx     2718 b- defN 24-May-06 14:23 Args.class
--rw-r--r--  2.0 unx       36 b- defN 24-May-06 14:23 META-INF/encryption-app.kotlin_module
--rw-r--r--  2.0 unx     1108 b- defN 24-May-06 14:23 EncryptorEntryPoint.class
--rw-r--r--  2.0 unx     1120 b- defN 24-May-06 14:23 MainKt.class
+drwxr-xr-x  2.0 unx        0 b- defN 24-May-06 14:46 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 24-May-06 14:46 META-INF/MANIFEST.MF
+-rw-r--r--  2.0 unx     2718 b- defN 24-May-06 14:46 Args.class
+-rw-r--r--  2.0 unx       36 b- defN 24-May-06 14:46 META-INF/encryption-app.kotlin_module
+-rw-r--r--  2.0 unx     1108 b- defN 24-May-06 14:46 EncryptorEntryPoint.class
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-06 14:46 MainKt.class
 6 files, 5007 bytes uncompressed, 2635 bytes compressed:  47.4%
```

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar` & `pysypt-1.0.2/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-1.0.1/src/pysypt.egg-info/PKG-INFO` & `pysypt-1.0.2/src/pysypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysypt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # pysypt
 
 Python wrapper around [jasypt](http://www.jasypt.org/) for encrypting and decrypting strings using the BouncyCastle
```

### Comparing `pysypt-1.0.1/src/pysypt.egg-info/SOURCES.txt` & `pysypt-1.0.2/src/pysypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

