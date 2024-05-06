# Comparing `tmp/msmanager-0.4.5.tar.gz` & `tmp/msmanager-0.4.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.4.5.tar", max compression
+gzip compressed data, was "msmanager-0.4.6.dev1.tar", max compression
```

## Comparing `msmanager-0.4.5.tar` & `msmanager-0.4.6.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.5/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.5/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.5/msmanager/__main__.py
--rw-r--r--   0        0        0    14376 2024-05-06 09:17:09.030180 msmanager-0.4.5/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.5/msmanager/config.py
--rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.5/msmanager/exceptions.py
--rw-r--r--   0        0        0     4201 2024-05-06 07:59:01.377630 msmanager-0.4.5/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-01-03 17:46:28.276066 msmanager-0.4.5/msmanager/models.py
--rw-r--r--   0        0        0     3232 2024-05-06 08:20:08.039284 msmanager-0.4.5/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.5/msmanager/types.py
--rw-r--r--   0        0        0      596 2024-05-06 09:17:58.608441 msmanager-0.4.5/msmanager/units.py
--rw-r--r--   0        0        0      662 2024-05-06 09:18:02.107390 msmanager-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      849 2024-01-03 18:16:46.197804 msmanager-0.4.5/README.md
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 msmanager-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.6.dev1/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.6.dev1/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.6.dev1/msmanager/__main__.py
+-rw-r--r--   0        0        0    15407 2024-05-06 13:26:25.644413 msmanager-0.4.6.dev1/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.6.dev1/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.6.dev1/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4190 2024-05-06 13:11:57.556601 msmanager-0.4.6.dev1/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-05-06 12:56:09.812783 msmanager-0.4.6.dev1/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-06 12:57:54.532626 msmanager-0.4.6.dev1/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.6.dev1/msmanager/types.py
+-rw-r--r--   0        0        0      601 2024-05-06 13:23:54.511899 msmanager-0.4.6.dev1/msmanager/units.py
+-rw-r--r--   0        0        0      667 2024-05-06 13:24:03.427458 msmanager-0.4.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0      928 2024-05-06 09:35:49.035878 msmanager-0.4.6.dev1/README.md
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 msmanager-0.4.6.dev1/PKG-INFO
```

### Comparing `msmanager-0.4.5/LICENSE` & `msmanager-0.4.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.5/msmanager/cli.py` & `msmanager-0.4.6.dev1/msmanager/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 )
 from .exceptions import (
     VBMLParseError, IncorrectConnectionDataError
 )
 
 # ! Vars
 console = Console()
-debag_mode = False
+debug_mode = False
 msmanager: MSManager = ...
 oformat: Literal['text', 'json'] = 'text'
 
 # ! Functions
 def printexcept(e: Exception):
-    if debag_mode:
+    if debug_mode:
         console.print_exception(word_wrap=True, show_locals=True)
     else:
         console.print(rich_exception(e))
 
 def hand_exception():
     def hand_exception_wrapper(func: Callable[..., Any]):
         def hand_exception_wrapped(*args, **kwargs):
@@ -309,16 +309,26 @@
     default=False, is_flag=True
 )
 @click.option(
     "--start-delay", "-d", "start_delay",
     help="The delay before watchdog starts (in secounds).",
     type=click.INT, default=120, show_default=True
 )
+@click.option(
+    "--check-timeout", "-ct", "-t", "check_timeout",
+    help="The delay between process checks (in secounds).",
+    type=click.INT, default=1, show_default=True
+)
+@click.option(
+    "--checks", "-c", "checks",
+    help="How many times to check one server.",
+    type=click.INT, default=3, show_default=True
+)
 @hand_exception()
-def watchdog(scn: str, localhost: bool, start_delay: int):
+def watchdog(scn: str, localhost: bool, start_delay: int, check_timeout: int, checks: int):
     screens_names = scn.split(",")
     servers_config: List[MindustryServerConfig] = []
     for screen_name in screens_names:
         if (server_config := msmanager.get_server_config(screen_name)) is not None:
             if (server_config.host is not None) or (server_config.port is not None):
                 servers_config.append(server_config)
                 console.print(f"[green]>[/green] The server was found in the config: {repr(screen_name)}")
@@ -328,20 +338,31 @@
             console.print(f"[red]>[/red] One of the listed servers was not found: {repr(screen_name)}")
     console.print(f"[green]>[/green] Waiting {start_delay} second(s) before starting the watchdog operation.")
     time.sleep(start_delay)
     console.print("[green]>[/green] Watchdog is started!")
     try:
         while True:
             for server_config in servers_config:
-                server_host = "localhost" if localhost else server_config.host
-                if not pingok(server_host, server_config.port):
+                oks, server_host = 0, "localhost" if localhost else server_config.host
+                if debug_mode:
+                    console.print(f"[yellow]>[/yellow] Checking: {repr(server_config.screen_name)}")
+                for _ in range(checks):
+                    if pingok(server_host, server_config.port):
+                        oks += 1
+                        if debug_mode:
+                            console.print(f"[yellow]>[/yellow] Checked: [green]ON[/green]")
+                    else:
+                        if debug_mode:
+                            console.print(f"[yellow]>[/yellow] Checked: [red]OFF[/red]")
+                    time.sleep(check_timeout)
+                if oks == 0:
                     console.print(f"[red]>[/red] Restarting server: {repr(server_config.screen_name)}")
                     msmanager.restart_server(server_config.screen_name)
                     wait_start_server(server_config.host, server_config.port, server_config.input_port)
-            time.sleep(0.1)
+                    console.print(f"[green]>[/green] Restarted server: {repr(server_config.screen_name)}")
     except KeyboardInterrupt:
         pass
     console.print("[green]>[/green] Watchdog is shutdown!")
 
 # ! Main Group
 @click.group()
 @click.option(
```

### Comparing `msmanager-0.4.5/msmanager/config.py` & `msmanager-0.4.6.dev1/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.5/msmanager/exceptions.py` & `msmanager-0.4.6.dev1/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.5/msmanager/functions.py` & `msmanager-0.4.6.dev1/msmanager/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         isinstance(server_host, str) and \
         isinstance(port, int) and \
         (isinstance(input_port, int) or (input_port is not None))
 
 def ping(host: str, port: int, timeout: int=10) -> pydustry.Status:
     return pydustry.Server(host, port).get_status(timeout)
 
-def pingok(host: str, port: int, timeout: int=10) -> pydustry.Status:
+def pingok(host: str, port: int, timeout: int=10) -> bool:
     try:
         pydustry.Server(host, port).get_status(timeout)
         return True
     except:
         pass
     return False
```

### Comparing `msmanager-0.4.5/msmanager/models.py` & `msmanager-0.4.6.dev1/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.5/msmanager/msm.py` & `msmanager-0.4.6.dev1/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.5/msmanager/units.py` & `msmanager-0.4.6.dev1/msmanager/units.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __prog_name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.4.5"
+__version__ = "0.4.6.dev1"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.4.5/pyproject.toml` & `msmanager-0.4.6.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.4.5"
+version = "0.4.6.dev1"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.4.5/README.md` & `msmanager-0.4.6.dev1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,16 @@
                             support.
   -d, --debug               Enables debug mode of operation.
   -f, --format [text|json]  The output format.  [default: text]
   --version                 Show the version and exit.
   --help                    Show this message and exit.
 
 Commands:
-  add      Add a server to the config.
-  list     List of servers in the config.
-  ping     Server status check.
-  remove   Remove the server from the config.
-  restart  Restart the server(s).
-  start    Run the server(s).
-  stop     Stop the server(s).
+  add       Add a server to the config.
+  list      List of servers in the config.
+  ping      Server status check.
+  remove    Remove the server from the config.
+  restart   Restart the server(s).
+  start     Run the server(s).
+  stop      Stop the server(s).
+  watchdog  The active process of monitoring servers, which, if the...
 ```
```

### Comparing `msmanager-0.4.5/PKG-INFO` & `msmanager-0.4.6.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.4.5
+Version: 0.4.6.dev1
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -41,16 +41,17 @@
                             support.
   -d, --debug               Enables debug mode of operation.
   -f, --format [text|json]  The output format.  [default: text]
   --version                 Show the version and exit.
   --help                    Show this message and exit.
 
 Commands:
-  add      Add a server to the config.
-  list     List of servers in the config.
-  ping     Server status check.
-  remove   Remove the server from the config.
-  restart  Restart the server(s).
-  start    Run the server(s).
-  stop     Stop the server(s).
+  add       Add a server to the config.
+  list      List of servers in the config.
+  ping      Server status check.
+  remove    Remove the server from the config.
+  restart   Restart the server(s).
+  start     Run the server(s).
+  stop      Stop the server(s).
+  watchdog  The active process of monitoring servers, which, if the...
 ```
```

