# Comparing `tmp/ansar_connect-0.1.208.tar.gz` & `tmp/ansar_connect-0.1.209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.208.tar", last modified: Mon May  6 08:31:01 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.209.tar", last modified: Mon May  6 12:47:30 2024, max compression
```

## Comparing `ansar_connect-0.1.208.tar` & `ansar_connect-0.1.209.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.208/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.208/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.208/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.208/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.974940 ansar_connect-0.1.208/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.208/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.208/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 08:30:58.000000 ansar_connect-0.1.208/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    80294 2024-05-06 08:29:05.000000 ansar_connect-0.1.208/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7966 2024-05-06 06:48:12.000000 ansar_connect-0.1.208/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.208/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.208/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.208/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.208/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.208/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.208/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.208/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.208/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.208/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.208/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.208/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.208/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.208/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.208/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.208/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 08:31:01.978940 ansar_connect-0.1.208/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 08:31:01.000000 ansar_connect-0.1.208/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.209/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.209/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.209/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.209/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.629995 ansar_connect-0.1.209/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.209/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.209/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 12:47:27.000000 ansar_connect-0.1.209/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    81505 2024-05-06 12:46:44.000000 ansar_connect-0.1.209/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7966 2024-05-06 06:48:12.000000 ansar_connect-0.1.209/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.209/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.209/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.209/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.209/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.209/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.209/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.209/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.209/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.209/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.209/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.209/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.209/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.209/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.209/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.209/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 12:47:30.633995 ansar_connect-0.1.209/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 12:47:30.000000 ansar_connect-0.1.209/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.208/LICENSE` & `ansar_connect-0.1.209/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/PKG-INFO` & `ansar_connect-0.1.209/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.208
+Version: 0.1.209
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.208/README.md` & `ansar_connect-0.1.209/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/pyproject.toml` & `ansar_connect-0.1.209/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/setup.py` & `ansar_connect-0.1.209/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.209/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.209/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.209/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.209/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/__init__.py` & `ansar_connect-0.1.209/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: 12f764d8bef33726863d1ac4045ecfffd634ec3d
-Version: 0.1.207 (2024-05-06@20:30:58+NZST)
+Commit: 187fa9c6010b081c3ec4d88ba9c153253528a328
+Version: 0.1.208 (2024-05-07@00:47:27+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.208/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.209/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/directory.py` & `ansar_connect-0.1.209/src/ansar/connect/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,53 +320,65 @@
 
 ar.bind(ServiceRoute, SERVICE_ROUTE_DISPATCH)
 
 # Messages from match object (ServiceRoute) to the two different
 # ends of the relation. The PublishingAgent and SubscriptionAgent objects
 # will receive and initiate "calls" based on these messages.
 class RouteToAddress(object):
-	def __init__(self, matched_scope=None, agent_address=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, agent_address=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.agent_address = agent_address
 		self.route_key = route_key
 
 class InboundFromAddress(object):
-	def __init__(self, matched_scope=None, agent_address=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, agent_address=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.agent_address = agent_address
 		self.route_key = route_key
 
 class RouteOverConnected(object):
-	def __init__(self, matched_scope=None, connecting_ipp=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, connecting_ipp=None, route_key=None):
 		self.matched_scope = matched_scope
 		self.connecting_ipp = connecting_ipp or HostPort()
 		self.route_key = route_key
 
 class InboundOverAccepted(object):
-	def __init__(self, matched_scope=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 
 class RouteByRelay():
-	def __init__(self, matched_scope=None, redirect=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, redirect=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.redirect = redirect or RelayRedirect()
 		self.route_key = route_key
 
 class InboundByRelay():
-	def __init__(self, matched_scope=None, redirect=None, route_key=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, redirect=None, route_key=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.redirect = redirect or RelayRedirect()
 		self.route_key = route_key
 
 IO_SCHEMA = {
 	'agent_address': ar.Address(),
 	'route_key': str,
 	'name': str,
 	'connecting_ipp': ar.UserDefined(HostPort),
+	'matched_search': ar.Unicode(),
+	'matched_name': ar.Unicode(),
 	'matched_scope': ScopeOfService,
 	'redirect': ar.UserDefined(RelayRedirect),
 }
 
 ar.bind(RouteToAddress, object_schema=IO_SCHEMA)
 ar.bind(InboundFromAddress, object_schema=IO_SCHEMA)
 ar.bind(RouteOverConnected, object_schema=IO_SCHEMA)
@@ -420,50 +432,59 @@
 # of connection between subscriber and publisher.
 class DirectService(object):
 	def __init__(self, find, listing):
 		self.find = find
 		self.listing = listing
 
 	def outbound(self, route_key):
-		return RouteToAddress(matched_scope=ScopeOfService.PROCESS, agent_address=self.listing.agent_address, route_key=route_key)
+		return RouteToAddress(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=ScopeOfService.PROCESS,
+			agent_address=self.listing.agent_address, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundFromAddress(matched_scope=ScopeOfService.PROCESS, agent_address=self.find.agent_address, route_key=route_key)
+		return InboundFromAddress(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=ScopeOfService.PROCESS,
+			agent_address=self.find.agent_address, route_key=route_key)
 
 # Between two objects needing a TCP connection from
 # subscribing process to publishing process. Listening
 # address needs tuning based on whether its intra-host
 # or across a LAN.
 class ServiceOverConnection(object):
 	def __init__(self, matched_scope, find, listing):
 		self.find = find
 		self.listing = listing
 		self.matched_scope = matched_scope
 
 	def outbound(self, route_key):
-		return RouteOverConnected(matched_scope=self.matched_scope, connecting_ipp=self.listing.connecting_ipp, route_key=route_key)
+		return RouteOverConnected(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=self.matched_scope,
+			connecting_ipp=self.listing.connecting_ipp, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundOverAccepted(matched_scope=self.matched_scope, route_key=route_key)
+		return InboundOverAccepted(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=self.matched_scope, route_key=route_key)
 
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
-		return RouteByRelay(matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
+		return RouteByRelay(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
 
 	def inbound(self, route_key):
-		return InboundByRelay(matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
+		return InboundByRelay(matched_search=self.find.requested_search, matched_name=self.listing.requested_name,
+			matched_scope=ScopeOfService.WAN, redirect=self.redirect, route_key=route_key)
 
 # The per-process part of the distributed name service.
 # Accepts local listings and searches and creates matches.
 # Receives listings and searches from below as well. All
 # information forwarded to next level up.
 def key_service(route_key):
 	try:
```

### Comparing `ansar_connect-0.1.208/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.209/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.209/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/group_if.py` & `ansar_connect-0.1.209/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/grouping.py` & `ansar_connect-0.1.209/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/moving.py` & `ansar_connect-0.1.209/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/networking.py` & `ansar_connect-0.1.209/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.209/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/node.py` & `ansar_connect-0.1.209/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.209/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/procedure.py` & `ansar_connect-0.1.209/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/product.py` & `ansar_connect-0.1.209/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/socketry.py` & `ansar_connect-0.1.209/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/standard.py` & `ansar_connect-0.1.209/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/transporting.py` & `ansar_connect-0.1.209/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.209/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar/connect/wan.py` & `ansar_connect-0.1.209/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.208/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.209/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.208
+Version: 0.1.209
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.208/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.209/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

