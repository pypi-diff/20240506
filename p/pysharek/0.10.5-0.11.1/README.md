# Comparing `tmp/pysharek-0.10.5.tar.gz` & `tmp/pysharek-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysharek-0.10.5.tar", last modified: Thu Apr 18 18:48:19 2024, max compression
+gzip compressed data, was "pysharek-0.11.1.tar", last modified: Mon May  6 10:36:57 2024, max compression
```

## Comparing `pysharek-0.10.5.tar` & `pysharek-0.11.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:48:19.760622 pysharek-0.10.5/
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2024-04-18 18:14:26.000000 pysharek-0.10.5/LICENSE
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-18 18:48:19.760622 pysharek-0.10.5/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2024-04-18 18:14:26.000000 pysharek-0.10.5/README.md
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1011 2024-04-18 18:14:26.000000 pysharek-0.10.5/pyproject.toml
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:48:19.759621 pysharek-0.10.5/pysharek/
--rw-r--r--   0 the220th  (1000) the220th  (1000)       63 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/__init__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/__main__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-04-18 18:48:09.000000 pysharek-0.10.5/pysharek/__version__.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     2810 2024-04-18 18:48:09.000000 pysharek-0.10.5/pysharek/args.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     6799 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/crypto.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/hashes_work.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)      969 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/main.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2024-04-18 18:14:26.000000 pysharek-0.10.5/pysharek/net.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)     4138 2024-04-18 18:48:09.000000 pysharek-0.10.5/pysharek/sup.py
--rw-r--r--   0 the220th  (1000) the220th  (1000)    16446 2024-04-18 18:48:09.000000 pysharek-0.10.5/pysharek/work.py
-drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-04-18 18:48:19.760622 pysharek-0.10.5/pysharek.egg-info/
--rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/PKG-INFO
--rw-r--r--   0 the220th  (1000) the220th  (1000)      418 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/SOURCES.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/dependency_links.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/entry_points.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/requires.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-04-18 18:48:19.000000 pysharek-0.10.5/pysharek.egg-info/top_level.txt
--rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-04-18 18:48:19.760622 pysharek-0.10.5/setup.cfg
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.456393 pysharek-0.11.1/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1066 2024-04-18 18:14:26.000000 pysharek-0.11.1/LICENSE
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 10:36:57.456393 pysharek-0.11.1/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      103 2024-04-18 18:14:26.000000 pysharek-0.11.1/README.md
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1011 2024-04-18 18:14:26.000000 pysharek-0.11.1/pyproject.toml
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.455393 pysharek-0.11.1/pysharek/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       63 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/__init__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      390 2024-04-28 07:38:11.000000 pysharek-0.11.1/pysharek/__main__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 10:33:47.000000 pysharek-0.11.1/pysharek/__version__.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     2811 2024-05-06 09:54:03.000000 pysharek-0.11.1/pysharek/args.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     8657 2024-05-06 10:19:40.000000 pysharek-0.11.1/pysharek/crypto.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     1512 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/hashes_work.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      969 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/main.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     5646 2024-04-18 18:14:26.000000 pysharek-0.11.1/pysharek/net.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)     4355 2024-05-06 10:35:25.000000 pysharek-0.11.1/pysharek/sup.py
+-rw-r--r--   0 the220th  (1000) the220th  (1000)    18112 2024-05-06 10:30:30.000000 pysharek-0.11.1/pysharek/work.py
+drwxr-xr-x   0 the220th  (1000) the220th  (1000)        0 2024-05-06 10:36:57.456393 pysharek-0.11.1/pysharek.egg-info/
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      693 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/PKG-INFO
+-rw-r--r--   0 the220th  (1000) the220th  (1000)      418 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/SOURCES.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        1 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/dependency_links.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       48 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/entry_points.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       37 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/requires.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)        9 2024-05-06 10:36:57.000000 pysharek-0.11.1/pysharek.egg-info/top_level.txt
+-rw-r--r--   0 the220th  (1000) the220th  (1000)       38 2024-05-06 10:36:57.456393 pysharek-0.11.1/setup.cfg
```

### Comparing `pysharek-0.10.5/LICENSE` & `pysharek-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.5/PKG-INFO` & `pysharek-0.11.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.10.5
+Version: 0.11.1
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pysharek-0.10.5/pyproject.toml` & `pysharek-0.11.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.5/pysharek/args.py` & `pysharek-0.11.1/pysharek/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     parser.add_argument("--ip", type=str, default=None,
                         help="If connect=\"client\", define ip to connect")
 
     parser.add_argument("--port", type=int, required=True,
                         help="Define port for bind/connect")
 
-    parser.add_argument("--password", type=str, required=True,
+    parser.add_argument("--password", type=str, required=False,
                         help="Define password for encryption while transferring. "
                              "Password must be same for the sender and receiver")
     parser.add_argument("--yes", default=False, required=False, action="store_true",
                         help="Answer \"yes\" on any questions")
     parser.add_argument("--continue_from", type=str, required=False, default=None,
                         help="continue from {file}:{block}.")
```

### Comparing `pysharek-0.10.5/pysharek/crypto.py` & `pysharek-0.11.1/pysharek/crypto.py`

 * *Files 17% similar despite different names*

```diff
@@ -207,14 +207,18 @@
             c = 0
         c += 1
         i += 1
         j += 1
     return bytes(res)
 
 
+def transfer_shared_key(shared_key: bytes) -> str:
+    return hashlib.sha256(shared_key).hexdigest()
+
+
 def __test_salt():
     import random
     from alive_progress import alive_bar
     # v, k = 10**9, 256
     # v, k = 10**9, 10**3
     v, k = 10**9, 250000
     # v, k = 10**9, 10**6
@@ -242,10 +246,50 @@
             data_i = os.urandom(random.randint(k - 100, k + 100))
             data_en = cipher.encrypt(data_i)
             data_de = cipher.decrypt(data_en)
             assert data_i == data_de
             bar()
 
 
+def __test_key_exchange():
+    from cryptography.hazmat.primitives.asymmetric.x448 import X448PublicKey
+    from cryptography.hazmat.primitives.asymmetric.x448 import X448PrivateKey
+    from cryptography.hazmat.primitives import serialization
+
+    private_key1 = X448PrivateKey.generate()
+    public_key1 = private_key1.public_key()
+    public_key1_bytes = public_key1.public_bytes(encoding=serialization.Encoding.Raw,
+                                                 format=serialization.PublicFormat.Raw)
+    print(f"Pub key 1 bytes: {public_key1_bytes}")
+    public_key1_text = base64.b64encode(public_key1_bytes).decode("ascii")
+    print(f"Pub key 1: {public_key1_text}")
+
+    private_key2 = X448PrivateKey.generate()
+    public_key2 = private_key2.public_key()
+    public_key2_bytes = public_key2.public_bytes(encoding=serialization.Encoding.Raw,
+                                                 format=serialization.PublicFormat.Raw)
+
+    print(f"Pub key 2 bytes: {public_key2_bytes}")
+    public_key2_text = base64.b64encode(public_key2_bytes).decode("ascii")
+    print(f"Pub key 2: {public_key2_text}")
+
+    # =============================
+
+    pubkey1_bytes = base64.b64decode(public_key1_text.encode("ascii"))
+    pubkey1 = X448PublicKey.from_public_bytes(pubkey1_bytes)
+
+    pubkey2_bytes = base64.b64decode(public_key2_text.encode("ascii"))
+    pubkey2 = X448PublicKey.from_public_bytes(pubkey2_bytes)
+
+    shared_key1 = private_key2.exchange(pubkey1)
+    shared_key1 = base64.b64encode(shared_key1).decode("ascii")
+    print(f"shared_key1: {shared_key1}")
+
+    shared_key2 = private_key1.exchange(pubkey2)
+    shared_key2 = base64.b64encode(shared_key2).decode("ascii")
+    print(f"shared_key2: {shared_key2}")
+
+
 if __name__ == "__main__":
     # __test_salt()
-    __test_cipher()
+    # __test_cipher()
+    __test_key_exchange()
```

### Comparing `pysharek-0.10.5/pysharek/hashes_work.py` & `pysharek-0.11.1/pysharek/hashes_work.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.5/pysharek/main.py` & `pysharek-0.11.1/pysharek/main.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.5/pysharek/net.py` & `pysharek-0.11.1/pysharek/net.py`

 * *Files identical despite different names*

### Comparing `pysharek-0.10.5/pysharek/sup.py` & `pysharek-0.11.1/pysharek/sup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     file_dir = None
     sock: "socket" = None
     cipher: "PycaAES256CBC or PycaFernet" = None
     file_size_4_message = 262144  # 256 KB  # 1048576  # 1 MB
     hash_4_thread = None
     continue_from = None
 
+    priv_key = None
+    pub_key = None
+    pub_key_2 = None
+    shared_key = None
+
 
 def pout(msg: str, endl=True):
     if not endl:
         pout_low(msg)
     else:
         pout_low(msg + "\n")
 
@@ -147,14 +152,18 @@
     return S
 
 
 def get_nice_size(size_bytes: int) -> str:
     if size_bytes < 1024:
         return f"{size_bytes} B"
     elif size_bytes < 1024*1024:
-        return f"{size_bytes // 1024} KB"
+        devider = 1024
+        return f"{round(size_bytes / devider, 3)} KB"
     elif size_bytes < 1024*1024*1024:
-        return f"{size_bytes // (1024*1024)} MB"
+        devider = 1024*1024
+        return f"{round(size_bytes / devider, 3)} MB"
     elif size_bytes < 1024*1024*1024*1024:
-        return f"{size_bytes // (1024*1024*1024)} GB"
+        devider = 1024*1024*1024
+        return f"{round(size_bytes / devider, 3)} GB"
     else:
-        return f"{size_bytes // (1024*1024*1024*1024)} TB"
+        devider = 1024*1024*1024*1024
+        return f"{round(size_bytes / devider, 3)} TB"
```

### Comparing `pysharek-0.10.5/pysharek/work.py` & `pysharek-0.11.1/pysharek/work.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import traceback
 
 from .sup import *
 from .net import *
 from .hashes_work import calc_hash_file
 from .hashes_work import calc_hash_dir
 from .sup import get_dirs_needed_for_files
+from .crypto import transfer_shared_key
 
 
 def work_as_sender(args: "argparse.Namespace"):
     # python -m pysharek --mode send --connect server --port 1337
     #                           --password 123 /tmp/123.mp4 --log_file /tmp/log2.txt --log_debug
     plog("I am sender", 1)
     common_block_of_sender_and_receiver(args)
@@ -351,15 +352,47 @@
 
 def common_block_of_sender_and_receiver(args: "argparse.Namespace"):
     plog(f"Common part achieved", 1)
     sock = init_socks_by_connect_and_do_handshake(args)
     plog(f"Handshaked", 1)
     Global.sock = sock
 
-    Global.cipher.set_password(args.password)
+    if args.password is None:
+        from cryptography.hazmat.primitives.asymmetric.x448 import X448PublicKey
+        from cryptography.hazmat.primitives.asymmetric.x448 import X448PrivateKey
+        from cryptography.hazmat.primitives import serialization
+
+        Global.priv_key = X448PrivateKey.generate()
+        Global.pub_key = Global.priv_key.public_key()
+        Global.pub_key = Global.pub_key.public_bytes(encoding=serialization.Encoding.Raw,
+                                                     format=serialization.PublicFormat.Raw)
+        pub_key_2 = None
+        if args.connect == "server":  # TODO: remove args.* == *
+            send_msg(sock, {"key_exchange": "1"}, Global.pub_key)
+            d, pub_key_2 = recv_msg(sock)
+            if "key_exchange" not in d or d["key_exchange"] != "2":
+                pout("Cannot key_exchange-2")
+                plog("Cannot key_exchange-2")
+                socket_close(sock)
+                exit()
+        elif args.connect == "client":
+            d, pub_key_2 = recv_msg(sock)
+            if "key_exchange" not in d or d["key_exchange"] != "1":
+                pout("Cannot key_exchange-1")
+                plog("Cannot key_exchange-1")
+                socket_close(sock)
+                exit()
+            else:
+                send_msg(sock, {"key_exchange": "2"}, Global.pub_key)
+        Global.pub_key_2 = pub_key_2
+        Global.shared_key = Global.priv_key.exchange(X448PublicKey.from_public_bytes(Global.pub_key_2))
+        Global.shared_key = transfer_shared_key(Global.shared_key)
+        Global.cipher.set_password(Global.shared_key)
+    else:
+        Global.cipher.set_password(args.password)
     Global.cipher.start()
 
     plog(f"Inited cipher in common part", 1)
 
     challenge_cipher(sock)
```

### Comparing `pysharek-0.10.5/pysharek.egg-info/PKG-INFO` & `pysharek-0.11.1/pysharek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysharek
-Version: 0.10.5
+Version: 0.11.1
 Summary: Share file with encryption and hash checking
 Author-email: The220th <author@example.com>
 Project-URL: Homepage, https://github.com/The220th/pysharek
 Project-URL: Issues, https://github.com/The220th/pysharek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

