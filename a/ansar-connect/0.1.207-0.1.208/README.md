# Comparing `tmp/ansar_connect-0.1.207.tar.gz` & `tmp/ansar_connect-0.1.208.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.207.tar", last modified: Mon May  6 06:48:21 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.208.tar", last modified: Mon May  6 08:31:01 2024, max compression
```

## Comparing `ansar_connect-0.1.207.tar` & `ansar_connect-0.1.208.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.207/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.207/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.207/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.207/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.207/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.207/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.207/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.207/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 06:48:18.000000 ansar_connect-0.1.207/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.207/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79615 2024-05-06 04:44:43.000000 ansar_connect-0.1.207/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7966 2024-05-06 06:48:12.000000 ansar_connect-0.1.207/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.207/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.207/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.207/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.207/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.207/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.207/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.207/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.207/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.207/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.207/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.207/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.207/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.207/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.207/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.207/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 06:48:21.600052 ansar_connect-0.1.207/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 06:48:21.000000 ansar_connect-0.1.207/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.208/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.208/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.208/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.208/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.208/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.208/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 08:30:58.000000 ansar_connect-0.1.208/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    80294 2024-05-06 08:29:05.000000 ansar_connect-0.1.208/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7966 2024-05-06 06:48:12.000000 ansar_connect-0.1.208/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.208/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.208/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.208/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.208/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.208/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.208/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.208/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.208/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.208/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.208/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.208/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.208/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.208/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.208/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.207/LICENSE` & `ansar_connect-0.1.208/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/PKG-INFO` & `ansar_connect-0.1.208/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.207
+Version: 0.1.208
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.207/README.md` & `ansar_connect-0.1.208/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/pyproject.toml` & `ansar_connect-0.1.208/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/setup.py` & `ansar_connect-0.1.208/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.208/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.208/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.208/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.208/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/__init__.py` & `ansar_connect-0.1.208/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: 9fb169a16d775a3cce8fe4279bc2164df049d45d
-Version: 0.1.206 (2024-05-06@18:48:18+NZST)
+Commit: 12f764d8bef33726863d1ac4045ecfffd634ec3d
+Version: 0.1.207 (2024-05-06@20:30:58+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.207/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.208/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/directory.py` & `ansar_connect-0.1.208/src/ansar/connect/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,54 +320,54 @@
 
 ar.bind(ServiceRoute, SERVICE_ROUTE_DISPATCH)
 
 # Messages from match object (ServiceRoute) to the two different
 # ends of the relation. The PublishingAgent and SubscriptionAgent objects
 # will receive and initiate "calls" based on these messages.
 class RouteToAddress(object):
-	def __init__(self, scope=None, address=None, route_key=None):
-		self.scope = scope
-		self.address = address
+	def __init__(self, matched_scope=None, agent_address=None, route_key=None):
+		self.matched_scope = matched_scope
+		self.agent_address = agent_address
 		self.route_key = route_key
 
 class InboundFromAddress(object):
-	def __init__(self, scope=None, address=None, route_key=None):
-		self.scope = scope
-		self.address = address
+	def __init__(self, matched_scope=None, agent_address=None, route_key=None):
+		self.matched_scope = matched_scope
+		self.agent_address = agent_address
 		self.route_key = route_key
 
 class RouteOverConnected(object):
-	def __init__(self, scope=None, connecting_ipp=None, route_key=None):
-		self.scope = scope
+	def __init__(self, matched_scope=None, connecting_ipp=None, route_key=None):
+		self.matched_scope = matched_scope
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.route_key = route_key
 
 class InboundOverAccepted(object):
-	def __init__(self, scope=None, route_key=None):
-		self.scope = scope
+	def __init__(self, matched_scope=None, route_key=None):
+		self.matched_scope = matched_scope
 		self.route_key = route_key
 
 class RouteByRelay():
-	def __init__(self, scope=None, redirect=None, route_key=None):
-		self.scope = scope
+	def __init__(self, matched_scope=None, redirect=None, route_key=None):
+		self.matched_scope = matched_scope
 		self.redirect = redirect or RelayRedirect()
 		self.route_key = route_key
 
 class InboundByRelay():
-	def __init__(self, scope=None, redirect=None, route_key=None):
-		self.scope = scope
+	def __init__(self, matched_scope=None, redirect=None, route_key=None):
+		self.matched_scope = matched_scope
 		self.redirect = redirect or RelayRedirect()
 		self.route_key = route_key
 
 IO_SCHEMA = {
-	'address': ar.Address(),
+	'agent_address': ar.Address(),
 	'route_key': str,
 	'name': str,
 	'connecting_ipp': ar.UserDefined(HostPort),
-	'scope': ScopeOfService,
+	'matched_scope': ScopeOfService,
 	'redirect': ar.UserDefined(RelayRedirect),
 }
 
 ar.bind(RouteToAddress, object_schema=IO_SCHEMA)
 ar.bind(InboundFromAddress, object_schema=IO_SCHEMA)
 ar.bind(RouteOverConnected, object_schema=IO_SCHEMA)
 ar.bind(InboundOverAccepted, object_schema=IO_SCHEMA)
@@ -420,50 +420,50 @@
 # of connection between subscriber and publisher.
 class DirectService(object):
 	def __init__(self, find, listing):
 		self.find = find
 		self.listing = listing
 
 	def outbound(self, route_key):
-		return RouteToAddress(ScopeOfService.PROCESS, self.listing.agent_address, route_key)
+		return RouteToAddress(matched_scope=ScopeOfService.PROCESS, agent_address=self.listing.agent_address, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundFromAddress(ScopeOfService.PROCESS, self.find.agent_address, route_key)
+		return InboundFromAddress(matched_scope=ScopeOfService.PROCESS, agent_address=self.find.agent_address, route_key=route_key)
 
 # Between two objects needing a TCP connection from
 # subscribing process to publishing process. Listening
 # address needs tuning based on whether its intra-host
 # or across a LAN.
 class ServiceOverConnection(object):
-	def __init__(self, scope, find, listing):
+	def __init__(self, matched_scope, find, listing):
 		self.find = find
 		self.listing = listing
-		self.scope = scope
+		self.matched_scope = matched_scope
 
 	def outbound(self, route_key):
-		return RouteOverConnected(self.scope, self.listing.connecting_ipp, route_key)
+		return RouteOverConnected(matched_scope=self.matched_scope, connecting_ipp=self.listing.connecting_ipp, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundOverAccepted(self.scope, route_key)
+		return InboundOverAccepted(matched_scope=self.matched_scope, route_key=route_key)
 
 # The extra step needed for relay setup. A query/response
 # needed with the relay manager before the connection
 # messages can be sent to the ends of the call.
 class ServiceByRelay(object):
 	def __init__(self, find, listing, relay_address):
 		self.find = find
 		self.listing = listing
 		self.relay_address = relay_address
 		self.redirect = None
 
 	def outbound(self, route_key):
-		return RouteByRelay(ScopeOfService.WAN, self.redirect, route_key)
+		return RouteByRelay(matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundByRelay(ScopeOfService.WAN, self.redirect, route_key)
+		return InboundByRelay(matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
 
 # The per-process part of the distributed name service.
 # Accepts local listings and searches and creates matches.
 # Receives listings and searches from below as well. All
 # information forwarded to next level up.
 def key_service(route_key):
 	try:
@@ -1342,30 +1342,30 @@
 	route_key = message.route_key
 
 	try:
 		m = self.matching[route_key]
 	except KeyError:
 		m = [message, None, None]
 		self.matching[route_key] = m
-		self.trace(f'Added direct route [{ScopeOfService.to_name(message.scope)}]({route_key})')
+		self.trace(f'Added direct route [{ScopeOfService.to_name(message.matched_scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 
 ### PS-pub-4 Agent accepts peer route.
 
 def PublishingAgent_READY_InboundOverAccepted(self, message):
 	route_key = message.route_key
 
 	try:
 		m = self.matching[route_key]
 	except KeyError:
 		m = [message, None, None]
 		self.matching[route_key] = m
-		self.trace(f'Added peer route [{ScopeOfService.to_name(message.scope)}]({route_key})')
+		self.trace(f'Added peer route [{ScopeOfService.to_name(message.matched_scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 
 def PublishingAgent_READY_InboundByRelay(self, message):
 	route_key = message.route_key
 	try:
@@ -1402,15 +1402,15 @@
 	# Assume the same state as for other route types, i.e.
 	# ready for the OpenLoop that is sure to follow.
 	try:
 		m = self.matching[route_key]
 	except KeyError:
 		m = [relay, None, None]
 		self.matching[route_key] = m
-		self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({route_key})')
+		self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.matched_scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 	
 def PublishingAgent_READY_PeerOpened(self, message):
 	k = ipp_key(message.connecting_ipp)
 	try:
@@ -1426,15 +1426,15 @@
 		# Assume the same state as for other route types, i.e.
 		# ready for the OpenLoop that is sure to follow.
 		try:
 			m = self.matching[route_key]
 		except KeyError:
 			m = [relay, None, None]
 			self.matching[route_key] = m
-			self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({route_key})')
+			self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.matched_scope)}]({route_key})')
 			continue
 		looped(self, message, m[1], m[2])
 	return READY
 
 def PublishingAgent_READY_RetractRoute(self, message):
 	route_key = message.route_key
 
@@ -1443,15 +1443,15 @@
 		self.trace(f'Unknown route_key "{route_key}"')
 		return READY
 
 	if m[0] is None:
 		self.trace(f'Known route_key "{route_key}" never routed')
 		return READY
 
-	self.trace(f'Retracted route [{ScopeOfService.to_name(m[0].scope)}]({route_key})')
+	self.trace(f'Retracted route [{ScopeOfService.to_name(m[0].matched_scope)}]({route_key})')
 	return READY
 
 ### PS-pub-5 Agent accepts remote loop.
 def PublishingAgent_READY_OpenLoop(self, message):
 	route_key = message.route_key
 	try:
 		m = self.matching[route_key]
@@ -1470,26 +1470,26 @@
 	return READY
 
 def PublishingAgent_READY_CapRoutes(self, message):
 	self.trace(f'Scope cap {message.service_scope}, {len(self.matching)} routes to consider')
 
 	removing = set()
 	for k, m in self.matching.items():
-		if message.service_scope < m[0].scope:
+		if message.service_scope < m[0].matched_scope:
 			removing.add(k)
 
 	self.trace(f'Removing {len(removing)} routes')
 	for k in removing:
 		m = self.matching.pop(k, None)
 		if m is None:
 			continue
 		m0 = m[0]
 		if m0 is None:
 			continue
-		self.trace(f'Capped route [{ScopeOfService.to_name(m0.scope)}]({k})')
+		self.trace(f'Capped route [{ScopeOfService.to_name(m0.matched_scope)}]({k})')
 	return READY
 
 def PublishingAgent_READY_Clear(self, message):
 	if message.session is None:
 		for a in self.loop.values():
 			self.send(Close(message.value), a)
 		return READY
@@ -1585,19 +1585,19 @@
 
 SECONDS_OF_LOOPING = 4.0
 SECONDS_OF_PEERING = 4.0
 
 # Pick out the best route in the
 # given table.
 def best_route(table):
-	scope, route = None, None
+	matched_scope, route = None, None
 	for s, r in table.items():
-		if scope is None or s < scope:
-			scope, route = s, r
-	return scope, route
+		if matched_scope is None or s < matched_scope:
+			matched_scope, route = s, r
+	return matched_scope, route
 
 def find_route(table, route_key):
 	for s, r in table.items():
 		if r.route_key == route_key:
 			return s
 	return None
 
@@ -1700,15 +1700,15 @@
 	def close_relay(self):
 		self.send(CloseRelay(self.route.redirect), self.peer_address)
 
 #
 #
 def SubscriberLoop_INITIAL_Start(self, message):
 	route = self.route
-	e = ScopeOfService.to_name(route.scope)
+	e = ScopeOfService.to_name(route.matched_scope)
 	self.trace(f'Initiate route [{e}]({route.route_key})')
 
 	if isinstance(route, RouteToAddress):
 		self.open_loop(route.route_key, route.address)
 		return LOOPING
 	elif isinstance(route, RouteOverConnected):
 		self.open_peer()
@@ -2147,31 +2147,31 @@
 		self.subscriber_address = subscriber_address
 		self.create_session = create_session
 		self.requested_scope = requested_scope
 		self.service_looping = {}
 
 	def open_route(self, route, tag):
 		name = key_service(route.route_key)
-		scope = route.scope
-		sos = ScopeOfService.to_name(scope)
+		matched_scope = route.matched_scope
+		sos = ScopeOfService.to_name(matched_scope)
 
 		looping = self.service_looping.get(name, None)
 		if looping is None:
 			self.trace(f'Start loop "{name}" [{sos}] {tag}')
-			table = {scope: route}
+			table = {matched_scope: route}
 			a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
 			self.assign(a, name)
 			looping = [table, route, a, False]		# Table, route, loop, completion.
 			self.service_looping[name] = looping
 			return
 
 		table, opened, loop, completed = looping
-		table[scope] = route
+		table[matched_scope] = route
 
-		if route.scope == opened.scope:
+		if route.matched_scope == opened.matched_scope:
 			if loop:
 				self.trace(f'Replacement [{sos}] route (loop running)')
 				return
 			if completed:
 				self.trace(f'Replacement [{sos}] route (previous positive completion)')
 				return
 
@@ -2192,15 +2192,15 @@
 			self.trace(f'Start replacement [{sos}] route for "{name}", change of {s}')
 			a = self.create(SubscriberLoop, route, self.subscriber_address, self.create_session)
 			self.assign(a, name)
 			looping[1] = route
 			looping[2] = a
 			return
 
-		if route.scope < opened.scope:
+		if route.matched_scope < opened.matched_scope:
 			if loop:
 				self.trace(f'Upgrade [{sos}] route, pushing current loop')
 				self.send(ar.Stop(), loop)
 				return
 			if completed:
 				self.trace(f'Upgrade [{sos}] route, (previous positive completion)')
 				return
@@ -2243,20 +2243,20 @@
 
 	looping = self.service_looping.get(name, None)
 	if looping is None:
 		self.trace(f'Retract for unknown service "{name}"')
 		return READY
 	table = looping[0]
 
-	scope = find_route(table, route_key)
-	if scope is None:
+	matched_scope = find_route(table, route_key)
+	if matched_scope is None:
 		self.trace(f'Retract for unknown route "{route_key}"')
 		return READY
 
-	r = table.pop(scope, None)
+	r = table.pop(matched_scope, None)
 	if r is None:
 		self.warning(f'Find/pop failed for route "{route_key}"')
 		return READY
 
 	return READY
 
 def SubscriptionAgent_READY_CapRoutes(self, message):
@@ -2299,20 +2299,20 @@
 	looping[3] = message.value
 
 	table, route, loop, completed = looping
 
 	if completed:			# This subscriber/publisher match is done.
 		return READY
 
-	scope, best = best_route(table)		# Nothing to route to.
-	if scope is None:
+	matched_scope, best = best_route(table)		# Nothing to route to.
+	if matched_scope is None:
 		return READY
 
-	sos = ScopeOfService.to_name(route.scope)
-	if best.scope == route.scope:
+	sos = ScopeOfService.to_name(route.matched_scope)
+	if best.matched_scope == route.matched_scope:
 		self.trace(f'Replacement [{sos}] route')
 		if key_id(best.route_key) == key_id(route.route_key):
 			self.trace(f'Replacement route for "{name}" has not changed')
 			return READY
 
 	self.trace(f'Start continuation loop "{name}" [{sos}]')
 	a = self.create(SubscriberLoop, message, self.subscriber_address, self.create_session)
```

### Comparing `ansar_connect-0.1.207/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.208/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.208/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/group_if.py` & `ansar_connect-0.1.208/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/grouping.py` & `ansar_connect-0.1.208/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/moving.py` & `ansar_connect-0.1.208/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/networking.py` & `ansar_connect-0.1.208/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.208/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/node.py` & `ansar_connect-0.1.208/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.208/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/procedure.py` & `ansar_connect-0.1.208/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/product.py` & `ansar_connect-0.1.208/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/socketry.py` & `ansar_connect-0.1.208/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/standard.py` & `ansar_connect-0.1.208/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/transporting.py` & `ansar_connect-0.1.208/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.208/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar/connect/wan.py` & `ansar_connect-0.1.208/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.207/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.208/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.207
+Version: 0.1.208
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.207/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.208/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

