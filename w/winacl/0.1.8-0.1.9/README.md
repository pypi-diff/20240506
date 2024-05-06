# Comparing `tmp/winacl-0.1.8.tar.gz` & `tmp/winacl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winacl-0.1.8.tar", last modified: Tue Oct 24 16:23:58 2023, max compression
+gzip compressed data, was "winacl-0.1.9.tar", last modified: Mon May  6 07:23:13 2024, max compression
```

## Comparing `winacl-0.1.8.tar` & `winacl-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.574349 winacl-0.1.8/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-03-05 19:48:16.000000 winacl-0.1.8/LICENSE
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       26 2023-03-05 19:48:16.000000 winacl-0.1.8/MANIFEST.in
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      418 2023-10-24 16:23:58.574349 winacl-0.1.8/PKG-INFO
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       83 2023-03-05 19:48:16.000000 winacl-0.1.8/README.md
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:16.000000 winacl-0.1.8/pyproject.toml
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-10-24 16:23:58.574349 winacl-0.1.8/setup.cfg
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1192 2023-03-05 19:48:16.000000 winacl-0.1.8/setup.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.570349 winacl-0.1.8/winacl/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      127 2023-10-24 12:29:05.000000 winacl-0.1.8/winacl/_version.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.570349 winacl-0.1.8/winacl/dtyp/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)   166082 2023-10-24 16:21:19.000000 winacl-0.1.8/winacl/dtyp/ace.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4721 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/acl.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1116 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/guid.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    13161 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/security_descriptor.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    20438 2023-10-24 11:09:59.000000 winacl-0.1.8/winacl/dtyp/sid.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.570349 winacl-0.1.8/winacl/dtyp/wcee/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/wcee/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      711 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/wcee/backupkey.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      847 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/wcee/ecdhprivkey.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2366 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/wcee/pvkfile.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2033 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/dtyp/wcee/rsaprivkey.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.570349 winacl-0.1.8/winacl/examples/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/examples/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3498 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/examples/serviceacl.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      133 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/examples/userinfo.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.574349 winacl-0.1.8/winacl/functions/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    33059 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/advapi32.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      967 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/constants.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    23612 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/defines.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1326 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/dnsapi.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     7541 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/highlevel.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2902 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/kernel32.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      805 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/membuff.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3150 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/netapi32.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3607 2023-10-24 11:14:20.000000 winacl-0.1.8/winacl/functions/rights_calc.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1195 2023-03-05 19:48:16.000000 winacl-0.1.8/winacl/functions/winregistry.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-10-24 16:23:58.570349 winacl-0.1.8/winacl.egg-info/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      418 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/PKG-INFO
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      960 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/SOURCES.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/dependency_links.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       21 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/requires.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        7 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/top_level.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-10-24 16:23:58.000000 winacl-0.1.8/winacl.egg-info/zip-safe
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.448026 winacl-0.1.9/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-12-28 12:44:03.000000 winacl-0.1.9/LICENSE
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       26 2023-12-28 12:44:03.000000 winacl-0.1.9/MANIFEST.in
+-rw-r--r--   0 webdev    (1000) webdev    (1000)      454 2024-05-06 07:23:13.448026 winacl-0.1.9/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      455 2023-12-28 12:44:03.000000 winacl-0.1.9/README.md
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-12-28 12:44:03.000000 winacl-0.1.9/pyproject.toml
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2024-05-06 07:23:13.448026 winacl-0.1.9/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1192 2023-12-28 12:44:03.000000 winacl-0.1.9/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.440026 winacl-0.1.9/winacl/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      127 2024-04-28 17:34:07.000000 winacl-0.1.9/winacl/_version.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.444026 winacl-0.1.9/winacl/dtyp/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)   166082 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/ace.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4721 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/acl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1116 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/guid.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13161 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/security_descriptor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20438 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/sid.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.444026 winacl-0.1.9/winacl/dtyp/wcee/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3525 2024-05-06 06:45:23.000000 winacl-0.1.9/winacl/dtyp/wcee/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      711 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/wcee/backupkey.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5072 2024-05-06 05:22:16.000000 winacl-0.1.9/winacl/dtyp/wcee/cryptoapikey.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1948 2024-05-06 06:26:59.000000 winacl-0.1.9/winacl/dtyp/wcee/ecdhprivkey.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2366 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/dtyp/wcee/pvkfile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4291 2024-05-06 06:28:18.000000 winacl-0.1.9/winacl/dtyp/wcee/rsaprivkey.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.444026 winacl-0.1.9/winacl/examples/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/examples/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3498 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/examples/serviceacl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      133 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/examples/userinfo.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.448026 winacl-0.1.9/winacl/functions/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    33059 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/advapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      967 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23612 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/defines.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1326 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/dnsapi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7541 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/highlevel.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2902 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/kernel32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      805 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/membuff.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3150 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/netapi32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3607 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/rights_calc.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1195 2023-12-28 12:44:03.000000 winacl-0.1.9/winacl/functions/winregistry.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2024-05-06 07:23:13.448026 winacl-0.1.9/winacl.egg-info/
+-rw-r--r--   0 webdev    (1000) webdev    (1000)      454 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      993 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       21 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        7 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2024-05-06 07:23:13.000000 winacl-0.1.9/winacl.egg-info/zip-safe
```

### Comparing `winacl-0.1.8/LICENSE` & `winacl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/setup.py` & `winacl-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/ace.py` & `winacl-0.1.9/winacl/dtyp/ace.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/acl.py` & `winacl-0.1.9/winacl/dtyp/acl.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/guid.py` & `winacl-0.1.9/winacl/dtyp/guid.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/security_descriptor.py` & `winacl-0.1.9/winacl/dtyp/security_descriptor.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/sid.py` & `winacl-0.1.9/winacl/dtyp/sid.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/wcee/backupkey.py` & `winacl-0.1.9/winacl/dtyp/wcee/backupkey.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/dtyp/wcee/pvkfile.py` & `winacl-0.1.9/winacl/dtyp/wcee/pvkfile.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/examples/serviceacl.py` & `winacl-0.1.9/winacl/examples/serviceacl.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/advapi32.py` & `winacl-0.1.9/winacl/functions/advapi32.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/constants.py` & `winacl-0.1.9/winacl/functions/constants.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/defines.py` & `winacl-0.1.9/winacl/functions/defines.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/dnsapi.py` & `winacl-0.1.9/winacl/functions/dnsapi.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/highlevel.py` & `winacl-0.1.9/winacl/functions/highlevel.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/kernel32.py` & `winacl-0.1.9/winacl/functions/kernel32.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/membuff.py` & `winacl-0.1.9/winacl/functions/membuff.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/netapi32.py` & `winacl-0.1.9/winacl/functions/netapi32.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/rights_calc.py` & `winacl-0.1.9/winacl/functions/rights_calc.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl/functions/winregistry.py` & `winacl-0.1.9/winacl/functions/winregistry.py`

 * *Files identical despite different names*

### Comparing `winacl-0.1.8/winacl.egg-info/SOURCES.txt` & `winacl-0.1.9/winacl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 winacl/dtyp/ace.py
 winacl/dtyp/acl.py
 winacl/dtyp/guid.py
 winacl/dtyp/security_descriptor.py
 winacl/dtyp/sid.py
 winacl/dtyp/wcee/__init__.py
 winacl/dtyp/wcee/backupkey.py
+winacl/dtyp/wcee/cryptoapikey.py
 winacl/dtyp/wcee/ecdhprivkey.py
 winacl/dtyp/wcee/pvkfile.py
 winacl/dtyp/wcee/rsaprivkey.py
 winacl/examples/__init__.py
 winacl/examples/serviceacl.py
 winacl/examples/userinfo.py
 winacl/functions/__init__.py
```

