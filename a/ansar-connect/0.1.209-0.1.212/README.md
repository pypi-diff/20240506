# Comparing `tmp/ansar_connect-0.1.209.tar.gz` & `tmp/ansar_connect-0.1.212.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.209.tar", last modified: Mon May  6 12:47:30 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.212.tar", last modified: Mon May  6 13:49:21 2024, max compression
```

## Comparing `ansar_connect-0.1.209.tar` & `ansar_connect-0.1.212.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.209/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.209/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.209/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.209/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.629995 ansar_connect-0.1.209/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.209/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.209/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 12:47:27.000000 ansar_connect-0.1.209/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    81505 2024-05-06 12:46:44.000000 ansar_connect-0.1.209/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7966 2024-05-06 06:48:12.000000 ansar_connect-0.1.209/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.209/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.209/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.209/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.209/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.209/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.209/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.209/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.209/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.209/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.209/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.209/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.209/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.209/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.209/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.212/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.212/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.212/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.212/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.212/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.212/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 13:49:18.000000 ansar_connect-0.1.212/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    81926 2024-05-06 13:38:36.000000 ansar_connect-0.1.212/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8338 2024-05-06 13:45:27.000000 ansar_connect-0.1.212/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.212/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.212/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.212/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.212/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.212/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.212/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.212/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.212/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.212/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.212/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.212/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.212/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.212/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.212/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.209/LICENSE` & `ansar_connect-0.1.212/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/PKG-INFO` & `ansar_connect-0.1.212/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.209
+Version: 0.1.212
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.209/README.md` & `ansar_connect-0.1.212/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/pyproject.toml` & `ansar_connect-0.1.212/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/setup.py` & `ansar_connect-0.1.212/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.212/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.212/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.212/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.212/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/__init__.py` & `ansar_connect-0.1.212/src/ansar/connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: 187fa9c6010b081c3ec4d88ba9c153253528a328
-Version: 0.1.208 (2024-05-07@00:47:27+NZST)
+Commit: 64ea7a0bfcf8702d22e0d3d2a39ede6593dd58c0
+Version: 0.1.211 (2024-05-07@01:49:18+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.209/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.212/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/directory.py` & `ansar_connect-0.1.212/src/ansar/connect/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,14 +337,16 @@
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.agent_address = agent_address
 		self.route_key = route_key
 
 class RouteOverConnected(object):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, connecting_ipp=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.route_key = route_key
 
 class InboundOverAccepted(object):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None):
 		self.matched_search = matched_search
@@ -1192,15 +1194,18 @@
 		self.session_address = self.created_session
 		self.origin_address = self.created_session
 	else:
 		self.session_address = self.publisher_address
 		self.origin_address = self.remote_session
 
 	self.send(LoopOpened(self.session_address, self.route_key), self.remote_loop)
-	self.forward(Delivered(self.route_key, self.parent_address), self.publisher_address, self.origin_address)
+	delivered = Delivered(matched_search=self.route.matched_search, matched_name=self.route.matched_name,
+			matched_scope=self.route.matched_scope,
+			route_key=self.route_key, agent_address=self.parent_address)
+	self.forward(delivered, self.publisher_address, self.origin_address)
 	return LOOPED
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
 	if self.created_session and self.return_address == self.created_session:
 		self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
@@ -1692,15 +1697,18 @@
 			# Latch clears additional session alias on stop
 			hand = ar.SwitchOver()
 		# Sending session control message from Latch is flawed - doesnt know
 		# about "origin_address".
 		s = address_to_text(self.subscriber_address)
 		p = address_to_text(self.origin_address)
 		self.trace(f'Loop opened between subscriber [{s}] and publisher [{p}]')
-		self.forward(Available(message.route_key, self.parent_address), self.subscriber_address, self.origin_address)
+		available = Available(matched_search=self.route.matched_search, matched_name=self.route.matched_name,
+			matched_scope=self.route.matched_scope,
+			route_key=message.route_key, agent_address=self.parent_address)
+		self.forward(available, self.subscriber_address, self.origin_address)
 		self.send(hand, self.latch)
 		# LATCH MUST CONTINUE FOR THOSE MESSAGES THAT WERE
 		# SITTING IN THE QUEUE AFTER THE HANDOVER MESSAGE
 	
 	def latch_loop(self):
 		j = self.address_job.pop(self.latch, None)
 		if j is None:
```

### Comparing `ansar_connect-0.1.209/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.212/src/ansar/connect/directory_if.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,18 @@
 
 # The actual service directory with listings and searches.
 #
 
 # Session messages to publish/listen controllers.
 # Subscribe/client/calling/outbound end.
 class Available(object):
-	def __init__(self, route_key=None, agent_address=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, agent_address=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
 	def __init__(self, route_key=None, reason=None, agent_address=None):
 		self.route_key = route_key
 		self.reason = reason
@@ -92,15 +95,18 @@
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
 # Publish/service/answering/inbound end.
 class Delivered(object):
-	def __init__(self, route_key=None, agent_address=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, agent_address=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
 	def __init__(self, requested_name=None, remote_address=None):
 		self.requested_name = requested_name
 		self.remote_address = remote_address
@@ -146,16 +152,17 @@
 SHARED_SCHEMA = {
 	#'route_key': ar.VectorOf(ar.Integer8()),
 	'route_key': str,
 	'name': str,
 	'requested_name': str,
 	'requested_search': str,
 	'requested_name': str,
-	'requested_search': str,
-	'requested_name': str,
+	'matched_search': str,
+	'matched_name': str,
+	'matched_scope': ScopeOfService,
 	'remote_address': ar.Address(),
 	'session_address': ar.Address(),
 	'requested_scope': ScopeOfService,
 	'service_scope': ScopeOfService,
 	'reason': ar.String(),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'connecting_ipp': ar.UserDefined(HostPort),
```

### Comparing `ansar_connect-0.1.209/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.212/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/group_if.py` & `ansar_connect-0.1.212/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/grouping.py` & `ansar_connect-0.1.212/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/moving.py` & `ansar_connect-0.1.212/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/networking.py` & `ansar_connect-0.1.212/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.212/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/node.py` & `ansar_connect-0.1.212/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.212/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/procedure.py` & `ansar_connect-0.1.212/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/product.py` & `ansar_connect-0.1.212/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/socketry.py` & `ansar_connect-0.1.212/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/standard.py` & `ansar_connect-0.1.212/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/transporting.py` & `ansar_connect-0.1.212/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.212/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar/connect/wan.py` & `ansar_connect-0.1.212/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.209/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.212/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.209
+Version: 0.1.212
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.209/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.212/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

