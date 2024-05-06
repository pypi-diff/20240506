# Comparing `tmp/mpflash-0.7.4.tar.gz` & `tmp/mpflash-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.7.4.tar", max compression
+gzip compressed data, was "mpflash-0.7.5.tar", max compression
```

## Comparing `mpflash-0.7.4.tar` & `mpflash-0.7.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.4/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.4/mpflash/__init__.py
--rw-r--r--   0        0        0     8442 2024-05-02 20:53:12.953952 mpflash-0.7.4/mpflash/ask_input.py
--rw-r--r--   0        0        0     3266 2024-05-02 20:53:12.958850 mpflash-0.7.4/mpflash/cli_download.py
--rw-r--r--   0        0        0     5847 2024-05-02 20:53:12.961542 mpflash-0.7.4/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.4/mpflash/cli_group.py
--rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.4/mpflash/cli_list.py
--rw-r--r--   0        0        0      656 2024-04-29 18:55:09.408806 mpflash-0.7.4/mpflash/cli_main.py
--rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.4/mpflash/common.py
--rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.4/mpflash/config.py
--rw-r--r--   0        0        0    10991 2024-05-02 20:53:12.964386 mpflash-0.7.4/mpflash/download.py
--rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.4/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.4/mpflash/errors.py
--rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.4/mpflash/flash.py
--rw-r--r--   0        0        0     2316 2024-05-02 20:53:12.964386 mpflash-0.7.4/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.4/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2093 2024-05-02 20:53:12.968640 mpflash-0.7.4/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.4/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4298 2024-05-02 20:53:12.968640 mpflash-0.7.4/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     1072 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     3252 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.4/mpflash/logger.py
--rw-r--r--   0        0        0     3509 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     2361 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.4/mpflash/mpboard_id/board_info.csv
--rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.4/mpflash/mpboard_id/board_info.json
--rw-r--r--   0        0        0     7017 2024-05-02 20:53:12.977648 mpflash-0.7.4/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.4/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.4/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.4/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.4/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.4/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3629 2024-04-29 18:55:09.425429 mpflash-0.7.4/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5299 2024-05-02 20:53:12.993284 mpflash-0.7.4/mpflash/worklist.py
--rw-r--r--   0        0        0     1630 2024-05-02 20:54:16.528433 mpflash-0.7.4/pyproject.toml
--rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.4/README.md
--rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.7.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.7.5/mpflash/__init__.py
+-rw-r--r--   0        0        0     9010 2024-05-03 13:05:36.158081 mpflash-0.7.5/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3642 2024-05-03 13:05:36.159263 mpflash-0.7.5/mpflash/cli_download.py
+-rw-r--r--   0        0        0     5845 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1967 2024-04-29 18:55:09.407466 mpflash-0.7.5/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1024 2024-04-29 18:55:09.408806 mpflash-0.7.5/mpflash/cli_list.py
+-rw-r--r--   0        0        0      656 2024-05-05 21:39:33.092998 mpflash-0.7.5/mpflash/cli_main.py
+-rw-r--r--   0        0        0     1049 2024-04-29 18:55:09.409821 mpflash-0.7.5/mpflash/common.py
+-rw-r--r--   0        0        0      419 2024-04-05 19:52:32.888852 mpflash-0.7.5/mpflash/config.py
+-rw-r--r--   0        0        0    11120 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/download.py
+-rw-r--r--   0        0        0     3803 2024-04-29 18:55:09.412110 mpflash-0.7.5/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.7.5/mpflash/errors.py
+-rw-r--r--   0        0        0     2490 2024-04-29 18:55:09.414103 mpflash-0.7.5/mpflash/flash.py
+-rw-r--r--   0        0        0     2314 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.7.5/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2115 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.7.5/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4319 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.7.5/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     4713 2024-05-03 13:05:36.167441 mpflash-0.7.5/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-03-08 22:48:27.382922 mpflash-0.7.5/mpflash/logger.py
+-rw-r--r--   0        0        0     3621 2024-05-03 13:05:36.168458 mpflash-0.7.5/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     2592 2024-05-05 21:35:23.329974 mpflash-0.7.5/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    96983 2024-04-05 19:52:32.903789 mpflash-0.7.5/mpflash/mpboard_id/board_info.csv
+-rw-r--r--   0        0        0   674442 2024-04-30 08:26:55.864409 mpflash-0.7.5/mpflash/mpboard_id/board_info.json
+-rw-r--r--   0        0        0     7110 2024-05-05 21:00:42.554839 mpflash-0.7.5/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.7.5/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.7.5/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0     5739 2024-04-29 18:55:09.422436 mpflash-0.7.5/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.7.5/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.7.5/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3629 2024-05-05 21:35:22.350460 mpflash-0.7.5/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5297 2024-05-03 13:05:36.171762 mpflash-0.7.5/mpflash/worklist.py
+-rw-r--r--   0        0        0     1648 2024-05-05 21:40:12.443828 mpflash-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    13159 2024-04-29 21:19:09.956495 mpflash-0.7.5/README.md
+-rw-r--r--   0        0        0    14633 1970-01-01 00:00:00.000000 mpflash-0.7.5/PKG-INFO
```

### Comparing `mpflash-0.7.4/LICENSE` & `mpflash-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/ask_input.py` & `mpflash-0.7.5/mpflash/ask_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List, Sequence, Tuple, Union
 
 from loguru import logger as log
 
 from mpflash.config import config
-from mpflash.mpboard_id import get_stored_boards_for_port, known_stored_boards, local_mp_ports
+from mpflash.mpboard_id import get_known_boards_for_port, get_known_ports, known_stored_boards
 from mpflash.mpremoteboard import MPRemoteBoard
 from mpflash.vendor.versions import micropython_versions
 
 
 @dataclass
 class Params:
     ports: List[str] = field(default_factory=list)
@@ -75,30 +75,39 @@
         ask_versions(questions, action=action)
     else:
         # versions is used to show only the boards for the selected versions
         answers["versions"] = params.versions  # type: ignore
 
     if not params.boards or "?" in params.boards:
         ask_port_board(questions, action=action)
-
-    answers = inquirer.prompt(questions, answers=answers)
+    if questions:
+        answers = inquirer.prompt(questions, answers=answers)
     if not answers:
         # input cancelled by user
         return []  # type: ignore
     # print(repr(answers))
     if isinstance(params, FlashParams) and "serial" in answers:
         params.serial = answers["serial"]
     if "port" in answers:
-        params.ports = [answers["port"]]
+        params.ports = [p for p in params.ports if p != "?"]  # remove the "?" if present
+        params.ports.extend(answers["port"])
     if "boards" in answers:
-        params.boards = answers["boards"] if isinstance(answers["boards"], list) else [answers["boards"]]
+        params.boards = [b for b in params.boards if b != "?"]  # remove the "?" if present
+        params.boards.extend(answers["boards"] if isinstance(answers["boards"], list) else [answers["boards"]])
     if "versions" in answers:
+        params.versions = [v for v in params.versions if v != "?"]  # remove the "?" if present
         # make sure it is a list
-        params.versions = answers["versions"] if isinstance(answers["versions"], list) else [answers["versions"]]
-
+        if isinstance(answers["versions"], (list, tuple)):
+            params.versions.extend(answers["versions"])
+        else:
+            params.versions.append(answers["versions"])
+    # remove duplicates
+    params.ports = list(set(params.ports))
+    params.boards = list(set(params.boards))
+    params.versions = list(set(params.versions))
     log.debug(repr(params))
 
     return params
 
 
 def filter_matching_boards(answers: dict) -> Sequence[Tuple[str, str]]:
     """
@@ -145,22 +154,23 @@
 
     Returns:
         None
     """
     # import only when needed to reduce load time
     import inquirer
 
-    # TODO: if action = flash, Use Inquirer.List for boards
+    # if action flash,  single input
+    # if action download, multiple input
     inquirer_ux = inquirer.Checkbox if action == "download" else inquirer.List
     questions.extend(
         (
             inquirer.List(
                 "port",
                 message="Which port do you want to {action} " + "to {serial} ?" if action == "flash" else "?",
-                choices=local_mp_ports(),
+                choices=get_known_ports(),
                 autocomplete=True,
             ),
             inquirer_ux(
                 "boards",
                 message=(
                     "Which {port} board firmware do you want to {action} " + "to {serial} ?"
                     if action == "flash"
@@ -190,15 +200,15 @@
 
     input_ux = inquirer.Checkbox if action == "download" else inquirer.List
     mp_versions: List[str] = micropython_versions()
     mp_versions = [v for v in mp_versions if "preview" not in v]
 
     # remove the versions for which there are no known boards in the board_info.json
     # todo: this may be a little slow
-    mp_versions = [v for v in mp_versions if get_stored_boards_for_port("stm32", [v])]
+    mp_versions = [v for v in mp_versions if get_known_boards_for_port("stm32", [v])]
 
     mp_versions.append("preview")
     mp_versions.reverse()  # newest first
 
     def at_least_one_validation(answers, current) -> bool:
         if not current:
             raise inquirer.errors.ValidationError("", reason="Please select at least one version")
```

### Comparing `mpflash-0.7.4/mpflash/cli_download.py` & `mpflash-0.7.5/mpflash/cli_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import List, Tuple
 
 import rich_click as click
 from loguru import logger as log
 
 from mpflash.errors import MPFlashError
-from mpflash.mpboard_id import find_stored_board
+from mpflash.mpboard_id import find_known_board
 from mpflash.vendor.versions import clean_version
 
 from .ask_input import DownloadParams, ask_missing_params
 from .cli_group import cli
 from .cli_list import list_mcus
 from .config import config
 from .download import download
@@ -64,18 +64,25 @@
     help="""Force download of firmware even if it already exists.""",
 )
 def cli_download(**kwargs) -> int:
     params = DownloadParams(**kwargs)
     params.versions = list(params.versions)
     params.boards = list(params.boards)
     if params.boards:
-        pass
-        # TODO Clean board - same as in cli_flash.py
+        if not params.ports:
+            # no ports specified - resolve ports from specified boards by resolving board IDs
+            for board in params.boards:
+                if board != "?":
+                    try:
+                        board_ = find_known_board(board)
+                        params.ports.append(board_["port"])
+                    except MPFlashError as e:
+                        log.error(f"{e}")
     else:
-        # no boards specified - detect connected boards
+        # no boards specified - detect connected ports and boards
         params.ports, params.boards = connected_ports_boards()
 
     params = ask_missing_params(params, action="download")
     if not params:  # Cancelled by user
         return 2
     params.versions = [clean_version(v, drop_v=True) for v in params.versions]
     assert isinstance(params, DownloadParams)
```

### Comparing `mpflash-0.7.4/mpflash/cli_flash.py` & `mpflash-0.7.5/mpflash/cli_flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import rich_click as click
 from loguru import logger as log
 
 from mpflash.errors import MPFlashError
-from mpflash.mpboard_id import find_stored_board
+from mpflash.mpboard_id import find_known_board
 from mpflash.vendor.versions import clean_version
 
 from .ask_input import FlashParams, ask_missing_params
 from .cli_download import connected_ports_boards
 from .cli_group import cli
 from .cli_list import show_mcus
 from .config import config
@@ -112,15 +112,15 @@
     else:
         for board_id in params.boards:
             if board_id == "":
                 params.boards.remove(board_id)
                 continue
             if " " in board_id:
                 try:
-                    info = find_stored_board(board_id)
+                    info = find_known_board(board_id)
                     if info:
                         log.info(f"Resolved board description: {info['board']}")
                         params.boards.remove(board_id)
                         params.boards.append(info["board"])
                 except Exception as e:
                     log.warning(f"unable to resolve board description: {e}")
```

### Comparing `mpflash-0.7.4/mpflash/cli_group.py` & `mpflash-0.7.5/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/cli_list.py` & `mpflash-0.7.5/mpflash/cli_list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/cli_main.py` & `mpflash-0.7.5/mpflash/cli_main.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/common.py` & `mpflash-0.7.5/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/download.py` & `mpflash-0.7.5/mpflash/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import requests
 from bs4 import BeautifulSoup
 from loguru import logger as log
 from rich.progress import track
 
 from mpflash.common import PORT_FWTYPES
 from mpflash.errors import MPFlashError
+from mpflash.mpboard_id import get_known_ports
 
 jsonlines.ujson = None  # type: ignore
 # #########################################################################################################
 
 
 MICROPYTHON_ORG_URL = "https://micropython.org/"
 
@@ -105,24 +106,26 @@
         clean (bool): A flag indicating whether to perform a clean retrieval.
 
     Returns:
         List[FirmwareInfo]: A list of firmware information for the specified ports and boards.
 
     """
     board_urls: List[FirmwareInfo] = []
+    if ports is None:
+        ports = get_known_ports()
     for port in ports:
         download_page_url = f"{MICROPYTHON_ORG_URL}download/?port={port}"
         _urls = get_board_urls(download_page_url)
         # filter out boards we don't care about
         _urls = [board for board in _urls if board["board"] in boards]
         # add the port to the board urls
         for board in _urls:
             board["port"] = port
 
-        for board in track(_urls, description=f"Checking {port} download pages", transient=True):
+        for board in track(_urls, description=f"Checking {port} download pages", transient=True,refresh_per_second=2):
             # add a board to the list for each firmware found
             firmwares = []
             for ext in PORT_FWTYPES[port]:
                 firmwares += board_firmware_urls(board["url"], MICROPYTHON_ORG_URL, ext)
 
             for _url in firmwares:
                 board["firmware"] = _url
@@ -166,14 +169,15 @@
     *,
     force: bool = False,
     clean: bool = True,
 ) -> int:
     skipped = downloaded = 0
     if versions is None:
         versions = []
+
     unique_boards = get_firmware_list(ports, boards, versions, clean)
 
     for b in unique_boards:
         log.debug(b["filename"])
     # relevant
 
     log.info(f"Found {len(unique_boards)} relevant unique firmwares")
```

### Comparing `mpflash-0.7.4/mpflash/downloaded.py` & `mpflash-0.7.5/mpflash/downloaded.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/flash.py` & `mpflash-0.7.5/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/flash_esp.py` & `mpflash-0.7.5/mpflash/flash_esp.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 from pathlib import Path
 from typing import List, Optional
 
 import esptool
 from loguru import logger as log
 
-from mpflash.mpboard_id import find_stored_board
+from mpflash.mpboard_id import find_known_board
 from mpflash.mpremoteboard import MPRemoteBoard
 
 
 def flash_esp(mcu: MPRemoteBoard, fw_file: Path, *, erase: bool = True) -> Optional[MPRemoteBoard]:
     if mcu.port not in ["esp32", "esp8266"] or mcu.board in ["ARDUINO_NANO_ESP32"]:
         log.error(f"esptool not supported for {mcu.port} {mcu.board} on {mcu.serialport}")
         return None
 
     log.info(f"Flashing {fw_file} on {mcu.board} on {mcu.serialport}")
     if not mcu.cpu:
         # Lookup CPU based on the board name
-        mcu.cpu = find_stored_board(mcu.board)["cpu"]
+        mcu.cpu = find_known_board(mcu.board)["cpu"]
 
     cmds: List[List[str]] = []
     if erase:
         cmds.append(f"esptool --chip {mcu.cpu} --port {mcu.serialport} erase_flash".split())
 
     if mcu.cpu.upper().startswith("ESP32"):
         baud_rate = str(921_600)
```

### Comparing `mpflash-0.7.4/mpflash/flash_stm32.py` & `mpflash-0.7.5/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/flash_stm32_cube.py` & `mpflash-0.7.5/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/flash_stm32_dfu.py` & `mpflash-0.7.5/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/flash_uf2.py` & `mpflash-0.7.5/mpflash/flash_uf2.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 
     log.info("Board is in bootloader mode")
     log.info(f"Copying {fw_file} to {destination}.")
     shutil.copy(fw_file, destination)
     log.success("Done copying, resetting the board and wait for it to restart")
     if sys.platform in ["linux", "darwin"]:
         dismount_uf2()
-    for _ in track(range(5 + 2), description="Waiting for the board to restart", transient=True):
+    for _ in track(range(5 + 2), description="Waiting for the board to restart", transient=True, refresh_per_second=2):
         time.sleep(1)  # 5 secs to short on linux
     return mcu
```

### Comparing `mpflash-0.7.4/mpflash/flash_uf2_linux.py` & `mpflash-0.7.5/mpflash/flash_uf2_linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 def wait_for_UF2_linux(s_max: int = 10):
     destination = ""
     wait = 10
     uf2_drives = []
     # while not destination and wait > 0:
-    for _ in track(range(s_max), description="Waiting for mcu to mount as a drive", transient=True):
+    for _ in track(range(s_max), description="Waiting for mcu to mount as a drive", transient=True,refresh_per_second=2):
         # log.info(f"Waiting for mcu to mount as a drive : {wait} seconds left")
         uf2_drives += list(get_uf2_drives())
         for drive in get_uf2_drives():
             pmount(drive)
             time.sleep(1)
             try:
                 if Path(drive.mountpoint, "INFO_UF2.TXT").exists():
```

### Comparing `mpflash-0.7.4/mpflash/flash_uf2_windows.py` & `mpflash-0.7.5/mpflash/flash_uf2_windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def wait_for_UF2_windows(s_max: int = 10):
     """Wait for the MCU to mount as a drive"""
     if s_max < 1:
         s_max = 10
     destination = ""
-    for _ in track(range(s_max), description="Waiting for mcu to mount as a drive", transient=True):
+    for _ in track(range(s_max), description="Waiting for mcu to mount as a drive", transient=True,refresh_per_second=2):
         # log.info(f"Waiting for mcu to mount as a drive : {n} seconds left")
         drives = [drive.device for drive in psutil.disk_partitions()]
         for drive in drives:
             try:
                 if Path(drive, "INFO_UF2.TXT").exists():
                     board_id = get_board_id(Path(drive))  # type: ignore
                     destination = Path(drive)
```

### Comparing `mpflash-0.7.4/mpflash/logger.py` & `mpflash-0.7.5/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/mpboard_id/__init__.py` & `mpflash-0.7.5/mpflash/mpboard_id/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 """
 
 import json
 from functools import lru_cache
 from pathlib import Path
 from typing import List, Optional, Tuple, TypedDict, Union
 
-from mpflash.errors import MPFlashError
 from mpflash.common import PORT_FWTYPES
+from mpflash.errors import MPFlashError
 from mpflash.vendor.versions import clean_version
 
+# KNOWN ports and boards are sourced from the micropython repo,
+# this info is stored in the board_info.json file
+
 
 # Board  based on the dataclass Board but changed to TypedDict
 # - source : get_boardnames.py
 class Board(TypedDict):
     """MicroPython Board definition"""
 
     description: str
@@ -26,35 +29,35 @@
     mcu_name: str
     path: Union[Path, str]
     version: str
     cpu: str
 
 
 @lru_cache(maxsize=None)
-def read_stored_boardinfo() -> List[Board]:
+def read_known_boardinfo() -> List[Board]:
     """Reads the board_info.json file and returns the data as a list of Board objects"""
     with open(Path(__file__).parent / "board_info.json", "r") as file:
         return json.load(file)
 
 
-def local_mp_ports() -> List[str]:
+def get_known_ports() -> List[str]:
     # TODO: Filter for Version
-    mp_boards = read_stored_boardinfo()
+    mp_boards = read_known_boardinfo()
     # select the unique ports from info
     ports = set({board["port"] for board in mp_boards if board["port"] in PORT_FWTYPES.keys()})
     return sorted(list(ports))
 
 
-def get_stored_boards_for_port(port: str, versions: Optional[List[str]] = None):
+def get_known_boards_for_port(port: str, versions: Optional[List[str]] = None):
     """
     Returns a list of boards for the given port and version(s)
 
     port : str : The Micropython port to filter for
     versions : List[str] : The Micropython versions to filter for (actual versions required)"""
-    mp_boards = read_stored_boardinfo()
+    mp_boards = read_known_boardinfo()
 
     # filter for 'preview' as they are not in the board_info.json
     # instead use stable version
     versions = versions or []
     if "preview" in versions:
         versions.remove("preview")
         versions.append("stable")
@@ -71,24 +74,24 @@
 def known_stored_boards(port: str, versions: Optional[List[str]] = None) -> List[Tuple[str, str]]:
     """
     Returns a list of tuples with the description and board name for the given port and version
 
     port : str : The Micropython port to filter for
     versions : List[str] : The Micropython versions to filter for (actual versions required)
     """
-    mp_boards = get_stored_boards_for_port(port, versions)
+    mp_boards = get_known_boards_for_port(port, versions)
 
     boards = set({(f'{board["version"]} {board["description"]}', board["board"]) for board in mp_boards})
     return sorted(list(boards))
 
 
 @lru_cache(maxsize=20)
-def find_stored_board(board_id: str) -> Board:
-    """Find the board for the given board_ID or 'board description' and return the board info as a Board object"""
-    info = read_stored_boardinfo()
+def find_known_board(board_id: str) -> Board:
+    """Find the board for the given BOARD_ID or 'board description' and return the board info as a Board object"""
+    info = read_known_boardinfo()
     for board_info in info:
         if board_id in (board_info["board"], board_info["description"]):
             if "cpu" not in board_info or not board_info["cpu"]:
                 if " with " in board_info["description"]:
                     board_info["cpu"] = board_info["description"].split(" with ")[-1]
                 else:
                     board_info["cpu"] = board_info["port"]
```

### Comparing `mpflash-0.7.4/mpflash/mpboard_id/board_id.py` & `mpflash-0.7.5/mpflash/mpboard_id/board_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,60 +4,69 @@
 
 import functools
 import json
 from pathlib import Path
 from typing import Optional
 
 from mpflash.errors import MPFlashError
-from mpflash.vendor.versions import clean_version
+from mpflash.vendor.versions import clean_version, get_stable_mp_version
 
 ###############################################################################################
 HERE = Path(__file__).parent
 ###############################################################################################
 
 
-def find_board_id(
-    descr: str, short_descr: str, board_info: Optional[Path] = None, version: str = "stable"
+def find_board_id_by_description(
+    descr: str,
+    short_descr: str,
+    *,
+    version: str,
+    board_info: Optional[Path] = None,
 ) -> Optional[str]:
     """Find the MicroPython BOARD_ID based on the description in the firmware"""
+
     try:
-        boards = find_board_id_by_description(
+        boards = _find_board_id_by_description(
             descr=descr,
             short_descr=short_descr,
             board_info=board_info,
-            version=clean_version(version),
+            version=clean_version(version) if version else None,
         )
         return boards[-1]["board"]
     except MPFlashError:
         return "UNKNOWN_BOARD"
 
 
 @functools.lru_cache(maxsize=20)
-def find_board_id_by_description(*, descr: str, short_descr: str, version="v1.21.0", board_info: Optional[Path] = None):
+def _find_board_id_by_description(
+    *, descr: str, short_descr: str, version: Optional[str] = None, board_info: Optional[Path] = None
+):
     """
     Find the MicroPython BOARD_ID based on the description in the firmware
     using the pre-built board_info.json file
     """
     if not board_info:
         board_info = HERE / "board_info.json"
     if not board_info.exists():
         raise FileNotFoundError(f"Board info file not found: {board_info}")
 
-    info = _read_board_info(board_info)
+    candidate_boards = _read_board_info(board_info)
 
-    # filter for matching version
-    if version == "preview":
-        # TODO: match last stable
-        version = "v1.22.2"
-    version_matches = [b for b in info if b["version"].startswith(version)]
-    if not version_matches:
-        raise MPFlashError(f"No board info found for version {version}")
-    matches = [b for b in version_matches if b["description"] == descr]
+    if version:
+        # filter for matching version
+        if version in ("preview", "stable"):
+            # match last stable
+            version = get_stable_mp_version()
+        version_matches = [b for b in candidate_boards if b["version"].startswith(version)]
+        if not version_matches:
+            raise MPFlashError(f"No board info found for version {version}")
+        candidate_boards = version_matches
+    matches = [b for b in candidate_boards if b["description"] == descr]
     if not matches and short_descr:
-        matches = [b for b in version_matches if b["description"] == short_descr]
+        matches = [b for b in candidate_boards if b["description"] == short_descr]
     if not matches:
         raise MPFlashError(f"No board info found for description '{descr}' or '{short_descr}'")
     return sorted(matches, key=lambda x: x["version"])
 
 
 @functools.lru_cache(maxsize=20)
 def _read_board_info(board_info):
```

### Comparing `mpflash-0.7.4/mpflash/mpboard_id/board_info.csv` & `mpflash-0.7.5/mpflash/mpboard_id/board_info.csv`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/mpboard_id/board_info.json` & `mpflash-0.7.5/mpflash/mpboard_id/board_info.json`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/mpremoteboard/__init__.py` & `mpflash-0.7.5/mpflash/mpremoteboard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import serial.tools.list_ports
 from loguru import logger as log
 from rich.progress import track
 from tenacity import retry, stop_after_attempt, wait_fixed
 
 from mpflash.errors import MPFlashError
-from mpflash.mpboard_id.board_id import find_board_id
+from mpflash.mpboard_id.board_id import find_board_id_by_description
 from mpflash.mpremoteboard.runner import run
 
 ###############################################################################################
 # TODO : make this a bit nicer
 HERE = Path(__file__).parent
 
 OK = 0
@@ -112,18 +112,18 @@
             self.port = info["port"]
             self.cpu = info["cpu"]
             self.arch = info["arch"]
             self.mpy = info["mpy"]
             self.description = descr = info["board"]
             pos = descr.rfind(" with")
             short_descr = descr[:pos].strip() if pos != -1 else ""
-            if board_name := find_board_id(descr, short_descr):
+            if board_name := find_board_id_by_description(descr, short_descr, version=self.version):
                 self.board = board_name
             else:
-                self.board = "UNKNOWN"
+                self.board = "UNKNOWN_BOARD"
 
     def disconnect(self) -> bool:
         """
         Disconnect from a board.
 
         Returns:
         - bool: True if successfully disconnected, False otherwise.
@@ -196,14 +196,15 @@
         """wait for the board to restart"""
         for _ in track(
             range(timeout),
             description="Waiting for the board to restart",
             transient=True,
             get_time=lambda: time.time(),
             show_speed=False,
+            refresh_per_second=1,
         ):
             time.sleep(1)
             try:
                 self.get_mcu_info()
                 break
             except (ConnectionError, MPFlashError):
                 pass
```

### Comparing `mpflash-0.7.4/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.7.5/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/mpremoteboard/runner.py` & `mpflash-0.7.5/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/vendor/dfu.py` & `mpflash-0.7.5/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/vendor/pydfu.py` & `mpflash-0.7.5/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/vendor/versions.py` & `mpflash-0.7.5/mpflash/vendor/versions.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/mpflash/worklist.py` & `mpflash-0.7.5/mpflash/worklist.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mpflash.common import FWInfo
 from mpflash.errors import MPFlashError
 
 from .config import config
 from .downloaded import find_downloaded_firmware
 from .list import show_mcus
-from .mpboard_id import find_stored_board
+from .mpboard_id import find_known_board
 from .mpremoteboard import MPRemoteBoard
 
 # #########################################################################################################
 WorkList = List[Tuple[MPRemoteBoard, FWInfo]]
 # #########################################################################################################
 
 
@@ -127,15 +127,15 @@
     Returns:
         WorkList: List of boards and firmware information to update
     """
     mcu = MPRemoteBoard(serial_port)
     # TODO : Find a way to avoid needing to specify the port
     # Lookup the matching port and cpu in board_info based in the board name
     try:
-        info = find_stored_board(board)
+        info = find_known_board(board)
         mcu.port = info["port"]
         # need the CPU type for the esptool
         mcu.cpu = info["cpu"]
     except (LookupError, MPFlashError) as e:
         log.error(f"Board {board} not found in board_info.json")
         return []
     mcu.board = board
```

### Comparing `mpflash-0.7.4/pyproject.toml` & `mpflash-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.7.4"
+version = "0.7.5"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
@@ -46,12 +46,13 @@
 pytest-github-actions-annotate-failures = ">=0.1.7,<0.3.0"
 pytest-json-report = "^1.5.0"
 pytest-metadata = ">=2.0.2,<4.0.0"
 pytest-mock = "^3.10.0"
 mock = "^4.0.3"
 distro = "^1.8.0"
 fasteners = "^0.19"
+jsons = "^1.6.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpflash-0.7.4/README.md` & `mpflash-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `mpflash-0.7.4/PKG-INFO` & `mpflash-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.7.4
+Version: 0.7.5
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
```

