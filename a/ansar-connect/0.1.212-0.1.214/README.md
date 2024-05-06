# Comparing `tmp/ansar_connect-0.1.212.tar.gz` & `tmp/ansar_connect-0.1.214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.212.tar", last modified: Mon May  6 13:49:21 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.214.tar", last modified: Mon May  6 19:54:40 2024, max compression
```

## Comparing `ansar_connect-0.1.212.tar` & `ansar_connect-0.1.214.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.212/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.212/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.212/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.212/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.212/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.212/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 13:49:18.000000 ansar_connect-0.1.212/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    81926 2024-05-06 13:38:36.000000 ansar_connect-0.1.212/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8338 2024-05-06 13:45:27.000000 ansar_connect-0.1.212/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.212/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.212/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.212/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.212/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.212/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.212/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.212/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.212/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.212/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.212/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.212/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.212/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.212/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.212/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.212/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 13:49:21.898658 ansar_connect-0.1.212/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 13:49:21.000000 ansar_connect-0.1.212/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.214/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.214/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.214/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.214/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.783226 ansar_connect-0.1.214/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.214/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.214/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-06 19:54:37.000000 ansar_connect-0.1.214/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87301 2024-05-06 19:38:10.000000 ansar_connect-0.1.214/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8884 2024-05-06 19:54:12.000000 ansar_connect-0.1.214/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.214/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.214/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.214/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.214/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.214/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.214/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.214/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.214/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.214/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.214/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41125 2024-04-19 08:12:26.000000 ansar_connect-0.1.214/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.214/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.214/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.214/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.214/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-06 19:54:40.787226 ansar_connect-0.1.214/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-06 19:54:40.000000 ansar_connect-0.1.214/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.212/LICENSE` & `ansar_connect-0.1.214/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/PKG-INFO` & `ansar_connect-0.1.214/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.212
+Version: 0.1.214
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.212/README.md` & `ansar_connect-0.1.214/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/pyproject.toml` & `ansar_connect-0.1.214/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/setup.py` & `ansar_connect-0.1.214/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.214/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.214/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.214/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.214/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/__init__.py` & `ansar_connect-0.1.214/src/ansar/connect/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: upgrade-pub-sub-messages
-Commit: 64ea7a0bfcf8702d22e0d3d2a39ede6593dd58c0
-Version: 0.1.211 (2024-05-07@01:49:18+NZST)
+Commit: d5844a4bdaa789206ad19a9b3198c0ecc33c1a51
+Version: 0.1.213 (2024-05-07@07:54:37+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.212/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.214/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/directory.py` & `ansar_connect-0.1.214/src/ansar/connect/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1204,15 +1204,18 @@
 	self.forward(delivered, self.publisher_address, self.origin_address)
 	return LOOPED
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
 	if self.created_session and self.return_address == self.created_session:
-		self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=message.value)
+		self.forward(cleared, self.publisher_address, self.origin_address)
 		self.send(CloseLoop(self.route_key), self.remote_loop)
 		self.close_route()
 		self.complete(ar.Aborted())
 	self.warning('Unexpected termination')
 	return LOOPED
 
 ### PS-pub-8 Loop terminates by local clear().
@@ -1220,49 +1223,64 @@
 	self.closing, self.value = True, message.value
 	self.send(CloseLoop(self.route_key), self.remote_loop)
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
-	self.forward(Cleared(message.value), self.publisher_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=message.value)
+	self.forward(cleared, self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by remote close.
 def PublisherLoop_LOOPED_CloseLoop(self, message):
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
-	self.forward(Dropped('abandoned by remote'), self.publisher_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by remote')
+	self.forward(dropped, self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by local exit.
 def PublisherLoop_LOOPED_Stop(self, message):
 	self.send(CloseLoop(self.route_key), self.remote_loop)
 	if self.created_session:
 		self.send(message, self.created_session)
 		return CLEARING
 	self.close_route()
 
-	self.forward(Dropped('aborted'), self.publisher_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='aborted')
+	self.forward(dropped, self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 def PublisherLoop_CLEARING_Completed(self, message):
 	if self.created_session is None or self.return_address != self.created_session:
 		return CLEARING
 
 	self.create_session = None
 	self.close_route()
 
 	if self.closing:
-		self.forward(Cleared(self.value), self.publisher_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=self.value)
+		self.forward(cleared, self.publisher_address, self.origin_address)
 	else:
-		self.forward(Dropped('aborted'), self.publisher_address, self.origin_address)
+		dropped = Dropped(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, reason='aborted')
+		self.forward(dropped, self.publisher_address, self.origin_address)
 
 	self.complete(ar.Aborted())
 
 PUBLISHER_LOOP_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
@@ -1774,51 +1792,69 @@
 # CloseLoop -> remote termination
 # PeerLost -> network abandoned
 # Stop -> application
 def SubscriberLoop_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
-		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=message.value)
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
-		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=f)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=f)
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Local termination.
 def SubscriberLoop_LOOPED_Close(self, message):
-	self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=message.value)
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by remote')
+	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_LOOPED_Stop(self, message):
-	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=ar.Aborted())
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -1829,30 +1865,38 @@
 	self.peer_address = self.return_address
 	self.open_loop(message.route_key, self.return_address)
 	return CONNECTION_LOOPING
 
 def SubscriberLoop_CONNECTION_PEERING_NotPeered(self, message):
 	name = key_service(message.route_key)
 	self.trace(f'Cannot loop to {name} ({message.reason})')
-	self.forward(NotAvailable(message.route_key, message.reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot loop to {name} ({reason})')
-	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -1872,15 +1916,19 @@
 	return CONNECTION_LATCHING
 
 def SubscriberLoop_CONNECTION_LOOPING_T1(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot loop to {name} ({reason})')
-	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
@@ -1901,62 +1949,80 @@
 	self.latch_loop()
 	return CONNECTION_LOOPED
 
 def SubscriberLoop_CONNECTION_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
-		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=ar.Aborted())
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
-		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=f)
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 def SubscriberLoop_CONNECTION_LOOPED_Close(self, message):
-	self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=message.value)
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 def SubscriberLoop_CONNECTION_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by remote')
+	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPED_PeerLost(self, message):
-	self.forward(Dropped('abandoned by peer'), self.subscriber_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by remote')
+	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPED_Stop(self, message):
-	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=ar.Aborted())
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
@@ -1969,30 +2035,38 @@
 	self.reply(self.route)
 	self.open_loop(message.route_key, self.return_address)
 	return RELAY_LOOPING
 
 def SubscriberLoop_RELAY_PEERING_NotPeered(self, message):
 	name = key_service(message.route_key)
 	self.trace(f'Cannot relay to {name} ({message.reason})')
-	self.forward(NotAvailable(message.route_key, message.reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_RELAY_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot relay to {name} ({reason})')
-	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
@@ -2010,17 +2084,21 @@
 def SubscriberLoop_RELAY_LOOPING_LoopOpened(self, message):
 	self.open_latch(message)
 	return RELAY_LATCHING
 
 def SubscriberLoop_RELAY_LOOPING_T1(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
-	reason = 'timed out on loop'
+	reason = 'loop time exceeded'
 	self.trace(f'Cannot relay to {name} ({reason})')
-	self.forward(NotAvailable(route_key, reason, self.parent_address), self.subscriber_address, self.address)
+	na = NotAvailable(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason=message.reason,
+		agent_address=self.parent_address)
+	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2043,69 +2121,87 @@
 	self.latch_loop()
 	return RELAY_LOOPED
 
 def SubscriberLoop_RELAY_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
-		self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=message.value)
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
-		self.forward(Cleared(f), self.subscriber_address, self.origin_address)
+		cleared = Cleared(matched_search=self.route.matched_search,
+			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+			route_key=message.route_key, value=f)
+		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Local termination.
 def SubscriberLoop_RELAY_LOOPED_Close(self, message):
-	self.forward(Cleared(message.value), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=message.value)
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_RELAY_LOOPED_CloseLoop(self, message):
-	self.forward(Dropped('abandoned by remote'), self.subscriber_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by remote')
+	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 # Termination by loss of peer.
 def SubscriberLoop_RELAY_LOOPED_PeerLost(self, message):
-	self.forward(Dropped('abandoned by peer'), self.subscriber_address, self.origin_address)
+	dropped = Dropped(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, reason='abandoned by peer')
+	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_RELAY_LOOPED_Stop(self, message):
-	self.forward(Cleared(ar.Aborted()), self.subscriber_address, self.origin_address)
+	cleared = Cleared(matched_search=self.route.matched_search,
+		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
+		route_key=message.route_key, value=ar.Aborted())
+	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
```

### Comparing `ansar_connect-0.1.212/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.214/src/ansar/connect/directory_if.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,19 +83,22 @@
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
-	def __init__(self, route_key=None, reason=None, agent_address=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
 		self.agent_address = agent_address
-		ar.Faulted.__init__(self, 'no peer available', reason)
+		ar.Faulted.__init__(self, 'no subscibe peer', reason)
 		#self.condition = cannot
 		#self.explanation = reason
 		self.error_code = None
 		self.error_text = None
 
 # Publish/service/answering/inbound end.
 class Delivered(object):
@@ -103,42 +106,54 @@
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
-	def __init__(self, requested_name=None, remote_address=None):
-		self.requested_name = requested_name
-		self.remote_address = remote_address
-		ar.Faulted.__init__(self, 'no service to peer')
-		#self.condition = cannot
-		#self.explanation = reason
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
+		self.route_key = route_key
+		self.reason = reason
+		self.agent_address = agent_address
+		ar.Faulted.__init__(self, 'no publish peer', reason)
 		self.error_code = None
 		self.error_text = None
 
 class Clear(object):
 	def __init__(self, session=None, value=None):
 		self.session = session
 		self.value = value
 
 class Cleared(object):
-	def __init__(self, value=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, value=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
+		self.route_key = route_key
 		self.value = value
 
 class Dropped(ar.Faulted):
-	def __init__(self, reason=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None):
+		self.matched_search = matched_search
+		self.matched_name = matched_name
+		self.matched_scope = matched_scope
+		self.route_key = route_key
 		self.reason = reason
-		ar.Faulted.__init__(self, 'established peer lost', reason)
-		#self.condition = cannot
-		#self.explanation = reason
+		ar.Faulted.__init__(self, 'peer lost', reason)
 		self.error_code = None
 		self.error_text = None
 
 ENDING_SCHEMA = {
+	'matched_search': str,
+	'matched_name': str,
+	'matched_scope': ScopeOfService,
+	'route_key': str,
 	'session': ar.Any,
 	'value': ar.Any,
 	'reason': str,
 	'condition': str,
 	'explanation': str,
 	'error_text': str,
 	'error_code': ar.Integer8(),
@@ -147,31 +162,24 @@
 
 ar.bind(Clear, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Cleared, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Dropped, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 SHARED_SCHEMA = {
 	#'route_key': ar.VectorOf(ar.Integer8()),
-	'route_key': str,
 	'name': str,
 	'requested_name': str,
 	'requested_search': str,
 	'requested_name': str,
-	'matched_search': str,
-	'matched_name': str,
-	'matched_scope': ScopeOfService,
 	'remote_address': ar.Address(),
 	'session_address': ar.Address(),
 	'requested_scope': ScopeOfService,
 	'service_scope': ScopeOfService,
 	'reason': ar.String(),
 	'listening_ipp': ar.UserDefined(HostPort),
-	'connecting_ipp': ar.UserDefined(HostPort),
-	'parent_ipp': ar.UserDefined(HostPort),
-	'child_ipp': ar.UserDefined(HostPort),
 	'agent_address': ar.Address(),
 	'address': ar.Address(),
 	'published_at': ar.WorldTime(),
 	'subscribed_at': ar.WorldTime(),
 }
 
 SHARED_SCHEMA.update(ENDING_SCHEMA)
```

### Comparing `ansar_connect-0.1.212/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.214/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/group_if.py` & `ansar_connect-0.1.214/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/grouping.py` & `ansar_connect-0.1.214/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/moving.py` & `ansar_connect-0.1.214/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/networking.py` & `ansar_connect-0.1.214/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.214/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/node.py` & `ansar_connect-0.1.214/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.214/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/procedure.py` & `ansar_connect-0.1.214/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/product.py` & `ansar_connect-0.1.214/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/socketry.py` & `ansar_connect-0.1.214/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/standard.py` & `ansar_connect-0.1.214/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/transporting.py` & `ansar_connect-0.1.214/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.214/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar/connect/wan.py` & `ansar_connect-0.1.214/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.212/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.214/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.212
+Version: 0.1.214
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.212/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.214/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

