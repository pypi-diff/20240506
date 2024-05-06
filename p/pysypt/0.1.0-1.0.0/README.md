# Comparing `tmp/pysypt-0.1.0.tar.gz` & `tmp/pysypt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysypt-0.1.0.tar", last modified: Wed Oct 25 12:03:02 2023, max compression
+gzip compressed data, was "pysypt-1.0.0.tar", last modified: Mon May  6 11:52:29 2024, max compression
```

## Comparing `pysypt-0.1.0.tar` & `pysypt-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.216399 pysypt-0.1.0/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 11:39:00.000000 pysypt-0.1.0/MANIFEST.in
--rw-r--r--   0 fabianberinger   (501) staff       (20)      996 2023-10-25 12:03:02.216201 pysypt-0.1.0/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)      772 2023-10-25 11:39:00.000000 pysypt-0.1.0/README.md
--rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2023-10-25 11:55:26.000000 pysypt-0.1.0/pyproject.toml
--rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2023-10-25 12:03:02.216444 pysypt-0.1.0/setup.cfg
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.208042 pysypt-0.1.0/src/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.207638 pysypt-0.1.0/src/java/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.207692 pysypt-0.1.0/src/java/encryption-app/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.207740 pysypt-0.1.0/src/java/encryption-app/build/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.207789 pysypt-0.1.0/src/java/encryption-app/build/distributions/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.207910 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.208697 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8836 2023-10-25 12:02:56.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
--rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3188 2023-10-25 12:02:56.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.214561 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
--rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-07-04 10:19:08.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2023-10-24 14:27:24.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)     6621 2023-10-25 12:02:56.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-07-04 14:36:00.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
--rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2023-10-24 13:43:52.000000 pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.215267 pysypt-0.1.0/src/pysypt/
--rw-r--r--   0 fabianberinger   (501) staff       (20)       70 2023-10-25 11:21:00.000000 pysypt-0.1.0/src/pysypt/__init__.py
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1417 2023-10-25 11:44:41.000000 pysypt-0.1.0/src/pysypt/encryption.py
-drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2023-10-25 12:03:02.215953 pysypt-0.1.0/src/pysypt.egg-info/
--rw-r--r--   0 fabianberinger   (501) staff       (20)      996 2023-10-25 12:03:02.000000 pysypt-0.1.0/src/pysypt.egg-info/PKG-INFO
--rw-r--r--   0 fabianberinger   (501) staff       (20)     1418 2023-10-25 12:03:02.000000 pysypt-0.1.0/src/pysypt.egg-info/SOURCES.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2023-10-25 12:03:02.000000 pysypt-0.1.0/src/pysypt.egg-info/dependency_links.txt
--rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2023-10-25 12:03:02.000000 pysypt-0.1.0/src/pysypt.egg-info/top_level.txt
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.079297 pysypt-1.0.0/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       85 2023-10-25 12:03:35.000000 pysypt-1.0.0/MANIFEST.in
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1318 2024-05-06 11:52:29.079111 pysypt-1.0.0/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1093 2024-05-06 11:51:55.000000 pysypt-1.0.0/README.md
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      689 2024-05-06 11:47:46.000000 pysypt-1.0.0/pyproject.toml
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       38 2024-05-06 11:52:29.079335 pysypt-1.0.0/setup.cfg
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072135 pysypt-1.0.0/src/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071777 pysypt-1.0.0/src/java/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071823 pysypt-1.0.0/src/java/encryption-app/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071865 pysypt-1.0.0/src/java/encryption-app/build/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.071914 pysypt-1.0.0/src/java/encryption-app/build/distributions/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072021 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.072747 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     8868 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app
+-rwxr-xr-x   0 fabianberinger   (501) staff       (20)     3221 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078152 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    17536 2023-12-18 12:41:30.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  5743920 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     4933 2024-05-06 11:52:24.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   142255 2023-12-18 12:43:10.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    89638 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)  1708006 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   225141 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      958 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)      963 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)   124506 2024-05-06 10:11:56.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
+-rw-r--r--   0 fabianberinger   (501) staff       (20)    12890 2024-05-06 09:44:04.000000 pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078383 pysypt-1.0.0/src/pysypt/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       69 2024-05-06 11:47:46.000000 pysypt-1.0.0/src/pysypt/__init__.py
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1564 2024-05-06 11:38:32.000000 pysypt-1.0.0/src/pysypt/encryption.py
+drwxr-xr-x   0 fabianberinger   (501) staff       (20)        0 2024-05-06 11:52:29.078925 pysypt-1.0.0/src/pysypt.egg-info/
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1318 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/PKG-INFO
+-rw-r--r--   0 fabianberinger   (501) staff       (20)     1512 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/SOURCES.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)        1 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/dependency_links.txt
+-rw-r--r--   0 fabianberinger   (501) staff       (20)       12 2024-05-06 11:52:29.000000 pysypt-1.0.0/src/pysypt.egg-info/top_level.txt
```

### Comparing `pysypt-0.1.0/pyproject.toml` & `pysypt-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysypt"
-version = "0.1.0"
+version = "1.0.0"
 description = "Python wrapper around jasypt for encrypting and decrypting strings using the BouncyCastle Provider."
 readme = "README.md"
 requires-python = ">=3.11"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 case "$( uname )" in                #(
   CYGWIN* )         cygwin=true  ;; #(
   Darwin* )         darwin=true  ;; #(
   MSYS* | MINGW* )  msys=true    ;; #(
   NONSTOP* )        nonstop=true ;;
 esac
 
-CLASSPATH=$APP_HOME/lib/encryption-app-1.0-SNAPSHOT.jar:$APP_HOME/lib/kotlin-stdlib-jdk8-1.9.0.jar:$APP_HOME/lib/bcprov-jdk15on-1.69.jar:$APP_HOME/lib/jasypt-1.9.3.jar:$APP_HOME/lib/kotlin-argparser-2.0.7.jar:$APP_HOME/lib/kotlin-stdlib-jdk7-1.9.0.jar:$APP_HOME/lib/xenocom-0.0.7.jar:$APP_HOME/lib/kotlin-stdlib-1.9.0.jar:$APP_HOME/lib/kotlin-stdlib-common-1.9.0.jar:$APP_HOME/lib/annotations-13.0.jar
+CLASSPATH=$APP_HOME/lib/encryption-app-1.0-SNAPSHOT.jar:$APP_HOME/lib/kotlin-stdlib-jdk8-1.9.0.jar:$APP_HOME/lib/bcprov-jdk15on-1.69.jar:$APP_HOME/lib/jasypt-1.9.3.jar:$APP_HOME/lib/kotlin-argparser-2.0.7.jar:$APP_HOME/lib/py4j-0.10.9.7.jar:$APP_HOME/lib/kotlin-stdlib-jdk7-1.9.0.jar:$APP_HOME/lib/xenocom-0.0.7.jar:$APP_HOME/lib/kotlin-stdlib-1.9.0.jar:$APP_HOME/lib/kotlin-stdlib-common-1.9.0.jar:$APP_HOME/lib/annotations-13.0.jar
 
 
 # Determine the Java command to use to start the JVM.
 if [ -n "$JAVA_HOME" ] ; then
     if [ -x "$JAVA_HOME/jre/sh/java" ] ; then
         # IBM's JDK on AIX uses strange locations for the executables
         JAVACMD=$JAVA_HOME/jre/sh/java
```

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/bin/encryption-app.bat`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 echo location of your Java installation.
 
 goto fail
 
 :execute
 @rem Setup the command line
 
-set CLASSPATH=%APP_HOME%\lib\encryption-app-1.0-SNAPSHOT.jar;%APP_HOME%\lib\kotlin-stdlib-jdk8-1.9.0.jar;%APP_HOME%\lib\bcprov-jdk15on-1.69.jar;%APP_HOME%\lib\jasypt-1.9.3.jar;%APP_HOME%\lib\kotlin-argparser-2.0.7.jar;%APP_HOME%\lib\kotlin-stdlib-jdk7-1.9.0.jar;%APP_HOME%\lib\xenocom-0.0.7.jar;%APP_HOME%\lib\kotlin-stdlib-1.9.0.jar;%APP_HOME%\lib\kotlin-stdlib-common-1.9.0.jar;%APP_HOME%\lib\annotations-13.0.jar
+set CLASSPATH=%APP_HOME%\lib\encryption-app-1.0-SNAPSHOT.jar;%APP_HOME%\lib\kotlin-stdlib-jdk8-1.9.0.jar;%APP_HOME%\lib\bcprov-jdk15on-1.69.jar;%APP_HOME%\lib\jasypt-1.9.3.jar;%APP_HOME%\lib\kotlin-argparser-2.0.7.jar;%APP_HOME%\lib\py4j-0.10.9.7.jar;%APP_HOME%\lib\kotlin-stdlib-jdk7-1.9.0.jar;%APP_HOME%\lib\xenocom-0.0.7.jar;%APP_HOME%\lib\kotlin-stdlib-1.9.0.jar;%APP_HOME%\lib\kotlin-stdlib-common-1.9.0.jar;%APP_HOME%\lib\annotations-13.0.jar
 
 
 @rem Execute encryption-app
 "%JAVA_EXE%" %DEFAULT_JVM_OPTS% %JAVA_OPTS% %ENCRYPTION_APP_OPTS%  -classpath "%CLASSPATH%" MainKt %*
 
 :end
 @rem End local scope for the variables with windows NT shell
```

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/annotations-13.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/bcprov-jdk15on-1.69.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar` & `pysypt-1.0.0/src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar`

 * *Files identical despite different names*

### Comparing `pysypt-0.1.0/src/pysypt.egg-info/SOURCES.txt` & `pysypt-1.0.0/src/pysypt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/encryption-app-1.0-SNAPSHOT.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/jasypt-1.9.3.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-argparser-2.0.7.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-1.9.0.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-common-1.9.0.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk7-1.9.0.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/kotlin-stdlib-jdk8-1.9.0.jar
+src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/py4j-0.10.9.7.jar
 src/java/encryption-app/build/distributions/encryption-app-1.0-SNAPSHOT/lib/xenocom-0.0.7.jar
 src/pysypt/__init__.py
 src/pysypt/encryption.py
 src/pysypt.egg-info/PKG-INFO
 src/pysypt.egg-info/SOURCES.txt
 src/pysypt.egg-info/dependency_links.txt
 src/pysypt.egg-info/top_level.txt
```

