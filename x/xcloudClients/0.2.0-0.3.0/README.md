# Comparing `tmp/xcloudClients-0.2.0.tar.gz` & `tmp/xcloudClients-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcloudClients-0.2.0.tar", last modified: Sun May  5 09:41:01 2024, max compression
+gzip compressed data, was "xcloudClients-0.3.0.tar", last modified: Sun May  5 15:36:27 2024, max compression
```

## Comparing `xcloudClients-0.2.0.tar` & `xcloudClients-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 09:41:01.268992 xcloudClients-0.2.0/
--rw-rw-rw-   0        0        0       37 2024-05-05 09:12:00.000000 xcloudClients-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      566 2024-05-05 09:41:01.266992 xcloudClients-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-05 08:48:43.000000 xcloudClients-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 09:41:01.268992 xcloudClients-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-05-05 09:40:01.000000 xcloudClients-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:41:01.212993 xcloudClients-0.2.0/xcloudClients/
--rw-rw-rw-   0        0        0      539 2024-05-05 09:39:46.000000 xcloudClients-0.2.0/xcloudClients/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:41:01.262993 xcloudClients-0.2.0/xcloudClients/resources/
--rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudClients-0.2.0/xcloudClients/resources/XCloudJDBC-2.10.6.7.jar
--rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudClients-0.2.0/xcloudClients/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
--rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudClients-0.2.0/xcloudClients/resources/libthrift-0.9.2.jar
--rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudClients-0.2.0/xcloudClients/resources/log4j-1.2.17.jar
--rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudClients-0.2.0/xcloudClients/resources/lz4-1.3.0.jar
--rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudClients-0.2.0/xcloudClients/resources/slf4j-api-1.7.5.jar
--rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudClients-0.2.0/xcloudClients/resources/slf4j-log4j12-1.7.5.jar
--rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudClients-0.2.0/xcloudClients/resources/slf4j-simple-1.7.5.jar
--rw-rw-rw-   0        0        0     8520 2024-05-05 09:06:58.000000 xcloudClients-0.2.0/xcloudClients/xcloudClients.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:41:01.229994 xcloudClients-0.2.0/xcloudClients.egg-info/
--rw-rw-rw-   0        0        0      566 2024-05-05 09:41:00.000000 xcloudClients-0.2.0/xcloudClients.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2024-05-05 09:41:01.000000 xcloudClients-0.2.0/xcloudClients.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 09:41:00.000000 xcloudClients-0.2.0/xcloudClients.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-05 09:41:00.000000 xcloudClients-0.2.0/xcloudClients.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 09:41:00.000000 xcloudClients-0.2.0/xcloudClients.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 15:36:27.982788 xcloudClients-0.3.0/
+-rw-rw-rw-   0        0        0       37 2024-05-05 09:12:00.000000 xcloudClients-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      566 2024-05-05 15:36:27.980785 xcloudClients-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-05 08:48:43.000000 xcloudClients-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:36:27.982788 xcloudClients-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      685 2024-05-05 15:35:03.000000 xcloudClients-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:36:27.921820 xcloudClients-0.3.0/xcloudClients/
+-rw-rw-rw-   0        0        0      539 2024-05-05 15:35:11.000000 xcloudClients-0.3.0/xcloudClients/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:36:27.977800 xcloudClients-0.3.0/xcloudClients/resources/
+-rw-rw-rw-   0        0        0  1358472 2021-10-15 08:05:30.000000 xcloudClients-0.3.0/xcloudClients/resources/XCloudJDBC-2.10.6.7.jar
+-rw-rw-rw-   0        0        0   275539 2021-10-15 08:05:26.000000 xcloudClients-0.3.0/xcloudClients/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar
+-rw-rw-rw-   0        0        0   227712 2019-07-16 09:51:20.000000 xcloudClients-0.3.0/xcloudClients/resources/libthrift-0.9.2.jar
+-rw-rw-rw-   0        0        0   489884 2019-07-16 09:51:20.000000 xcloudClients-0.3.0/xcloudClients/resources/log4j-1.2.17.jar
+-rw-rw-rw-   0        0        0   236880 2019-07-16 09:51:20.000000 xcloudClients-0.3.0/xcloudClients/resources/lz4-1.3.0.jar
+-rw-rw-rw-   0        0        0    26084 2018-10-10 07:16:32.000000 xcloudClients-0.3.0/xcloudClients/resources/slf4j-api-1.7.5.jar
+-rw-rw-rw-   0        0        0     8869 2021-10-15 08:05:28.000000 xcloudClients-0.3.0/xcloudClients/resources/slf4j-log4j12-1.7.5.jar
+-rw-rw-rw-   0        0        0    10680 2019-09-11 10:52:28.000000 xcloudClients-0.3.0/xcloudClients/resources/slf4j-simple-1.7.5.jar
+-rw-rw-rw-   0        0        0     8513 2024-05-05 15:33:29.000000 xcloudClients-0.3.0/xcloudClients/xcloudClients.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:36:27.938782 xcloudClients-0.3.0/xcloudClients.egg-info/
+-rw-rw-rw-   0        0        0      566 2024-05-05 15:36:26.000000 xcloudClients-0.3.0/xcloudClients.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2024-05-05 15:36:27.000000 xcloudClients-0.3.0/xcloudClients.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:36:26.000000 xcloudClients-0.3.0/xcloudClients.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-05 15:36:27.000000 xcloudClients-0.3.0/xcloudClients.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 15:36:27.000000 xcloudClients-0.3.0/xcloudClients.egg-info/top_level.txt
```

### Comparing `xcloudClients-0.2.0/PKG-INFO` & `xcloudClients-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudClients
-Version: 0.2.0
+Version: 0.3.0
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudClients-0.2.0/xcloudClients/__init__.py` & `xcloudClients-0.3.0/xcloudClients/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2'
+__version__ = '0.3'
 __author__ = 'bailu'
 __com__ = 'China telecom Shannxi'
 __mail__ = 'yabailu@chinatelecom.cn'
 __tel__ = '15399117834'
 
 
 import pkg_resources
```

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/XCloudJDBC-2.10.6.7.jar` & `xcloudClients-0.3.0/xcloudClients/resources/XCloudJDBC-2.10.6.7.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar` & `xcloudClients-0.3.0/xcloudClients/resources/XCloudJDBC_SP_Procedure_Parser-0.1.3.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/libthrift-0.9.2.jar` & `xcloudClients-0.3.0/xcloudClients/resources/libthrift-0.9.2.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/log4j-1.2.17.jar` & `xcloudClients-0.3.0/xcloudClients/resources/log4j-1.2.17.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/lz4-1.3.0.jar` & `xcloudClients-0.3.0/xcloudClients/resources/lz4-1.3.0.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/slf4j-api-1.7.5.jar` & `xcloudClients-0.3.0/xcloudClients/resources/slf4j-api-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/slf4j-log4j12-1.7.5.jar` & `xcloudClients-0.3.0/xcloudClients/resources/slf4j-log4j12-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/resources/slf4j-simple-1.7.5.jar` & `xcloudClients-0.3.0/xcloudClients/resources/slf4j-simple-1.7.5.jar`

 * *Files identical despite different names*

### Comparing `xcloudClients-0.2.0/xcloudClients/xcloudClients.py` & `xcloudClients-0.3.0/xcloudClients/xcloudClients.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import jpype.imports
 from jpype.types import *
 import atexit
 
 
 def start_jvm():
     if not jpype.isJVMStarted():
-        jpype.startJVM(classpath=["./resources/*"])
+        jpype.startJVM(classpath= JAR_FILES)
         atexit.register(jpype.shutdownJVM)
 
 # 确保 JVM 在程序结束时正确关闭
 
 start_jvm()  # 在程序启动时调用
 
 class DatabaseClient:
```

### Comparing `xcloudClients-0.2.0/xcloudClients.egg-info/PKG-INFO` & `xcloudClients-0.3.0/xcloudClients.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcloudClients
-Version: 0.2.0
+Version: 0.3.0
 Summary: 这是一个国信行云数据库并发查询python程序,主要应用于自动通报
 Home-page: https://github.com/bailulue
 Author: bailu
 Author-email: yabailu@chinatelecom.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xcloudClients-0.2.0/xcloudClients.egg-info/SOURCES.txt` & `xcloudClients-0.3.0/xcloudClients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

