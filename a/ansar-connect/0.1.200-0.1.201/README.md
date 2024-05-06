# Comparing `tmp/ansar_connect-0.1.200.tar.gz` & `tmp/ansar_connect-0.1.201.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.200.tar", last modified: Fri Apr 19 08:13:54 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.201.tar", last modified: Sun May  5 23:29:18 2024, max compression
```

## Comparing `ansar_connect-0.1.200.tar` & `ansar_connect-0.1.201.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.424318 ansar_connect-0.1.200/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.200/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-19 08:13:54.424318 ansar_connect-0.1.200/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.200/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.200/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-19 08:13:54.424318 ansar_connect-0.1.200/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.200/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.420318 ansar_connect-0.1.200/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.420318 ansar_connect-0.1.200/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.420318 ansar_connect-0.1.200/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.200/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.200/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.424318 ansar_connect-0.1.200/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-19 08:13:51.000000 ansar_connect-0.1.200/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77775 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.200/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.200/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.200/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.200/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.200/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.200/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.200/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.200/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.200/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.200/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.200/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.200/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.200/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.200/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.200/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 08:13:54.424318 ansar_connect-0.1.200/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-19 08:13:54.000000 ansar_connect-0.1.200/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.201/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.201/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.201/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.201/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.201/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.201/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-05 23:29:15.000000 ansar_connect-0.1.201/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    79308 2024-05-05 21:57:14.000000 ansar_connect-0.1.201/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7833 2024-05-05 21:45:40.000000 ansar_connect-0.1.201/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.201/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.201/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.201/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-05 21:23:08.000000 ansar_connect-0.1.201/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.201/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.201/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.201/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.201/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.201/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.201/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.201/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.201/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.201/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.201/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-05 23:29:18.778078 ansar_connect-0.1.201/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-05 23:29:18.000000 ansar_connect-0.1.201/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.200/LICENSE` & `ansar_connect-0.1.201/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/PKG-INFO` & `ansar_connect-0.1.201/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.200
+Version: 0.1.201
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.200/README.md` & `ansar_connect-0.1.201/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/pyproject.toml` & `ansar_connect-0.1.201/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/setup.py` & `ansar_connect-0.1.201/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.201/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.201/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.201/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.201/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/__init__.py` & `ansar_connect-0.1.201/src/ansar/connect/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: b8c835b34e67358ab8fea9dd22b1d5665da043a6
-Version: 0.1.199 (2024-04-19@20:13:51+NZST)
+Commit: 7dff7b9c46fc0778d7e56b0cfa9b2dc756c3cb7d
+Version: 0.1.200 (2024-05-06@11:29:15+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.200/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.201/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/directory.py` & `ansar_connect-0.1.201/src/ansar/connect/directory.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,87 +118,87 @@
 		root.select(ar.Ack, seconds=5.0)
 
 ar.AddOn(create_directory, stop_directory)
 
 # Private communications from the pub-sub api (i.e. ar.publish()) to
 # the operational machinery.
 class PublishAsName(object):
-	def __init__(self, requested_name=None, create_session=None, declared_scope=ScopeOfService.WAN):
+	def __init__(self, requested_name=None, create_session=None, requested_scope=ScopeOfService.WAN):
 		self.requested_name = requested_name
 		self.create_session = create_session
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 
 class SubscribeToName(object):
-	def __init__(self, requested_search=None, create_session=None, declared_scope=ScopeOfService.WAN):
+	def __init__(self, requested_search=None, create_session=None, requested_scope=ScopeOfService.WAN):
 		self.requested_search = requested_search
 		self.create_session = create_session
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 
 class Retract(object):
 	def __init__(self, address=None):
 		self.address = address
 
 # Private communications within the directory hierarchy, e.g. ServiceListing is sent from
 # the PublishingAgent to the local directory and is then passed up the chain of directories.
 class ServiceListing(object):
-	def __init__(self, requested_name=None, agent_address=None, declared_scope=ScopeOfService.WAN, listing_id=None, listening_ipp=None, connecting_ipp=None):
+	def __init__(self, requested_name=None, agent_address=None, requested_scope=ScopeOfService.WAN, listing_id=None, listening_ipp=None, connecting_ipp=None):
 		self.requested_name = requested_name
 		self.agent_address = agent_address
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 		self.listing_id = listing_id
 		self.listening_ipp = listening_ipp or HostPort()
 		self.connecting_ipp = connecting_ipp or HostPort()
 
 class FindService(object):
-	def __init__(self, requested_search=None, agent_address=None, declared_scope=ScopeOfService.WAN):
+	def __init__(self, requested_search=None, agent_address=None, requested_scope=ScopeOfService.WAN):
 		self.requested_search = requested_search
 		self.agent_address = agent_address
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 
 class PushedDirectory(object):
 	def __init__(self, listing=None, find=None):
 		self.listing = listing
 		self.find = find
 
 	def empty(self):
 		if len(self.listing) == 0 and len(self.find) == 0:
 			return True
 		return False
 
 class UnlistService(object):
-	def __init__(self, requested_name=None, agent_address=None, declared_scope=None):
+	def __init__(self, requested_name=None, agent_address=None, requested_scope=None):
 		self.requested_name = requested_name
 		self.agent_address = agent_address
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 
 class UnlistFind(object):
-	def __init__(self, subscribed_search=None, agent_address=None, declared_scope=None):
-		self.subscribed_search = subscribed_search
+	def __init__(self, requested_search=None, agent_address=None, requested_scope=None):
+		self.requested_search = requested_search
 		self.agent_address = agent_address
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 
 class TrimRoutes(object):
 	def __init__(self, address=None):
 		self.address = address
 
 class CapRoutes(object):
 	def __init__(self, service_scope=None):
 		self.service_scope = service_scope
 
 class RetractRoute(object):
-	def __init__(self, key=None):
-		self.key = key
+	def __init__(self, route_key=None):
+		self.route_key = route_key
 
 SHARED_SCHEMA = {
-	#'key': ar.VectorOf(ar.Integer8()),
-	'key': str,
+	#'route_key': ar.VectorOf(ar.Integer8()),
+	'route_key': str,
 	'requested_name': str,
 	'requested_search': str,
-	'subscribed_search': str,
-	'declared_scope': ScopeOfService,
+	'requested_search': str,
+	'requested_scope': ScopeOfService,
 	'listing_id': ar.UUID(),
 	'service_scope': ScopeOfService,
 	'create_session': ar.Type(),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'connecting_ipp': ar.UserDefined(HostPort),
 	'parent_ipp': ar.UserDefined(HostPort),
 	'child_ipp': ar.UserDefined(HostPort),
@@ -234,33 +234,33 @@
 # updates the two parties as needed. Routes are fairly static.
 # They are only affected by changes to the directory tree. Routes
 # are the basis for sessions. The session abstraction is in the
 # SubscriptionAgent object using "loop" messages to establish
 # a "subscriber loop" to a remote end over dedicated transports,
 # i.e. not the same transports used by the directory tree.
 class ServiceRoute(ar.Point, ar.StateMachine):
-	def __init__(self, key, find_address, listing_address, connection):
+	def __init__(self, route_key, find_address, listing_address, connection):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
-		self.key = key
+		self.route_key = route_key
 		self.find_address = find_address
 		self.listing_address = listing_address
 		self.connection = connection
 
 def ServiceRoute_INITIAL_Start(self, message):
 	if isinstance(self.connection, ServiceByRelay):
 		# Start creating the relay. This goes to the
 		# object that created this instance of a
 		# directory, e.g. an instance of wan process.
 		relay_id = uuid.uuid4()
 		self.send(RelayLookup(relay_id=relay_id), self.connection.relay_address)
 		self.start(ar.T1, 5.0)
 		return RELAYING
-	outbound = self.connection.outbound(self.key)
-	inbound = self.connection.inbound(self.key)
+	outbound = self.connection.outbound(self.route_key)
+	inbound = self.connection.inbound(self.route_key)
 
 	out_type = outbound.__art__.name
 	in_type = inbound.__art__.name
 
 	out_address = address_to_text(self.find_address)
 	in_address = address_to_text(self.listing_address)
 
@@ -269,16 +269,16 @@
 
 	self.send(outbound, self.find_address)
 	self.send(inbound, self.listing_address)
 	return NORMAL
 
 def ServiceRoute_RELAYING_RelayRedirect(self, message):
 	self.connection.redirect = message
-	outbound = self.connection.outbound(self.key)
-	inbound = self.connection.inbound(self.key)
+	outbound = self.connection.outbound(self.route_key)
+	inbound = self.connection.inbound(self.route_key)
 
 	out_type = outbound.__art__.name
 	in_type = inbound.__art__.name
 
 	out_address = address_to_text(self.find_address)
 	in_address = address_to_text(self.listing_address)
 
@@ -298,16 +298,16 @@
 
 def ServiceRoute_NORMAL_Stop(self, message):
 	out_address = address_to_text(self.find_address)
 	in_address = address_to_text(self.listing_address)
 
 	self.trace(f'Match sends RetractRoute to [{out_address}] and [{in_address}] and completes')
 	
-	self.send(RetractRoute(self.key), self.find_address)
-	self.send(RetractRoute(self.key), self.listing_address)
+	self.send(RetractRoute(self.route_key), self.find_address)
+	self.send(RetractRoute(self.route_key), self.listing_address)
 	self.complete(ar.Aborted())
 
 SERVICE_ROUTE_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	RELAYING: (
@@ -320,51 +320,51 @@
 
 ar.bind(ServiceRoute, SERVICE_ROUTE_DISPATCH)
 
 # Messages from match object (ServiceRoute) to the two different
 # ends of the relation. The PublishingAgent and SubscriptionAgent objects
 # will receive and initiate "calls" based on these messages.
 class RouteToAddress(object):
-	def __init__(self, scope=None, address=None, key=None):
+	def __init__(self, scope=None, address=None, route_key=None):
 		self.scope = scope
 		self.address = address
-		self.key = key
+		self.route_key = route_key
 
 class InboundFromAddress(object):
-	def __init__(self, scope=None, address=None, key=None):
+	def __init__(self, scope=None, address=None, route_key=None):
 		self.scope = scope
 		self.address = address
-		self.key = key
+		self.route_key = route_key
 
 class RouteOverConnected(object):
-	def __init__(self, scope=None, connecting_ipp=None, key=None):
+	def __init__(self, scope=None, connecting_ipp=None, route_key=None):
 		self.scope = scope
 		self.connecting_ipp = connecting_ipp or HostPort()
-		self.key = key
+		self.route_key = route_key
 
 class InboundOverAccepted(object):
-	def __init__(self, scope=None, key=None):
+	def __init__(self, scope=None, route_key=None):
 		self.scope = scope
-		self.key = key
+		self.route_key = route_key
 
 class RouteByRelay():
-	def __init__(self, scope=None, redirect=None, key=None):
+	def __init__(self, scope=None, redirect=None, route_key=None):
 		self.scope = scope
 		self.redirect = redirect or RelayRedirect()
-		self.key = key
+		self.route_key = route_key
 
 class InboundByRelay():
-	def __init__(self, scope=None, redirect=None, key=None):
+	def __init__(self, scope=None, redirect=None, route_key=None):
 		self.scope = scope
 		self.redirect = redirect or RelayRedirect()
-		self.key = key
+		self.route_key = route_key
 
 IO_SCHEMA = {
 	'address': ar.Address(),
-	'key': str,
+	'route_key': str,
 	'name': str,
 	'connecting_ipp': ar.UserDefined(HostPort),
 	'scope': ScopeOfService,
 	'redirect': ar.UserDefined(RelayRedirect),
 }
 
 ar.bind(RouteToAddress, object_schema=IO_SCHEMA)
@@ -373,43 +373,43 @@
 ar.bind(InboundOverAccepted, object_schema=IO_SCHEMA)
 ar.bind(RouteByRelay, object_schema=IO_SCHEMA)
 ar.bind(InboundByRelay, object_schema=IO_SCHEMA)
 
 #
 #
 class OpenPeer(object):
-	def __init__(self, connecting_ipp=None, key=None, encrypted=None):
+	def __init__(self, connecting_ipp=None, route_key=None, encrypted=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
-		self.key = key
+		self.route_key = route_key
 		self.encrypted = encrypted
 
 class PeerOpened(object):
-	def __init__(self, connecting_ipp=None, key=None):
+	def __init__(self, connecting_ipp=None, route_key=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
-		self.key = key
+		self.route_key = route_key
 
 class NotPeered(object):
-	def __init__(self, key=None, reason=None, connecting_ipp=None):
-		self.key = key
+	def __init__(self, route_key=None, reason=None, connecting_ipp=None):
+		self.route_key = route_key
 		self.reason = reason
 		self.connecting_ipp = connecting_ipp or HostPort()
 
 class PeerLost(object):
-	def __init__(self, connecting_ipp=None, key=None):
+	def __init__(self, connecting_ipp=None, route_key=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
-		self.key = key
+		self.route_key = route_key
 
 class ClosePeer(object):
-	def __init__(self, connecting_ipp=None, key=None):
+	def __init__(self, connecting_ipp=None, route_key=None):
 		self.connecting_ipp = connecting_ipp or HostPort()
-		self.key = key
+		self.route_key = route_key
 
 PEER_SCHEMA = {
 	'connecting_ipp': ar.UserDefined(HostPort),
-	'key': str,
+	'route_key': str,
 	'reason': str,
 	'encrypted': ar.Any(),
 }
 
 ar.bind(OpenPeer, object_schema=PEER_SCHEMA)
 ar.bind(PeerOpened, object_schema=PEER_SCHEMA)
 ar.bind(NotPeered, object_schema=PEER_SCHEMA)
@@ -419,68 +419,68 @@
 # Objects that capture the requirements for 3 different methods
 # of connection between subscriber and publisher.
 class DirectService(object):
 	def __init__(self, find, listing):
 		self.find = find
 		self.listing = listing
 
-	def outbound(self, key):
-		return RouteToAddress(ScopeOfService.PROCESS, self.listing.agent_address, key)
+	def outbound(self, route_key):
+		return RouteToAddress(ScopeOfService.PROCESS, self.listing.agent_address, route_key)
 
-	def inbound(self, key):
-		return InboundFromAddress(ScopeOfService.PROCESS, self.find.agent_address, key)
+	def inbound(self, route_key):
+		return InboundFromAddress(ScopeOfService.PROCESS, self.find.agent_address, route_key)
 
 # Between two objects needing a TCP connection from
 # subscribing process to publishing process. Listening
 # address needs tuning based on whether its intra-host
 # or across a LAN.
 class ServiceOverConnection(object):
 	def __init__(self, scope, find, listing):
 		self.scope = scope
 		self.find = find
 		self.listing = listing
 
-	def outbound(self, key):
-		return RouteOverConnected(self.scope, self.listing.connecting_ipp, key)
+	def outbound(self, route_key):
+		return RouteOverConnected(self.scope, self.listing.connecting_ipp, route_key)
 
-	def inbound(self, key):
-		return InboundOverAccepted(self.scope, key)
+	def inbound(self, route_key):
+		return InboundOverAccepted(self.scope, route_key)
 
 # The extra step needed for relay setup. A query/response
 # needed with the relay manager before the connection
 # messages can be sent to the ends of the call.
 class ServiceByRelay(object):
 	def __init__(self, finding, listing, relay_address):
 		self.relay_address = relay_address
 		self.redirect = None
 
-	def outbound(self, key):
-		return RouteByRelay(ScopeOfService.WAN, self.redirect, key)
+	def outbound(self, route_key):
+		return RouteByRelay(ScopeOfService.WAN, self.redirect, route_key)
 
-	def inbound(self, key):
-		return InboundByRelay(ScopeOfService.WAN, self.redirect, key)
+	def inbound(self, route_key):
+		return InboundByRelay(ScopeOfService.WAN, self.redirect, route_key)
 
 # The per-process part of the distributed name service.
 # Accepts local listings and searches and creates matches.
 # Receives listings and searches from below as well. All
 # information forwarded to next level up.
-def key_service(key):
+def key_service(route_key):
 	try:
-		i = key.index(':')
+		i = route_key.index(':')
 	except ValueError:
 		return None
-	return key[i + 1:]
+	return route_key[i + 1:]
 
-def key_id(key):
+def key_id(route_key):
 	try:
-		a = key.index('@')
-		c = key.index(':')
+		a = route_key.index('@')
+		c = route_key.index(':')
 	except ValueError:
 		return None
-	return key[a + 1:c]
+	return route_key[a + 1:c]
 
 def id_connection(kid):
 	try:
 		a = kid.index('(')
 		c = kid.index(')')
 	except ValueError:
 		return None
@@ -532,38 +532,38 @@
 		find_matched = f[1]
 		listing_address = listing.agent_address
 		listing_id = listing.listing_id
 		listing_matched = d[1]
 
 		# As well as being unique within this directory the
 		# connection engine in the subscriber agent relies on
-		# content and layout of this key. Refer to
+		# content and layout of this route_key. Refer to
 		# key_service(), key_id(), etc.
 		who = address_to_text(find_address)
-		key = f'{who}@{listing_address}{listing_id}:{listing.requested_name}'
+		route_key = f'{who}@{listing_address}{listing_id}:{listing.requested_name}'
 
-		if key in self.matched:
-			self.warning(f'Duplicate find/service match [{ScopeOfService.to_name(self.scope)}] "{key}"')
+		if route_key in self.matched:
+			self.warning(f'Duplicate find/service match [{ScopeOfService.to_name(self.scope)}] "{route_key}"')
 			return
-		self.trace(f'Adds route [{ScopeOfService.to_name(self.scope)}] "{key}"')
+		self.trace(f'Adds route [{ScopeOfService.to_name(self.scope)}] "{route_key}"')
 
 		# Everything lines up - we have a relation. Connection details
 		# are dependent on where this directory is running.
 		if self.scope == ScopeOfService.PROCESS:
-			a = self.create(ServiceRoute, key, find_address, listing_address, DirectService(find, listing))
+			a = self.create(ServiceRoute, route_key, find_address, listing_address, DirectService(find, listing))
 		elif self.scope in (ScopeOfService.GROUP, ScopeOfService.HOST, ScopeOfService.LAN):
-			a = self.create(ServiceRoute, key, find_address, listing_address, ServiceOverConnection(self.scope, find, listing))
+			a = self.create(ServiceRoute, route_key, find_address, listing_address, ServiceOverConnection(self.scope, find, listing))
 		elif self.scope == ScopeOfService.WAN:
-			a = self.create(ServiceRoute, key, find_address, listing_address, ServiceByRelay(find, listing, self.parent_address))
+			a = self.create(ServiceRoute, route_key, find_address, listing_address, ServiceByRelay(find, listing, self.parent_address))
 		else:
 			self.warning(f'Directory at unknown scope "{self.scope}"')
-		self.assign(a, key)
-		self.matched[key] = a
-		find_matched.add(key)
-		listing_matched.add(key)
+		self.assign(a, route_key)
+		self.matched[route_key] = a
+		find_matched.add(route_key)
+		listing_matched.add(route_key)
 
 	def conclude_host(self, address, message):
 		"""Determine a host address suitable for connection.
 
 		Combine the network info accumulated for accepted connections
 		and the information offered in a service listing to resolve
 		the most appropriate host address to use for connection. Most
@@ -671,15 +671,15 @@
 		
 		for k in d[1]:
 			a = self.matched.get(k, None)
 			if a:
 				self.send(ar.Stop(), a)
 
 	def remove_find(self, message):
-		find_name = message.subscribed_search
+		find_name = message.requested_search
 		find_address = message.agent_address
 
 		jf = address_to_text(find_address)
 		k = f'{jf}/{find_name}'
 
 		# Remove the entry and terminate any routes that
 		# were based on its existence.
@@ -692,16 +692,16 @@
 		
 		for k in f[1]:
 			a = self.matched.get(k, None)
 			if a:
 				self.send(ar.Stop(), a)
 
 	def top_of_directory(self):
-		listing = [v[0] for k, v in self.directory.items() if v[0].declared_scope > self.scope]
-		find = [v[0] for k, v in self.find.items() if v[0].declared_scope > self.scope]
+		listing = [v[0] for k, v in self.directory.items() if v[0].requested_scope > self.scope]
+		find = [v[0] for k, v in self.find.items() if v[0].requested_scope > self.scope]
 		return PushedDirectory(listing, find)
 
 	# self.directory[service_name] = [FindService, set()]
 	# self.find[search_key] = [FindService, set()]
 	#
 	# All the finds that matched to a service.
 	# for k in self.find[search_key][1]:
@@ -896,75 +896,75 @@
 	nl = len(message.listing)
 	nf = len(message.find)
 
 	self.trace(f'Pushed "{nl}" listings and "{nf}" finds')
 
 	for s in message.listing:
 		# Suppress those listings at lower levels.
-		if s.declared_scope < self.scope:
+		if s.requested_scope < self.scope:
 			continue
 		# Patch the connecting ipp for those scenarios involving
 		# a secondary connection, i.e. a peer.
 		if self.scope in (ScopeOfService.GROUP, ScopeOfService.HOST, ScopeOfService.LAN):
 			self.conclude_host(self.return_address, s)
 
 		self.add_listing(s)
 
 	for f in message.find:
 		# Suppress those listings at lower levels.
-		if f.declared_scope < self.scope:
+		if f.requested_scope < self.scope:
 			continue
 		self.add_find(f)
 
 	if self.connected_up:
 		self.send(message, self.connected_up)
 	return NORMAL
 
 ### PS-pub-9 Directory accepts listing.
 def ServiceDirectory_NORMAL_ServiceListing(self, message):
 	# Suppress those listings at lower levels.
-	if message.declared_scope < self.scope:
+	if message.requested_scope < self.scope:
 		return NORMAL
 	if self.scope in (ScopeOfService.GROUP, ScopeOfService.HOST, ScopeOfService.LAN):
 		### PS-pub-9 Directory patches listing IP-port.
 		self.conclude_host(self.return_address, message)
 	self.add_listing(message)
 
 	### PS-pub-9 Directory propagates listing.
-	if self.connected_up and message.declared_scope > self.scope:
+	if self.connected_up and message.requested_scope > self.scope:
 		self.send(message, self.connected_up)
 	return NORMAL
 
 ### PS-sub-8 Directory accepts find.
 def ServiceDirectory_NORMAL_FindService(self, message):
 	# Suppress those listings at lower levels.
-	if message.declared_scope < self.scope:
+	if message.requested_scope < self.scope:
 		return NORMAL
 	self.add_find(message)
 
 	### PS-sub-8 Directory propagates find.
-	if self.connected_up and message.declared_scope > self.scope:
+	if self.connected_up and message.requested_scope > self.scope:
 		self.send(message, self.connected_up)
 	return NORMAL
 
 def ServiceDirectory_NORMAL_UnlistService(self, message):
 	# Suppress those listings at lower levels.
-	if message.declared_scope < self.scope:
+	if message.requested_scope < self.scope:
 		return NORMAL
 	self.remove_listing(message)
-	if self.connected_up and message.declared_scope > self.scope:
+	if self.connected_up and message.requested_scope > self.scope:
 		self.send(message, self.connected_up)
 	return NORMAL
 
 def ServiceDirectory_NORMAL_UnlistFind(self, message):
 	# Suppress those listings at lower levels.
-	if message.declared_scope < self.scope:
+	if message.requested_scope < self.scope:
 		return NORMAL
 	self.remove_find(message)
-	if self.connected_up and message.declared_scope > self.scope:
+	if self.connected_up and message.requested_scope > self.scope:
 		self.send(message, self.connected_up)
 	return NORMAL
 
 def ServiceDirectory_NORMAL_CapRoutes(self, message):
 	self.forward(message, pb.house, self.return_address)
 
 	self.trace(f'Broadcasting cap to {len(self.accepted)} sub-directories')
@@ -1038,28 +1038,28 @@
 	m, a = self.reconnecting[0], self.reconnecting[1]
 	self.connect_above = m.connect_above
 	self.send(ar.Anything(m.connect_above), self.ctd)
 	self.send(ar.Ack(), a)
 	return NORMAL
 
 def ServiceDirectory_NORMAL_Completed(self, message):
-	key = self.debrief()
-	a = self.matched.pop(key, None)
+	route_key = self.debrief()
+	a = self.matched.pop(route_key, None)
 	if a is None:
 		return NORMAL
 
-	# Clear key from pub/sub.
+	# Clear route_key from pub/sub.
 	for d in self.directory.values():
-		if key in d[1]:
-			d[1].discard(key)
+		if route_key in d[1]:
+			d[1].discard(route_key)
 			break
 
 	for f in self.find.values():
-		if key in f[1]:
-			f[1].discard(key)
+		if route_key in f[1]:
+			f[1].discard(route_key)
 			break
 
 	return NORMAL
 
 def ServiceDirectory_NORMAL_Stop(self, message):
 	self.stopped = self.return_address
 	self.abort()
@@ -1105,45 +1105,45 @@
 }
 
 ar.bind(ServiceDirectory, SERVICE_DIRECTORY_DISPATCH)
 
 # The preliminary exchange to trade end-point addresses
 #
 class OpenLoop(object):
-	def __init__(self, subscriber_session=None, key=None):
+	def __init__(self, subscriber_session=None, route_key=None):
 		self.subscriber_session = subscriber_session
-		self.key = key
+		self.route_key = route_key
 
 class LoopOpened(object):
-	def __init__(self, publisher_session=None, key=None):
+	def __init__(self, publisher_session=None, route_key=None):
 		self.publisher_session = publisher_session
-		self.key = key
+		self.route_key = route_key
 
 class CloseLoop(object):
-	def __init__(self, key=None):
-		self.key = key
+	def __init__(self, route_key=None):
+		self.route_key = route_key
 
 INTRODUCTION_SCHEMA = {
 	'subscriber_session': ar.Address(),
 	'publisher_session': ar.Address(),
-	'key': str,
+	'route_key': str,
 }
 
 ar.bind(OpenLoop, object_schema=INTRODUCTION_SCHEMA)
 ar.bind(LoopOpened, object_schema=INTRODUCTION_SCHEMA)
 ar.bind(CloseLoop, object_schema=INTRODUCTION_SCHEMA)
 
 #
 #
 class PublisherLoop(ar.Point, ar.StateMachine):
 	def __init__(self, route, remote_session, remote_loop, publisher_address, create_session, relay_address):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.route = route
-		self.key = route.key
+		self.route_key = route.route_key
 		self.remote_session = remote_session
 		self.remote_loop = remote_loop
 		self.publisher_address = publisher_address
 		self.create_session = create_session
 		self.relay_address = relay_address
 
 		self.session_address = None
@@ -1168,33 +1168,33 @@
 			**cs.kw)
 		self.session_address = self.created_session
 		self.origin_address = self.created_session
 	else:
 		self.session_address = self.publisher_address
 		self.origin_address = self.remote_session
 
-	self.send(LoopOpened(self.session_address, self.key), self.remote_loop)
-	self.forward(Delivered(self.key, self.address), self.publisher_address, self.origin_address)
+	self.send(LoopOpened(self.session_address, self.route_key), self.remote_loop)
+	self.forward(Delivered(self.route_key, self.address), self.publisher_address, self.origin_address)
 	return LOOPED
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
 	if self.created_session and self.return_address == self.created_session:
 		self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
-		self.send(CloseLoop(self.key), self.remote_loop)
+		self.send(CloseLoop(self.route_key), self.remote_loop)
 		self.close_route()
 		self.complete(ar.Aborted())
 	self.warning('Unexpected termination')
 	return LOOPED
 
 ### PS-pub-8 Loop terminates by local clear().
 def PublisherLoop_LOOPED_Close(self, message):
 	self.closing, self.value = True, message.value
-	self.send(CloseLoop(self.key), self.remote_loop)
+	self.send(CloseLoop(self.route_key), self.remote_loop)
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
 	self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
@@ -1207,15 +1207,15 @@
 	self.close_route()
 
 	self.forward(Dropped('abandoned by remote'), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by local exit.
 def PublisherLoop_LOOPED_Stop(self, message):
-	self.send(CloseLoop(self.key), self.remote_loop)
+	self.send(CloseLoop(self.route_key), self.remote_loop)
 	if self.created_session:
 		self.send(message, self.created_session)
 		return CLEARING
 	self.close_route()
 
 	self.forward(Dropped('aborted'), self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
@@ -1247,220 +1247,220 @@
 }
 
 ar.bind(PublisherLoop, PUBLISHER_LOOP_DISPATCH, thread='published')
 
 # An object to maintain a listen on behalf of a published
 # name. Enters name and listen into the service directory.
 class PublishingAgent(ar.Point, ar.StateMachine):
-	def __init__(self, requested_name, publisher_address, create_session, declared_scope):
+	def __init__(self, requested_name, publisher_address, create_session, requested_scope):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.requested_name = requested_name
 		self.publisher_address = publisher_address
 		self.create_session = create_session
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 		self.listening = None
 		self.matching = {}
 		self.loop = {}
 		self.relay = {}
 		self.peered = {}
 		self.relay_address = {}
 
 def PublishingAgent_INITIAL_Start(self, message):
-	if self.declared_scope == ScopeOfService.PROCESS:
+	if self.requested_scope == ScopeOfService.PROCESS:
 		### PS-pub-3 Agent sends listing to directory.
 		listing_id = uuid.uuid4()
 		self.send(ServiceListing(requested_name=self.requested_name,
-			agent_address=self.address, declared_scope=self.declared_scope,
+			agent_address=self.address, requested_scope=self.requested_scope,
 			listing_id=listing_id), pb.directory)
-		self.send(Published(self.requested_name, self.declared_scope), self.publisher_address)
+		self.send(Published(self.requested_name, self.requested_scope), self.publisher_address)
 		return READY
-	elif self.declared_scope in (ScopeOfService.GROUP, ScopeOfService.HOST):
+	elif self.requested_scope in (ScopeOfService.GROUP, ScopeOfService.HOST):
 		### PS-pub-3 Agent arranges for inbound listen.
 		listen(self, LocalPort(0))
 		return PENDING
-	elif self.declared_scope in (ScopeOfService.LAN, ScopeOfService.WAN):
+	elif self.requested_scope in (ScopeOfService.LAN, ScopeOfService.WAN):
 		listen(self, HostPort('0.0.0.0', 0))
 		return PENDING
 	return READY
 
 def PublishingAgent_PENDING_Listening(self, message):
 	self.listening = message
 	listing_id = uuid.uuid4()
 	self.send(ServiceListing(requested_name=self.requested_name,
-		agent_address=self.address, declared_scope=self.declared_scope,
+		agent_address=self.address, requested_scope=self.requested_scope,
 		listing_id=listing_id,
 		listening_ipp=message.listening_ipp), pb.directory)
-	self.send(Published(self.requested_name, self.declared_scope, message.listening_ipp), self.publisher_address)
+	self.send(Published(self.requested_name, self.requested_scope, message.listening_ipp), self.publisher_address)
 	return READY
 
 def PublishingAgent_PENDING_NotListening(self, message):
 	ipp = message.requested_ipp
 	t = message.error_text
 	self.warning(f'Cannot allocate a listen for {ipp} ({t})')
 	self.start(ar.T1, 60.0)
 	return GLARING
 
 def PublishingAgent_PENDING_Stop(self, message):
-	self.send(UnlistService(self.requested_name, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistService(self.requested_name, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 def PublishingAgent_GLARING_T1(self, message):
-	if self.declared_scope in (ScopeOfService.GROUP, ScopeOfService.HOST):
+	if self.requested_scope in (ScopeOfService.GROUP, ScopeOfService.HOST):
 		listen(self, LocalPort(0))
 		return PENDING
-	elif self.declared_scope in (ScopeOfService.LAN, ScopeOfService.WAN):
+	elif self.requested_scope in (ScopeOfService.LAN, ScopeOfService.WAN):
 		listen(self, HostPort('0.0.0.0', 0))
 		return PENDING
 	return READY
 
 def PublishingAgent_GLARING_Stop(self, message):
-	self.send(UnlistService(self.requested_name, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistService(self.requested_name, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 def looped(self, inbound, open, return_address):
 	if inbound is None or open is None or return_address is None:
 		return
-	key = open.key
-	relay_address = self.relay_address.get(key, None)
+	route_key = open.route_key
+	relay_address = self.relay_address.get(route_key, None)
 	### PS-pub-6 Agent creates local loop.
 	a = self.create(PublisherLoop, inbound, open.subscriber_session, return_address,
 		self.publisher_address, self.create_session,
 		relay_address)
-	self.assign(a, key)
-	self.loop[key] = a
+	self.assign(a, route_key)
+	self.loop[route_key] = a
 
 ### PS-pub-4 Agent accepts internal route.
 def PublishingAgent_READY_InboundFromAddress(self, message):
-	key = message.key
+	route_key = message.route_key
 
 	try:
-		m = self.matching[key]
+		m = self.matching[route_key]
 	except KeyError:
 		m = [message, None, None]
-		self.matching[key] = m
-		self.trace(f'Added direct route [{ScopeOfService.to_name(message.scope)}]({key})')
+		self.matching[route_key] = m
+		self.trace(f'Added direct route [{ScopeOfService.to_name(message.scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 
 ### PS-pub-4 Agent accepts peer route.
 
 def PublishingAgent_READY_InboundOverAccepted(self, message):
-	key = message.key
+	route_key = message.route_key
 
 	try:
-		m = self.matching[key]
+		m = self.matching[route_key]
 	except KeyError:
 		m = [message, None, None]
-		self.matching[key] = m
-		self.trace(f'Added peer route [{ScopeOfService.to_name(message.scope)}]({key})')
+		self.matching[route_key] = m
+		self.trace(f'Added peer route [{ScopeOfService.to_name(message.scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 
 def PublishingAgent_READY_InboundByRelay(self, message):
-	key = message.key
+	route_key = message.route_key
 	try:
-		relay = self.relay[key]
-		self.warning(f'Duplicate relay "{key}" (ignored)')
+		relay = self.relay[route_key]
+		self.warning(f'Duplicate relay "{route_key}" (ignored)')
 		return READY
 	except KeyError:
 		relay = message
-		self.relay[key] = relay
+		self.relay[route_key] = relay
 
 	ipp = relay.redirect.redirect_ipp
 	k = ipp_key(ipp)
 
 	try:
 		r = self.peered[k]
-		r[1][key] = relay
+		r[1][route_key] = relay
 		n = len(r[1])
-		self.trace(f'Peer for relay "{key}" already known ({n} routes pending)')
+		self.trace(f'Peer for relay "{route_key}" already known ({n} routes pending)')
 	except KeyError:
-		r = [None, {key: relay}]
+		r = [None, {route_key: relay}]
 		self.peered[k] = r
 
-		self.trace(f'Opening peer "{k}" (relay {key})')
+		self.trace(f'Opening peer "{k}" (relay {route_key})')
 		encrypted = message.redirect.encrypted
-		open = OpenPeer(ipp, key, encrypted=encrypted)
+		open = OpenPeer(ipp, route_key, encrypted=encrypted)
 		self.send(open, pb.house)
 		return READY
 
 	if r[0] is None:
 		return READY
 
 	self.send(relay, r[0])
-	self.relay_address[key] = r[0]
+	self.relay_address[route_key] = r[0]
 	# Assume the same state as for other route types, i.e.
 	# ready for the OpenLoop that is sure to follow.
 	try:
-		m = self.matching[key]
+		m = self.matching[route_key]
 	except KeyError:
 		m = [relay, None, None]
-		self.matching[key] = m
-		self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({key})')
+		self.matching[route_key] = m
+		self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({route_key})')
 		return READY
 	looped(self, message, m[1], m[2])
 	return READY
 	
 def PublishingAgent_READY_PeerOpened(self, message):
 	k = ipp_key(message.connecting_ipp)
 	try:
 		r = self.peered[k]
 	except KeyError:
 		self.warning(f'Unknown peer opened"{k}"')
 		return READY
 	r[0] = self.return_address
 
-	for key, relay in r[1].items():
+	for route_key, relay in r[1].items():
 		self.reply(relay)
-		self.relay_address[key] = self.return_address
+		self.relay_address[route_key] = self.return_address
 		# Assume the same state as for other route types, i.e.
 		# ready for the OpenLoop that is sure to follow.
 		try:
-			m = self.matching[key]
+			m = self.matching[route_key]
 		except KeyError:
 			m = [relay, None, None]
-			self.matching[key] = m
-			self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({key})')
+			self.matching[route_key] = m
+			self.trace(f'Added relay peer [{ScopeOfService.to_name(relay.scope)}]({route_key})')
 			continue
 		looped(self, message, m[1], m[2])
 	return READY
 
 def PublishingAgent_READY_RetractRoute(self, message):
-	key = message.key
+	route_key = message.route_key
 
-	m = self.matching.pop(key, None)
+	m = self.matching.pop(route_key, None)
 	if m is None:
-		self.trace(f'Unknown key "{key}"')
+		self.trace(f'Unknown route_key "{route_key}"')
 		return READY
 
 	if m[0] is None:
-		self.trace(f'Known key "{key}" never routed')
+		self.trace(f'Known route_key "{route_key}" never routed')
 		return READY
 
-	self.trace(f'Retracted route [{ScopeOfService.to_name(m[0].scope)}]({key})')
+	self.trace(f'Retracted route [{ScopeOfService.to_name(m[0].scope)}]({route_key})')
 	return READY
 
 ### PS-pub-5 Agent accepts remote loop.
 def PublishingAgent_READY_OpenLoop(self, message):
-	key = message.key
+	route_key = message.route_key
 	try:
-		m = self.matching[key]
+		m = self.matching[route_key]
 	except KeyError:
 		m = [None, message, self.return_address]
-		self.matching[key] = m
+		self.matching[route_key] = m
 		return READY
 	looped(self, m[0], message, self.return_address)
 	return READY
 
 def PublishingAgent_READY_CloseLoop(self, message):
-	key = message.key
-	loop = self.loop.get(key, None)
+	route_key = message.route_key
+	loop = self.loop.get(route_key, None)
 	if loop:
 		self.forward(message, loop, self.return_address)
 	return READY
 
 def PublishingAgent_READY_CapRoutes(self, message):
 	self.trace(f'Scope cap {message.service_scope}, {len(self.matching)} routes to consider')
 
@@ -1482,62 +1482,62 @@
 
 def PublishingAgent_READY_Clear(self, message):
 	if message.session is None:
 		for a in self.loop.values():
 			self.send(Close(message.value), a)
 		return READY
 
-	key = message.session.key
+	route_key = message.session.route_key
 	try:
-		a = self.loop[key]
+		a = self.loop[route_key]
 	except KeyError:
 		return READY
 	self.send(Close(message.value), a)
 
 	return READY
 
 def PublishingAgent_READY_NotPeered(self, message):
 	if message.session is None:
 		for a in self.loop.values():
 			# Was CloseLoop().
 			self.send(ar.Stop(), a)
 		return READY
 
-	key = message.key
+	route_key = message.route_key
 	try:
-		a = self.loop[key]
+		a = self.loop[route_key]
 	except KeyError:
 		return READY
 	# Was CloseLoop().
 	self.send(ar.Stop(), a)
 
 	return READY
 
 def PublishingAgent_READY_Completed(self, message):
-	key = self.debrief()
-	self.loop.pop(key, None)
+	route_key = self.debrief()
+	self.loop.pop(route_key, None)
 	return READY
 
 def PublishingAgent_READY_Ping(self, message):
 	self.reply(ar.Ack())
 	return READY
 
 def PublishingAgent_READY_Stop(self, message):
 	if self.working():
 		self.abort()
 		return CLEARING
-	self.send(UnlistService(self.requested_name, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistService(self.requested_name, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 def PublishingAgent_CLEARING_Completed(self, message):
-	key = self.debrief()
-	self.loop.pop(key, None)
+	route_key = self.debrief()
+	self.loop.pop(route_key, None)
 	if self.working():
 		return CLEARING
-	self.send(UnlistService(self.requested_name, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistService(self.requested_name, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 PUBLISHING_AGENT_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	PENDING: (
@@ -1583,17 +1583,17 @@
 def best_route(table):
 	scope, route = None, None
 	for s, r in table.items():
 		if scope is None or s < scope:
 			scope, route = s, r
 	return scope, route
 
-def find_route(table, key):
+def find_route(table, route_key):
 	for s, r in table.items():
-		if r.key == key:
+		if r.route_key == route_key:
 			return s
 	return None
 
 class SubscriberLoop(ar.Point, ar.StateMachine):
 	def __init__(self, route, subscriber_address, create_session):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
@@ -1609,39 +1609,39 @@
 
 		# Context of a looped route
 		self.latch = None
 		self.remote_session = None
 		self.session_address = None
 		self.origin_address = None
 
-	def open_loop(self, key, remote_agent):
+	def open_loop(self, route_key, remote_agent):
 		self.remote_agent = remote_agent
 		# WARNING - ADDRESS OF LATCH CHANGES
-		self.trace(f'Initiate latch/loop to "{key}"')
-		a = self.create(ar.Latch, key, self.subscriber_address)
+		self.trace(f'Initiate latch/loop to "{route_key}"')
+		a = self.create(ar.Latch, route_key, self.subscriber_address)
 		self.assign(a, 0)
 		self.latch = a
-		self.send(OpenLoop(a, key), remote_agent)
+		self.send(OpenLoop(a, route_key), remote_agent)
 		self.start(ar.T1, SECONDS_OF_LOOPING)
 
 	def open_peer(self):
-		key = self.route.key
+		route_key = self.route.route_key
 		ipp = self.route.connecting_ipp
 		self.peer_ipp = ipp
-		self.trace(f'Requests peer {ipp} for "{key}"')
-		self.send(OpenPeer(ipp, key), pb.house)
+		self.trace(f'Requests peer {ipp} for "{route_key}"')
+		self.send(OpenPeer(ipp, route_key), pb.house)
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_relay(self):
-		key = self.route.key
+		route_key = self.route.route_key
 		ipp = self.route.redirect.redirect_ipp
 		self.peer_ipp = ipp
-		self.trace(f'Requests relay {ipp} for "{key}"')
+		self.trace(f'Requests relay {ipp} for "{route_key}"')
 		encrypted = self.route.redirect.encrypted
-		open = OpenPeer(ipp, key, encrypted=encrypted)
+		open = OpenPeer(ipp, route_key, encrypted=encrypted)
 		self.send(open, pb.house)
 		self.start(ar.T2, SECONDS_OF_PEERING)
 
 	def open_latch(self, message):
 		self.remote_loop = self.return_address
 		self.remote_session = message.publisher_session
 		if self.create_session:
@@ -1663,57 +1663,57 @@
 			# Latch clears additional session alias on stop
 			hand = ar.SwitchOver()
 		# Sending session control message from Latch is flawed - doesnt know
 		# about "origin_address".
 		s = address_to_text(self.subscriber_address)
 		p = address_to_text(self.origin_address)
 		self.trace(f'Loop opened between subscriber [{s}] and publisher [{p}]')
-		self.forward(Available(message.key, self.parent_address), self.subscriber_address, self.origin_address)
+		self.forward(Available(message.route_key, self.parent_address), self.subscriber_address, self.origin_address)
 		self.send(hand, self.latch)
 		# LATCH MUST CONTINUE FOR THOSE MESSAGES THAT WERE
 		# SITTING IN THE QUEUE AFTER THE HANDOVER MESSAGE
 	
 	def latch_loop(self):
 		j = self.address_job.pop(self.latch, None)
 		if j is None:
 			self.warning(f'Where is the latch entry?')
 		self.assign(self.return_address, 0)
 
 	def close_loop(self):
-		key = self.route.key
-		self.trace(f'Close loop for "{key}"')
-		self.send(CloseLoop(key), self.remote_agent)
+		route_key = self.route.route_key
+		self.trace(f'Close loop for "{route_key}"')
+		self.send(CloseLoop(route_key), self.remote_agent)
 
 	def close_peer(self):
-		key = self.route.key
+		route_key = self.route.route_key
 		ipp = self.peer_ipp
-		self.trace(f'Close peer {ipp} for "{key}"')
-		self.send(ClosePeer(ipp, key), pb.house)
+		self.trace(f'Close peer {ipp} for "{route_key}"')
+		self.send(ClosePeer(ipp, route_key), pb.house)
 
 	def close_relay(self):
 		self.send(CloseRelay(self.route.redirect), self.peer_address)
 
 #
 #
 def SubscriberLoop_INITIAL_Start(self, message):
 	route = self.route
 	e = ScopeOfService.to_name(route.scope)
-	self.trace(f'Initiate route [{e}]({route.key})')
+	self.trace(f'Initiate route [{e}]({route.route_key})')
 
 	if isinstance(route, RouteToAddress):
-		self.open_loop(route.key, route.address)
+		self.open_loop(route.route_key, route.address)
 		return LOOPING
 	elif isinstance(route, RouteOverConnected):
 		self.open_peer()
 		return CONNECTION_PEERING
 	elif isinstance(route, RouteByRelay):
 		self.open_relay()
 		return RELAY_PEERING
 
-	unknown = ar.Faulted(f'Cannot initiate route ({route.key})', f'unknown scope [{e}]')
+	unknown = ar.Faulted(f'Cannot initiate route ({route.route_key})', f'unknown scope [{e}]')
 	self.warning(f'{unknown}')
 	self.complete(unknown)
 
 # LOOPING.
 def SubscriberLoop_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return LATCHING
@@ -1786,36 +1786,36 @@
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 # CONNECTION
 def SubscriberLoop_CONNECTION_PEERING_PeerOpened(self, message):
 	self.peer_address = self.return_address
-	self.open_loop(message.key, self.return_address)
+	self.open_loop(message.route_key, self.return_address)
 	return CONNECTION_LOOPING
 
 def SubscriberLoop_CONNECTION_PEERING_NotPeered(self, message):
-	name = key_service(message.key)
+	name = key_service(message.route_key)
 	self.trace(f'Cannot loop to {name} ({message.reason})')
-	self.forward(NotAvailable(message.key, message.reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(message.route_key, message.reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_PEERING_T2(self, message):
-	key = self.route.key
-	name = key_service(key)
+	route_key = self.route.route_key
+	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot loop to {name} ({reason})')
-	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -1831,19 +1831,19 @@
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return CONNECTION_LATCHING
 
 def SubscriberLoop_CONNECTION_LOOPING_T1(self, message):
-	key = self.route.key
-	name = key_service(key)
+	route_key = self.route.route_key
+	name = key_service(route_key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot loop to {name} ({reason})')
-	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
@@ -1926,36 +1926,36 @@
 		return CLEARING
 	self.complete(False)
 
 # RELAY
 def SubscriberLoop_RELAY_PEERING_PeerOpened(self, message):
 	self.peer_address = self.return_address
 	self.reply(self.route)
-	self.open_loop(message.key, self.return_address)
+	self.open_loop(message.route_key, self.return_address)
 	return RELAY_LOOPING
 
 def SubscriberLoop_RELAY_PEERING_NotPeered(self, message):
-	name = key_service(message.key)
+	name = key_service(message.route_key)
 	self.trace(f'Cannot relay to {name} ({message.reason})')
-	self.forward(NotAvailable(message.key, message.reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(message.route_key, message.reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_RELAY_PEERING_T2(self, message):
-	key = self.route.key
-	name = key_service(key)
+	route_key = self.route.route_key
+	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot relay to {name} ({reason})')
-	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -1971,19 +1971,19 @@
 	self.complete(True)
 
 def SubscriberLoop_RELAY_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return RELAY_LATCHING
 
 def SubscriberLoop_RELAY_LOOPING_T1(self, message):
-	key = self.route.key
-	name = key_service(key)
+	route_key = self.route.route_key
+	name = key_service(route_key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot relay to {name} ({reason})')
-	self.forward(NotAvailable(key, reason, self.parent_address), self.subscriber_address, self.address)
+	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2128,25 +2128,25 @@
 ar.bind(SubscriberLoop, SUBSCRIBER_LOOP_DISPATCH, thread='subscribed')
 
 # An object that represents a unique instance of a subscriber object
 # and a requested search, i.e. each subscriber can have multiple
 # active searches (as long as they are different) and each search can
 # match multiple publishers.
 class SubscriptionAgent(ar.Point, ar.StateMachine):
-	def __init__(self, requested_search, subscriber_address, create_session, declared_scope):
+	def __init__(self, requested_search, subscriber_address, create_session, requested_scope):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.requested_search = requested_search
 		self.subscriber_address = subscriber_address
 		self.create_session = create_session
-		self.declared_scope = declared_scope
+		self.requested_scope = requested_scope
 		self.service_looping = {}
 
 	def open_route(self, route, tag):
-		name = key_service(route.key)
+		name = key_service(route.route_key)
 		scope = route.scope
 		sos = ScopeOfService.to_name(scope)
 
 		looping = self.service_looping.get(name, None)
 		if looping is None:
 			self.trace(f'Start loop "{name}" [{sos}] {tag}')
 			table = {scope: route}
@@ -2163,16 +2163,16 @@
 			if loop:
 				self.trace(f'Replacement [{sos}] route (loop running)')
 				return
 			if completed:
 				self.trace(f'Replacement [{sos}] route (previous positive completion)')
 				return
 
-			route_id = key_id(route.key)
-			opened_id = key_id(opened.key)
+			route_id = key_id(route.route_key)
+			opened_id = key_id(opened.route_key)
 			if route_id == opened_id:
 				self.trace(f'Replacement [{sos}] route (no change)')
 				return
 
 			if id_process(route_id) != id_process(opened_id):
 				s = 'process'
 			elif id_connection(route_id) != id_connection(opened_id):
@@ -2205,15 +2205,15 @@
 			return
 
 		self.trace(f'Fallback [{sos}] route')
 
 
 # Register interest in services matching pattern.
 def SubscriptionAgent_INITIAL_Start(self, message):
-	self.send(FindService(self.requested_search, self.address, self.declared_scope), pb.directory)
+	self.send(FindService(self.requested_search, self.address, self.requested_scope), pb.directory)
 	return READY
 
 # Routes arrive from directories. This is the first moment of discovering
 # new matching service names. Instantiate per-match object as needed,
 # that will initiate and manage actual session with remote.
 def SubscriptionAgent_READY_RouteToAddress(self, message):
 	self.open_route(message, f'{message.address}')
@@ -2226,31 +2226,31 @@
 
 def SubscriptionAgent_READY_RouteByRelay(self, message):
 	tag = f'{message.redirect.redirect_ipp}'
 	self.open_route(message, tag)
 	return READY
 
 def SubscriptionAgent_READY_RetractRoute(self, message):
-	key = message.key
-	name = key_service(key)
+	route_key = message.route_key
+	name = key_service(route_key)
 
 	looping = self.service_looping.get(name, None)
 	if looping is None:
 		self.trace(f'Retract for unknown service "{name}"')
 		return READY
 	table = looping[0]
 
-	scope = find_route(table, key)
+	scope = find_route(table, route_key)
 	if scope is None:
-		self.trace(f'Retract for unknown route "{key}"')
+		self.trace(f'Retract for unknown route "{route_key}"')
 		return READY
 
 	r = table.pop(scope, None)
 	if r is None:
-		self.warning(f'Find/pop failed for route "{key}"')
+		self.warning(f'Find/pop failed for route "{route_key}"')
 		return READY
 
 	return READY
 
 def SubscriptionAgent_READY_CapRoutes(self, message):
 	for name, looping in self.service_looping.items():
 		table = looping[0]
@@ -2259,16 +2259,16 @@
 	return READY
 
 def SubscriptionAgent_READY_Clear(self, message):
 	if message.session is None:
 		self.warning('No session included')
 		return READY
 
-	key = message.session.key
-	name = key_service(key)
+	route_key = message.session.route_key
+	name = key_service(route_key)
 
 	looping = self.service_looping.get(name, None)
 	if looping is None:
 		self.warning(f'Clear of unknown service {name}')
 		return READY
 
 	self.send(Close(message.value), looping[2])
@@ -2298,41 +2298,41 @@
 	scope, best = best_route(table)		# Nothing to route to.
 	if scope is None:
 		return READY
 
 	sos = ScopeOfService.to_name(route.scope)
 	if best.scope == route.scope:
 		self.trace(f'Replacement [{sos}] route')
-		if key_id(best.key) == key_id(route.key):
+		if key_id(best.route_key) == key_id(route.route_key):
 			self.trace(f'Replacement route for "{name}" has not changed')
 			return READY
 
 	self.trace(f'Start continuation loop "{name}" [{sos}]')
 	a = self.create(SubscriberLoop, message, self.subscriber_address, self.create_session)
 	self.assign(a, name)
 	looping[1] = message
 	looping[2] = a
 	return READY
 
 def SubscriptionAgent_READY_Stop(self, message):
 	if self.working():
 		self.abort()
 		return COMPLETING
-	self.send(UnlistFind(self.requested_search, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistFind(self.requested_search, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 def SubscriptionAgent_COMPLETING_Completed(self, message):
 	name = self.debrief()
 	looping = self.service_looping.get(name, None)
 	if looping is None:
 		self.warning(f'Untidy completion of {name}')
 
 	if self.working():
 		return COMPLETING
-	self.send(UnlistFind(self.requested_search, self.address, self.declared_scope), pb.directory)
+	self.send(UnlistFind(self.requested_search, self.address, self.requested_scope), pb.directory)
 	self.complete(ar.Aborted())
 
 SUBSCRIPTION_AGENT_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	READY: (
@@ -2348,19 +2348,19 @@
 
 # WARNING agent and loop MUST be on same thread.
 ar.bind(SubscriptionAgent, SUBSCRIPTION_AGENT_DISPATCH, thread='subscribed')
 
 #
 #
 class ConnectToPeer(ar.Point, ar.StateMachine):
-	def __init__(self, connecting_ipp, key, client_address, encrypted):
+	def __init__(self, connecting_ipp, route_key, client_address, encrypted):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.connecting_ipp = connecting_ipp
-		self.key = key
+		self.route_key = route_key
 		self.connected = None
 		self.not_connected = None
 		self.client_address = set()
 		self.client_address.add(client_address)
 		self.encrypted = encrypted
 
 def ConnectToPeer_INITIAL_Start(self, message):
@@ -2369,55 +2369,55 @@
 
 # CONNECTING
 #
 def ConnectToPeer_CONNECTING_Connected(self, message):
 	self.connected = message
 
 	return_address = self.return_address
-	opened = PeerOpened(connecting_ipp=self.connecting_ipp, key=self.key)
+	opened = PeerOpened(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(opened, c, return_address)
 
 	return CONNECTED
 
 def ConnectToPeer_CONNECTING_NotConnected(self, message):
 	self.not_connected = str(message)
-	not_peered = NotPeered(connecting_ipp=self.connecting_ipp, key=self.key, reason=self.not_connected)
+	not_peered = NotPeered(connecting_ipp=self.connecting_ipp, route_key=self.route_key, reason=self.not_connected)
 	for c in self.client_address:
 		self.send(not_peered, c)
 
 	self.start(ar.T1, 4.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTING_Stop(self, message):
 	self.complete(ar.Aborted())
 
 # CONNECTED
 #
 def ConnectToPeer_CONNECTED_Abandoned(self, message):
 	self.not_connected = 'Abandoned by remote'
 	return_address = self.return_address
-	lost = PeerLost(connecting_ipp=self.connecting_ipp, key=self.key)
+	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(lost, c, return_address)
 	self.start(ar.T1, 4.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTED_Closed(self, message):
 	self.not_connected = 'Local termination'
 	return_address = self.return_address
-	lost = PeerLost(connecting_ipp=self.connecting_ipp, key=self.key)
+	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(lost, c, return_address)
 	self.start(ar.T1, 4.0)
 	return GLARING
 
 def ConnectToPeer_CONNECTED_OpenPeer(self, message):
 	self.client_address.add(self.return_address)
-	opened = PeerOpened(connecting_ipp=self.connecting_ipp, key=self.key)
+	opened = PeerOpened(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	self.forward(opened, self.return_address, self.connected.remote_address)
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_ClosePeer(self, message):
 	self.client_address.discard(self.return_address)
 	if len(self.client_address) < 1:
 		self.not_connected = 'Cleared last peer'
@@ -2425,27 +2425,27 @@
 		self.start(ar.T1, 4.0)
 		return GLARING
 	return CONNECTED
 
 def ConnectToPeer_CONNECTED_Stop(self, message):
 	self.not_connected = 'Process termination'
 	return_address = self.connected.remote_address
-	lost = PeerLost(connecting_ipp=self.connecting_ipp, key=self.key)
+	lost = PeerLost(connecting_ipp=self.connecting_ipp, route_key=self.route_key)
 	for c in self.client_address:
 		self.forward(lost, c, return_address)
 	self.send(Close(ar.Aborted()), return_address)
 	return CLOSING
 
 # GLARING
 def ConnectToPeer_GLARING_T1(self, message):
 	self.complete(ar.Aborted())
 
 def ConnectToPeer_GLARING_OpenPeer(self, message):
 	reason = self.not_connected
-	np = NotPeered(connecting_ipp=self.connecting_ipp, key=self.key, reason=reason)
+	np = NotPeered(connecting_ipp=self.connecting_ipp, route_key=self.route_key, reason=reason)
 	self.reply(np)
 	return GLARING
 
 def ConnectToPeer_GLARING_ClosePeer(self, message):
 	return GLARING
 
 def ConnectToPeer_GLARING_Closed(self, message):
@@ -2501,34 +2501,34 @@
 	try:
 		a = self.published[message.requested_name]
 		self.reply(NotPublished(message.requested_name, 'already published'))
 		return NORMAL
 	except KeyError:
 		pass
 	### PS-pub-2 Create the agent
-	a = self.create(PublishingAgent, message.requested_name, self.return_address, message.create_session, message.declared_scope)
+	a = self.create(PublishingAgent, message.requested_name, self.return_address, message.create_session, message.requested_scope)
 	p = [message, self.return_address]
 	self.assign(a, p)
 	self.published[message.requested_name] = a
 	return NORMAL
 
 ### PS-sub-1 Process the app request
 def PubSub_NORMAL_SubscribeToName(self, message):
 	k = address_to_text(self.return_address)
 	k += ':'
 	k += message.requested_search
 	try:
 		a = self.subscribed[k]
 	except KeyError:
 		### PS-sub-2 Create the agent
-		a = self.create(SubscriptionAgent, message.requested_search, self.return_address, message.create_session, message.declared_scope)
+		a = self.create(SubscriptionAgent, message.requested_search, self.return_address, message.create_session, message.requested_scope)
 		s = [message, self.return_address]
 		self.assign(a, s)
 		self.subscribed[k] = a
-	self.forward(Subscribed(message.requested_search, message.declared_scope), self.return_address, a)
+	self.forward(Subscribed(message.requested_search, message.requested_scope), self.return_address, a)
 	return NORMAL
 
 def PubSub_NORMAL_Retract(self, message):
 	self.trace(f'Retracting service/search at [{address_to_text(message.address)}]')
 	for t, a in self.running():
 		if t[1] == message.address:
 			self.send(ar.Stop(), a)
@@ -2536,37 +2536,37 @@
 
 def PubSub_NORMAL_Completed(self, message):
 	ma = self.debrief()
 	m, a = ma
 	if isinstance(m, PublishAsName):
 		p = self.published.pop(m.requested_name, None)
 		if p is None:
-			self.warning(f'Completion of unknown publication key {m.requested_name}')
+			self.warning(f'Completion of unknown publication route_key {m.requested_name}')
 	elif isinstance(m, SubscribeToName):
 		search = m.requested_search
 		k = address_to_text(a)
 		k += ':'
 		k += search
 		s = self.subscribed.pop(k, None)
 		if s is None:
-			self.warning(f'Completion of unknown subscription key {k}')
+			self.warning(f'Completion of unknown subscription route_key {k}')
 	elif isinstance(m, HostPort):
 		inet = m.inet()
 		connecting = self.connecting.pop(inet, None)
 		if connecting is None:
 			self.trace(f'Completion of unknown peer {inet}')
 	else:
 		self.warning(f'Completion of unknown type {type(m)}')
 	return NORMAL
 
 def PubSub_NORMAL_OpenPeer(self, message):
 	inet = message.connecting_ipp.inet()
 	connecting = self.connecting.get(inet, None)
 	if connecting is None:
-		connecting = self.create(ConnectToPeer, message.connecting_ipp, message.key, self.return_address, message.encrypted)
+		connecting = self.create(ConnectToPeer, message.connecting_ipp, message.route_key, self.return_address, message.encrypted)
 		p = [message.connecting_ipp, self.return_address]
 		self.assign(connecting, p)
 		self.connecting[inet] = connecting
 	else:
 		self.forward(message, connecting, self.return_address)
 	return NORMAL
 
@@ -2625,19 +2625,19 @@
 
 ar.bind(PubSub, PUBSUB_DISPATCH)
 
 # The public interface to the directory service.
 #
 
 ### PS-pub-0 Start of publish
-def publish(self, requested_name, create_session=None, declared_scope=ScopeOfService.WAN):
-	self.send(PublishAsName(requested_name, create_session, declared_scope), pb.house)
+def publish(self, requested_name, create_session=None, requested_scope=ScopeOfService.WAN):
+	self.send(PublishAsName(requested_name, create_session, requested_scope), pb.house)
 
 ### PS-sub-0 Start of subscribe
-def subscribe(self, requested_search, create_session=None, declared_scope=ScopeOfService.WAN):
-	self.send(SubscribeToName(requested_search, create_session, declared_scope), pb.house)
+def subscribe(self, requested_search, create_session=None, requested_scope=ScopeOfService.WAN):
+	self.send(SubscribeToName(requested_search, create_session, requested_scope), pb.house)
 
 def clear(self, session, value=None):
 	self.send(Clear(session, value), session.agent_address)
 
 def retract(self):
 	self.send(Retract(self.address), pb.house)
```

### Comparing `ansar_connect-0.1.200/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.201/src/ansar/connect/directory_if.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,64 +47,64 @@
 # Build the local published/subscribed objects.
 #
 ScopeOfService = ar.Enumeration(PROCESS=1, GROUP=2, HOST=3, LAN=4, WAN=5)
 
 #
 #
 class Published(object):
-	def __init__(self, published_name=None, declared_scope=ScopeOfService.WAN, listening_ipp=None):
-		self.published_name = published_name
-		self.declared_scope = declared_scope
+	def __init__(self, requested_name=None, requested_scope=ScopeOfService.WAN, listening_ipp=None):
+		self.requested_name = requested_name
+		self.requested_scope = requested_scope
 		self.listening_ipp = listening_ipp or HostPort()
 
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
-	def __init__(self, subscribed_search=None, declared_scope=ScopeOfService.WAN):
-		self.subscribed_search = subscribed_search
-		self.declared_scope = declared_scope
+	def __init__(self, requested_search=None, requested_scope=ScopeOfService.WAN):
+		self.requested_search = requested_search
+		self.requested_scope = requested_scope
 
 # The actual service directory with listings and searches.
 #
 
 # Session messages to publish/listen controllers.
 # Subscribe/client/calling/outbound end.
 class Available(object):
-	def __init__(self, key=None, agent_address=None):
-		self.key = key
+	def __init__(self, route_key=None, agent_address=None):
+		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
-	def __init__(self, key=None, reason=None, agent_address=None):
-		self.key = key
+	def __init__(self, route_key=None, reason=None, agent_address=None):
+		self.route_key = route_key
 		self.reason = reason
 		self.agent_address = agent_address
 		ar.Faulted.__init__(self, 'no peer available', reason)
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
 # Publish/service/answering/inbound end.
 class Delivered(object):
-	def __init__(self, key=None, agent_address=None):
-		self.key = key
+	def __init__(self, route_key=None, agent_address=None):
+		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
-	def __init__(self, published_name=None, remote_address=None):
-		self.published_name = published_name
+	def __init__(self, requested_name=None, remote_address=None):
+		self.requested_name = requested_name
 		self.remote_address = remote_address
 		ar.Faulted.__init__(self, 'no service to peer')
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
@@ -138,25 +138,25 @@
 }
 
 ar.bind(Clear, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Cleared, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Dropped, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 SHARED_SCHEMA = {
-	#'key': ar.VectorOf(ar.Integer8()),
-	'key': str,
+	#'route_key': ar.VectorOf(ar.Integer8()),
+	'route_key': str,
 	'name': str,
 	'requested_name': str,
 	'requested_search': str,
-	'published_name': str,
-	'subscribed_search': str,
-	'published_name': str,
+	'requested_name': str,
+	'requested_search': str,
+	'requested_name': str,
 	'remote_address': ar.Address(),
 	'session_address': ar.Address(),
-	'declared_scope': ScopeOfService,
+	'requested_scope': ScopeOfService,
 	'service_scope': ScopeOfService,
 	'reason': ar.String(),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'connecting_ipp': ar.UserDefined(HostPort),
 	'parent_ipp': ar.UserDefined(HostPort),
 	'child_ipp': ar.UserDefined(HostPort),
 	'subscription': ar.UserDefined(Subscribed),
@@ -169,17 +169,17 @@
 ar.bind(Subscribed, object_schema=SHARED_SCHEMA)
 ar.bind(Published, object_schema=SHARED_SCHEMA)
 ar.bind(Available, object_schema=SHARED_SCHEMA)
 ar.bind(NotAvailable, object_schema=SHARED_SCHEMA)
 ar.bind(Delivered, object_schema=SHARED_SCHEMA)
 ar.bind(NotDelivered, object_schema=SHARED_SCHEMA)
 
-# matched[key] = a (address of ServiceRoute)
+# matched[route_key] = a (address of ServiceRoute)
 # and
-# key added to each find and listing set
+# route_key added to each find and listing set
 # self.directory[service_name] = [message, set()]
 # self.find[k] = [message, set(), dfa]
 # where k =
 # f'{subscriber_address}/{requested_search}'
 class DirectoryRoute(object):
 	def __init__(self, search_or_listing=None, agent_address=None, route_key=None):
 		self.search_or_listing = search_or_listing
```

### Comparing `ansar_connect-0.1.200/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.201/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/group_if.py` & `ansar_connect-0.1.201/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/grouping.py` & `ansar_connect-0.1.201/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/moving.py` & `ansar_connect-0.1.201/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/networking.py` & `ansar_connect-0.1.201/src/ansar/connect/networking.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
 # INITIAL
 # Launch this object.
 def SubscribeToListing_INITIAL_Start(self, message):
 	self.group_address = self.group_address or self.parent_address
 
 	# Start from nothing.
 	self.started = ar.world_now()
-	subscribe(self, self.listing, create_session=self.session, declared_scope=self.scope)
+	subscribe(self, self.listing, create_session=self.session, requested_scope=self.scope)
 	self.attempts = 1
 	return PENDING
 
 # PENDING
 # Waiting for results of subscibe.
 # Subscription acknowledged.
 def SubscribeToListing_PENDING_Subscribed(self, message):
@@ -568,15 +568,15 @@
 # INITIAL
 # Launch this object.
 def PublishAListing_INITIAL_Start(self, message):
 	self.group_address = self.group_address or self.parent_address
 
 	# Start from nothing.
 	self.started = ar.world_now()
-	publish(self, self.listing, create_session=self.session, declared_scope=self.scope)
+	publish(self, self.listing, create_session=self.session, requested_scope=self.scope)
 	self.attempts = 1
 	return PENDING
 
 # PENDING
 # Waiting for results of publish.
 # Listing established.
 def PublishAListing_PENDING_Published(self, message):
@@ -703,15 +703,15 @@
 # INITIAL
 # Launch this object.
 def SubscribeToSearch_INITIAL_Start(self, message):
 	self.group_address = self.group_address or self.parent_address
 
 	# Start from nothing.
 	self.started = ar.world_now()
-	subscribe(self, self.search, create_session=self.session, declared_scope=self.scope)
+	subscribe(self, self.search, create_session=self.session, requested_scope=self.scope)
 	self.attempts = 1
 	return PENDING
 
 # PENDING
 # Waiting for results of publish.
 # Listing established.
 def SubscribeToSearch_PENDING_Subscribed(self, message):
```

### Comparing `ansar_connect-0.1.200/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.201/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/node.py` & `ansar_connect-0.1.201/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.201/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/procedure.py` & `ansar_connect-0.1.201/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/product.py` & `ansar_connect-0.1.201/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/socketry.py` & `ansar_connect-0.1.201/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/standard.py` & `ansar_connect-0.1.201/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/transporting.py` & `ansar_connect-0.1.201/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.201/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar/connect/wan.py` & `ansar_connect-0.1.201/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.200/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.201/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.200
+Version: 0.1.201
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.200/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.201/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

