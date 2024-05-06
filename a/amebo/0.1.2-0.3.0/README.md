# Comparing `tmp/amebo-0.1.2.tar.gz` & `tmp/amebo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amebo-0.1.2.tar", max compression
+gzip compressed data, was "amebo-0.3.0.tar", max compression
```

## Comparing `amebo-0.1.2.tar` & `amebo-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6314 2023-05-16 05:08:20.824236 amebo-0.1.2/README.md
--rw-r--r--   0        0        0     2544 2023-04-05 09:41:47.811252 amebo-0.1.2/amebo.py
--rw-r--r--   0        0        0      511 2023-05-16 05:07:01.705318 amebo-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 amebo-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7394 2024-05-05 03:08:04.783226 amebo-0.3.0/README.md
+-rw-r--r--   0        0        0     2564 2024-04-23 14:23:49.283283 amebo-0.3.0/amebo.py
+-rw-r--r--   0        0        0      522 2024-05-06 10:59:02.487107 amebo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8142 1970-01-01 00:00:00.000000 amebo-0.3.0/PKG-INFO
```

### Comparing `amebo-0.1.2/README.md` & `amebo-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 # AMEBO
 
 Amebo is the simplest pubsub server to use, deploy, understand or maintain. It was
 built to enable communication between applications i.e. microservices or
 modules (if you are using monoliths), and hopes to be able to serve as a small
 but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS.
 
-**STILL IN DEVELOPMENT: NOT READY FOR Production Use**
+1. Availability: Amebo runs on battle tested open source tools i.e. Redis, Postgres and provides the same level of availability guarantees
+
+1. Reliability: Amebo has been used at scale by open source projects to handle 100's of millions of request
+
+1. Latency: Amebo guarantees sub 100ms latencies at scale (barring network and hardware limitations)
+
 
 &nbsp;
 
 ## How It Works
 ---
 Amebo has only 4 concepts (first class objects) to understand or master.
 
 &nbsp;
 
-### 1. Microservices/Modules
+### 1. Applications
 ---
-These are applications or modules you register on amebo - they send and receive events ;-)
+These can be microservices or modules (in a monolith) - that create and receive notifications about [_**events**_](#2-events). All applications must be registered on
+    amebo ;-) before they can publish [_**events**_](#3-events).
 
 
-### 2. Events
+### 2. Action
 ---
-Something that can happen in an application, they are registered on Amebo by Microservices/Modules
+This is something that can happen in an [_**application**_](#1-applications) i.e. creating a customer, deleting an order. They are registered
+    on Amebo by their parent [_**application**_](#1-applications), and all actions must provide a valid JSON Schema (can be empty "{}") that Amebo
+    can use to validate action events before sending to [_**subscribers**_](#4-subscribers).
 
-### 3. Actions
+
+### 3. Events
 ---
-A HTTP request sent to Amebo to signal an event (action on event) has occured. Usually has a payload that
-    is forwarded by Amebo to all applications subscribed to the offending event
+An event is the occurence of an action and in practice is a HTTP request sent by an [_**application**_](#1-applications) to Amebo to signal it about the occurence of an action locally. Events can have a json payload that must match the JSON Schema of its parent action.
 
 ### 4. Subscribers
 ---
-HTTP endpoints registered to watch specific/particular events (by Microservices/Modules)
+These are HTTP URLs (can be valid hostname for loopback interface on TCP/IP as well) endpoints registered by [_**applications**_](#1-applications) to
+    receive [_**action**_](#3-actions) payloads.
 
 &nbsp;
 
 
 ## GETTING STARTED
 This assumes you have [installed](https://github.com/tersoo/amebo) Amebo on your machine. Amebo requires [Python3.6+](https://www.python.org/downloads)
 ```sh
@@ -93,52 +102,52 @@
 </td>
 </tr>
 </table>
 
 
 &nbsp;
 
-## 2nd : Register events that can happen in the registered microservices
+## 2nd : Register actions that can happen in the registered microservices
 ---
 
-`endpoint: /v1/events`
+`endpoint: /v1/actions`
 
 <table>
 <tr>
 <th>Endpoint JSON Schema</th>
 <th>Example Payload<th>
 </tr>
 <tr>
 <td>
 
 ```json
 {
     "type": "object",
     "properties": {
-        "event": {"type": "string"},
+        "action": {"type": "string"},
         "microservice": {"type": "string"},
         "schemata": {
             "type": "object",
             "properties": {
                 "type": {"type": "string"},
                 "properties": {"type": "object"},
                 "required": {"type": "array"}
             }
         }
     },
-    "required": ["event", "microservice", "schemata"]
+    "required": ["action", "microservice", "schemata"]
 }
 ```
 
 </td>
 <td>
 
 ```json
 {
-    "event": "customers.v1.created",
+    "action": "customers.v1.created",
     "microservice": "customers",
     "schemata": {
         "$id": "https://your-domain/customers/customer-created-schema-example.json",
         "$schema": "https://json-schema.org/draft/2020-12/schema",
         "type": "object",
         "properties": {
             "customer_id": {"type": "number"},
@@ -153,24 +162,24 @@
 
 </td>
 </tr>
 </table>
 
 &nbsp;
 
-## 3rd : Tell Amebo when an event occurs i.e. create an action
+## 3rd : Tell Amebo when an action occurs i.e. create an event
 ---
 
-`endpoint: /v1/actions`
+`endpoint: /v1/events`
 
 | Key | Description |
 |---|---|
-| **event** | Identifier name of the event. (As registered in the previous step.) |
-| **deduper** | Deduplication string. used to prevent the same action from being registered twice |
-| **payload** | JSON data (must confirm to the schema registerd with the event) |
+| **action** | Identifier name of the action. (As registered in the previous step.) |
+| **deduper** | Deduplication string. used to prevent the same event from being registered twice |
+| **payload** | JSON data (must confirm to the schema registerd with the action) |
 
 &nbsp;
 
 <table>
 <tr>
 <th>Endpoint JSON Schema</th>
 <th>Example Payload<th>
@@ -233,13 +242,17 @@
 1. Amebo comes complete with a Schema Registry, ensuring actions conform to event schema, and makes it easy for developers to search for events by
     microservice with commensurate schema (i.e. what is required, what is optional) as opposed to meetings with team mates continually.
 
 1. GUI for tracking events, actions, subscribers. Easy discovery of what events exist, what events failed and GUI retry for specific subscribers
 
 1. Gossiping is HTTP native i.e. subscribers receive http requests automatically at pre-registered endpoints
 
+1. Envelope format and transmission is web native and clearly outlined by schema registry
+
+1. Topic management is simplified as actions with versioning support baked in
+
 1. Infinite retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon)
 
 
 # Trivia
 
 The word `amebo` is a West African (Nigerian origin - but used in Ghana, Benin, Cameroon etc.) slang used to describe anyone that never keeps what you tell them to themselves. A talkative, never mind their business individual (a chronic gossip).
```

#### html2text {}

```diff
@@ -1,61 +1,72 @@
 # AMEBO Amebo is the simplest pubsub server to use, deploy, understand or
 maintain. It was built to enable communication between applications i.e.
 microservices or modules (if you are using monoliths), and hopes to be able to
 serve as a small but capable and simpler alternative to Kafka, RabbitMQ, SQS/
-SNS. **STILL IN DEVELOPMENT: NOT READY FOR Production Use**   ## How It Works -
--- Amebo has only 4 concepts (first class objects) to understand or master.  
-### 1. Microservices/Modules --- These are applications or modules you register
-on amebo - they send and receive events ;-) ### 2. Events --- Something that
-can happen in an application, they are registered on Amebo by Microservices/
-Modules ### 3. Actions --- A HTTP request sent to Amebo to signal an event
-(action on event) has occured. Usually has a payload that is forwarded by Amebo
-to all applications subscribed to the offending event ### 4. Subscribers --
-- HTTP endpoints registered to watch specific/particular events (by
-Microservices/Modules)   ## GETTING STARTED This assumes you have [installed]
-(https://github.com/tersoo/amebo) Amebo on your machine. Amebo requires
-[Python3.6+](https://www.python.org/downloads) ```sh # the easy path pip
-install amebo amebo --workers 2 --address 0.0.0.0:8701 # the hardway (manual
-installation) BUT not the only way... Sorry, I couldn't resist the pun ;-) git
-clone https://github.com/tersoo/amebo mv amebo /to/a/directory/of/your/choosing
-export $PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo location
-to your path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo about all
-your microservices or applications --- `endpoint: /v1/microservices`
+SNS. 1. Availability: Amebo runs on battle tested open source tools i.e. Redis,
+Postgres and provides the same level of availability guarantees 1. Reliability:
+Amebo has been used at scale by open source projects to handle 100's of
+millions of request 1. Latency: Amebo guarantees sub 100ms latencies at scale
+(barring network and hardware limitations)   ## How It Works --- Amebo has only
+4 concepts (first class objects) to understand or master.   ### 1. Applications
+--- These can be microservices or modules (in a monolith) - that create and
+receive notifications about [_**events**_](#2-events). All applications must be
+registered on amebo ;-) before they can publish [_**events**_](#3-events). ###
+2. Action --- This is something that can happen in an [_**application**_](#1-
+applications) i.e. creating a customer, deleting an order. They are registered
+on Amebo by their parent [_**application**_](#1-applications), and all actions
+must provide a valid JSON Schema (can be empty "{}") that Amebo can use to
+validate action events before sending to [_**subscribers**_](#4-subscribers).
+### 3. Events --- An event is the occurence of an action and in practice is a
+HTTP request sent by an [_**application**_](#1-applications) to Amebo to signal
+it about the occurence of an action locally. Events can have a json payload
+that must match the JSON Schema of its parent action. ### 4. Subscribers --
+- These are HTTP URLs (can be valid hostname for loopback interface on TCP/IP
+as well) endpoints registered by [_**applications**_](#1-applications) to
+receive [_**action**_](#3-actions) payloads.   ## GETTING STARTED This assumes
+you have [installed](https://github.com/tersoo/amebo) Amebo on your machine.
+Amebo requires [Python3.6+](https://www.python.org/downloads) ```sh # the easy
+path pip install amebo amebo --workers 2 --address 0.0.0.0:8701 # the hardway
+(manual installation) BUT not the only way... Sorry, I couldn't resist the pun
+;-) git clone https://github.com/tersoo/amebo mv amebo /to/a/directory/of/your/
+choosing export $PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo
+location to your path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo
+about all your microservices or applications --- `endpoint: /v1/microservices`
 SScchheemmaa                                 EExxaammppllee PPaayyllooaadd
 ```json { "$schema": "", "type":
 "object", "properties":
 { "microservice": {"type": "string"},  ```json { "microservice": "customers",
 "passkey": {"type": "string",          "passkey": "some-super-duper-secret-of-
 "format": "ipv4 | ipv6 | hostname |    the-module-or-microservice",
 idn-hostname"}, "location": {"type":   "location": "http://0.0.0.0:3300" } ```
 "web"} }, "required": ["microservice",
 "passkey", "location"] } ```
-  ## 2nd : Register events that can happen in the registered microservices --
-- `endpoint: /v1/events`
-EEnnddppooiinntt JJSSOONN SScchheemmaa                  EExxaammppllee PPaayyllooaadd
-                                      ```json { "event":
-                                      "customers.v1.created", "microservice":
-```json { "type": "object",           "customers", "schemata": { "$id":
-"properties": { "event": {"type":     "https://your-domain/customers/
-"string"}, "microservice": {"type":   customer-created-schema-example.json",
-"string"}, "schemata": { "type":      "$schema": "https://json-schema.org/
-"object", "properties": { "type":     draft/2020-12/schema", "type":
-{"type": "string"}, "properties":     "object", "properties":
-{"type": "object"}, "required":       { "customer_id": {"type": "number"},
-{"type": "array"} } } }, "required":  "first_name": {"type": "string"},
-["event", "microservice", "schemata"] "last_name": {"type": "string"},
-} ```                                 "email": {"type": "string", "format":
-                                      "email"} }, "required": ["customer_id",
-                                      "email"] } } ```
-  ## 3rd : Tell Amebo when an event occurs i.e. create an action --- `endpoint:
-/v1/actions` | Key | Description | |---|---| | **event** | Identifier name of
-the event. (As registered in the previous step.) | | **deduper** |
-Deduplication string. used to prevent the same action from being registered
+  ## 2nd : Register actions that can happen in the registered microservices --
+- `endpoint: /v1/actions`
+EEnnddppooiinntt JJSSOONN SScchheemmaa                   EExxaammppllee PPaayyllooaadd
+                                       ```json { "action":
+                                       "customers.v1.created", "microservice":
+```json { "type": "object",            "customers", "schemata": { "$id":
+"properties": { "action": {"type":     "https://your-domain/customers/
+"string"}, "microservice": {"type":    customer-created-schema-example.json",
+"string"}, "schemata": { "type":       "$schema": "https://json-schema.org/
+"object", "properties": { "type":      draft/2020-12/schema", "type":
+{"type": "string"}, "properties":      "object", "properties":
+{"type": "object"}, "required":        { "customer_id": {"type": "number"},
+{"type": "array"} } } }, "required":   "first_name": {"type": "string"},
+["action", "microservice", "schemata"] "last_name": {"type": "string"},
+} ```                                  "email": {"type": "string", "format":
+                                       "email"} }, "required": ["customer_id",
+                                       "email"] } } ```
+  ## 3rd : Tell Amebo when an action occurs i.e. create an event --- `endpoint:
+/v1/events` | Key | Description | |---|---| | **action** | Identifier name of
+the action. (As registered in the previous step.) | | **deduper** |
+Deduplication string. used to prevent the same event from being registered
 twice | | **payload** | JSON data (must confirm to the schema registerd with
-the event) |  
+the action) |  
 EEnnddppooiinntt JJSSOONN SScchheemmaa                EExxaammppllee PPaayyllooaadd
                                     ```json { "event":
                                     "customers.v1.created", "microservice":
                                     "customers", "schema": { "$id": "https:
 ```json { "type": "object",         //your-domain/customers/customer-
 "properties": { "event": {"type":   created-schema-example.json",
 "string"}, "microservice": {"type": "$schema": "https://json-schema.org/
@@ -76,13 +87,15 @@
 Why? Advantages over traditional Message Oriented Middleware(s) 1. Amebo comes
 complete with a Schema Registry, ensuring actions conform to event schema, and
 makes it easy for developers to search for events by microservice with
 commensurate schema (i.e. what is required, what is optional) as opposed to
 meetings with team mates continually. 1. GUI for tracking events, actions,
 subscribers. Easy discovery of what events exist, what events failed and GUI
 retry for specific subscribers 1. Gossiping is HTTP native i.e. subscribers
-receive http requests automatically at pre-registered endpoints 1. Infinite
-retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon) # Trivia The
-word `amebo` is a West African (Nigerian origin - but used in Ghana, Benin,
-Cameroon etc.) slang used to describe anyone that never keeps what you tell
-them to themselves. A talkative, never mind their business individual (a
+receive http requests automatically at pre-registered endpoints 1. Envelope
+format and transmission is web native and clearly outlined by schema registry
+1. Topic management is simplified as actions with versioning support baked in
+1. Infinite retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon) #
+Trivia The word `amebo` is a West African (Nigerian origin - but used in Ghana,
+Benin, Cameroon etc.) slang used to describe anyone that never keeps what you
+tell them to themselves. A talkative, never mind their business individual (a
 chronic gossip).
```

### Comparing `amebo-0.1.2/amebo.py` & `amebo-0.3.0/amebo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from asyncio import gather, sleep
 from http import HTTPStatus
 from sqlite3 import Connection, Cursor
-from typing import List
 
 # installed libs
+from heaven import Router
 from httpx import AsyncClient
 from orjson import loads
 
 # src code
-from washika import Washika as Router
+from constants.literals import DB
 
 
 async def amebo(router: Router):
-    db: Connection = router.peek('db')
+    db: Connection = router.peek(DB)
     accepters = []
     rejecters = []
     async def notify(endpoint: str, data: dict, passkey: str, gist_id: int):
         headers = {
             'Content-Type': 'application/json',
             'X-Secret-Key': passkey
         }
@@ -28,15 +28,15 @@
                 rejecters.append(int(gist_id))
             else:
                 accepters.append(int(gist_id))
         except Exception as exc:
             rejecters.append(gist_id)
         finally:
             await client.aclose()
-        
+
         try:
             cursor: Cursor = db.cursor()
             cursor.execute(f'''
                 UPDATE
                     gists
                 SET
                     completed = 1
@@ -45,34 +45,35 @@
             db.commit()
         except Exception as exc:
             print('Could not update in notify: ', exc)
         finally:
             cursor.close()
 
     async def traverse():
+        cursor = None
         try:
             cursor: Cursor = db.cursor()
             gists = cursor.execute(f'''
                 SELECT
-                    m.location || s.endpoint AS endpoint, a.payload, m.passkey, g.rowid as gid
-                FROM gists AS g JOIN actions a ON
-                    g.action = a.action
+                    m.location || s.endpoint AS endpoint, e.payload, m.passkey, g.rowid as gid
+                FROM gists AS g JOIN events e ON
+                    g.event = e.event
                 JOIN subscribers s ON
                     s.subscriber = g.subscriber
-                JOIN events e ON
-                    a.event = e.event
+                JOIN actions a ON
+                    e.action = a.action
                 JOIN microservices m ON
                     s.microservice = m.microservice
                 WHERE g.completed <> 1
-                ORDER BY g.action LIMIT {router.CONFIG('envelope_size')};
+                ORDER BY g.event LIMIT {router.CONFIG('envelope_size')};
             ''').fetchall()
 
             if len(gists) < router.CONFIG('rest_when'): await sleep(router.CONFIG('idles'))
             await gather(*[notify(endpoint, loads(payload), passkey, gid) for endpoint, payload, passkey, gid in gists])
 
             db.commit()
         except Exception as exc:
             print('Exception occured: ', exc)
         finally:
-            cursor.close()
+            if cursor: cursor.close()
 
     await traverse()
```

### Comparing `amebo-0.1.2/PKG-INFO` & `amebo-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 Metadata-Version: 2.1
 Name: amebo
-Version: 0.1.2
+Version: 0.3.0
 Summary: HTTP Event Notifications Server - Asynchronous Communication Engine
 License: MIT
 Author: Tersoo
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastjsonschema (==2.19.1)
 Requires-Dist: httpx (==0.23.3)
 Requires-Dist: jinja2 (==3.1.2)
-Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: orjson (==3.8.9)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: pyjwt (==2.7.0)
 Requires-Dist: routerling (==0.5.1)
 Requires-Dist: uvicorn (==0.14.0)
 Description-Content-Type: text/markdown
 
 # AMEBO
 
 Amebo is the simplest pubsub server to use, deploy, understand or maintain. It was
 built to enable communication between applications i.e. microservices or
 modules (if you are using monoliths), and hopes to be able to serve as a small
 but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS.
 
-**STILL IN DEVELOPMENT: NOT READY FOR Production Use**
+1. Availability: Amebo runs on battle tested open source tools i.e. Redis, Postgres and provides the same level of availability guarantees
+
+1. Reliability: Amebo has been used at scale by open source projects to handle 100's of millions of request
+
+1. Latency: Amebo guarantees sub 100ms latencies at scale (barring network and hardware limitations)
+
 
 &nbsp;
 
 ## How It Works
 ---
 Amebo has only 4 concepts (first class objects) to understand or master.
 
 &nbsp;
 
-### 1. Microservices/Modules
+### 1. Applications
 ---
-These are applications or modules you register on amebo - they send and receive events ;-)
+These can be microservices or modules (in a monolith) - that create and receive notifications about [_**events**_](#2-events). All applications must be registered on
+    amebo ;-) before they can publish [_**events**_](#3-events).
 
 
-### 2. Events
+### 2. Action
 ---
-Something that can happen in an application, they are registered on Amebo by Microservices/Modules
+This is something that can happen in an [_**application**_](#1-applications) i.e. creating a customer, deleting an order. They are registered
+    on Amebo by their parent [_**application**_](#1-applications), and all actions must provide a valid JSON Schema (can be empty "{}") that Amebo
+    can use to validate action events before sending to [_**subscribers**_](#4-subscribers).
 
-### 3. Actions
+
+### 3. Events
 ---
-A HTTP request sent to Amebo to signal an event (action on event) has occured. Usually has a payload that
-    is forwarded by Amebo to all applications subscribed to the offending event
+An event is the occurence of an action and in practice is a HTTP request sent by an [_**application**_](#1-applications) to Amebo to signal it about the occurence of an action locally. Events can have a json payload that must match the JSON Schema of its parent action.
 
 ### 4. Subscribers
 ---
-HTTP endpoints registered to watch specific/particular events (by Microservices/Modules)
+These are HTTP URLs (can be valid hostname for loopback interface on TCP/IP as well) endpoints registered by [_**applications**_](#1-applications) to
+    receive [_**action**_](#3-actions) payloads.
 
 &nbsp;
 
 
 ## GETTING STARTED
 This assumes you have [installed](https://github.com/tersoo/amebo) Amebo on your machine. Amebo requires [Python3.6+](https://www.python.org/downloads)
 ```sh
@@ -115,52 +124,52 @@
 </td>
 </tr>
 </table>
 
 
 &nbsp;
 
-## 2nd : Register events that can happen in the registered microservices
+## 2nd : Register actions that can happen in the registered microservices
 ---
 
-`endpoint: /v1/events`
+`endpoint: /v1/actions`
 
 <table>
 <tr>
 <th>Endpoint JSON Schema</th>
 <th>Example Payload<th>
 </tr>
 <tr>
 <td>
 
 ```json
 {
     "type": "object",
     "properties": {
-        "event": {"type": "string"},
+        "action": {"type": "string"},
         "microservice": {"type": "string"},
         "schemata": {
             "type": "object",
             "properties": {
                 "type": {"type": "string"},
                 "properties": {"type": "object"},
                 "required": {"type": "array"}
             }
         }
     },
-    "required": ["event", "microservice", "schemata"]
+    "required": ["action", "microservice", "schemata"]
 }
 ```
 
 </td>
 <td>
 
 ```json
 {
-    "event": "customers.v1.created",
+    "action": "customers.v1.created",
     "microservice": "customers",
     "schemata": {
         "$id": "https://your-domain/customers/customer-created-schema-example.json",
         "$schema": "https://json-schema.org/draft/2020-12/schema",
         "type": "object",
         "properties": {
             "customer_id": {"type": "number"},
@@ -175,24 +184,24 @@
 
 </td>
 </tr>
 </table>
 
 &nbsp;
 
-## 3rd : Tell Amebo when an event occurs i.e. create an action
+## 3rd : Tell Amebo when an action occurs i.e. create an event
 ---
 
-`endpoint: /v1/actions`
+`endpoint: /v1/events`
 
 | Key | Description |
 |---|---|
-| **event** | Identifier name of the event. (As registered in the previous step.) |
-| **deduper** | Deduplication string. used to prevent the same action from being registered twice |
-| **payload** | JSON data (must confirm to the schema registerd with the event) |
+| **action** | Identifier name of the action. (As registered in the previous step.) |
+| **deduper** | Deduplication string. used to prevent the same event from being registered twice |
+| **payload** | JSON data (must confirm to the schema registerd with the action) |
 
 &nbsp;
 
 <table>
 <tr>
 <th>Endpoint JSON Schema</th>
 <th>Example Payload<th>
@@ -255,14 +264,18 @@
 1. Amebo comes complete with a Schema Registry, ensuring actions conform to event schema, and makes it easy for developers to search for events by
     microservice with commensurate schema (i.e. what is required, what is optional) as opposed to meetings with team mates continually.
 
 1. GUI for tracking events, actions, subscribers. Easy discovery of what events exist, what events failed and GUI retry for specific subscribers
 
 1. Gossiping is HTTP native i.e. subscribers receive http requests automatically at pre-registered endpoints
 
+1. Envelope format and transmission is web native and clearly outlined by schema registry
+
+1. Topic management is simplified as actions with versioning support baked in
+
 1. Infinite retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon)
 
 
 # Trivia
 
 The word `amebo` is a West African (Nigerian origin - but used in Ghana, Benin, Cameroon etc.) slang used to describe anyone that never keeps what you tell them to themselves. A talkative, never mind their business individual (a chronic gossip).
```

#### html2text {}

```diff
@@ -1,71 +1,82 @@
-Metadata-Version: 2.1 Name: amebo Version: 0.1.2 Summary: HTTP Event
+Metadata-Version: 2.1 Name: amebo Version: 0.3.0 Summary: HTTP Event
 Notifications Server - Asynchronous Communication Engine License: MIT Author:
 Tersoo Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
-(==0.23.3) Requires-Dist: jinja2 (==3.1.2) Requires-Dist: jsonschema (==4.17.3)
-Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==1.10.7) Requires-
-Dist: pyjwt (==2.7.0) Requires-Dist: routerling (==0.5.1) Requires-Dist:
-uvicorn (==0.14.0) Description-Content-Type: text/markdown # AMEBO Amebo is the
-simplest pubsub server to use, deploy, understand or maintain. It was built to
-enable communication between applications i.e. microservices or modules (if you
-are using monoliths), and hopes to be able to serve as a small but capable and
-simpler alternative to Kafka, RabbitMQ, SQS/SNS. **STILL IN DEVELOPMENT: NOT
-READY FOR Production Use**   ## How It Works --- Amebo has only 4 concepts
-(first class objects) to understand or master.   ### 1. Microservices/Modules -
--- These are applications or modules you register on amebo - they send and
-receive events ;-) ### 2. Events --- Something that can happen in an
-application, they are registered on Amebo by Microservices/Modules ### 3.
-Actions --- A HTTP request sent to Amebo to signal an event (action on event)
-has occured. Usually has a payload that is forwarded by Amebo to all
-applications subscribed to the offending event ### 4. Subscribers --- HTTP
-endpoints registered to watch specific/particular events (by Microservices/
-Modules)   ## GETTING STARTED This assumes you have [installed](https://
-github.com/tersoo/amebo) Amebo on your machine. Amebo requires [Python3.6+]
-(https://www.python.org/downloads) ```sh # the easy path pip install amebo
-amebo --workers 2 --address 0.0.0.0:8701 # the hardway (manual installation)
-BUT not the only way... Sorry, I couldn't resist the pun ;-) git clone https://
-github.com/tersoo/amebo mv amebo /to/a/directory/of/your/choosing export
-$PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo location to your
-path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo about all your
-microservices or applications --- `endpoint: /v1/microservices`
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
+fastjsonschema (==2.19.1) Requires-Dist: httpx (==0.23.3) Requires-Dist: jinja2
+(==3.1.2) Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pyjwt (==2.7.0) Requires-Dist: routerling (==0.5.1) Requires-
+Dist: uvicorn (==0.14.0) Description-Content-Type: text/markdown # AMEBO Amebo
+is the simplest pubsub server to use, deploy, understand or maintain. It was
+built to enable communication between applications i.e. microservices or
+modules (if you are using monoliths), and hopes to be able to serve as a small
+but capable and simpler alternative to Kafka, RabbitMQ, SQS/SNS. 1.
+Availability: Amebo runs on battle tested open source tools i.e. Redis,
+Postgres and provides the same level of availability guarantees 1. Reliability:
+Amebo has been used at scale by open source projects to handle 100's of
+millions of request 1. Latency: Amebo guarantees sub 100ms latencies at scale
+(barring network and hardware limitations)   ## How It Works --- Amebo has only
+4 concepts (first class objects) to understand or master.   ### 1. Applications
+--- These can be microservices or modules (in a monolith) - that create and
+receive notifications about [_**events**_](#2-events). All applications must be
+registered on amebo ;-) before they can publish [_**events**_](#3-events). ###
+2. Action --- This is something that can happen in an [_**application**_](#1-
+applications) i.e. creating a customer, deleting an order. They are registered
+on Amebo by their parent [_**application**_](#1-applications), and all actions
+must provide a valid JSON Schema (can be empty "{}") that Amebo can use to
+validate action events before sending to [_**subscribers**_](#4-subscribers).
+### 3. Events --- An event is the occurence of an action and in practice is a
+HTTP request sent by an [_**application**_](#1-applications) to Amebo to signal
+it about the occurence of an action locally. Events can have a json payload
+that must match the JSON Schema of its parent action. ### 4. Subscribers --
+- These are HTTP URLs (can be valid hostname for loopback interface on TCP/IP
+as well) endpoints registered by [_**applications**_](#1-applications) to
+receive [_**action**_](#3-actions) payloads.   ## GETTING STARTED This assumes
+you have [installed](https://github.com/tersoo/amebo) Amebo on your machine.
+Amebo requires [Python3.6+](https://www.python.org/downloads) ```sh # the easy
+path pip install amebo amebo --workers 2 --address 0.0.0.0:8701 # the hardway
+(manual installation) BUT not the only way... Sorry, I couldn't resist the pun
+;-) git clone https://github.com/tersoo/amebo mv amebo /to/a/directory/of/your/
+choosing export $PATH=$PATH:/to/a/directory/of/your/choosing/amebo # add amebo
+location to your path ambeo -w 2 -a 0.0.0.0:8701 ```   ## 1st : Tell Amebo
+about all your microservices or applications --- `endpoint: /v1/microservices`
 SScchheemmaa                                 EExxaammppllee PPaayyllooaadd
 ```json { "$schema": "", "type":
 "object", "properties":
 { "microservice": {"type": "string"},  ```json { "microservice": "customers",
 "passkey": {"type": "string",          "passkey": "some-super-duper-secret-of-
 "format": "ipv4 | ipv6 | hostname |    the-module-or-microservice",
 idn-hostname"}, "location": {"type":   "location": "http://0.0.0.0:3300" } ```
 "web"} }, "required": ["microservice",
 "passkey", "location"] } ```
-  ## 2nd : Register events that can happen in the registered microservices --
-- `endpoint: /v1/events`
-EEnnddppooiinntt JJSSOONN SScchheemmaa                  EExxaammppllee PPaayyllooaadd
-                                      ```json { "event":
-                                      "customers.v1.created", "microservice":
-```json { "type": "object",           "customers", "schemata": { "$id":
-"properties": { "event": {"type":     "https://your-domain/customers/
-"string"}, "microservice": {"type":   customer-created-schema-example.json",
-"string"}, "schemata": { "type":      "$schema": "https://json-schema.org/
-"object", "properties": { "type":     draft/2020-12/schema", "type":
-{"type": "string"}, "properties":     "object", "properties":
-{"type": "object"}, "required":       { "customer_id": {"type": "number"},
-{"type": "array"} } } }, "required":  "first_name": {"type": "string"},
-["event", "microservice", "schemata"] "last_name": {"type": "string"},
-} ```                                 "email": {"type": "string", "format":
-                                      "email"} }, "required": ["customer_id",
-                                      "email"] } } ```
-  ## 3rd : Tell Amebo when an event occurs i.e. create an action --- `endpoint:
-/v1/actions` | Key | Description | |---|---| | **event** | Identifier name of
-the event. (As registered in the previous step.) | | **deduper** |
-Deduplication string. used to prevent the same action from being registered
+  ## 2nd : Register actions that can happen in the registered microservices --
+- `endpoint: /v1/actions`
+EEnnddppooiinntt JJSSOONN SScchheemmaa                   EExxaammppllee PPaayyllooaadd
+                                       ```json { "action":
+                                       "customers.v1.created", "microservice":
+```json { "type": "object",            "customers", "schemata": { "$id":
+"properties": { "action": {"type":     "https://your-domain/customers/
+"string"}, "microservice": {"type":    customer-created-schema-example.json",
+"string"}, "schemata": { "type":       "$schema": "https://json-schema.org/
+"object", "properties": { "type":      draft/2020-12/schema", "type":
+{"type": "string"}, "properties":      "object", "properties":
+{"type": "object"}, "required":        { "customer_id": {"type": "number"},
+{"type": "array"} } } }, "required":   "first_name": {"type": "string"},
+["action", "microservice", "schemata"] "last_name": {"type": "string"},
+} ```                                  "email": {"type": "string", "format":
+                                       "email"} }, "required": ["customer_id",
+                                       "email"] } } ```
+  ## 3rd : Tell Amebo when an action occurs i.e. create an event --- `endpoint:
+/v1/events` | Key | Description | |---|---| | **action** | Identifier name of
+the action. (As registered in the previous step.) | | **deduper** |
+Deduplication string. used to prevent the same event from being registered
 twice | | **payload** | JSON data (must confirm to the schema registerd with
-the event) |  
+the action) |  
 EEnnddppooiinntt JJSSOONN SScchheemmaa                EExxaammppllee PPaayyllooaadd
                                     ```json { "event":
                                     "customers.v1.created", "microservice":
                                     "customers", "schema": { "$id": "https:
 ```json { "type": "object",         //your-domain/customers/customer-
 "properties": { "event": {"type":   created-schema-example.json",
 "string"}, "microservice": {"type": "$schema": "https://json-schema.org/
@@ -86,13 +97,15 @@
 Why? Advantages over traditional Message Oriented Middleware(s) 1. Amebo comes
 complete with a Schema Registry, ensuring actions conform to event schema, and
 makes it easy for developers to search for events by microservice with
 commensurate schema (i.e. what is required, what is optional) as opposed to
 meetings with team mates continually. 1. GUI for tracking events, actions,
 subscribers. Easy discovery of what events exist, what events failed and GUI
 retry for specific subscribers 1. Gossiping is HTTP native i.e. subscribers
-receive http requests automatically at pre-registered endpoints 1. Infinite
-retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon) # Trivia The
-word `amebo` is a West African (Nigerian origin - but used in Ghana, Benin,
-Cameroon etc.) slang used to describe anyone that never keeps what you tell
-them to themselves. A talkative, never mind their business individual (a
+receive http requests automatically at pre-registered endpoints 1. Envelope
+format and transmission is web native and clearly outlined by schema registry
+1. Topic management is simplified as actions with versioning support baked in
+1. Infinite retries (stop after $MAX_RETRIES and $MAX_MINUTES coming soon) #
+Trivia The word `amebo` is a West African (Nigerian origin - but used in Ghana,
+Benin, Cameroon etc.) slang used to describe anyone that never keeps what you
+tell them to themselves. A talkative, never mind their business individual (a
 chronic gossip).
```

