# Comparing `tmp/pysharek-0.11.1.tar.gz` & `tmp/pysharek-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysharek-0.11.1.tar", last modified: Mon May  6 10:36:57 2024, max compression
+gzip compressed data, was "pysharek-0.12.0.tar", last modified: Mon May  6 11:17:00 2024, max compression
```

## Comparing `pysharek-0.11.1.tar` & `pysharek-0.12.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.456393 pysharek-0.11.1/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2024-04-18 18:14:26.000000 pysharek-0.11.1/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 10:36:57.456393 pysharek-0.11.1/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2024-04-18 18:14:26.000000 pysharek-0.11.1/README.md
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1011 2024-04-18 18:14:26.000000 pysharek-0.11.1/pyproject.toml
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.455393 pysharek-0.11.1/pysharek/
--rw-r--r--   0 the220th  (1000) the220th  (1000)       63 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-28 07:38:11.000000 pysharek-0.11.1/pysharek/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 10:33:47.000000 pysharek-0.11.1/pysharek/__version__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2811 2024-05-06 09:54:03.000000 pysharek-0.11.1/pysharek/args.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     8657 2024-05-06 10:19:40.000000 pysharek-0.11.1/pysharek/crypto.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/hashes_work.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      969 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/main.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/net.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     4355 2024-05-06 10:35:25.000000 pysharek-0.11.1/pysharek/sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    18112 2024-05-06 10:30:30.000000 pysharek-0.11.1/pysharek/work.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.456393 pysharek-0.11.1/pysharek.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      418 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-06 10:36:57.456393 pysharek-0.11.1/setup.cfg
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 11:17:00.382813 pysharek-0.12.0/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2024-04-18 18:14:26.000000 pysharek-0.12.0/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 11:17:00.382813 pysharek-0.12.0/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2024-04-18 18:14:26.000000 pysharek-0.12.0/README.md
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1011 2024-04-18 18:14:26.000000 pysharek-0.12.0/pyproject.toml
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 11:17:00.381813 pysharek-0.12.0/pysharek/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       63 2024-04-18 18:14:26.000000 pysharek-0.12.0/pysharek/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-28 07:38:11.000000 pysharek-0.12.0/pysharek/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 11:00:56.000000 pysharek-0.12.0/pysharek/__version__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2811 2024-05-06 09:54:03.000000 pysharek-0.12.0/pysharek/args.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     8657 2024-05-06 10:19:40.000000 pysharek-0.12.0/pysharek/crypto.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-18 18:14:26.000000 pysharek-0.12.0/pysharek/hashes_work.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      969 2024-04-18 18:14:26.000000 pysharek-0.12.0/pysharek/main.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2024-04-18 18:14:26.000000 pysharek-0.12.0/pysharek/net.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     4355 2024-05-06 10:35:25.000000 pysharek-0.12.0/pysharek/sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     3911 2024-05-06 11:15:40.000000 pysharek-0.12.0/pysharek/vs_man_on_middle.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    18169 2024-05-06 11:14:20.000000 pysharek-0.12.0/pysharek/work.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 11:17:00.382813 pysharek-0.12.0/pysharek.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      447 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-05-06 11:17:00.000000 pysharek-0.12.0/pysharek.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-06 11:17:00.382813 pysharek-0.12.0/setup.cfg
```

### Comparing `pysharek-0.11.1/LICENSE` & `pysharek-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/PKG-INFO` & `pysharek-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.11.1
+Version: 0.12.0
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pysharek-0.11.1/pyproject.toml` & `pysharek-0.12.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/args.py` & `pysharek-0.12.0/pysharek/args.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/crypto.py` & `pysharek-0.12.0/pysharek/crypto.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/hashes_work.py` & `pysharek-0.12.0/pysharek/hashes_work.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/main.py` & `pysharek-0.12.0/pysharek/main.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/net.py` & `pysharek-0.12.0/pysharek/net.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/sup.py` & `pysharek-0.12.0/pysharek/sup.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.11.1/pysharek/work.py` & `pysharek-0.12.0/pysharek/work.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 import time
 import traceback
 
 from .sup import *
 from .net import *
 from .hashes_work import calc_hash_file
 from .hashes_work import calc_hash_dir
-from .sup import get_dirs_needed_for_files
 from .crypto import transfer_shared_key
 
+from .vs_man_on_middle import challenge_with_words
+
 
 def work_as_sender(args: "argparse.Namespace"):
     # python -m pysharek --mode send --connect server --port 1337
     #                           --password 123 /tmp/123.mp4 --log_file /tmp/log2.txt --log_debug
     plog("I am sender", 1)
     common_block_of_sender_and_receiver(args)
     file = Global.file_dir
@@ -382,14 +383,15 @@
                 socket_close(sock)
                 exit()
             else:
                 send_msg(sock, {"key_exchange": "2"}, Global.pub_key)
         Global.pub_key_2 = pub_key_2
         Global.shared_key = Global.priv_key.exchange(X448PublicKey.from_public_bytes(Global.pub_key_2))
         Global.shared_key = transfer_shared_key(Global.shared_key)
+        challenge_with_words(Global.shared_key)
         Global.cipher.set_password(Global.shared_key)
     else:
         Global.cipher.set_password(args.password)
     Global.cipher.start()
 
     plog(f"Inited cipher in common part", 1)
```

### Comparing `pysharek-0.11.1/pysharek.egg-info/PKG-INFO` & `pysharek-0.12.0/pysharek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.11.1
+Version: 0.12.0
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

