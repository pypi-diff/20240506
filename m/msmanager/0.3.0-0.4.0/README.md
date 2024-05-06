# Comparing `tmp/msmanager-0.3.0.tar.gz` & `tmp/msmanager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.3.0.tar", max compression
+gzip compressed data, was "msmanager-0.4.0.tar", max compression
```

## Comparing `msmanager-0.3.0.tar` & `msmanager-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.3.0/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.3.0/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.3.0/msmanager/__main__.py
--rw-r--r--   0        0        0    12134 2024-01-03 18:08:39.852830 msmanager-0.3.0/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.3.0/msmanager/config.py
--rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.3.0/msmanager/exceptions.py
--rw-r--r--   0        0        0     3995 2023-06-27 12:16:45.380300 msmanager-0.3.0/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.3.0/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-10-06 21:55:35.299739 msmanager-0.3.0/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.3.0/msmanager/types.py
--rw-r--r--   0        0        0      596 2024-01-03 18:08:06.815040 msmanager-0.3.0/msmanager/units.py
--rw-r--r--   0        0        0      662 2024-01-03 18:15:34.882517 msmanager-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.3.0/README.md
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.0/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.0/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.0/msmanager/__main__.py
+-rw-r--r--   0        0        0    14071 2024-05-06 08:40:44.831088 msmanager-0.4.0/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.0/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.0/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.0/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.0/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.0/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.0/msmanager/types.py
+-rw-r--r--   0        0        0      596 2024-05-06 08:27:49.866154 msmanager-0.4.0/msmanager/units.py
+-rw-r--r--   0        0        0      662 2024-05-06 08:27:54.189427 msmanager-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.0/README.md
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.0/PKG-INFO
```

### Comparing `msmanager-0.3.0/LICENSE` & `msmanager-0.4.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 RCR - Organization Of Programmers
+Copyright (c) 2023 RCR
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `msmanager-0.3.0/msmanager/cli.py` & `msmanager-0.4.0/msmanager/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
+import time
 import json
 import click
 from rich.console import Console
-from typing import Literal, Optional, Union, Iterable, Callable, Dict, Any
+from typing import Literal, Optional, Union, Iterable, Callable, List, Dict, Any
 # > Local Imports
 from .msm import MSManager
 from .units import (
     __title__ as prog_name,
     __version__ as prog_version
 )
 from .models import (
     MindustryServerConfig,
     JsonOutput
 )
 from .functions import (
     rich_exception,
     is_server_connect_correct,
     wait_start_server,
-    ping, endicext, parse_connect_data
+    ping, pingok, endicext, parse_connect_data
 )
 from .exceptions import (
     VBMLParseError, IncorrectConnectionDataError
 )
 
 # ! Vars
 console = Console()
@@ -135,15 +136,15 @@
     is_flag=True
 )
 @hand_exception()
 def starter(scn: str, wait: bool):
     screens_names = scn.split(",")
     for screen_name in screens_names:
         msmanager.start_server(screen_name)
-        if (server_config:=msmanager.get_server_config(screen_name)) is not None:
+        if (server_config := msmanager.get_server_config(screen_name)) is not None:
             if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
                 wait_start_server(server_config.host, server_config.port, server_config.input_port)
         if oformat == 'text':
             console.print(f"[green]>[/green] Server [green]{screen_name}[/green] is [bold yellow]started[/bold yellow]!")
     if oformat == 'json':
         printjson(JsonOutput(status='success'))
 
@@ -156,14 +157,15 @@
     for screen_name in screens_names:
         msmanager.stop_server(screen_name)
         if oformat == 'text':
             console.print(f"[green]>[/green] Server [green]{screen_name}[/green] is [bold yellow]stoped[/bold yellow]!")
     if oformat == 'json':
         printjson(JsonOutput(status='success'))
 
+# ? Restart Command
 @click.command("restart", help="Restart the server(s).")
 @click.argument("scn", type=str)
 @click.option(
     "-w", "--wait", "wait",
     help="Waiting for the server to start up.",
     is_flag=True
 )
@@ -234,14 +236,15 @@
                 )
     else:
         if oformat == 'text':
             console.print("[green]>[/] The list of servers is [bold yellow]empty[/]!")
     if oformat == 'json':
         printjson(output)
 
+# ? Ping Command
 @click.command("ping", help="Server status check.")
 @click.argument("connect", type=str)
 @click.option(
     "-t", "--timeout", "timeout",
     help="Maximum response waiting time (in seconds).",
     type=int, default=10, show_default=True
 )
@@ -293,14 +296,52 @@
                     "ping": status.ping,
                     "version": status.version,
                     "vertype": status.vertype
                 }
             )
         )
 
+# ? Watchdog
+@click.command("watchdog", help="The active process of monitoring servers, which, if the server fails, restarts it.")
+@click.argument("scn", type=str)
+@click.option(
+    "--localhost", "-l", "localhost", 
+    help="The ping will take place not by the host settings, but by the local IP.",
+    defalut=False, is_flag=True
+)
+@click.option(
+    "--start-delay", "-d", "start_delay",
+    help="The delay before watchdog starts (in secounds).",
+    type=click.IntRange, default=120, show_default=True
+)
+@hand_exception()
+def watchdog(scn: str, localhost: bool, start_delay: int):
+    screens_names = scn.split(",")
+    servers_config: List[MindustryServerConfig] = []
+    for screen_name in screens_names:
+        if (server_config := msmanager.get_server_config(screen_name)) is not None:
+            if (server_config.host is not None) or (server_config.port is not None):
+                servers_config.append(server_config)
+                console.print(f"[green]>[/green] The server was found in the config: {repr(screen_name)}")
+            else:
+                console.print(f"[red]>[/red] There are no settings for ping: {repr(screen_name)}")
+        else:
+            console.print(f"[red]>[/red] One of the listed servers was not found: {repr(screen_name)}")
+    console.print(f"[green]>[/green] Waiting {start_delay} second(s) before starting the watchdog operation.")
+    time.sleep(start_delay)
+    console.print("[green]>[/green] Watchdog is started!")
+    try:
+        while True:
+            for server_config in servers_config:
+                if not pingok("localhost" if localhost else server_config.host, server_config.port):
+                    msmanager.restart_server(server_config.screen_name)
+    except KeyboardInterrupt:
+        pass
+    console.print("[green]>[/green] Watchdog is shutdown!")
+
 # ! Main Group
 @click.group()
 @click.option(
     "--check-environment", "check_environment",
     help="Enables checks for GNU Screen, Java and system support.",
     is_flag=True, default=False
 )
```

### Comparing `msmanager-0.3.0/msmanager/config.py` & `msmanager-0.4.0/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.3.0/msmanager/exceptions.py` & `msmanager-0.4.0/msmanager/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,57 +19,63 @@
             """The screen command returns an error when checked, check that the 'GNU Screen' program is working. \nIf the software is not available, the following program must be installed: https://www.gnu.org/software/screen""",
         )
 
 class JavaNotFound(Exception):
     """Indicates a lack of `Java`."""
     def __init__(self) -> None:
         """Called if the `Java` package environment could not be found."""
-        self.args = ("The `Java` environment package is not installed.",)
+        self.args = (
+            "The `Java` environment package is not installed.",
+        )
 
 # ! Parsing Error
 class VBMLParseError(Exception):
     """Indicates a parsing error."""
     def __init__(self) -> None:
         """Calls if `vbml` was unable to finish parsing."""
-        self.args = ("There was an error parsing through vbml.",)
+        self.args = (
+            "There was an error parsing through vbml.",
+        )
 
 
 # ! Config Exceptions
 class ServerExistsError(Exception):
     """Indicates that there is a server with this name."""
     def __init__(self, name: str) -> None:
         """Called if a server with this name is already present in the config."""
-        self.args = (f"A server named {repr(name)} already exists in the config.",)
+        self.args = (
+            f"A server named {repr(name)} already exists in the config.",
+        )
 
 class ServerNotExistsError(Exception):
     """Indicates that north does not exist in the config."""
     def __init__(self, name: str) -> None:
         """Called if a server with this name does not exist in the config."""
         self.args = (
-            f"A server named {repr(name)} does not exist in the config."
+            f"A server named {repr(name)} does not exist in the config.",
         )
 
 # ! Server Actions Exceptions
 class ServerIsStartedError(Exception):
     """Indicates that the server is already running."""
     def __init__(self, name: str) -> None:
         """Called when attempting to start an already running server."""
         self.args = (
-            f"A server named {repr(name)} is already up and running."
+            f"A server named {repr(name)} is already up and running.",
         )
 
 class ServerIsStoppedError(Exception):
     """Indicates that the server is already stopped."""
     def __init__(self, name: str) -> None:
         """Called if the server is already stopped."""
         self.args = (
-            f"The {repr(name)} server is stopped as it is."
+            f"The {repr(name)} server is stopped as it is.",
         )
 
 # ! CLI Exception
 class IncorrectConnectionDataError(Exception):
     """Indicates incorrect data to connect to the server."""
     def __init__(self, connect_data: str) -> None:
         """Called if the connection data is incorrect."""
         self.args = (
-            f"The data to connect to the server is not correct ({connect_data})."
+            f"The data to connect to the server is not correct ({connect_data}).",
         )
```

### Comparing `msmanager-0.3.0/msmanager/functions.py` & `msmanager-0.4.0/msmanager/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         isinstance(server_host, str) and \
         isinstance(port, int) and \
         (isinstance(input_port, int) or (input_port is not None))
 
 def ping(host: str, port: int, timeout: int=10) -> pydustry.Status:
     return pydustry.Server(host, port).get_status(timeout)
 
+def pingok(host: str, port: int, timeout: int=10) -> pydustry.Status:
+    try:
+        pydustry.Server(host, port).get_status(timeout)
+        return True
+    except:
+        pass
+    return False
+
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
 
 def exists_screen() -> bool:
     out = runner("screen", "-v")[0]
     return (out == 0) or (out == 1)
```

### Comparing `msmanager-0.3.0/msmanager/models.py` & `msmanager-0.4.0/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.3.0/msmanager/msm.py` & `msmanager-0.4.0/msmanager/msm.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,18 +20,25 @@
         self.config = MSManagerConfig(self.config_path)
         
         # * Test System
         if check_environment:
             checking_environment()
     
     # ? Config Managemant
-    def add_server_config(self, server: MindustryServerConfig) -> None: return self.config.add_server(server)
-    def get_server_config(self, screen_name: str) -> Optional[MindustryServerConfig]: return self.config.get_server(screen_name)
-    def exists_server_config(self, screen_name: str) -> bool: return self.config.exists_server(screen_name)
-    def remove_server_config(self, screen_name: str) -> None: return self.config.remove_server(screen_name)
+    def add_server_config(self, server: MindustryServerConfig) -> None:
+        return self.config.add_server(server)
+    
+    def get_server_config(self, screen_name: str) -> Optional[MindustryServerConfig]:
+        return self.config.get_server(screen_name)
+    
+    def exists_server_config(self, screen_name: str) -> bool:
+        return self.config.exists_server(screen_name)
+    
+    def remove_server_config(self, screen_name: str) -> None:
+        return self.config.remove_server(screen_name)
     
     # ? Server Managemant
     def check_server_version(self, screen_name: str) -> Version:
         if (server_config:=self.get_server_config(screen_name)) is not None:
             return get_mindustry_server_version(server_config.executable_filepath)
         raise ServerNotExistsError(screen_name)
     
@@ -58,7 +65,14 @@
             server_screen = screens.get_session_by_name(screen_name)
             if server_screen is not None:
                 server_screen.kill()
             else:
                 raise ServerIsStoppedError(screen_name)
         else:
             raise ServerNotExistsError(screen_name)
+    
+    def restart_server(self, screen_name: str) -> None:
+        try:
+            self.stop_server(screen_name)
+        except:
+            pass
+        self.start_server(screen_name)
```

### Comparing `msmanager-0.3.0/msmanager/units.py` & `msmanager-0.4.0/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __prog_name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.3.0/pyproject.toml` & `msmanager-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.3.0"
+version = "0.4.0"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.3.0/README.md` & `msmanager-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.3.0/PKG-INFO` & `msmanager-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.3.0
+Version: 0.4.0
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

