# Comparing `tmp/DFRobotUPS-0.4.3.tar.gz` & `tmp/DFRobotUPS-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.4.3.tar", last modified: Tue Apr 23 00:37:33 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.4.4.tar", last modified: Mon May  6 10:35:02 2024, max compression
```

## Comparing `DFRobotUPS-0.4.3.tar` & `DFRobotUPS-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-04-23 00:35:59.000000 DFRobotUPS-0.4.3/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6347 2024-04-23 00:35:19.000000 DFRobotUPS-0.4.3/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-22 21:59:25.000000 DFRobotUPS-0.4.3/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:37:33.736415 DFRobotUPS-0.4.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-23 00:37:33.736415 DFRobotUPS-0.4.3/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 10:35:02.491160 DFRobotUPS-0.4.4/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 10:35:02.487160 DFRobotUPS-0.4.4/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-05-06 10:31:23.000000 DFRobotUPS-0.4.4/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6376 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.4/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.4/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 10:35:02.487160 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-05-06 10:35:02.000000 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-05-06 10:35:02.000000 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-06 10:35:02.000000 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-06 10:35:02.000000 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-05-06 10:35:02.000000 DFRobotUPS-0.4.4/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.4/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-05-06 10:35:02.491160 DFRobotUPS-0.4.4/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.4/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-05-06 10:35:02.491160 DFRobotUPS-0.4.4/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.4/setup.py
```

### Comparing `DFRobotUPS-0.4.3/DFRobotUPS/__main__.py` & `DFRobotUPS-0.4.4/DFRobotUPS/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
          f" {MIN_INTERVAL}, max: {MAX_INTERVAL}, default:"
          f" {DEFAULT_INTERVAL})")
 
 parser.add_argument(
     "-c", "--cmd",
     nargs="+",
     default=("/sbin/halt", ),
+    metavar=("CMD", "ARG"),
     help="command to run to trigger shutdown")
 
 parser.add_argument(
     "-a", "--addr",
     type=functools.partial(int, base=0),
     default=DEFAULT_ADDR,
     help="I2C address for UPS HAT; can be specified in hex as 0xNN"
@@ -202,15 +203,15 @@
 
     sys.exit(1)
 
 
 # log some information about the UPS and, if we're debugging print it
 # there too
 
-logger.info(f"UPS HAT found with product ID 0x{ups.pid:02x} firmware"
+logger.info(f"UPS HAT found with product ID 0x{ups.pid:02x}, firmware"
             + (" version %d.%d" % ups.fwver))
 
 
 # if we're in shutdown polling mode, do that
 
 if args.shutdown:
     logger.info(
```

### Comparing `DFRobotUPS-0.4.3/DFRobotUPS/ups.py` & `DFRobotUPS-0.4.4/DFRobotUPS/ups.py`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.3/DFRobotUPS.egg-info/PKG-INFO` & `DFRobotUPS-0.4.4/DFRobotUPS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4.3
+Version: 0.4.4
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4.3/LICENSE` & `DFRobotUPS-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.3/PKG-INFO` & `DFRobotUPS-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4.3
+Version: 0.4.4
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4.3/README.md` & `DFRobotUPS-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.3/setup.py` & `DFRobotUPS-0.4.4/setup.py`

 * *Files identical despite different names*

