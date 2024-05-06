# Comparing `tmp/smartschoolapi_tkbstudios-1.0.1.tar.gz` & `tmp/smartschoolapi_tkbstudios-1.1.0.tar.gz`

## Comparing `smartschoolapi_tkbstudios-1.0.1.tar` & `smartschoolapi_tkbstudios-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/.env.example
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/requirements.txt
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/.github/workflows/publishpkg.yml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/examples/list_messages.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/examples/websocket_client.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/src/smartschoolapi_tkbstudios/__init__.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/src/smartschoolapi_tkbstudios/smartschool.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/LICENSE
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/.env.example
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/requirements.txt
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/.github/workflows/publishpkg.yml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/examples/get_courses.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/examples/list_messages.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/examples/websocket_client.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/src/smartschoolapi_tkbstudios/__init__.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/src/smartschoolapi_tkbstudios/smartschool.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/LICENSE
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 smartschoolapi_tkbstudios-1.1.0/PKG-INFO
```

### Comparing `smartschoolapi_tkbstudios-1.0.1/.github/workflows/publishpkg.yml` & `smartschoolapi_tkbstudios-1.1.0/.github/workflows/publishpkg.yml`

 * *Files identical despite different names*

### Comparing `smartschoolapi_tkbstudios-1.0.1/.github/workflows/pylint.yml` & `smartschoolapi_tkbstudios-1.1.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `smartschoolapi_tkbstudios-1.0.1/examples/list_messages.py` & `smartschoolapi_tkbstudios-1.1.0/examples/list_messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 List messages example
 """
 import os
 import logging
 import time
 import dotenv
-from smartschoolapi import SmartSchoolClient
+from smartschoolapi_tkbstudios import SmartSchoolClient
 
 
 if __name__ == '__main__':
     """
     List messages
     """
     os.makedirs("messages", exist_ok=True)
     dotenv.load_dotenv()
 
     smart_school_client = SmartSchoolClient(
         domain=os.getenv('SMARTSCHOOL_DOMAIN'),
-        phpsessid=os.getenv('SMARTSCHOOL_PHPSESSID'),
-        pid=os.getenv('SMARTSCHOOL_PID'),
-        user_id=os.getenv('SMARTSCHOOL_USER_ID'),
-        loglevel=logging.INFO,
+        loglevel=logging.DEBUG,
     )
+    smart_school_client.phpsessid = os.getenv('SMARTSCHOOL_PHPSESSID')
+    smart_school_client.pid = os.getenv('SMARTSCHOOL_PID')
+    smart_school_client.user_id = os.getenv('SMARTSCHOOL_USER_ID')
 
     messages = smart_school_client.list_messages()
     print(f"You have {len(messages)} messages.")
 
     for message in messages:
         message_data = smart_school_client.get_message_by_id(message["id"])
         print("Message data:")
```

### Comparing `smartschoolapi_tkbstudios-1.0.1/src/smartschoolapi_tkbstudios/smartschool.py` & `smartschoolapi_tkbstudios-1.1.0/src/smartschoolapi_tkbstudios/smartschool.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,72 +5,84 @@
 import logging
 from xml.etree import ElementTree
 from uuid import uuid4
 import colorlog
 import requests
 import websocket
 
+OFFICE365_SSO_INIT_URI = "/login/sso/init/office365"
+
 
 class ApiException(Exception):
     """
     Api exception
     """
 
 
+class AuthException(ApiException):
+    """
+    Auth exception
+    """
+
+
 class SmartSchoolClient:
     """
     SmartSchool client
 
     Args:
         domain: SmartSchool domain
-        phpsessid: PHPSESSID
-        pid: pid
-        user_id: user id
         loglevel: logging level
-        received_message_callback: callback function
 
     Attributes:
         domain: SmartSchool domain
         phpsessid: PHPSESSID
         pid: pid
         user_id: user id
         received_message_callback: callback function
 
+        api_logger: logger for API
+        websocket_logger: logger for Websocket
+        auth_logger: logger for Authentication
+
     Methods:
         get_token_from_api()
         get_messages_from_api()
         get_message_by_id(message_id)
         list_messages()
+        authenticate()
         run_websocket()
     """
-    def __init__(self, domain, phpsessid, pid, user_id, loglevel=logging.DEBUG, received_message_callback=None):
+
+    def __init__(self, domain, loglevel=logging.DEBUG):
         self.domain = domain
-        self.phpsessid = phpsessid
-        self.pid = pid
-        self.user_id = user_id
-        self.received_message_callback = received_message_callback
+        self.phpsessid = None
+        self.pid = None
+        self.user_id = None
+        self.received_message_callback = None
+        self.user_token = None
 
-        handler = colorlog.StreamHandler()
-        handler.setFormatter(
+        colorlog_handler = colorlog.StreamHandler()
+        colorlog_handler.setFormatter(
             colorlog.ColoredFormatter(
                 '%(log_color)s%(asctime)s - %(name)s - %(levelname)s - %(message)s'
             )
         )
 
         self.api_logger = colorlog.getLogger("Core/API")
-        self.api_logger.addHandler(handler)
+        self.api_logger.addHandler(colorlog_handler)
         self.api_logger.setLevel(loglevel)
 
         self.websocket_logger = colorlog.getLogger("Core/Websocket")
-        self.websocket_logger.addHandler(handler)
+        self.websocket_logger.addHandler(colorlog_handler)
         self.websocket_logger.setLevel(loglevel)
 
-        self.user_token = self.get_token_from_api()
+        self.auth_logger = colorlog.getLogger("Core/Authentication")
+        self.auth_logger.addHandler(colorlog_handler)
+        self.auth_logger.setLevel(loglevel)
 
-    # general stuff
     def get_token_from_api(self):
         """
         Get token from API
         """
         self.api_logger.info("Requesting token from API")
         self.api_logger.debug("Sending request to get token")
         response = requests.get(
@@ -81,15 +93,16 @@
             json={
                 'userID': self.user_id
             },
             timeout=10
         )
         if response.status_code == 200:
             self.api_logger.info("Token received")
-            return response.text
+            self.user_token = response.text
+            return self.user_token
         self.api_logger.error("Could not get token")
         raise ApiException("Could not get token")
 
     def find_users_by_name(self, name):
         """
         Find users by name
         """
@@ -185,15 +198,16 @@
             'body': message_elem.find('body').text,
             'status': message_elem.find('status').text,
             'attachment': message_elem.find('attachment').text,
             'unread': message_elem.find('unread').text,
             'label': message_elem.find('label').text,
             'receivers': [receiver.text for receiver in message_elem.findall('receivers/to')],
             'ccreceivers': [receiver.text for receiver in message_elem.findall('ccreceivers/cc')],
-            'bccreceivers': [receiver.text for receiver in message_elem.findall('bccreceivers/bcc')],
+            'bccreceivers': [receiver.text for receiver in
+                             message_elem.findall('bccreceivers/bcc')],
             'senderPicture': message_elem.find('senderPicture').text,
             'markedInLVS': message_elem.find('markedInLVS').text,
             'fromTeam': message_elem.find('fromTeam').text,
             'totalNrOtherToReciviers': message_elem.find('totalNrOtherToReciviers').text,
             'totalnrOtherCcReceivers': message_elem.find('totalnrOtherCcReceivers').text,
             'totalnrOtherBccReceivers': message_elem.find('totalnrOtherBccReceivers').text,
             'canReply': message_elem.find('canReply').text,
@@ -267,26 +281,50 @@
         )
         if response.status_code == 200:
             self.api_logger.info("Message received")
             return self.parse_single_message_response(response.text)
         self.api_logger.error("Could not get message")
         raise ApiException("Could not get message")
 
+    def get_courses(self):
+        """
+        Get courses
+        """
+        self.api_logger.info("Requesting courses from API")
+        self.api_logger.debug("Sending request to get courses")
+        headers = {
+            'Cookie': f'pid={self.pid}; PHPSESSID={self.phpsessid}',
+            'Content-Type': 'application/json, text/javascript, */*;',
+            'X-Requested-With': 'XMLHttpRequest',
+        }
+        response = requests.post(
+            f'https://{self.domain}/Topnav/getCourseConfig',
+            headers=headers,
+            timeout=10
+        )
+        if response.status_code == 200:
+            self.api_logger.info("Courses received")
+            courses_json = json.loads(response.text)
+            return courses_json['own']
+        self.api_logger.error("Could not get courses")
+        raise ApiException("Could not get courses")
+
     # websockets
     def ws_on_error(self, _, error):
         """
         Websocket error
         """
         self.websocket_logger.error("Error: %s", error)
 
     def ws_on_close(self, _, close_status_code, close_msg):
         """
         Websocket close
         """
-        self.websocket_logger.info("WebSocket connection closed: %s - %s", close_status_code, close_msg)
+        self.websocket_logger.info("WebSocket connection closed: %s - %s", close_status_code,
+                                   close_msg)
 
     def ws_on_open(self, ws):
         """
         Websocket open
         """
         self.websocket_logger.info("WebSocket connection opened")
         auth_message = {
@@ -300,17 +338,18 @@
         """
         Websocket message
         """
         self.websocket_logger.debug("Received message: %s", message)
         message_data = json.loads(message)
         message_type = message_data.get("type", None)
         message_text = message_data.get("text", None)
+        message_request = message_data.get("request", None)
 
         if message_type is not None:
-            if message_type == "auth":
+            if message_type == "auth" and message_request == "getToken":
                 self.websocket_logger.info("Authentication successful!")
             elif message_type == "notificationListStart":
                 self.websocket_logger.info("Notification list started.")
             elif message_type == "getNotificationConfig":
                 config_message = {
                     "type": "setConfig",
                     "queueUuid": uuid4().hex,
@@ -325,20 +364,20 @@
                         if message.get("module", None) == "Messages":
                             sender = message.get("title", None)
                             description = message.get("description", None)
                             url = message.get("url", None)
                             user_id = message.get("userID", None)
                             if sender is not None and description is not None and url is not None and user_id is not None:
                                 url = f"https://{self.domain}{url[1:]}"
-                                self.api_logger.info(
+                                self.api_logger.debug(
                                     "Received message from %s: %s (%s)",
                                     sender, description, url
                                 )
                                 if self.received_message_callback is not None:
-                                    self.received_message_callback(sender, description, url, user_id)
+                                    self.received_message_callback(message_data)
 
     def run_websocket(self):
         """
         Run Websocket
         """
         self.websocket_logger.info("Connecting to WebSocket")
         ws = websocket.WebSocketApp(
```

### Comparing `smartschoolapi_tkbstudios-1.0.1/LICENSE` & `smartschoolapi_tkbstudios-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartschoolapi_tkbstudios-1.0.1/README.md` & `smartschoolapi_tkbstudios-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SmartSchool Client
 I made this library to communicate with smartschool for some reason.  
 I was able to bind it with a voice assistant to tell me when I get a new message. (Home Assistant for reference)
 
 # How to use
-Install using ``pip install smartschoolapi-tkbstudios -U``
+Install using ``pip install smartschoolapi_tkbstudios -U``
 
 # Legal
 This library complies with the [SmartSchool User Agreement](https://www.smartschool.be/gebruikersovereenkomst/).  
 I am **NOT** responsible for anything that a user does with this library.  
 Please comply with the SS User Agreement! Not doing so will result in legal consequences.  
 Again, please do **NOT** break those rules, it's for your best.
```

### Comparing `smartschoolapi_tkbstudios-1.0.1/pyproject.toml` & `smartschoolapi_tkbstudios-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smartschoolapi_tkbstudios"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="TKB Studios", email="tkbstudios@mail.tkbstudios.com" },
 ]
 description = "A python package to interact with SmartSchool, a Belgian School Management System"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `smartschoolapi_tkbstudios-1.0.1/PKG-INFO` & `smartschoolapi_tkbstudios-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smartschoolapi_tkbstudios
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python package to interact with SmartSchool, a Belgian School Management System
 Project-URL: Homepage, https://github.com/tkbstudios/SmartSchoolPyClient
 Project-URL: Issues, https://github.com/tkbstudios/SmartSchoolPyClient/issues
 Author-email: TKB Studios <tkbstudios@mail.tkbstudios.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 
 # SmartSchool Client
 I made this library to communicate with smartschool for some reason.  
 I was able to bind it with a voice assistant to tell me when I get a new message. (Home Assistant for reference)
 
 # How to use
-Install using ``pip install smartschoolapi-tkbstudios -U``
+Install using ``pip install smartschoolapi_tkbstudios -U``
 
 # Legal
 This library complies with the [SmartSchool User Agreement](https://www.smartschool.be/gebruikersovereenkomst/).  
 I am **NOT** responsible for anything that a user does with this library.  
 Please comply with the SS User Agreement! Not doing so will result in legal consequences.  
 Again, please do **NOT** break those rules, it's for your best.
```

