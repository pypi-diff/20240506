# Comparing `tmp/sniffs-0.5.3.tar.gz` & `tmp/sniffs-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffs-0.5.3.tar", max compression
+gzip compressed data, was "sniffs-0.5.4.tar", max compression
```

## Comparing `sniffs-0.5.3.tar` & `sniffs-0.5.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      387 2024-03-31 18:01:11.732434 sniffs-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3576 2024-03-31 18:01:03.739019 sniffs-0.5.3/README.md
--rw-r--r--   0        0        0       68 2024-03-31 16:51:16.392132 sniffs-0.5.3/sniffs/__init__.py
--rw-r--r--   0        0        0     4853 2024-03-31 17:47:46.367958 sniffs-0.5.3/sniffs/router.py
--rw-r--r--   0        0        0     1350 2024-03-31 18:00:59.072605 sniffs-0.5.3/sniffs/sniffs.py
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 sniffs-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-06 16:08:40.397256 sniffs-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-06 16:08:40.397256 sniffs-0.5.4/README.md
+-rw-r--r--   0        0        0      368 2024-05-06 16:58:06.987597 sniffs-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/__init__.py
+-rw-r--r--   0        0        0     4729 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/router.py
+-rw-r--r--   0        0        0     1306 2024-05-06 16:08:40.397256 sniffs-0.5.4/sniffs/sniffs.py
+-rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 sniffs-0.5.4/PKG-INFO
```

### Comparing `sniffs-0.5.3/README.md` & `sniffs-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,139 @@
-# Sniffs - Python MQTT Router
-
-Sniffs is a lightweight Python package for routing MQTT messages using flexible topic patterns. It provides an easy-to-use interface for defining routes and handling incoming messages efficiently.
-
-## Features
-
-- Define routes with dynamic topic patterns
-- Support for named and unnamed placeholders in topic patterns
-- Integration with MQTT clients for seamless message routing
-
-## Installation
-
-You can install Sniffs via pip:
-
-```bash
-pip install sniffs
-```
-
-## Usage
-
-```python
-import paho.mqtt.client as mqtt
-import ssl
-from sniffs import Sniffs
-
-app = Sniffs()
-
-@app.route("<key>:{option_1,option_2}/log")
-def incredibly_broad_route(key, topic, message):
-    print(f"key: {key}")
-    print(f"topic: {topic}")
-    print(f"message: {message}")
-
-client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="client123")
-client.username_pw_set("username", "password")
-client.tls_set(cert_reqs=ssl.CERT_NONE)
-client.connect(
-    host="host",
-    port=9937,
-)
-
-app.bind(client)
-
-client.loop_forever()
-```
-
-## Documentation
-
-### Named Placeholders
-
-Placeholders can be used in your routes. For example, `room` here is used as a placeholder
-and the argument name is injected into the function arguments:
-
-```python
-@app.route("<room>:{living_room,kitchen}/temperature")
-def receive_temperature_data(room):
-    if room == "living_room":
-        # do something
-    elif room == "kitchen":
-        # do something else
-```
-
-Argument injection works by looking up the name of the placeholder, so using a different
-name is the arguments will not work:
-
-```python
-# DOES NOT WORK, DO NOT DO THIS!!!
-@app.route("<room>:{living_room,kitchen}/temperature")
-def receive_temperature_data(argument_one):
-    ...
-```
-
-### Wildcard Placeholders
-
-If you want to match on anything, you can create a wildcard placeholder by not specifying any placeholder options.
-This example effectively matches on the topic of `+/temperature`:
-
-```python
-@app.route("<room>/temperature")
-def receive_temperature_data(room):
-    ...
-```
-
-You can use any number of named and wildcard placeholders together:
-
-```python
-@app.route("<room>/<sensor>:{sensor_1,sensor_2}/<sensor_type>{temperature,humidity}")
-def receive_temperature_data(room, sensor, sensor_type):
-    ...
-```
-
-### `topic` and `message`
-
-The `topic` and `message` arguments are injected, sort of like pytest fixtures. Do not use
-them as your keys in your routes, as they are reserved.
-
-`topic` - The topic on which the message was received. This will be the _actual_ topic name,
-not the templated route. For instance, a route for `<room>:{living_room,kitchen}/temperature` will
-always have a topic that is one of the following: `living_room/temperature`, `kitchen/temperature`.
-This maps to the `on_message` function from paho mqtt client, with the value of `msg.topic`.
-
-`message` - This maps to the `on_message` function, with the value of `msg.payload`.
-
-```python
-@app.route("<room>:{living_room,kitchen}/temperature")
-def receive_temperature_data(room, topic, message):
-    ...
-```
-
-The arguments are optional, they do not need to be included in your arguments:
-
-```python
-@app.route("<room>:{living_room,kitchen}/temperature")
-def receive_temperature_data(room):
-    ...
-```
-
-## Contributing
-
-Contributions are welcome! Please feel free to open issues or submit pull requests.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+Metadata-Version: 2.1
+Name: sniffs
+Version: 0.5.4
+Summary: 
+Author: surdouski
+Author-email: michael.surdouski@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
+Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Description-Content-Type: text/markdown
+
+# Sniffs - Python MQTT Router
+
+Sniffs is a lightweight Python package for routing MQTT messages using flexible topic patterns. It provides an easy-to-use interface for defining routes and handling incoming messages efficiently.
+
+## Features
+
+- Define routes with dynamic topic patterns
+- Support for named and unnamed placeholders in topic patterns
+- Integration with MQTT clients for seamless message routing
+
+## Installation
+
+You can install Sniffs via pip:
+
+```bash
+pip install sniffs
+```
+
+## Usage
+
+```python
+import paho.mqtt.client as mqtt
+import ssl
+from sniffs import Sniffs
+
+app = Sniffs()
+
+@app.route("<key>:{option_1,option_2}/log")
+def incredibly_broad_route(key, topic, message):
+    print(f"key: {key}")
+    print(f"topic: {topic}")
+    print(f"message: {message}")
+
+client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION2, client_id="client123")
+client.username_pw_set("username", "password")
+client.tls_set(cert_reqs=ssl.CERT_NONE)
+client.connect(
+    host="host",
+    port=9937,
+)
+
+app.bind(client)
+
+client.loop_forever()
+```
+
+## Documentation
+
+### Named Placeholders
+
+Placeholders can be used in your routes. For example, `room` here is used as a placeholder
+and the argument name is injected into the function arguments:
+
+```python
+@app.route("<room>:{living_room,kitchen}/temperature")
+def receive_temperature_data(room):
+    if room == "living_room":
+        # do something
+    elif room == "kitchen":
+        # do something else
+```
+
+Argument injection works by looking up the name of the placeholder, so using a different
+name is the arguments will not work:
+
+```python
+# DOES NOT WORK, DO NOT DO THIS!!!
+@app.route("<room>:{living_room,kitchen}/temperature")
+def receive_temperature_data(argument_one):
+    ...
+```
+
+### Wildcard Placeholders
+
+If you want to match on anything, you can create a wildcard placeholder by not specifying any placeholder options.
+This example effectively matches on the topic of `+/temperature`:
+
+```python
+@app.route("<room>/temperature")
+def receive_temperature_data(room):
+    ...
+```
+
+You can use any number of named and wildcard placeholders together:
+
+```python
+@app.route("<room>/<sensor>:{sensor_1,sensor_2}/<sensor_type>{temperature,humidity}")
+def receive_temperature_data(room, sensor, sensor_type):
+    ...
+```
+
+### `topic` and `message`
+
+The `topic` and `message` arguments are injected, sort of like pytest fixtures. Do not use
+them as your keys in your routes, as they are reserved.
+
+`topic` - The topic on which the message was received. This will be the _actual_ topic name,
+not the templated route. For instance, a route for `<room>:{living_room,kitchen}/temperature` will
+always have a topic that is one of the following: `living_room/temperature`, `kitchen/temperature`.
+This maps to the `on_message` function from paho mqtt client, with the value of `msg.topic`.
+
+`message` - This maps to the `on_message` function, with the value of `msg.payload`.
+
+```python
+@app.route("<room>:{living_room,kitchen}/temperature")
+def receive_temperature_data(room, topic, message):
+    ...
+```
+
+The arguments are optional, they do not need to be included in your arguments:
+
+```python
+@app.route("<room>:{living_room,kitchen}/temperature")
+def receive_temperature_data(room):
+    ...
+```
+
+## Contributing
+
+Contributions are welcome! Please feel free to open issues or submit pull requests.
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+
```

### Comparing `sniffs-0.5.3/sniffs/router.py` & `sniffs-0.5.4/sniffs/router.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import re
-from typing import Callable
-import inspect
-import itertools
-
-LHS_VARIABLE_TOKEN = "<"
-RHS_VARIABLE_TOKEN = ">"
-VARIABLE_OPTIONS_DELIMITER = ":"
-LHS_OPTIONS_TOKEN = "{"
-RHS_OPTIONS_TOKEN = "}"
-OPTIONS_DELIMITER = ","
-
-
-class Router:
-    def __init__(self):
-        self.routes = []
-
-    def add_route(self, topic_pattern: str, handler: Callable):
-        """
-        Add a route to the router.
-
-        Args:
-            topic_pattern (str): MQTT topic pattern to match.
-            handler (Callable): Handler function to be called when a message is received on the matched topic.
-        """
-        # Parse the topic pattern to automatically add named capture groups
-        pattern = self._parse_topic_pattern(topic_pattern)
-        self.routes.append(
-            {
-                "topic_pattern": pattern,
-                "handler": handler,
-                "unparsed_pattern": topic_pattern,
-            }
-        )
-
-    def route(self, topic: str, message: str):
-        """
-        Route a received message to the appropriate handler based on the topic.
-
-        Args:
-            topic (str): MQTT topic of the received message.
-            message (str): Payload of the received message.
-        """
-        results = []
-        for route in self.routes:
-            match = route["topic_pattern"].match(topic)
-            if match:
-                _func = route["handler"]
-                _signature = inspect.signature(_func)
-                _parameter_names = list(_signature.parameters)
-                _all_available_kwargs = {
-                    **match.groupdict(),
-                    **{"topic": topic, "message": message},
-                }
-                kwargs_to_pass = {
-                    arg: value
-                    for arg, value in _all_available_kwargs.items()
-                    if arg in _parameter_names
-                }  # Get only keyword arguments that exist in the function signature
-
-                results.append(_func(**kwargs_to_pass))
-        return tuple(results) if len(results) else tuple()
-
-    def _parse_topic_pattern(self, topic_pattern: str) -> re.Pattern:
-        """
-        Parse MQTT topic pattern and add named capture groups automatically.
-
-        Args:
-            topic_pattern (str): MQTT topic pattern.
-
-        Returns:
-            re.Pattern: Compiled regular expression pattern.
-        """
-        pattern_parts = []
-        for part in topic_pattern.split("/"):
-            # going to do some hand-wavy stuff for now, can validate things better later
-            if LHS_OPTIONS_TOKEN in part and RHS_OPTIONS_TOKEN in part:
-                variable_string, options_string = part.split(VARIABLE_OPTIONS_DELIMITER)
-                variable = variable_string[1:-1]
-                options_string = options_string[1:-1]
-                options = options_string.split(OPTIONS_DELIMITER)
-                options = [option for option in options if option]
-                part = f"(?P<{re.escape(variable)}>{'|'.join(map(re.escape, options))})"
-            elif part.startswith(LHS_VARIABLE_TOKEN) and part.endswith(
-                RHS_VARIABLE_TOKEN
-            ):
-                variable = part[1:-1]
-                part = f"(?P<{re.escape(variable)}>[^/]+)"
-            pattern_parts.append(part)
-        pattern = "/".join(pattern_parts)
-        return re.compile(pattern)
-
-    def get_topic_paths(self):
-        return self._generate_subscription_topic_paths(
-            [route["unparsed_pattern"] for route in self.routes]
-        )
-
-    def _generate_subscription_topic_paths(self, topic_patterns):
-        generated_subscription_topics = []
-
-        for path in topic_patterns:
-            parts = path.split("/")
-            variables = []
-            for part in parts:
-                if "<" in part and ">" in part:
-                    var_name = part.replace("<", "").replace(">", "")
-                    var_options = var_name.split(":")
-                    if len(var_options) > 1:
-                        path = path.replace(part, var_options[0])
-                        variables.append(
-                            (var_options[0], var_options[1].strip("{}").split(","))
-                        )
-                    else:
-                        path = path.replace(part, var_name)
-                        variables.append((var_name, ["+"]))
-
-            combinations = itertools.product(*[options for _, options in variables])
-            for combo in combinations:
-                topic = path
-                for (var_name, _), val in zip(variables, combo):
-                    topic = topic.replace(f"{var_name}", val)
-                generated_subscription_topics.append(topic)
-
-        return generated_subscription_topics
+import re
+from typing import Callable
+import inspect
+import itertools
+
+LHS_VARIABLE_TOKEN = "<"
+RHS_VARIABLE_TOKEN = ">"
+VARIABLE_OPTIONS_DELIMITER = ":"
+LHS_OPTIONS_TOKEN = "{"
+RHS_OPTIONS_TOKEN = "}"
+OPTIONS_DELIMITER = ","
+
+
+class Router:
+    def __init__(self):
+        self.routes = []
+
+    def add_route(self, topic_pattern: str, handler: Callable):
+        """
+        Add a route to the router.
+
+        Args:
+            topic_pattern (str): MQTT topic pattern to match.
+            handler (Callable): Handler function to be called when a message is received on the matched topic.
+        """
+        # Parse the topic pattern to automatically add named capture groups
+        pattern = self._parse_topic_pattern(topic_pattern)
+        self.routes.append(
+            {
+                "topic_pattern": pattern,
+                "handler": handler,
+                "unparsed_pattern": topic_pattern,
+            }
+        )
+
+    def route(self, topic: str, message: str):
+        """
+        Route a received message to the appropriate handler based on the topic.
+
+        Args:
+            topic (str): MQTT topic of the received message.
+            message (str): Payload of the received message.
+        """
+        results = []
+        for route in self.routes:
+            match = route["topic_pattern"].match(topic)
+            if match:
+                _func = route["handler"]
+                _signature = inspect.signature(_func)
+                _parameter_names = list(_signature.parameters)
+                _all_available_kwargs = {
+                    **match.groupdict(),
+                    **{"topic": topic, "message": message},
+                }
+                kwargs_to_pass = {
+                    arg: value
+                    for arg, value in _all_available_kwargs.items()
+                    if arg in _parameter_names
+                }  # Get only keyword arguments that exist in the function signature
+
+                results.append(_func(**kwargs_to_pass))
+        return tuple(results) if len(results) else tuple()
+
+    def _parse_topic_pattern(self, topic_pattern: str) -> re.Pattern:
+        """
+        Parse MQTT topic pattern and add named capture groups automatically.
+
+        Args:
+            topic_pattern (str): MQTT topic pattern.
+
+        Returns:
+            re.Pattern: Compiled regular expression pattern.
+        """
+        pattern_parts = []
+        for part in topic_pattern.split("/"):
+            # going to do some hand-wavy stuff for now, can validate things better later
+            if LHS_OPTIONS_TOKEN in part and RHS_OPTIONS_TOKEN in part:
+                variable_string, options_string = part.split(VARIABLE_OPTIONS_DELIMITER)
+                variable = variable_string[1:-1]
+                options_string = options_string[1:-1]
+                options = options_string.split(OPTIONS_DELIMITER)
+                options = [option for option in options if option]
+                part = f"(?P<{re.escape(variable)}>{'|'.join(map(re.escape, options))})"
+            elif part.startswith(LHS_VARIABLE_TOKEN) and part.endswith(
+                RHS_VARIABLE_TOKEN
+            ):
+                variable = part[1:-1]
+                part = f"(?P<{re.escape(variable)}>[^/]+)"
+            pattern_parts.append(part)
+        pattern = "/".join(pattern_parts)
+        return re.compile(pattern)
+
+    def get_topic_paths(self):
+        return self._generate_subscription_topic_paths(
+            [route["unparsed_pattern"] for route in self.routes]
+        )
+
+    def _generate_subscription_topic_paths(self, topic_patterns):
+        generated_subscription_topics = []
+
+        for path in topic_patterns:
+            parts = path.split("/")
+            variables = []
+            for part in parts:
+                if "<" in part and ">" in part:
+                    var_name = part.replace("<", "").replace(">", "")
+                    var_options = var_name.split(":")
+                    if len(var_options) > 1:
+                        path = path.replace(part, var_options[0])
+                        variables.append(
+                            (var_options[0], var_options[1].strip("{}").split(","))
+                        )
+                    else:
+                        path = path.replace(part, var_name)
+                        variables.append((var_name, ["+"]))
+
+            combinations = itertools.product(*[options for _, options in variables])
+            for combo in combinations:
+                topic = path
+                for (var_name, _), val in zip(variables, combo):
+                    topic = topic.replace(f"{var_name}", val)
+                generated_subscription_topics.append(topic)
+
+        return generated_subscription_topics
```

### Comparing `sniffs-0.5.3/sniffs/sniffs.py` & `sniffs-0.5.4/sniffs/sniffs.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import functools
-from typing import Any, Callable
-import paho.mqtt.client as mqtt
-from sniffs.router import Router
-
-
-class Sniffs:
-    """A dynamic wrapper for the paho mqtt client."""
-
-    client: mqtt.Client
-    router: Router
-
-    def __init__(self, *args, **kwargs):
-        self.router = Router()
-
-    def bind(self, client: mqtt.Client):
-        self.client = client
-        self.client.on_connect = self._on_connect
-        self.client.on_message = self._on_message
-
-    def route(self, topic_pattern: str) -> Callable:
-        def decorator(func):
-            @functools.wraps(func)
-            def wrapper(*args, **kwargs):
-                return func(*args, **kwargs)
-
-            self.router.add_route(topic_pattern, func)
-            return wrapper
-
-        return decorator
-
-    def _on_connect(self, client, userdata, flags, reason_code, properties):
-        if reason_code.is_failure:
-            print(
-                f"Failed to connect: {reason_code}. loop_forever() will retry connection"
-            )
-        else:
-            paths = self.router.get_topic_paths()
-            for path in paths:
-                print(f"Subscribing to {path}")
-                client.subscribe(path)
-
-    def _on_message(self, client, userdata, msg):
-        self.router.route(msg.topic, msg.payload)
+import functools
+from typing import Any, Callable
+import paho.mqtt.client as mqtt
+from sniffs.router import Router
+
+
+class Sniffs:
+    """A dynamic wrapper for the paho mqtt client."""
+
+    client: mqtt.Client
+    router: Router
+
+    def __init__(self, *args, **kwargs):
+        self.router = Router()
+
+    def bind(self, client: mqtt.Client):
+        self.client = client
+        self.client.on_connect = self._on_connect
+        self.client.on_message = self._on_message
+
+    def route(self, topic_pattern: str) -> Callable:
+        def decorator(func):
+            @functools.wraps(func)
+            def wrapper(*args, **kwargs):
+                return func(*args, **kwargs)
+
+            self.router.add_route(topic_pattern, func)
+            return wrapper
+
+        return decorator
+
+    def _on_connect(self, client, userdata, flags, reason_code, properties):
+        if reason_code.is_failure:
+            print(
+                f"Failed to connect: {reason_code}. loop_forever() will retry connection"
+            )
+        else:
+            paths = self.router.get_topic_paths()
+            for path in paths:
+                print(f"Subscribing to {path}")
+                client.subscribe(path)
+
+    def _on_message(self, client, userdata, msg):
+        self.router.route(msg.topic, msg.payload)
```

### Comparing `sniffs-0.5.3/PKG-INFO` & `sniffs-0.5.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sniffs
-Version: 0.5.3
-Summary: 
-Author: surdouski
-Author-email: michael.surdouski@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: paho-mqtt (>=2.0.0,<3.0.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
-Description-Content-Type: text/markdown
-
 # Sniffs - Python MQTT Router
 
 Sniffs is a lightweight Python package for routing MQTT messages using flexible topic patterns. It provides an easy-to-use interface for defining routes and handling incoming messages efficiently.
 
 ## Features
 
 - Define routes with dynamic topic patterns
@@ -132,8 +118,7 @@
 ## Contributing
 
 Contributions are welcome! Please feel free to open issues or submit pull requests.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
```

