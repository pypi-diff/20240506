# Comparing `tmp/ansar_connect-0.1.201.tar.gz` & `tmp/ansar_connect-0.1.203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.201.tar", last modified: Sun May  5 23:29:18 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.203.tar", last modified: Mon May  6 04:44:02 2024, max compression
```

## Comparing `ansar_connect-0.1.201.tar` & `ansar_connect-0.1.203.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.201/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.201/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.201/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.201/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.201/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.201/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-05 23:29:15.000000 ansar_connect-0.1.201/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79308 2024-05-05 21:57:14.000000 ansar_connect-0.1.201/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7833 2024-05-05 21:45:40.000000 ansar_connect-0.1.201/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.201/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.201/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.201/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-05 21:23:08.000000 ansar_connect-0.1.201/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.201/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.201/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.201/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.201/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.201/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.201/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.201/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.201/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.201/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.675796 ansar_connect-0.1.203/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.203/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 04:44:02.675796 ansar_connect-0.1.203/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.203/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.203/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 04:44:02.675796 ansar_connect-0.1.203/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.203/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.671796 ansar_connect-0.1.203/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.671796 ansar_connect-0.1.203/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.671796 ansar_connect-0.1.203/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.203/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.203/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.203/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.203/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.675796 ansar_connect-0.1.203/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 04:43:59.000000 ansar_connect-0.1.203/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.203/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    79574 2024-05-06 04:43:32.000000 ansar_connect-0.1.203/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7977 2024-05-06 04:43:32.000000 ansar_connect-0.1.203/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.203/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.203/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.203/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.203/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.203/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.203/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.203/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.203/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.203/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.203/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.203/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.203/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.203/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.203/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.203/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 04:44:02.675796 ansar_connect-0.1.203/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 04:44:02.000000 ansar_connect-0.1.203/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.201/LICENSE` & `ansar_connect-0.1.203/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/PKG-INFO` & `ansar_connect-0.1.203/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.201
+Version: 0.1.203
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.201/README.md` & `ansar_connect-0.1.203/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/pyproject.toml` & `ansar_connect-0.1.203/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/setup.py` & `ansar_connect-0.1.203/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.203/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.203/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.203/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.203/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/__init__.py` & `ansar_connect-0.1.203/src/ansar/connect/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
-Branch: main
-Commit: 7dff7b9c46fc0778d7e56b0cfa9b2dc756c3cb7d
-Version: 0.1.200 (2024-05-06@11:29:15+NZST)
+Branch: upgrade-pub-sub-messages
+Commit: b8ba9a752d188fc49b2b82c83ecb3793859ec0cd
+Version: 0.1.202 (2024-05-06@16:43:59+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.201/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.203/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/directory.py` & `ansar_connect-0.1.203/src/ansar/connect/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,15 +521,15 @@
 		self.connected = None
 		self.listening = None
 		self.accepted = {}
 		self.started = None
 		self.stopped = None
 		self.reconnecting = None
 
-	def found(self, service_name, f, d):
+	def found(self, f, d):
 		find = f[0]
 		listing = d[0]
 		find_address = find.agent_address
 		find_matched = f[1]
 		listing_address = listing.agent_address
 		listing_id = listing.listing_id
 		listing_matched = d[1]
@@ -602,15 +602,15 @@
 
 		# Match listing to finds.
 		for _, f in self.find.items():
 			dfa = f[2]
 			m = dfa.match(service_name)
 			if m:
 				### PS-pub-10 New service matches existing search.
-				self.found(service_name, f, d)
+				self.found(f, d)
 
 		return
 
 		# Not duplicates - yet.
 		if service_name in self.directory:
 			self.warning(f'Duplicate listing for "{service_name}"')
 			return
@@ -622,15 +622,15 @@
 
 		# Match listing to finds.
 		for _, f in self.find.items():
 			dfa = f[2]
 			m = dfa.match(service_name)
 			if m:
 				### PS-pub-10 New service matches existing search.
-				self.found(service_name, f, d)
+				self.found(f, d)
 
 	### PS-sub-9 Directory installs a new search.
 	def add_find(self, message):
 		find_name = message.requested_search
 		find_address = message.agent_address
 
 		jf = address_to_text(find_address)
@@ -651,15 +651,15 @@
 		self.trace(f'Added search "{k}"')
 
 		# Match find to listings.
 		for service_name, d in self.directory.items():
 			m = dfa.match(service_name)
 			if m:
 				### PS-sub-9 New find matches existing service.
-				self.found(service_name, f, d)
+				self.found(f, d)
 
 	def remove_listing(self, message):
 		service_name = message.requested_name
 
 		# Remove the entry and terminate any routes that
 		# were based on its existence.
 		# d = [message, set()]
@@ -1169,15 +1169,15 @@
 		self.session_address = self.created_session
 		self.origin_address = self.created_session
 	else:
 		self.session_address = self.publisher_address
 		self.origin_address = self.remote_session
 
 	self.send(LoopOpened(self.session_address, self.route_key), self.remote_loop)
-	self.forward(Delivered(self.route_key, self.address), self.publisher_address, self.origin_address)
+	self.forward(Delivered(self.route_key, self.parent_address), self.publisher_address, self.origin_address)
 	return LOOPED
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
 	if self.created_session and self.return_address == self.created_session:
 		self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
@@ -1268,15 +1268,18 @@
 def PublishingAgent_INITIAL_Start(self, message):
 	if self.requested_scope == ScopeOfService.PROCESS:
 		### PS-pub-3 Agent sends listing to directory.
 		listing_id = uuid.uuid4()
 		self.send(ServiceListing(requested_name=self.requested_name,
 			agent_address=self.address, requested_scope=self.requested_scope,
 			listing_id=listing_id), pb.directory)
-		self.send(Published(self.requested_name, self.requested_scope), self.publisher_address)
+		published_at = ar.world_now()
+		self.send(Published(requested_name=self.requested_name, requested_scope=self.requested_scope,
+			published_at=published_at),
+			self.publisher_address)
 		return READY
 	elif self.requested_scope in (ScopeOfService.GROUP, ScopeOfService.HOST):
 		### PS-pub-3 Agent arranges for inbound listen.
 		listen(self, LocalPort(0))
 		return PENDING
 	elif self.requested_scope in (ScopeOfService.LAN, ScopeOfService.WAN):
 		listen(self, HostPort('0.0.0.0', 0))
@@ -1286,15 +1289,18 @@
 def PublishingAgent_PENDING_Listening(self, message):
 	self.listening = message
 	listing_id = uuid.uuid4()
 	self.send(ServiceListing(requested_name=self.requested_name,
 		agent_address=self.address, requested_scope=self.requested_scope,
 		listing_id=listing_id,
 		listening_ipp=message.listening_ipp), pb.directory)
-	self.send(Published(self.requested_name, self.requested_scope, message.listening_ipp), self.publisher_address)
+	published_at = ar.world_now()
+	self.send(Published(requested_name=self.requested_name, requested_scope=self.requested_scope,
+		listening_ipp=message.listening_ipp, published_at=published_at),
+		self.publisher_address)
 	return READY
 
 def PublishingAgent_PENDING_NotListening(self, message):
 	ipp = message.requested_ipp
 	t = message.error_text
 	self.warning(f'Cannot allocate a listen for {ipp} ({t})')
 	self.start(ar.T1, 60.0)
@@ -2496,15 +2502,15 @@
 def PubSub_INITIAL_Start(self, message):
 	return NORMAL
 
 ### PS-pub-1 Process the app request
 def PubSub_NORMAL_PublishAsName(self, message):
 	try:
 		a = self.published[message.requested_name]
-		self.reply(NotPublished(message.requested_name, 'already published'))
+		self.reply(NotPublished(requested_name=message.requested_name, reason='duplicate'))
 		return NORMAL
 	except KeyError:
 		pass
 	### PS-pub-2 Create the agent
 	a = self.create(PublishingAgent, message.requested_name, self.return_address, message.create_session, message.requested_scope)
 	p = [message, self.return_address]
 	self.assign(a, p)
@@ -2520,15 +2526,18 @@
 		a = self.subscribed[k]
 	except KeyError:
 		### PS-sub-2 Create the agent
 		a = self.create(SubscriptionAgent, message.requested_search, self.return_address, message.create_session, message.requested_scope)
 		s = [message, self.return_address]
 		self.assign(a, s)
 		self.subscribed[k] = a
-	self.forward(Subscribed(message.requested_search, message.requested_scope), self.return_address, a)
+	subscribed_at = ar.world_now()
+	self.forward(Subscribed(requested_search=message.requested_search, requested_scope=message.requested_scope,
+		subscribed_at=subscribed_at),
+		self.return_address, a)
 	return NORMAL
 
 def PubSub_NORMAL_Retract(self, message):
 	self.trace(f'Retracting service/search at [{address_to_text(message.address)}]')
 	for t, a in self.running():
 		if t[1] == message.address:
 			self.send(ar.Stop(), a)
```

### Comparing `ansar_connect-0.1.201/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.203/src/ansar/connect/directory_if.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,33 +47,35 @@
 # Build the local published/subscribed objects.
 #
 ScopeOfService = ar.Enumeration(PROCESS=1, GROUP=2, HOST=3, LAN=4, WAN=5)
 
 #
 #
 class Published(object):
-	def __init__(self, requested_name=None, requested_scope=ScopeOfService.WAN, listening_ipp=None):
+	def __init__(self, requested_name=None, requested_scope=ScopeOfService.WAN, listening_ipp=None, published_at=None):
 		self.requested_name = requested_name
 		self.requested_scope = requested_scope
 		self.listening_ipp = listening_ipp or HostPort()
+		self.published_at = published_at
 
 class NotPublished(ar.Faulted):
 	def __init__(self, requested_name=None, reason=None):
 		self.requested_name = requested_name
 		self.reason = reason
 		ar.Faulted.__init__(self, f'cannot publish "{requested_name}"', reason)
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
 class Subscribed(object):
-	def __init__(self, requested_search=None, requested_scope=ScopeOfService.WAN):
+	def __init__(self, requested_search=None, requested_scope=ScopeOfService.WAN, subscribed_at=None):
 		self.requested_search = requested_search
 		self.requested_scope = requested_scope
+		self.subscribed_at = subscribed_at
 
 # The actual service directory with listings and searches.
 #
 
 # Session messages to publish/listen controllers.
 # Subscribe/client/calling/outbound end.
 class Available(object):
@@ -158,14 +160,15 @@
 	'listening_ipp': ar.UserDefined(HostPort),
 	'connecting_ipp': ar.UserDefined(HostPort),
 	'parent_ipp': ar.UserDefined(HostPort),
 	'child_ipp': ar.UserDefined(HostPort),
 	'subscription': ar.UserDefined(Subscribed),
 	'agent_address': ar.Address(),
 	'address': ar.Address(),
+	'published_at': ar.WorldTime(),
 }
 
 SHARED_SCHEMA.update(ENDING_SCHEMA)
 
 ar.bind(Subscribed, object_schema=SHARED_SCHEMA)
 ar.bind(Published, object_schema=SHARED_SCHEMA)
 ar.bind(Available, object_schema=SHARED_SCHEMA)
```

### Comparing `ansar_connect-0.1.201/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.203/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/group_if.py` & `ansar_connect-0.1.203/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/grouping.py` & `ansar_connect-0.1.203/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/moving.py` & `ansar_connect-0.1.203/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/networking.py` & `ansar_connect-0.1.203/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.203/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/node.py` & `ansar_connect-0.1.203/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.203/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/procedure.py` & `ansar_connect-0.1.203/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/product.py` & `ansar_connect-0.1.203/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/socketry.py` & `ansar_connect-0.1.203/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/standard.py` & `ansar_connect-0.1.203/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/transporting.py` & `ansar_connect-0.1.203/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.203/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.201/src/ansar/connect/wan.py` & `ansar_connect-0.1.203/src/ansar/connect/wan.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,7 +201,9 @@
 CLOSE_SCHEMA = {
 	"redirect": ar.UserDefined(RelayRedirect),
 }
 
 ar.bind(CloseRelay, object_schema=CLOSE_SCHEMA)
 
 FOH_HOST = 'ansar-mx.net'
+
+
```

### Comparing `ansar_connect-0.1.201/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.203/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.201
+Version: 0.1.203
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.201/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.203/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

