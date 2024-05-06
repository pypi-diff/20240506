# Comparing `tmp/ansar_connect-0.1.214.tar.gz` & `tmp/ansar_connect-0.1.215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.214.tar", last modified: Mon May  6 19:54:40 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.215.tar", last modified: Mon May  6 20:46:47 2024, max compression
```

## Comparing `ansar_connect-0.1.214.tar` & `ansar_connect-0.1.215.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.214/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.214/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.214/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.214/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.214/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.214/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 19:54:37.000000 ansar_connect-0.1.214/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87301 2024-05-06 19:38:10.000000 ansar_connect-0.1.214/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8884 2024-05-06 19:54:12.000000 ansar_connect-0.1.214/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.214/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.214/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.214/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.214/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.214/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.214/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.214/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.214/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.214/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.214/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.214/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.214/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.214/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.214/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.215/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.215/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.215/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.215/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.215/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.215/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.215/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.215/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 20:46:44.000000 ansar_connect-0.1.215/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.215/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87301 2024-05-06 20:46:26.000000 ansar_connect-0.1.215/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8884 2024-05-06 19:54:12.000000 ansar_connect-0.1.215/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.215/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.215/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.215/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.215/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.215/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.215/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.215/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.215/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.215/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.215/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.215/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.215/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.215/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.215/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.215/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 20:46:47.423815 ansar_connect-0.1.215/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 20:46:47.000000 ansar_connect-0.1.215/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.214/LICENSE` & `ansar_connect-0.1.215/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/PKG-INFO` & `ansar_connect-0.1.215/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.214
+Version: 0.1.215
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.214/README.md` & `ansar_connect-0.1.215/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/pyproject.toml` & `ansar_connect-0.1.215/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/setup.py` & `ansar_connect-0.1.215/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.215/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.215/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.215/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.215/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/__init__.py` & `ansar_connect-0.1.215/src/ansar/connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: d5844a4bdaa789206ad19a9b3198c0ecc33c1a51
-Version: 0.1.213 (2024-05-07@07:54:37+NZST)
+Commit: 1744b61988d86ea9d4d8fd418bb098655c957292
+Version: 0.1.214 (2024-05-07@08:46:44+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.214/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.215/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/directory.py` & `ansar_connect-0.1.215/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -2514,52 +2514,52 @@
 
 def ConnectToPeer_CONNECTING_NotConnected(self, message):
 	self.not_connected = str(message)
 	not_peered = NotPeered(connecting_ipp=self.connecting_ipp, route_key=self.route_key, reason=self.not_connected)
 	for c in self.client_address:
 		self.send(not_peered, c)
 
-	self.start(ar.T1, 4.0)
+	self.start(ar.T1, 2.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTING_Stop(self, message):
 	self.complete(ar.Aborted())
 
 # CONNECTED
 #
 def ConnectToPeer_CONNECTED_Abandoned(self, message):
 	self.not_connected = 'Abandoned by remote'
 	return_address = self.return_address
 	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(lost, c, return_address)
-	self.start(ar.T1, 4.0)
+	self.start(ar.T1, 2.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTED_Closed(self, message):
 	self.not_connected = 'Local termination'
 	return_address = self.return_address
 	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(lost, c, return_address)
-	self.start(ar.T1, 4.0)
+	self.start(ar.T1, 2.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTED_OpenPeer(self, message):
 	self.client_address.add(self.return_address)
 	opened = PeerOpened(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	self.forward(opened, self.return_address, self.connected.remote_address)
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_ClosePeer(self, message):
 	self.client_address.discard(self.return_address)
 	if len(self.client_address) < 1:
 		self.not_connected = 'Cleared last peer'
 		self.send(Close(ar.Aborted()), self.connected.remote_address)
-		self.start(ar.T1, 4.0)
+		self.start(ar.T1, 2.0)
 		return GLARING
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_Stop(self, message):
 	self.not_connected = 'Process termination'
 	return_address = self.connected.remote_address
 	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
```

### Comparing `ansar_connect-0.1.214/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.215/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.215/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/group_if.py` & `ansar_connect-0.1.215/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/grouping.py` & `ansar_connect-0.1.215/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/moving.py` & `ansar_connect-0.1.215/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/networking.py` & `ansar_connect-0.1.215/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.215/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/node.py` & `ansar_connect-0.1.215/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.215/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/procedure.py` & `ansar_connect-0.1.215/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/product.py` & `ansar_connect-0.1.215/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/socketry.py` & `ansar_connect-0.1.215/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/standard.py` & `ansar_connect-0.1.215/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/transporting.py` & `ansar_connect-0.1.215/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.215/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar/connect/wan.py` & `ansar_connect-0.1.215/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.214/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.215/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.214
+Version: 0.1.215
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.214/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.215/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

