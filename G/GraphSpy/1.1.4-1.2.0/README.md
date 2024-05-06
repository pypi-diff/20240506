# Comparing `tmp/GraphSpy-1.1.4.tar.gz` & `tmp/GraphSpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSpy-1.1.4.tar", last modified: Wed Apr 10 06:45:16 2024, max compression
+gzip compressed data, was "GraphSpy-1.2.0.tar", last modified: Mon May  6 19:51:14 2024, max compression
```

## Comparing `GraphSpy-1.1.4.tar` & `GraphSpy-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    41189 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/GraphSpy.py
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/__init__.py
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.163317 GraphSpy-1.1.4/GraphSpy/static/
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/static/css/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      340 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/css/style.css
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/static/js/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    11892 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/js/functions.js
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/static/js/theme.js
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy/templates/
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/OneDrive.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePoint.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePointDrives.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/SharePointSites.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6336 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/access_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9996 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/access_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/custom_requests.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6512 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/device_codes.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/generic_search.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/index.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17710 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/layout.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/outlook.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/recent_files.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/refresh_token_modal.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/refresh_tokens.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/settings.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/templates/shared_with_me.html
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/GraphSpy/version.txt
-drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/GraphSpy.egg-info/
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7098 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/PKG-INFO
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1037 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/SOURCES.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/dependency_links.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/entry_points.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/requires.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-04-10 06:45:16.000000 GraphSpy-1.1.4/GraphSpy.egg-info/top_level.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/LICENSE.txt
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/MANIFEST.in
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7098 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/PKG-INFO
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6990 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/README.md
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/requirements.txt
--rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-04-10 06:45:16.167318 GraphSpy-1.1.4/setup.cfg
--rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-04-10 06:45:12.000000 GraphSpy-1.1.4/setup.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    52022 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/GraphSpy.py
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/__init__.py
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/css/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      821 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/css/style.css
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/static/js/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    14019 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/functions.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    21835 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/purify.min.js
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     2430 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/static/js/theme.js
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy/templates/
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7747 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/OneDrive.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     8554 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePoint.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5757 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePointDrives.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6379 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/SharePointSites.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6336 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/access_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     9996 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/access_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    17378 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/custom_requests.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6512 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/device_codes.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7933 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/generic_search.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      847 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/index.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    18474 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/layout.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1923 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/outlook.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5094 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/recent_files.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5679 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/refresh_token_modal.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     6820 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/refresh_tokens.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7886 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/settings.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     5108 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/shared_with_me.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)    22318 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/templates/teams.html
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)        5 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/GraphSpy/version.txt
+drwxr-xr-x   0 redbyte   (1001) redbyte   (1001)        0 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/GraphSpy.egg-info/
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/PKG-INFO
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     1100 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/SOURCES.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        1 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/dependency_links.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       52 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/entry_points.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       28 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/requires.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)        9 2024-05-06 19:51:14.000000 GraphSpy-1.2.0/GraphSpy.egg-info/top_level.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     1527 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/LICENSE.txt
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       54 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/MANIFEST.in
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)     7401 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/PKG-INFO
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)     7303 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/README.md
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)       28 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/requirements.txt
+-rw-r--r--   0 redbyte   (1001) redbyte   (1001)       38 2024-05-06 19:51:14.261536 GraphSpy-1.2.0/setup.cfg
+-rwxr-x---   0 redbyte   (1001) redbyte   (1001)      916 2024-05-06 19:51:09.000000 GraphSpy-1.2.0/setup.py
```

### Comparing `GraphSpy-1.1.4/GraphSpy/static/js/functions.js` & `GraphSpy-1.2.0/GraphSpy/static/js/functions.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -199,14 +199,86 @@
         data: {
             "database": database_name
         }
     });
     bootstrapToast("Duplicate database", response.responseText)
 }
 
+// ========== Teams ==========
+
+function getTeamsConversations(access_token_id) {
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/get_teams_conversations",
+        data: {
+            "access_token_id": access_token_id
+        }
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Teams Conversations", response.responseText, "danger");
+        return;
+    }
+    return response.responseJSON;
+}
+
+function getTeamsConversationMessages(access_token_id, conversation_link) {
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/get_teams_conversation_messages",
+        data: {
+            "access_token_id": access_token_id,
+            "conversation_link": conversation_link
+        }
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Teams Conversation Messages", response.responseText, "danger");
+        return;
+    }
+    return response.responseJSON;
+}
+
+function sendTeamsConversationMessage(access_token_id, conversation_link, message_content) {
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/send_teams_conversation_message",
+        data: {
+            "access_token_id": access_token_id,
+            "conversation_link": conversation_link,
+            "message_content": message_content
+        }
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Send Teams Messages", response.responseText, "danger");
+        return;
+    }
+    bootstrapToast("Send Teams Messages", `Teams message with ID ${response.responseText} created.`, "success");
+    return response.responseText;
+}
+
+function getTeamsConversationMembers(access_token_id, conversation_id) {
+    let response = $.ajax({
+        type: "POST",
+        async: false,
+        url: "/api/get_teams_conversation_members",
+        data: {
+            "access_token_id": access_token_id,
+            "conversation_id": conversation_id
+        }
+    });
+    if (response.status >= 400) {
+        bootstrapToast("Teams Members", response.responseText, "danger");
+        return;
+    }
+    return response.responseJSON;
+}
+
+
 // ========== Settings ==========
 
 function setTableErorMessages(state) {
     let response = $.ajax({
         type: "POST",
         async: false,
         url: "/api/set_table_error_messages",
```

### Comparing `GraphSpy-1.1.4/GraphSpy/static/js/theme.js` & `GraphSpy-1.2.0/GraphSpy/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/OneDrive.html` & `GraphSpy-1.2.0/GraphSpy/templates/OneDrive.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/SharePoint.html` & `GraphSpy-1.2.0/GraphSpy/templates/SharePoint.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/SharePointDrives.html` & `GraphSpy-1.2.0/GraphSpy/templates/SharePointDrives.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/SharePointSites.html` & `GraphSpy-1.2.0/GraphSpy/templates/SharePointSites.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/access_token_modal.html` & `GraphSpy-1.2.0/GraphSpy/templates/access_token_modal.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/access_tokens.html` & `GraphSpy-1.2.0/GraphSpy/templates/access_tokens.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/custom_requests.html` & `GraphSpy-1.2.0/GraphSpy/templates/custom_requests.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/device_codes.html` & `GraphSpy-1.2.0/GraphSpy/templates/device_codes.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/generic_search.html` & `GraphSpy-1.2.0/GraphSpy/templates/generic_search.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/index.html` & `GraphSpy-1.2.0/GraphSpy/templates/index.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/layout.html` & `GraphSpy-1.2.0/GraphSpy/templates/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     <link rel='stylesheet' href='https://cdn-uicons.flaticon.com/2.0.0/uicons-solid-rounded/css/uicons-solid-rounded.css'>
     <link rel='stylesheet' href='https://cdn-uicons.flaticon.com/2.0.0/uicons-bold-rounded/css/uicons-bold-rounded.css'>
     <!-- DataTables & jQuery -->
     <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.13.5/css/jquery.dataTables.min.css">
     <script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.5.1.js"></script>
     <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.11.1/js/jquery.dataTables.min.js"></script>
     <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.11.1/js/dataTables.bootstrap5.min.js"></script>
+    <!-- DOMPurify -->
+    <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/purify.min.js')}}"></script>
     <!-- Static JS $ CSS -->
     <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/theme.js')}}"></script>
     <script type="text/javascript" language="javascript" src="{{url_for('static', filename='js/functions.js')}}"></script>
     <link rel="stylesheet" type="text/css" href="{{url_for('static', filename='css/style.css')}}">
 
     <title>{{title}}</title>
 </head>
@@ -75,31 +77,40 @@
                             <li><a class="dropdown-item" href="{{url_for('sharepoint')}}">SharePoint Files</a></li>
                         </ul>
                     </li>
                     <li class="nav-item">
                         <a class="nav-link" href="{{url_for('outlook')}}">Outlook</a>
                     </li>
                     <li class="nav-item">
-                        <span class="d-inline-block" id="nav-teams-disabled" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Coming soon!" data-bs-placement="bottom">
-                            <a class="nav-link disabled">Teams</a>
+                        <a class="nav-link" href="{{url_for('teams')}}">Teams</a>
+                    </li>
+                    <li class="nav-item">
+                        <span class="d-inline-block" id="nav-entra-disabled" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Coming soon!" data-bs-placement="bottom">
+                            <a class="nav-link disabled">Entra ID</a>
+                        </span>
+                    </li>
+                    <li class="nav-item">
+                        <span class="d-inline-block" id="nav-azure-disabled" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Coming soon!" data-bs-placement="bottom">
+                            <a class="nav-link disabled">Azure</a>
                         </span>
                     </li>
                 </ul>
             </div>
             <div>
                 <ul class="navbar-nav justify-content-end">
                     <li class="nav-item">
                         <a class="nav-link" data-bs-toggle="offcanvas" href="#offcanvas-side-menu" role="button">Token Options</a>
                     </li>
                 </ul>
             </div>
         </div>
     </nav>
     <script>
-        const disabledPopover = new bootstrap.Popover(document.getElementById('nav-teams-disabled'))
+        const entraPopover = new bootstrap.Popover(document.getElementById('nav-entra-disabled'))
+        const azurePopover = new bootstrap.Popover(document.getElementById('nav-azure-disabled'))
     </script>
     <!-- Placeholders -->
     <div id="alert_placeholder"></div>
     <div id="toast_placeholder" class="toast-container position-fixed end-0 p-3"></div>
     <!-- Side Menu -->
     <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvas-side-menu" aria-labelledby="offcanvasLabel">
         <div class="offcanvas-header">
```

#### html2text {}

```diff
@@ -12,15 +12,17 @@
           o _F_i_l_e_s_ _S_h_a_r_e_d_ _W_i_t_h_ _M_e
           o _O_n_e_D_r_i_v_e
     * _S_h_a_r_e_P_o_i_n_t
           o _S_h_a_r_e_P_o_i_n_t_ _S_i_t_e_s
           o _S_h_a_r_e_P_o_i_n_t_ _D_r_i_v_e_s
           o _S_h_a_r_e_P_o_i_n_t_ _F_i_l_e_s
     * _O_u_t_l_o_o_k
-    * Teams
+    * _T_e_a_m_s
+    * Entra ID
+    * Azure
     * _T_o_k_e_n_ _O_p_t_i_o_n_s
 ********** TTookkeenn OOppttiioonnss **********
 Resource[                    ]
 Defined in Refresh Token
 MSGraph
 AAD Graph
 Outlook
```

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/outlook.html` & `GraphSpy-1.2.0/GraphSpy/templates/outlook.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/recent_files.html` & `GraphSpy-1.2.0/GraphSpy/templates/recent_files.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/refresh_token_modal.html` & `GraphSpy-1.2.0/GraphSpy/templates/refresh_token_modal.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/refresh_tokens.html` & `GraphSpy-1.2.0/GraphSpy/templates/refresh_tokens.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/settings.html` & `GraphSpy-1.2.0/GraphSpy/templates/settings.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy/templates/shared_with_me.html` & `GraphSpy-1.2.0/GraphSpy/templates/shared_with_me.html`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/GraphSpy.egg-info/PKG-INFO` & `GraphSpy-1.2.0/GraphSpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.4
+Version: 1.2.0
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# GraphSpy
+[![PyPi Version](https://img.shields.io/pypi/v/GraphSpy.svg)](https://pypi.org/project/GraphSpy/)
+![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
+[![Twitter](https://img.shields.io/twitter/follow/RedByte1337?label=RedByte1337&style=social)](https://twitter.com/intent/follow?screen_name=RedByte1337)
 
+# GraphSpy
 
 ```
    ________                             _________
   /       /  by RedByte1337    __      /        /           
  /  _____/___________  ______ |  |__  /   _____/_____ ______
 /   \  __\_  __ \__  \ \____ \|  |  \ \_____  \\____ \   |  |
 \    \_\  \  | \/  __ \|  |_> |   \  \/        \  |_> \___  |
@@ -117,14 +120,20 @@
 
 Open the user's Outlook with a single click using just an Outlook access token (FOCI)!
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
+## MS Teams
+
+Read and send messages using the Microsoft Teams module with a FOCI access token of the skype API (https://api.spaces.skype.com/).
+
+![MS Teams GraphSpy](images/ms_teams.png)
+
 ## Graph Searching
 
 Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
@@ -156,17 +165,18 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Microsoft Teams
-	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
-	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
+* Improve Microsoft Teams Module
+  * Download authenticated files
+  * Create new conversations
+  * Upload files and images
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
 
 # Credits
```

### Comparing `GraphSpy-1.1.4/GraphSpy.egg-info/SOURCES.txt` & `GraphSpy-1.2.0/GraphSpy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 GraphSpy.egg-info/SOURCES.txt
 GraphSpy.egg-info/dependency_links.txt
 GraphSpy.egg-info/entry_points.txt
 GraphSpy.egg-info/requires.txt
 GraphSpy.egg-info/top_level.txt
 GraphSpy/static/css/style.css
 GraphSpy/static/js/functions.js
+GraphSpy/static/js/purify.min.js
 GraphSpy/static/js/theme.js
 GraphSpy/templates/OneDrive.html
 GraphSpy/templates/SharePoint.html
 GraphSpy/templates/SharePointDrives.html
 GraphSpy/templates/SharePointSites.html
 GraphSpy/templates/access_token_modal.html
 GraphSpy/templates/access_tokens.html
@@ -27,8 +28,9 @@
 GraphSpy/templates/index.html
 GraphSpy/templates/layout.html
 GraphSpy/templates/outlook.html
 GraphSpy/templates/recent_files.html
 GraphSpy/templates/refresh_token_modal.html
 GraphSpy/templates/refresh_tokens.html
 GraphSpy/templates/settings.html
-GraphSpy/templates/shared_with_me.html
+GraphSpy/templates/shared_with_me.html
+GraphSpy/templates/teams.html
```

### Comparing `GraphSpy-1.1.4/LICENSE.txt` & `GraphSpy-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphSpy-1.1.4/PKG-INFO` & `GraphSpy-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: GraphSpy
-Version: 1.1.4
+Version: 1.2.0
 Summary: Initial Access and Post-Exploitation Tool for AAD and O365 with a browser-based GUI
 Home-page: https://github.com/RedByte1337/GraphSpy
 Author: RedByte1337
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# GraphSpy
+[![PyPi Version](https://img.shields.io/pypi/v/GraphSpy.svg)](https://pypi.org/project/GraphSpy/)
+![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
+[![Twitter](https://img.shields.io/twitter/follow/RedByte1337?label=RedByte1337&style=social)](https://twitter.com/intent/follow?screen_name=RedByte1337)
 
+# GraphSpy
 
 ```
    ________                             _________
   /       /  by RedByte1337    __      /        /           
  /  _____/___________  ______ |  |__  /   _____/_____ ______
 /   \  __\_  __ \__  \ \____ \|  |  \ \_____  \\____ \   |  |
 \    \_\  \  | \/  __ \|  |_> |   \  \/        \  |_> \___  |
@@ -117,14 +120,20 @@
 
 Open the user's Outlook with a single click using just an Outlook access token (FOCI)!
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
+## MS Teams
+
+Read and send messages using the Microsoft Teams module with a FOCI access token of the skype API (https://api.spaces.skype.com/).
+
+![MS Teams GraphSpy](images/ms_teams.png)
+
 ## Graph Searching
 
 Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
@@ -156,17 +165,18 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Microsoft Teams
-	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
-	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
+* Improve Microsoft Teams Module
+  * Download authenticated files
+  * Create new conversations
+  * Upload files and images
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
 
 # Credits
```

### Comparing `GraphSpy-1.1.4/README.md` & `GraphSpy-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# GraphSpy
+[![PyPi Version](https://img.shields.io/pypi/v/GraphSpy.svg)](https://pypi.org/project/GraphSpy/)
+![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
+[![Twitter](https://img.shields.io/twitter/follow/RedByte1337?label=RedByte1337&style=social)](https://twitter.com/intent/follow?screen_name=RedByte1337)
 
+# GraphSpy
 
 ```
    ________                             _________
   /       /  by RedByte1337    __      /        /           
  /  _____/___________  ______ |  |__  /   _____/_____ ______
 /   \  __\_  __ \__  \ \____ \|  |  \ \_____  \\____ \   |  |
 \    \_\  \  | \/  __ \|  |_> |   \  \/        \  |_> \___  |
@@ -108,14 +111,20 @@
 
 Open the user's Outlook with a single click using just an Outlook access token (FOCI)!
 
 ![Outlook GraphSpy](images/outlook_1.png)
 
 ![Outlook](images/outlook_2.png)
 
+## MS Teams
+
+Read and send messages using the Microsoft Teams module with a FOCI access token of the skype API (https://api.spaces.skype.com/).
+
+![MS Teams GraphSpy](images/ms_teams.png)
+
 ## Graph Searching
 
 Search for keywords through all Microsoft 365 applications using the Microsoft Search API.
 
 For instance, use this to search for any files or emails containing keywords such as "password", "secret", ...
 
 ![Graph Search](images/graph_search_2.png)
@@ -147,17 +156,18 @@
 # Upcoming Features
 
 * Upload, Delete and Rename Files
 * More authentication options
 	* Password, ESTSAuth Cookie, PRT, ...
 * Advanced token customization options and optional v2 API support (CAE)
 * Automatic Access Token Refreshing
-* Microsoft Teams
-	* Sadly, most MSGrapgh scopes required for Microsoft Teams can not be obtained through a FOCI client id, limiting the usecases where it could be accessed.
-	* So the best option would be to use the Skype API, which is a FOCI resource, although this API is not documented by Microsoft or intended for public use
+* Improve Microsoft Teams Module
+  * Download authenticated files
+  * Create new conversations
+  * Upload files and images
 * Azure AD
 	* List Users, Groups, Applications, Devices, Conditional Access Policies, ...
 * Cleaner exception handling
 	* While this should not have any direct impact on the user, edge cases might currently throw exceptions to the GraphSpy output instead of handling them in a cleaner way.
 
 # Credits
```

### Comparing `GraphSpy-1.1.4/setup.py` & `GraphSpy-1.2.0/setup.py`

 * *Files identical despite different names*

