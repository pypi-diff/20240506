# Comparing `tmp/pydfuutil-0.0.2b3.tar.gz` & `tmp/pydfuutil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.2b3.tar", last modified: Thu May  2 20:44:37 2024, max compression
+gzip compressed data, was "pydfuutil-0.0.3.tar", last modified: Mon May  6 09:58:21 2024, max compression
```

## Comparing `pydfuutil-0.0.2b3.tar` & `pydfuutil-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.226199 pydfuutil-0.0.3/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35908 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19557 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 09:58:21.000000 pydfuutil-0.0.3/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:58:21.230199 pydfuutil-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-06 09:58:11.000000 pydfuutil-0.0.3/tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.2b3/LICENSE` & `pydfuutil-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/PKG-INFO` & `pydfuutil-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b3
+Version: 0.0.3
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -320,16 +320,22 @@
 - [x] dfu_load
 - [x] portable
 - [x] quirks
 - [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [ ] dfuse (not fully supported yet)
-- [ ] dfu-util cli entry point (not fully supported yet)
+- [x] dfuse
+- [x] dfu-util cli entry point (not fully supported yet)
+
+#### Todo
+- [ ] Update sources to latest original version "dfu-util-0.11"
+
+[//]: # (https://dfu-util.sourceforge.net/)
+[//]: # (- https://sourceforge.net/p/dfu-util/dfu-util/ci/master/tree/)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b3/README.md` & `pydfuutil-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -120,16 +120,22 @@
 - [x] dfu_load
 - [x] portable
 - [x] quirks
 - [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [ ] dfuse (not fully supported yet)
-- [ ] dfu-util cli entry point (not fully supported yet)
+- [x] dfuse
+- [x] dfu-util cli entry point (not fully supported yet)
+
+#### Todo
+- [ ] Update sources to latest original version "dfu-util-0.11"
+
+[//]: # (https://dfu-util.sourceforge.net/)
+[//]: # (- https://sourceforge.net/p/dfu-util/dfu-util/ci/master/tree/)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil/__main__.py` & `pydfuutil-0.0.3/pydfuutil/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 pydfuutil
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 Based on existing code of dfu-programmer-0.4
 """
 import argparse
 import errno
+import importlib.metadata
 import logging
 import os
 import re
 import sys
 from enum import Enum
-from typing import Any, Callable, Literal
-import importlib.metadata
+from typing import Literal, Optional
+
+import usb.core
 
 from pydfuutil import dfu
-from pydfuutil import dfuse
-from pydfuutil import dfu_load
 from pydfuutil import dfu_file
+from pydfuutil import dfu_load
+from pydfuutil import dfuse
 from pydfuutil import quirks
 from pydfuutil import usb_dfu
-from pydfuutil.portable import milli_sleep
+from pydfuutil.exceptions import GeneralError, MisuseError, CapabilityError
 from pydfuutil.logger import logger
-
-import usb.core
+from pydfuutil.portable import milli_sleep
 
 try:
     import libusb_package
     from usb.backend import libusb1
 
     libusb1.get_backend(libusb_package.find_library)
 finally:
@@ -44,43 +45,52 @@
 
 def atoi(s: str) -> int:
     """
     Regular expression to match the integer part of the string
     :param s: input
     :return: Return 0 if no integer is found
     """
-    match = re.match(r'^\s*([-+]?\d+)', s)
+    # match hex
+    match = re.match(r'^\dx([\da-fA-F]+)', s)
+    if match:
+        result = int(match.group(1), 16)
+        return result
 
+    # match tens
+    match = re.match(r'^\s*([-+]?\d+)', s)
     if match:
         result = int(match.group(1))
         return result
+
     return 0
 
 
 def usb_path2devnum(path: str) -> int:
     """parse the dev bus/port"""
-    # TODO: wrong implementation
-    parts = path.split('.')
-    if len(parts) == 2:
-        return int(parts[0]), int(parts[1])
-    return 0
 
+    parts = path.split('-')
+    # bus_number = int(parts[0])
+    # port_numbers, config_interface = parts[1].split(':')
+    port_numbers, _ = parts[1].split(':')
+    port_numbers = list(map(int, port_numbers.split('.')))
+    # config, interface = map(int, config_interface.split('.'))
+
+    devnum = 0
+    for port in port_numbers:
+        devnum <<= 4
+        devnum += port
+    return devnum
 
-def find_dfu_if(dev: usb.core.Device,
-                handler: Callable[[dfu.DfuIf, Any], Any] = None,
-                v: Any = None) -> int:
+
+def find_dfu_if(dev: usb.core.Device) -> list[dfu.DfuIf]:
     """
     Find DFU interface for a given USB device.
-
     :param dev: The USB device.
-    :param handler: Callback function to handle the found DFU interface.
-    :param v: Additional user-defined data for the callback function.
     :return: 0 if no DFU interface is found, or the result of the handler function.
     """
-
     configs = dev.configurations()  # .desc
 
     for cfg in configs:
         for intf in cfg:
             if intf.bInterfaceClass == 0xfe and intf.bInterfaceSubClass == 1:
                 dfu_if = dfu.DfuIf(
                     vendor=dev.idVendor,
@@ -93,99 +103,65 @@
                     bus=dev.bus,
                     devnum=dev.address,
                     path=dev.address,
                     flags=0,
                     count=0,
                     dev=dev
                 )
+                yield dfu_if
 
-                logger.debug(f"{handler.__name__}, {handler}, {v}")
-                if handler:
-                    rc = handler(dfu_if, v)
-                    if rc != 0:
-                        return rc
-
-    return 0
 
-
-def _get_first_cb(dif: dfu.DfuIf, v: dfu.DfuIf) -> int:
-    """
-    Callback function to copy the first found DFU interface.
-
-    :param dif: The DFU interface struct.
-    :param v: The DFU interface struct to copy to.
-    :return: 1 to indicate that the interface has been found.
-    """
-    # Copy everything except the device handle. This depends heavily on this member being last!
-    v.__dict__.update((k, getattr(dif, k)) for k in dif.__dict__ if k != 'dev')
-
-    # Return a value that makes find_dfu_if return immediately
-    return 1
-
-
-def _get_first_dfu_if(dif: dfu.DfuIf) -> int:
+def get_first_dfu_if(dev: usb.core.Device) -> dfu.DfuIf:
     """
     Fills in dif with the first found DFU interface.
-
-    :param dif: The DFU interface struct.
+    :param dev: the DFU capable USB device
     :return: 0 if no DFU interface is found, 1 otherwise.
     """
-    return find_dfu_if(dif.dev, _get_first_cb, dif)
+    if dfu_if := next((i for i in find_dfu_if(dev) if i is not None), None):
+        return dfu_if
+    raise GeneralError("Cannot open device")
 
 
-def _check_match_cb(dif: dfu.DfuIf, v: dfu.DfuIf) -> int:
-    """
-    Callback function to check matching DFU interfaces/altsettings.
-
-    :param dif: The DFU interface struct.
-    :param v: The DFU interface struct to match against.
-    :return: 0 if no match is found, or the result of _get_first_cb.
-    """
-    if v.flags & dfu.Mode.IFF_IFACE and dif.interface != v.interface:
+def _check_match_cb(dif: dfu.DfuIf, other: dfu.DfuIf):
+    if other.flags & dfu.Mode.IFF_IFACE and dif.interface != other.interface:
         return 0
-    if v.flags & dfu.Mode.IFF_ALT and dif.altsetting != v.altsetting:
+    if other.flags & dfu.Mode.IFF_ALT and dif.altsetting != other.altsetting:
         return 0
-    return _get_first_cb(dif, v)
+    return 1
 
 
 def get_matching_dfu_if(dif: dfu.DfuIf) -> int:
     """
     Fills in dif from the matching DFU interface/altsetting.
-
     :param dif: The DFU interface struct.
     :return: 0 if no matching interface/altsetting is found, 1 otherwise.
     """
-    return find_dfu_if(dif.dev, _check_match_cb, dif)
-
-
-def _count_match_cb(dif: dfu.DfuIf, v: dfu.DfuIf) -> int:
-    """
-    Callback function to count matching DFU interfaces/altsettings.
-
-    :param dif: The DFU interface struct.
-    :param v: The DFU interface struct to match against.
-    :return: Always returns 0.
-    """
-    if v.flags & dfu.Mode.IFF_IFACE and dif.interface != v.interface:
-        return 0
-    if v.flags & dfu.Mode.IFF_ALT and dif.altsetting != v.altsetting:
-        return 0
-    v.count += 1
+    for dfu_if in find_dfu_if(dif.dev):
+        if _check_match_cb(dif, dfu_if):
+            # Copy everything except the device handle.
+            # This depends heavily on this member being last!
+            dfu_if.__dict__.update(
+                (k, getattr(dif, k)) for k in dif.__dict__
+                if k != 'dev'
+            )
+            return 1
     return 0
 
 
 def count_matching_dfu_if(dif: dfu.DfuIf) -> int:
     """
     Count matching DFU interfaces/altsettings.
-
     :param dif: The DFU interface struct.
     :return: The number of matching DFU interfaces/altsettings.
     """
     dif.count = 0
-    find_dfu_if(dif.dev, _count_match_cb, dif)
+    for dfu_if in find_dfu_if(dif.dev):
+        if _check_match_cb(dif, dfu_if):
+            dif.count += 1
+
     return dif.count
 
 
 def get_alt_name(dfu_if: dfu.DfuIf) -> [int, str]:
     """
     Retrieves alternate interface name string.
 
@@ -193,70 +169,55 @@
     :return: The alternate interface name string or a negative integer on error.
     """
     dev = dfu_if.dev
     cfg = dev.get_active_configuration()
     intf: usb.core.Interface = cfg[(dfu_if.interface, dfu_if.altsetting)]
 
     alt_name_str_idx = intf.iInterface
-
-    if alt_name_str_idx:
-        if not dfu_if.dev:
-            try:
-                dfu_if.dev = usb.util.find_descriptor(dev, find_all=True)
-            except usb.core.USBError:
-                dfu_if.dev = None
-
-        if dfu_if.dev:
-            try:
-                return usb.util.get_string(dev, alt_name_str_idx)
-            except usb.core.USBError:
-                return -1
-
-    return -1
+    if not alt_name_str_idx:
+        return -1
+    try:
+        return usb.util.get_string(dev, alt_name_str_idx)
+    except usb.core.USBError:
+        return -1
 
 
-def print_dfu_if(dfu_if: dfu.DfuIf, v: Any) -> int:
+def print_dfu_if(dfu_if: dfu.DfuIf) -> int:
     """
     Print DFU interface information.
-
     :param dfu_if: The DFU interface struct.
-    :param v: Unused (can be any value).
     :return: Always returns 0.
     """
-
-    name: str = get_alt_name(dfu_if)
-    if name is None:
-        name = "UNDEFINED"
-
+    name = get_alt_name(dfu_if) or "UNDEFINED"
     logger.info(f"Found {'DFU' if dfu_if.flags & dfu.Mode.IFF_DFU else 'Runtime'}: "
-                f"[{dfu_if.vendor:04x}:{dfu_if.product:04x}] devnum={dfu_if.devnum}, "
-                f"cfg={dfu_if.configuration}, intf={dfu_if.interface}, "
-                f"alt={dfu_if.altsetting}, name=\"{name}\"")
-
+                f"[{dfu_if.vendor:04x}:{dfu_if.product:04x}] "
+                f"devnum={dfu_if.devnum}, cfg={dfu_if.configuration}, "
+                f"intf={dfu_if.interface}, alt={dfu_if.altsetting}, "
+                f"name=\"{name}\"")
+    if sys.platform != "win32":
+        logger.debug(get_device_path(dfu_if.dev))
     return 0
 
 
 def list_dfu_interfaces(ctx: list[usb.core.Device]) -> int:
     """
     Walk the device tree and print out DFU devices.
-
     :param ctx: libusb context
     :return: 0 on success.
     """
-
     for dev in ctx:
-        find_dfu_if(dev, print_dfu_if, None)
+        for dfu_if in find_dfu_if(dev):
+            print_dfu_if(dfu_if)
         usb.util.dispose_resources(dev)
     return 0
 
 
-def alt_by_name(dfu_if: dfu.DfuIf, v: bytes) -> int:
+def alt_by_name(dfu_if: dfu.DfuIf, v: str) -> int:
     """
     Find alternate setting by name.
-
     :param dfu_if: The DFU interface struct.
     :param v: The name of the alternate setting.
     :return: The alternate setting number if found, 0 otherwise.
     """
     name = get_alt_name(dfu_if)
     if name is None:
         return 0
@@ -266,115 +227,121 @@
     # use return value 0 to indicate not found
     return dfu_if.altsetting + 1
 
 
 def count_dfu_interfaces(dev: usb.core.Device) -> int:
     """
     Count DFU interfaces within a single device.
-
     :param dev: The USB device.
     :return: The number of DFU interfaces found.
     """
-    num_found: int = 0
-
-    def count_cb(dif, v):
-        nonlocal num_found
-        num_found += v
-        return 0
-
-    find_dfu_if(dev, count_cb, 1)
-    return num_found
+    return sum(1 for _ in find_dfu_if(dev))
 
 
 def iterate_dfu_devices(ctx: list[usb.core.Device], dif: dfu.DfuIf) -> list[usb.core.Device]:
     """
     Iterate over all matching DFU capable devices within the system.
-
     :param ctx: The USB context.
     :param dif: The DFU interface.
-    :return: 0 on success, or an error code.
+    :return: List of matching DFU capable devices.
     """
     retval = []
     for dev in ctx:
-
-        if (dif and (dif.flags & dfu.Mode.IFF_DEVNUM)
-                and (dev.bus != dif.bus or dev.address != dif.devnum)):
-            continue
-        if dif and (dif.flags & dfu.Mode.IFF_VENDOR) and dev.idVendor != dif.vendor:
-            continue
-        if dif and (dif.flags & dfu.Mode.IFF_PRODUCT) and dev.idProduct != dif.product:
-            continue
-        if not count_dfu_interfaces(dev):
-            continue
+        if dif:
+            if ((dif.flags & dfu.Mode.IFF_DEVNUM)
+                    and (dev.bus != dif.bus or dev.address != dif.devnum)):
+                continue
+            if (dif.flags & dfu.Mode.IFF_VENDOR) and dev.idVendor != dif.vendor:
+                continue
+            if (dif.flags & dfu.Mode.IFF_PRODUCT) and dev.idProduct != dif.product:
+                continue
+        if count_dfu_interfaces(dev):
+            retval.append(dev)
         usb.util.dispose_resources(dev)
-        retval.append(dev)
-
     return retval
 
 
-def found_dfu_device(dev: usb.core.Device, dif: dfu.DfuIf) -> int:
-    """
-    Save the DFU-capable device in dif.dev.
-
-    :param dev: The USB device.
-    :param dif: The DFU interface instance.
-    :return: 1 always.
-    """
-    dif.dev = dev
-    return 1
-
-
 def parse_vid_pid(string: str) -> tuple[int, int]:
     """
     Parse a string containing vendor and product IDs in hexadecimal format.
-
     :param string: The string containing vendor and product IDs separated by ':'.
     :return: A tuple containing the vendor and product IDs.
     """
-    vendor = 0
-    product = 0
+    vendor, product = 0, 0
+    try:
+        vendor_str, product_str = string.split(':')
+        if vendor_str:
+            vendor = int(vendor_str, 16)
+        if product_str:
+            product = int(product_str, 16)
+    except (ValueError, TypeError, AttributeError):
+        pass
+    return vendor, product
 
-    vendor_str, product_str = string.split(':')
 
-    if vendor_str:
-        vendor = atoi(vendor_str)
-    if product_str:
-        product = atoi(product_str)
+def get_device_path(dev: usb.core.Device) -> str:
+    """
+    Get device path
+    :param dev:
+    :return str:
+    """
+    # Retrieve bus and device numbers
+    bus_number = dev.bus
+    device_number = dev.address
+    parent = dev.parent
+    # Retrieve port numbers
+    port_numbers = [device_number]
+    while parent is not None:
+        port_numbers.insert(0, parent.port_number)
+        parent = parent.parent
+
+    # Construct device path
+    device_path = f"{bus_number}-{port_numbers.pop(0)}"
+    for port in port_numbers:
+        device_path += f".{port}"
 
-    return vendor, product
+    # Append configuration and interface numbers
+    cfg = dev.get_active_configuration()
+    device_path += f":{cfg.bConfigurationValue}.{cfg[(0, 0)].bInterfaceNumber}"
 
+    return device_path
 
-# TODO: maybe useless if pyusb uses
+
+# FIXME: maybe useless if pyusb uses?
 def resolve_device_path(dif: dfu.DfuIf) -> int:
     """
     :param dif: DfuIf instance
     """
     try:
+        if sys.platform == "win32":
+            raise SystemError("USB device paths are not supported by Windows")
         res: int = usb_path2devnum(dif.path)
         if res < 0:
             return -errno.EINVAL
         if not res:
             return 0
 
         dif.bus = atoi(dif.path)
         dif.devnum = res
         dif.flags |= dfu.Mode.IFF_DEVNUM
+        logger.debug(f"DIF PATH: {dif.path}: {dif.bus}")
         return res
+    except SystemError as err:
+        logger.error(err)
     except Exception as err:
-        logger.error("USB device paths are not supported by this dfu-util.\n")
+        logger.error("USB device paths are not supported by this dfu-util")
         logger.debug(err)
-        sys.exit(1)
+    raise GeneralError
 
 
 def find_descriptor(desc_list: list, desc_type: int, desc_index: int,
                     res_buf: bytes) -> int:
     """
     Look for a descriptor in a concatenated descriptor list
     Will return desc_index'th match of given descriptor type
-
     :param desc_list: The concatenated descriptor list.
     :param desc_type: The type of descriptor to search for.
     :param desc_index: The index of the descriptor to find.
     :param res_buf: The buffer to store the found descriptor.
     :return: length of found descriptor, limited to res_size
     """
 
@@ -448,31 +415,31 @@
     # This is not supported on all devices for non-standard types
     # return dev.ctrl_transfer(usb.util.ENDPOINT_IN, usb.util.GET_DESCRIPTOR,
     #                          (desc_type << 8) | desc_index, 0, resbuf)
     return usb.control.get_descriptor(dev, usb.DT_CONFIG_SIZE, desc_type, desc_index).tobytes()
 
 
 # pylint: disable=invalid-name
-def get_cached_extra_descriptor(dev: usb.core.Device,
-                                bConfValue: int,
-                                intf: int,
+def get_cached_extra_descriptor(dfu_if: dfu.DfuIf,
                                 desc_type: int,
                                 desc_index: int,
-                                resbuf: bytes) -> int:
+                                res_buf: bytes) -> int:
     """
     Get cached extra descriptor from libusb for an interface.
-
-    :param dev: The USB device.
-    :param bConfValue: The configuration value.
-    :param intf: The interface number.
+    :param dfu_if: DFU interface.
     :param desc_type: The descriptor type.
     :param desc_index: The descriptor index.
-    :param resbuf: The buffer to store the descriptor.
+    :param res_buf: The buffer to store the descriptor.
     :return: The length of the found descriptor.
     """
+
+    dev = dfu_if.dev
+    bConfValue = dfu_if.configuration
+    intf = dfu_if.interface
+
     cfg = dev.configurations()[bConfValue - 1]
     try:
         intf_desc = cfg.interfaces()[intf]
     except usb.core.USBError as e:
         if e.errno == errno.ENOENT:
             logger.error("Device is unconfigured")
         else:
@@ -482,26 +449,26 @@
     ret = -1
 
     for altsetting in intf_desc:
         extra = altsetting.extra
         extra_len = altsetting.extra_length
 
         if extra_len > 1:
-            ret = find_descriptor(extra, desc_type, desc_index, resbuf)
+            ret = find_descriptor(extra, desc_type, desc_index, res_buf)
 
         if ret > 1:
             break
 
     if ret < 2:
         logger.debug("Did not find cached descriptor")
 
     return ret
 
 
-VERSION = (f"{__version__}\n\n"
+VERSION = (f"pydfuutil {__version__}\n\n"
            f"2023 Yaroshenko Dmytro (https://github.com/o-murphy)\n")
 
 
 class Mode(Enum):
     """dfu-util cli mode"""
     NONE = 0
     VERSION = 1
@@ -518,86 +485,114 @@
 
 def le16_to_cpu(data: bytes) -> int:
     """Convert uint16le to int"""
     return int.from_bytes(data, byteorder='little')
 
 
 def int_(value: [int, bytes, bytearray],
-         order: Literal["little", "big"] = 'little') -> int:
+         order: Optional[Literal["little", "big"]] = 'little') -> int:
     """coerce value to int"""
     if isinstance(value, int):
         return value
     if isinstance(value, (bytes, bytearray)):
         return int.from_bytes(value, order)
     raise TypeError("Unsupported type")
 
 
-def main(argv) -> None:
-    """Cli entry point"""
-
-    # Create argument parser
-    parser = argparse.ArgumentParser(
-        prog=f"pydfuutil v{__version__}",
-        description="Python implementation of DFU-Util tools"
-    )
-
-    # Add arguments
+def add_cli_options(parser: argparse.ArgumentParser) -> None:
+    """Add cli options"""
     parser.add_argument("-V", "--version", action="version", version=VERSION,
                         help="Print the version number")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="Print verbose debug statements")
     parser.add_argument("-l", "--list", action="store_true",
                         help="List the currently attached DFU capable USB devices")
     parser.add_argument("-e", "--detach", action="store_true",
                         help="Detach the currently attached DFU capable USB devices")
+    # TODO: Not implemented
+    # parser.add_argument("-E", "--detach-delay", action="store",
+    #                     type=int, default=1, metavar="<seconds>",
+    #                     help="Time to wait before reopening a device after detach")
     parser.add_argument("-d", "--device", metavar="<deviceID>:<productID>",
                         help="Specify Vendor/Product ID of DFU device")
-    parser.add_argument("-p", "--path", metavar="<bus/port>",
+    # TODO: Not implemented
+    # parser.add_argument("-n", "--devnum", metavar="<dnum>",
+    #                     help="Match given device number (devnum from --list)")
+    parser.add_argument("-p", "--path", metavar="<bus-port. ... .port>",
                         help="Specify path to DFU device")
-    parser.add_argument("-c", "--cfg", metavar="<config>",
+    parser.add_argument("-c", "--cfg", metavar="<config_nr>",
                         help="Specify the Configuration of DFU device")
-    parser.add_argument("-i", "--intf", metavar="<interface>",
+    parser.add_argument("-i", "--intf", metavar="<intf_nr>",
                         help="Specify the DFU Interface number")
+    # TODO: Not implemented
+    # parser.add_argument("-S", "--serial", metavar="<serial_string>[,<serial_string_dfu>]",
+    #                     help="Specify the DFU Interface number")
     parser.add_argument("-a", "--alt", metavar="<alt>",
                         help="Specify the Altsetting of the DFU Interface")
     parser.add_argument("-t", "--transfer-size", metavar="<size>",
                         help="Specify the number of bytes per USB Transfer")
     parser.add_argument("-U", "--upload", metavar="<file>",
                         help="Read firmware from device into <file>")
+    # TODO: Not implemented
+    # parser.add_argument("-Z", "--upload-size", metavar="<bytes>",
+    #                     help="Specify the expected upload size in bytes")
     parser.add_argument("-D", "--download", metavar="<file>",
                         help="Write firmware from <file> into device")
     parser.add_argument("-R", "--reset", action="store_true",
                         help="Issue USB Reset signalling once we're finished")
+    #  TODO: Not implemented
+    # parser.add_argument("-w", "--wait", action="store_true",
+    #                     help="Wait for device to appear")
     parser.add_argument("-s", "--dfuse-address", metavar="<address>",
                         help="ST DfuSe mode, specify target address "
                              "for raw file download or upload. "
                              "Not applicable for DfuSe file (.dfu) downloads")
+    #
+    #                         ST DfuSe mode string, specifying target
+    #                                 address for raw file download or upload (not
+    #                                 applicable for DfuSe file (.dfu) downloads).
+    #                                 Add more DfuSe options separated with ':'
+    #                 leave           Leave DFU mode (jump to application)
+    #                 mass-erase      Erase the whole device (requires "force")
+    #                 unprotect       Erase read protected device (requires "force")
+    #                 will-reset      Expect device to reset (e.g. option bytes write)
+    #                 force           You really know what you are doing!
+    #                 <length>        Length of firmware to upload from device
+    #
+    parser.add_argument("-y", "--yes-to-all", action="store_true",
+                        help="Say yes to all prompts")
+
+
+def main() -> None:
+    """Cli entry point"""
 
-    # Parse arguments
-    if argv[0] == __file__:
-        argv.pop(0)
-    args = parser.parse_args(argv)
-    verbose = False
+    # Create argument parser
+    parser = argparse.ArgumentParser(
+        prog="pydfuutil",
+        description="Python implementation of DFU-Util tools"
+    )
+    add_cli_options(parser)
+
+    print(f"v{__version__}")
+    # parse options
+    args = parser.parse_args()
     dif: dfu.DfuIf = dfu.DfuIf()
     file = dfu_file.DFUFile(None)
     mode = Mode.NONE
     device_id_filter = None
     alt_name = None
     transfer_size = 0
     dfuse_device = 0
     dfuse_options = None
     final_reset = 0
 
-    # func_dfu_rt = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
-    # func_dfu = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
     func_dfu_rt = usb_dfu.FuncDescriptor()
     func_dfu = usb_dfu.FuncDescriptor()
 
     if args.verbose:
-        verbose = True
         logger.setLevel(logging.DEBUG)
         usb_logger.setLevel(logging.DEBUG)
 
     if args.list:
         mode = Mode.LIST
 
     if args.detach:
@@ -606,19 +601,17 @@
     if args.device:
         device_id_filter = args.device
 
     if args.path:
         dif.path = args.path
         dif.flags |= dfu.Mode.IFF_PATH
         if ret := resolve_device_path(dif):
-            logger.error(f"unable to parse {args.path}")
-            sys.exit(2)
+            raise MisuseError(f"unable to parse {args.path}")
         if not ret:
-            logger.error(f"cannot find {args.path}")
-            sys.exit(1)
+            raise GeneralError(f"cannot find {args.path}")
 
     if args.cfg:
         dif.configuration = atoi(args.cfg)
         dif.flags |= dfu.Mode.IFF_CONFIG
 
     if args.intf:
         dif.interface = atoi(args.intf)
@@ -648,313 +641,261 @@
 
     if args.dfuse_address:
         dfuse_options = args.dfuse_address
 
     if mode == Mode.NONE:
         logger.error("You need to specify one of -D or -U\n\n")
         parser.print_help()
-        sys.exit(2)
+        raise MisuseError
 
     if device_id_filter:
         dif.vendor, dif.product = parse_vid_pid(device_id_filter)
         logger.info(f"Filter on VID = 0x{dif.vendor:04X} PID = 0x{dif.product:04X}\n")
         if dif.vendor:
             dif.flags |= dfu.Mode.IFF_VENDOR
         if dif.product:
             dif.flags |= dfu.Mode.IFF_PRODUCT
 
+    apply_all = args.yes_to_all
+
     # libusb init
     libusb_ctx = list(usb.core.find(find_all=True, **dif.device_ids))
 
     if mode == Mode.LIST:
+        logger.debug(mode)
         list_dfu_interfaces(libusb_ctx)
         sys.exit(0)
 
     dfu.init(5000)
 
     dfu_capable = iterate_dfu_devices(libusb_ctx, dif)
 
     if len(dfu_capable) == 0:
-        logger.error("No DFU capable USB device found")
-        sys.exit(1)
+        raise GeneralError("No DFU capable USB device found")
     elif len(dfu_capable) > 1:
         # We cannot safely support more than one DFU capable device
         # with same vendor/product ID, since during DFU we need to do
         # a USB bus reset, after which the target device will get a
         # new address */
-        logger.error("More than one DFU capable USB device found, "
-                     "you might try `--list' and then disconnect all but one "
-                     "device")
-        sys.exit(3)
+        raise CapabilityError("More than one DFU capable USB device found, "
+                              "you might try `--list' and then disconnect all but one "
+                              "device")
 
     # get_first_dfu_device
     if not (dev := dfu_capable[0]):
-        sys.exit(3)
+        raise CapabilityError("Can't get DFU capable USB device")
 
     # We have exactly one device. Its libusb_device is now in dif->dev
-
     logger.info("Opening DFU capable USB device... ")
 
-    _rt_dif: dfu.DfuIf = None
-
-    def get_first_dfu_if(dif_: dfu.DfuIf, v: Any = None):
-        nonlocal _rt_dif
-        _rt_dif = dif_
-        if not _rt_dif:
-            logger.error("Cannot open device")
-            sys.exit(1)
-
-    find_dfu_if(dev, get_first_dfu_if)
-    logger.debug(_rt_dif)
+    _rt_dif: dfu.DfuIf = get_first_dfu_if(dev)
 
     logger.info(f"ID 0x{_rt_dif.vendor:04X}:0x{_rt_dif.product:04X}")
 
     _quirks = quirks.set_quirks(_rt_dif.vendor, _rt_dif.product, _rt_dif.bcdDevice)
 
     # Obtain run-time DFU functional descriptor without asking device
     # E.g. Free runner does not like to be requested at this point
 
-    ret = get_cached_extra_descriptor(
-        _rt_dif.dev, _rt_dif.configuration, _rt_dif.interface,
-        usb_dfu.USB_DT_DFU, 0,
-        cpu_to_le16(func_dfu_rt.bcdDFUVersion)
-    )
-    ret = int_(ret)
+    ret = get_cached_extra_descriptor(_rt_dif, usb_dfu.USB_DT_DFU,
+                                      0, cpu_to_le16(func_dfu_rt.bcdDFUVersion))
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor "
                     "length")
         func_dfu_rt.bcdDFUVersion = 0x0100
     elif ret < 9:
-        logger.warning("Can not find cached DFU functional "
-                       "descriptor")
+        logger.warning("Can not find cached DFU functional descriptor")
         logger.warning("Assuming DFU version 1.0")
         func_dfu_rt.bcdDFUVersion = 0x0100
 
     logger.info(f"Run-time device DFU version 0x{func_dfu_rt.bcdDFUVersion:04X}")
 
     # Transition from run-Time mode to DFU mode
 
-    # status_again
-    def check_status():
+    def check_status(dfu_if: dfu.DfuIf):
+        # status_again
         logger.debug('Status again')
         _log_msg = "Determining device status: "
-        if int(status_ := dif.get_status()) < 0:
-            logger.error(f"{_log_msg}error get_status")
-            sys.exit(1)
+        if int(status_ := dfu_if.get_status()) < 0:
+            raise GeneralError(f"{_log_msg}error get_status")
         logger.info(f"{_log_msg}state = {status_.bState.to_string()}, "
                     f"status = {status_.bStatus}")
-
         if not _quirks & quirks.QUIRK_POLLTIMEOUT:
             milli_sleep(status_.bwPollTimeout)
         return status_
 
-    while not _rt_dif.flags & dfu.Mode.IFF_DFU:
+    if not _rt_dif.flags & dfu.Mode.IFF_DFU:
         # In the 'first round' during runtime mode, there can only be one
         # DFU Interface descriptor according to the DFU Spec.
-
-        # TODO: check if the selected device really has only one
+        # Note: future warning: check if the selected device really has only one
 
         logger.info("Claiming USB DFU Runtime Interface...")
         try:
             usb.util.claim_interface(_rt_dif.dev, _rt_dif.interface)
         except usb.core.USBError:
-            logger.error(f"Cannot claim interface {_rt_dif.interface}")
-            sys.exit(1)
+            raise GeneralError(f"Cannot claim interface {_rt_dif.interface}")
 
         try:
             _rt_dif.dev.set_interface_altsetting(_rt_dif.interface, 0)
         except usb.core.USBError:
-            logger.error("Cannot set alt interface zero")
-            sys.exit(1)
+            raise GeneralError("Cannot set alt interface zero")
 
-        status = check_status()
+        status = check_status(_rt_dif)
 
         if status.bState in (dfu.State.APP_IDLE, dfu.State.APP_DETACH):
             logger.info("Device really in Runtime Mode, send DFU "
                         "detach request...")
 
             if int_(_rt_dif.detach(1000)) < 0:
-                logger.error("error detaching")
-                sys.exit(1)
+                raise GeneralError("error detaching")
 
             if func_dfu_rt.bmAttributes & usb_dfu.BmAttributes.USB_DFU_WILL_DETACH:
                 logger.info("Device will detach and reattach...")
             else:
                 logger.info("Resetting USB...\n")
                 try:
                     _rt_dif.dev.reset()
                 except usb.core.USBError:
                     logger.error("error resetting after detach")
             milli_sleep(2000)
-            break  # TODO: wtf? break there?
         elif status.bState == dfu.State.DFU_ERROR:
             logger.error("dfuERROR, clearing status")
             if dfu.clear_status(_rt_dif.dev, _rt_dif.interface) < 0:
-                logger.error("error detaching")
-                sys.exit(1)
+                raise GeneralError("error detaching")
         else:
             logger.info("Runtime device already in DFU state ?!?")
-            break
 
         usb.util.release_interface(_rt_dif.dev, _rt_dif.interface)
         usb.util.dispose_resources(_rt_dif.dev)
 
         if mode == Mode.DETACH:
             usb.util.release_interface(_rt_dif.dev, _rt_dif.interface)
             usb.util.dispose_resources(_rt_dif.dev)
             sys.exit(0)
 
         if dif.flags & dfu.Mode.IFF_PATH:
             ret = resolve_device_path(dif)
-            if int_(ret) < 0:
-                logger.error(f"internal error: cannot re-parse {dif.path}")
-                sys.exit(1)
             if not ret:
-                logger.error("Cannot resolve path after RESET?")
-                sys.exit(1)
+                raise GeneralError("Cannot resolve path after RESET?")
+            if int_(ret) < 0:
+                raise GeneralError(f"internal error: cannot re-parse {dif.path}")
 
         dfu_capable = iterate_dfu_devices(libusb_ctx, dif)
         if len(dfu_capable) == 0:
-            logger.error("Lost device after RESET?")
-            sys.exit(1)
+            raise GeneralError("Lost device after RESET?")
         elif len(dfu_capable) > 1:
-            logger.error("More than one DFU capable USB "
-                         "device found, you might try `--list' and "
-                         "then disconnect all but one device")
-            sys.exit(1)
-
-    def get_first_detached_dfu_if(dif_: dfu.DfuIf, v: Any = None):
-        nonlocal dif
-        dif = dif_
-        if not dif:
-            logger.error("Cannot open device")
-            sys.exit(1)
+            raise GeneralError("More than one DFU capable USB "
+                               "device found, you might try `--list' and "
+                               "then disconnect all but one device")
 
-    find_dfu_if(dev, get_first_detached_dfu_if)
-    logger.debug(dif)
+    # get first detached dfu if
+    dif: dfu.DfuIf = get_first_dfu_if(dev)
 
+    logger.debug(dif)
     logger.info("Opening DFU USB Device...")
 
-    # we're already in DFU mode, so we can skip the detach/reset
-    # procedure
+    # we're already in DFU mode, so we can skip the detach/reset procedure
 
-    # dfustate
-    logger.debug('Dfu state...')
+    logger.debug('Dfu state...')  # dfustate
 
     if alt_name:
-        if not (n := find_dfu_if(dif.dev, alt_by_name, alt_name)):
-            logger.error(f"No such Alternate Setting: {alt_name}")
-            sys.exit(1)
+        n = next((alt_by_name(dfu_if, alt_name) for dfu_if in find_dfu_if(dev)), None)
+        if not n:
+            raise GeneralError(f"No such Alternate Setting: {alt_name}")
         if n < 0:
-            logger.error(f"Error {n} in name lookup")
-            sys.exit(1)
+            raise GeneralError(f"Error {n} in name lookup")
         dif.altsetting = n - 1
 
     if (num_ifs := count_matching_dfu_if(dif)) < 0:
-        logger.error("No matching DFU Interface after RESET?!?")
-        sys.exit(1)
+        raise GeneralError("No matching DFU Interface after RESET?!?")
     elif num_ifs > 1:
         logger.warning("Detected interfaces after DFU transition")
         list_dfu_interfaces(libusb_ctx)
-        logger.error(f"We have {num_ifs} DFU Interfaces/Altsettings,"
-                     " you have to specify one via --intf / --alt"
-                     " options")
-        sys.exit(1)
+        raise GeneralError(f"We have {num_ifs} DFU Interfaces/Altsettings,"
+                           " you have to specify one via --intf / --alt"
+                           " options")
 
     if not get_matching_dfu_if(dif):
-        logger.error("Can't find the matching DFU interface/altsetting")
-        sys.exit(1)
+        raise GeneralError("Can't find the matching DFU interface/altsetting")
 
-    print_dfu_if(dif, None)
+    print_dfu_if(dif)
     if (active_alt_name := get_alt_name(dif)) and len(active_alt_name) > 0:
         dif.alt_name = active_alt_name
     else:
         dif.alt_name = None
 
     # # Note: uncomment on need
     # logger.info(f"Setting Configuration {dif.configuration}...")
     # try:
     #     dif.dev.set_configuration(dif.configuration)
     # except usb.core.USBError as e:
-    #     logger.error("Cannot set configuration")
-    #     sys.exit(1)
+    #     raise GeneralError("Cannot set configuration")
 
     logger.info("Claiming USB DFU Interface...")
     try:
         usb.util.claim_interface(dif.dev, dif.interface)
     except usb.core.USBError:
-        logger.error("Cannot claim interface")
-        sys.exit(1)
+        raise GeneralError("Cannot claim interface")
 
     logger.info(f"Setting Alternate Setting {dif.altsetting} ...\n")
     try:
         dif.dev.set_interface_altsetting(dif.interface, dif.altsetting)
     except usb.core.USBError:
-        logger.error("Cannot set alternate interface")
-        sys.exit(1)
+        raise GeneralError("Cannot set alternate interface")
 
-    status = check_status()
+    status = check_status(dif)
     while status.bState != dfu.State.DFU_IDLE:
 
         if status.bState in (dfu.State.APP_IDLE, dfu.State.APP_DETACH):
-            logger.error("Device still in Runtime Mode!")
-            sys.exit(1)
+            raise GeneralError("Device still in Runtime Mode!")
 
         elif status.bState == dfu.State.DFU_ERROR:
             logger.error("dfuERROR, clearing status")
             if dfu.clear_status(dif.dev, dif.interface) < 0:
-                logger.error("error clear_status")
-                sys.exit(1)
+                raise GeneralError("error clear_status")
 
-            status = check_status()
+            status = check_status(dif)
 
         elif status.bState == (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_UPLOAD_IDLE):
             logger.warning("aborting previous incomplete transfer")
             if dif.abort() < 0:
-                logger.error("can't send DFU_ABORT")
-                sys.exit(1)
+                raise GeneralError("can't send DFU_ABORT")
 
-            status = check_status()
+            status = check_status(dif)
 
         elif status.bState == dfu.State.DFU_IDLE:
             logger.info("dfuIDLE, continuing")
             break
 
     if status.bStatus != dfu.Status.OK:
         logger.warning(f"DFU Status: {status.bStatus.to_string()}")
 
         # Clear our status & try again.
         dfu.clear_status(dif.dev, dif.interface)
         _ = int(status := dif.get_status())
         if status.bStatus != dfu.Status.OK:
-            logger.error(f"{status.bStatus}")
-            sys.exit(1)
+            raise GeneralError(f"{status.bStatus}")
         if not _quirks & quirks.QUIRK_POLLTIMEOUT:
             milli_sleep(status.bwPollTimeout)
 
     logger.debug(f"State: {status.bState.to_string()}, "
                  f"Status: {status.bStatus.to_string()} Continue...")
 
     # Get the DFU mode DFU functional descriptor
     # If it is not found cached, we will request it from the device
 
-    ret = get_cached_extra_descriptor(
-        dif.dev, dif.configuration, dif.interface,
-        usb_dfu.USB_DT_DFU, 0, cpu_to_le16(func_dfu.bcdDFUVersion)
-    )
-    ret = int_(ret)
-
+    ret = get_cached_extra_descriptor(dif, usb_dfu.USB_DT_DFU,
+                                      0, cpu_to_le16(func_dfu.bcdDFUVersion))
     if ret < 7:
         logger.error("obtaining cached DFU functional descriptor")
         ret = usb_get_any_descriptor(
             dif.dev, usb_dfu.USB_DT_DFU, 0,
             cpu_to_le16(func_dfu_rt.bcdDFUVersion)
         )
         ret = int_(ret)
-
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor length")
         func_dfu.bcdDFUVersion = 0x0100
     elif ret < 9:
         logger.error("Error obtaining DFU functional descriptor")
         logger.info("Please report this as a bug!")
         logger.warning("Assuming DFU version 1.0")
@@ -967,112 +908,120 @@
 
     logger.info(f"DFU mode device DFU version  0x{func_dfu.bcdDFUVersion:04X}")
 
     if func_dfu.bcdDFUVersion == 0x11a:
         dfuse_device = 1
 
     # If not overridden by the user
+    # FIXME: can't got how the total size specified
     if transfer_size:
         logger.info(f"Device returned transfer size {transfer_size}")
     else:
-        logger.error("Transfer size must be specified")
-        sys.exit(1)
+        raise GeneralError("Transfer size must be specified")
 
     # autotools lie when cross-compiling for Windows using mingw32/64
     if HAVE_GET_PAGESIZE:
         # limitation of Linux usbdevio
         page_size = os.sysconf(os.sysconf_names['SC_PAGE_SIZE'])
         if transfer_size > page_size:
             transfer_size = page_size
             logger.info(f"Limited transfer size to {transfer_size}")
 
     # DFU specification
     # if dif.dev:  # strange think, unreachable
-    #     logger.error(f"Failed to get device descriptor")
-    #     sys.exit(1)
+    #     raise GeneralError(f"Failed to get device descriptor")
 
     # pylint: disable=no-member
     if transfer_size < dif.dev.bMaxPacketSize0:
         logger.info(f"Adjusted transfer size to {transfer_size}")
 
     if mode == Mode.UPLOAD:
         # open for "exclusive" writing in a portable way
         try:
-            with open(file.name, "ab") as file.file_p:
-                if os.path.getsize(file.name) != 0:
-                    logger.info(f"{file.name}: File exists")
-                    sys.exit(1)
+            file_mode = "ab"
+            if os.path.isfile(file.name) and os.path.getsize(file.name) != 0:
+                # ask to overwrite file that exist
+                if not apply_all:
+                    _y = input(f"{file.name} File exists, print `yes` to overwrite: ")
+                    if not _y.lower() in ('y', 'yes'):
+                        raise GeneralError(f"{file.name}: File exists")
+                file_mode = 'wb'
+
+            with open(file.name, file_mode) as file.file_p:
 
                 if dfuse_device or dfuse_options:
                     if dfuse.do_upload(dif, transfer_size, file, dfuse_options) < 0:
-                        sys.exit(1)
+                        raise GeneralError
                 else:
                     if dfu_load.do_upload(dif, transfer_size, file) < 0:
-                        sys.exit(1)
+                        raise GeneralError
 
         except OSError as e:
-            logger.error(e)
-            sys.exit(1)
+            raise GeneralError(e)
 
     elif mode == Mode.DOWNLOAD:
         try:
             # Open file for reading in binary mode
             with open(file.name, "rb") as file_p:
                 if not file_p:
-                    logger.error(f"Error: Failed to open {file.name}")
-                    sys.exit(1)
+                    raise GeneralError(f"Error: Failed to open {file.name}")
 
                 # Parse DFU suffix
                 # ret = dfu_file.parse_dfu_suffix(file)
                 ret = file.parse_dfu_suffix()
                 if ret < 0:
-                    sys.exit(1)
+                    raise GeneralError
                 elif ret == 0:
                     logger.warning("File has no DFU suffix")
                 elif file.bcdDFU not in (0x0100, 0x011a):
-                    logger.error(f"Unsupported DFU file revision 0x{file.bcdDFU:04x}")
-                    sys.exit(1)
+                    raise GeneralError(f"Unsupported DFU file revision 0x{file.bcdDFU:04x}")
 
                 # Check vendor ID
                 if file.idVendor not in (0xffff, dif.vendor):
                     logger.warning(f"Warning: File vendor ID 0x{file.idVendor:04x} "
                                    f"does not match device 0x{dif.vendor:04x}")
 
                 # Check product ID
                 if file.idProduct not in (0xffff, dif.product):
                     logger.warning(f"File product ID 0x{file.idProduct:04x} "
                                    f"does not match device 0x{dif.product:04x}")
 
                 # Perform download based on conditions
                 if dfuse_device or dfuse_options or file.bcdDFU == 0x011a:
                     if dfuse.do_dnload(dif, transfer_size, file, dfuse_options) < 0:
-                        sys.exit(1)
+                        raise GeneralError
                 else:
-                    if dfu_load.do_dnload(dif, transfer_size, file, _quirks, verbose) < 0:
-                        sys.exit(1)
+                    if dfu_load.do_dnload(dif, transfer_size, file, _quirks) < 0:
+                        raise GeneralError
 
         except OSError as e:
-            logger.error(e)
-            sys.exit(1)
+            raise GeneralError(e)
 
     else:
-        logger.error(f"Unsupported mode: {mode}")
-        sys.exit(1)
+        raise GeneralError(f"Unsupported mode: {mode}")
 
     if final_reset:
         # if IntOrBytes(dfu.detach(dif.dev, dif.interface, 1000)) < 0:
         if int_(dif.detach(1000)) < 0:
             logger.error("can't detach")
         logger.info("Resetting USB to switch back to runtime mode")
         try:
             dif.dev.reset()
         except usb.core.USBError as e:
             logger.error("error resetting after download")
             logger.debug(e)
 
     usb.util.release_interface(dif.dev, dif.interface)
     usb.util.dispose_resources(dif.dev)
-    sys.exit(0)
 
 
 if __name__ == '__main__':
-    main(sys.argv)
+    try:
+        main()
+    except GeneralError as err:
+        if err.__str__():
+            logger.error(err)
+        sys.exit(err.exit_code)
+    except Exception as err:
+        logger.error(err)
+        sys.exit(1)
+    sys.exit(0)
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil/dfu.py` & `pydfuutil-0.0.3/pydfuutil/dfu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 """
-low-level DFU message sending routines (part of dfu-programmer).
+Low-level DFU communication routines (part of dfu-programmer).
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
+
+This program is free software; you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation; either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program; if not, write to the Free Software
+Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 
-import inspect
-import logging
+# import inspect
+import sys
 from dataclasses import dataclass
 from enum import IntEnum, IntFlag
 
 import usb.util
 
 from pydfuutil.logger import logger
-
+from pydfuutil.portable import milli_sleep
+from pydfuutil.usb_dfu import FuncDescriptor
 
 _logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
-_logger.setLevel(logging.DEBUG)
 
 
 class State(IntEnum):
     """Dfu states"""
     APP_IDLE = 0x00
     APP_DETACH = 0x01
     DFU_IDLE = 0x02
@@ -36,27 +50,15 @@
     def to_string(self):
         """
         :return: State.self name by State Enum
         """
         return state_to_string(self)
 
 
-_STATES_NAMES = {
-    State.APP_IDLE: 'appIDLE',
-    State.APP_DETACH: 'appDETACH',
-    State.DFU_IDLE: 'dfuIDLE',
-    State.DFU_DOWNLOAD_SYNC: 'dfuDNLOAD-SYNC',
-    State.DFU_DOWNLOAD_BUSY: 'dfuDNBUSY',
-    State.DFU_DOWNLOAD_IDLE: 'dfuDNLOAD-IDLE',
-    State.DFU_MANIFEST_SYNC: 'dfuMANIFEST-SYNC',
-    State.DFU_MANIFEST: 'dfuMANIFEST',
-    State.DFU_MANIFEST_WAIT_RESET: 'dfuMANIFEST-WAIT-RESET',
-    State.DFU_UPLOAD_IDLE: 'dfuUPLOAD-IDLE',
-    State.DFU_ERROR: 'dfuERROR',
-}
+
 
 
 class Status(IntEnum):
     """Dfu statuses"""
     OK = 0x00
     ERROR_TARGET = 0x01
     ERROR_FILE = 0x02
@@ -77,37 +79,14 @@
     def to_string(self):
         """
         :return: Status.self name by Status Enum
         """
         return status_to_string(self)
 
 
-_DFU_STATUS_NAMES = {
-    Status.OK: "No error condition is present",
-    Status.ERROR_TARGET: "File is not targeted for use by this device",
-    Status.ERROR_FILE: "File is for this device but fails some vendor-specific test",
-    Status.ERROR_WRITE: "Device is unable to write memory",
-    Status.ERROR_ERASE: "Memory erase function failed",
-    Status.ERROR_CHECK_ERASED: "Memory erase check failed",
-    Status.ERROR_PROG: "Program memory function failed",
-    Status.ERROR_VERIFY: "Programmed memory failed verification",
-    Status.ERROR_ADDRESS: "Cannot program memory due to received address that is out of range",
-    Status.ERROR_NOTDONE: "Received DNLOAD with wLength = 0, "
-                          "but device does not think that it has all data yet",
-    Status.ERROR_FIRMWARE: "Device's firmware is corrupt. "
-                           "It cannot return to run-time (non-DFU) operations",
-    Status.ERROR_VENDOR: "iString indicates a vendor specific error",
-    Status.ERROR_USBR: "Device detected unexpected USB reset signalling",
-    Status.ERROR_POR: "Device detected unexpected power on reset",
-    Status.ERROR_UNKNOWN: "Something went wrong, but the device does not know what it was",
-    Status.ERROR_STALLEDPKT: "Device stalled an unexpected request"
-
-}
-
-
 class Command(IntEnum):
     """Dfu commands"""
     DETACH = 0
     DNLOAD = 1
     UPLOAD = 2
     GETSTATUS = 3
     CLRSTATUS = 4
@@ -122,20 +101,24 @@
     IFF_VENDOR = 0x0100
     IFF_PRODUCT = 0x0200
     IFF_CONFIG = 0x0400
     IFF_IFACE = 0x0800
     IFF_ALT = 0x1000
     IFF_DEVNUM = 0x2000
     IFF_PATH = 0x4000
+    # DFU_IFF_DFU = 0x0001  /* DFU Mode, (not Runtime) */
+    # DFU_IFF_ALT = 0x0002  /* Multiple alternate settings */
 
 
 @dataclass(frozen=True)
 class StatusRetVal:
     """
     Converts dfu_get_status result bytes to applicable dataclass
+    This is based off of DFU_GETSTATUS
+    the data structure to be populated with the results
     """
     # pylint: disable=invalid-name
     bStatus: Status = Status.ERROR_UNKNOWN
     bwPollTimeout: int = 0
     bState: State = State.DFU_ERROR
     iString: int = 0
 
@@ -168,31 +151,34 @@
 
     def __int__(self):
         return int.from_bytes(self, 'little')
 
 
 @dataclass
 class DfuIf:  # pylint: disable=too-many-instance-attributes
-
     """DFU Interface dataclass"""
     # pylint: disable=invalid-name
-
     vendor: int = None
     product: int = None
     bcdDevice: int = None
     configuration: int = None
     interface: int = None
     altsetting: int = None
     alt_name: str = None
     bus: int = None
     devnum: int = None
     path: [str, int] = None
-    flags: [Mode, int] = None
+    flags: [Mode, int] = 0
     count: int = None
     dev: usb.core.Device = None
+    quirks: int = None
+    bwPollTimeout: int = 0
+    serial_name: str = ""
+    usb_dfu_func_desc: FuncDescriptor = None
+
 
     @property
     def device_ids(self) -> dict:
         """Returns filter dict for usb.core.find() by VID:PID"""
         id_filter = {}
         if self.vendor:
             id_filter["idVendor"] = self.vendor
@@ -223,14 +209,18 @@
         """Binds self to dfu.get_status()"""
         return get_status(self.dev, self.interface)
 
     def get_state(self) -> State:
         """Binds self to dfu.get_state()"""
         return get_state(self.dev, self.interface)
 
+    def abort_to_idle(self):
+        """Binds self to dfu.abort_to_idle()"""
+        return abort_to_idle(self)
+
 
 def init(timeout: int) -> None:
     """
     Initiate dfu_util library with specified commands timeout
     :param timeout in milliseconds
     :return: None
     """
@@ -241,26 +231,26 @@
     if timeout > 0:
         TIMEOUT = timeout
     else:
         if 0 != DEBUG_LEVEL:
             raise ValueError(f"dfu_init: Invalid timeout value {timeout}")
 
 
-def verify_init() -> int:
-    """
-    Verifies provided TIMEOUT and DEBUG_LEVEL
-    NOTE: (function: typing.Callable) not needed cause python can get it from stack
-    :raise ValueError with caller function name
-    :return: 0
-    """
-    caller = inspect.stack()[0][3]
-    if INVALID_DFU_TIMEOUT == TIMEOUT:
-        if 0 != DEBUG_LEVEL:
-            raise ValueError(f'"{caller}": dfu system not initialized properly.')
-    return 0
+# def verify_init() -> int:
+#     """
+#     Verifies provided TIMEOUT and DEBUG_LEVEL
+#     NOTE: (function: typing.Callable) not needed cause python can get it from stack
+#     :raise ValueError with caller function name
+#     :return: 0
+#     """
+#     caller = inspect.stack()[0][3]
+#     if INVALID_DFU_TIMEOUT == TIMEOUT:
+#         if 0 != DEBUG_LEVEL:
+#             raise ValueError(f'"{caller}": dfu system not initialized properly.')
+#     return 0
 
 
 def debug(level: int) -> None:
     """
     NOTE: Maybe not needed cause python can define globals after
     :param level: logging level (DEBUG, INFO, WARNING, ERROR)
     """
@@ -269,32 +259,24 @@
     global DEBUG_LEVEL
     DEBUG_LEVEL = level
     _logger.setLevel(level)
 
 
 def detach(device: usb.core.Device, interface: int, timeout: int) -> bytes:
     """
-
-     *  DETACH Request (DFU Spec 1.0, Section 5.1)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *  timeout   - the timeout in ms the USB device should wait for a pending
-     *              USB reset before giving up and terminating the operation
-     *
-     *  returns 0 or < 0 on error
+    DETACH Request (DFU Spec 1.0, Section 5.1)
 
     Sends to device command to switch it to DFU mode
     u have to free device and handle it again
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
-    :param timeout: timeout to dfu detach
-    :return: returns error code
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
+    :param timeout: the timeout in ms the USB device should wait for a pending
+    :return: bytes or < 0 on error
     """
-    verify_init()
+    # verify_init()
     _logger.debug('DETACH...')
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.DETACH,
         wValue=timeout,
@@ -307,32 +289,24 @@
 
 
 def download(device: usb.core.Device,
              interface: int,
              transaction: int,
              data_or_length: [bytes, int]) -> int:
     """
-     *  DNLOAD Request (DFU Spec 1.0, Section 6.1.1)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *  length    - the total number of bytes to transfer to the USB
-     *              device - must be less than wTransferSize
-     *  data      - the data to transfer
-     *
-     *  returns the number of bytes written or < 0 on error
+    DNLOAD Request (DFU Spec 1.0, Section 6.1.1)
 
     Download data to special page of DFU device
-    :param device: usb.core.Device
-    :param interface: usb.core.interface.bInterfaceNumber
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
     :param transaction: start page int(total_data_size/xfer_size)
-    :param data_or_length: page size bytes(xfer_size) or xfer_size
+    :param data_or_length: the data to transfer
     :return: downloaded data or error code in bytes
     """
-    verify_init()
+    # verify_init()
     _logger.debug('DFU_DOWNLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.DNLOAD,
@@ -347,32 +321,24 @@
 
 
 def upload(device: usb.core.Device,
            interface: int,
            transaction: int,
            data_or_length: [bytes, int]) -> bytes:
     """
-     *  UPLOAD Request (DFU Spec 1.0, Section 6.2)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *  length    - the maximum number of bytes to receive from the USB
-     *              device - must be less than wTransferSize
-     *  data      - the buffer to put the received data in
-     *
-     *  returns the number of bytes received or < 0 on error
+    UPLOAD Request (DFU Spec 1.0, Section 6.2)
 
     Uploads data from special page of DFU device
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
     :param transaction: start page int(total_data_size/xfer_size)
-    :param data_or_length: page size bytes(xfer_size) or xfer_size
-    :return: uploaded data or error code in bytes
+    :param data_or_length: the buffer to put the received data in
+    :return: uploaded bytes or < 0 on error
     """
-    verify_init()
+    # verify_init()
     _logger.debug('UPLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.UPLOAD,
@@ -385,28 +351,22 @@
     _logger.debug(f'UPLOAD {len(result) >= 0}')
 
     return result.tobytes()
 
 
 def get_status(device: usb.core.Device, interface: int) -> StatusRetVal:
     """
-     *  GETSTATUS Request (DFU Spec 1.0, Section 6.1.2)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *  status    - the data structure to be populated with the results
-     *
-     *  return the number of bytes read in or < 0 on an error
+     GETSTATUS Request (DFU Spec 1.0, Section 6.1.2)
 
     Returns DFU interface status
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
-    :return: error code and _STATUS [Container, dict] object
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
+    :return: StatusRetVal
     """
-    verify_init()
+    # verify_init()
     _logger.debug('DFU_GET_STATUS...')
 
     length = 6
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
@@ -423,27 +383,22 @@
         _logger.debug(f'CURRENT STATE {status.bState.to_string()}')
         return status
     return StatusRetVal.from_bytes(result)
 
 
 def clear_status(device: usb.core.Device, interface: int) -> int:
     """
-     *  CLRSTATUS Request (DFU Spec 1.0, Section 6.1.3)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *
-     *  return 0 or < 0 on an error
+    CLRSTATUS Request (DFU Spec 1.0, Section 6.1.3)
 
     Clears DFU interface status
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
-    :return: error code
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
+    :return: return 0 or < 0 on an error
     """
-    verify_init()
+    # verify_init()
     _logger.debug('CLEAR_STATUS...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.CLRSTATUS,
@@ -455,30 +410,22 @@
     _logger.debug(f'CLEAR_STATUS {result >= 0}')
 
     return result
 
 
 def get_state(device: usb.core.Device, interface: int) -> [State, int]:
     """
-     *  GETSTATE Request (DFU Spec 1.0, Section 6.1.5)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *  length    - the maximum number of bytes to receive from the USB
-     *              device - must be less than wTransferSize
-     *  data      - the buffer to put the received data in
-     *
-     *  returns the state or < 0 on error
+    GETSTATE Request (DFU Spec 1.0, Section 6.1.5)
 
     Returns DFU interface state
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
-    :return: dfu state or error code
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
+    :return: returns the state or < 0 on error
     """
-    verify_init()
+    # verify_init()
 
     length = 1
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.GETSTATE,
@@ -493,27 +440,22 @@
     if value in State.__members__.values():
         value = State(value)
     return value
 
 
 def abort(device: usb.core.Device, interface: int) -> int:
     """
-     *  ABORT Request (DFU Spec 1.0, Section 6.1.4)
-     *
-     *  device    - the usb_dev_handle to communicate with
-     *  interface - the interface to communicate with
-     *
-     *  returns 0 or < 0 on an error
+    ABORT Request (DFU Spec 1.0, Section 6.1.4)
 
     Aborts DFU command
-    :param device: usb.core.Device
-    :param interface: usb.core.Interface.bInterfaceNumber
-    :return: error code
+    :param device: the usb_dev_handle to communicate with
+    :param interface: the interface to communicate with
+    :return: returns 0 or < 0 on an error
     """
-    verify_init()
+    # verify_init()
     _logger.debug('ABORT...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.ABORT,
@@ -546,14 +488,65 @@
     """
     try:
         return _DFU_STATUS_NAMES[Status(status)]
     except (ValueError, KeyError):
         return None
 
 
+_STATES_NAMES = {
+    State.APP_IDLE: 'appIDLE',
+    State.APP_DETACH: 'appDETACH',
+    State.DFU_IDLE: 'dfuIDLE',
+    State.DFU_DOWNLOAD_SYNC: 'dfuDNLOAD-SYNC',
+    State.DFU_DOWNLOAD_BUSY: 'dfuDNBUSY',
+    State.DFU_DOWNLOAD_IDLE: 'dfuDNLOAD-IDLE',
+    State.DFU_MANIFEST_SYNC: 'dfuMANIFEST-SYNC',
+    State.DFU_MANIFEST: 'dfuMANIFEST',
+    State.DFU_MANIFEST_WAIT_RESET: 'dfuMANIFEST-WAIT-RESET',
+    State.DFU_UPLOAD_IDLE: 'dfuUPLOAD-IDLE',
+    State.DFU_ERROR: 'dfuERROR',
+}
+
+
+_DFU_STATUS_NAMES = {
+    Status.OK: "No error condition is present",
+    Status.ERROR_TARGET: "File is not targeted for use by this device",
+    Status.ERROR_FILE: "File is for this device but fails some vendor-specific test",
+    Status.ERROR_WRITE: "Device is unable to write memory",
+    Status.ERROR_ERASE: "Memory erase function failed",
+    Status.ERROR_CHECK_ERASED: "Memory erase check failed",
+    Status.ERROR_PROG: "Program memory function failed",
+    Status.ERROR_VERIFY: "Programmed memory failed verification",
+    Status.ERROR_ADDRESS: "Cannot program memory due to received address that is out of range",
+    Status.ERROR_NOTDONE: "Received DNLOAD with wLength = 0, "
+                          "but device does not think that it has all data yet",
+    Status.ERROR_FIRMWARE: "Device's firmware is corrupt. "
+                           "It cannot return to run-time (non-DFU) operations",
+    Status.ERROR_VENDOR: "iString indicates a vendor specific error",
+    Status.ERROR_USBR: "Device detected unexpected USB reset signalling",
+    Status.ERROR_POR: "Device detected unexpected power on reset",
+    Status.ERROR_UNKNOWN: "Something went wrong, but the device does not know what it was",
+    Status.ERROR_STALLEDPKT: "Device stalled an unexpected request"
+}
+
+
+def abort_to_idle(dif: DfuIf):
+    if dif.abort() < 0:
+        _logger.error("Error sending dfu abort request")
+        sys.exit(1)
+    if (ret := int(dst := dif.get_status())) < 0:
+        _logger.error("Error during abort get_status")
+        sys.exit(1)
+    if dst.bState != State.DFU_IDLE:
+        _logger.error("Failed to enter idle state on abort")
+        sys.exit(1)
+    milli_sleep(dst.bwPollTimeout)
+    return ret
+
+
 # global definitions
 DEBUG: int = 0
 
 INVALID_DFU_TIMEOUT = -1
 
 TIMEOUT: int = INVALID_DFU_TIMEOUT
 TRANSACTION: int = 0
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil/dfuse.py` & `pydfuutil-0.0.3/pydfuutil/dfuse.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from enum import Enum
 
 import usb.util
 
 from pydfuutil import dfu
 from pydfuutil.dfu_file import DFUFile
 from pydfuutil.dfuse_mem import find_segment, DFUSE, parse_memory_layout, MemSegment
+from pydfuutil.exceptions import GeneralError
 from pydfuutil.logger import logger
 from pydfuutil.portable import milli_sleep
+from pydfuutil.progress import Progress
 
 _logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 VERBOSE = False
 MEM_LAYOUT: [MemSegment, None] = None
 
 TIMEOUT = 5000
@@ -148,15 +150,15 @@
             raise IOError("Error during abort get_status")
 
         if dst.bState != dfu.State.DFU_IDLE:
             raise IOError("Failed to enter idle state on abort")
 
     except (ValueError, IOError) as err:
         _logger.error(err)
-        sys.exit(1)
+        raise GeneralError
 
     milli_sleep(dst.bwPollTimeout)
     return ret
 
 
 def upload(dif: dfu.DfuIf, data: bytes, transaction: int) -> int:
     """
@@ -209,15 +211,14 @@
                      f"libusb_control_transfer returned {status}")
 
     return status
 
 
 def do_upload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, dfuse_options: [str, bytes]) -> int:
     """
-    TODO: implementation
     :param dif:
     :param xfer_size:
     :param file:
     :param dfuse_options:
     :return:
     """
 
@@ -253,42 +254,50 @@
         else:
             # Bootloader decides the start address, unknown to us
             # Use a short length to lower risk of running out of bounds
             if not upload_limit:
                 upload_limit = 0x4000
             _logger.info("Limiting default upload to %i bytes", upload_limit)
 
-        _logger.info(f"bytes_per_hash={xfer_size}")
-        print("Starting upload: [")  # TODO: Progress
     except (ValueError, IOError) as err:
         _logger.error(err)
         return -1
 
-    while True:
-        xfer_size = min(xfer_size, upload_limit - total_bytes)
-        rc = upload(dif, buf, transaction)
-        if rc < 0:
-            _logger.error("Error during upload")
-            ret = rc
-            break
-        write_rc = file.file_p.write(buf[:rc])
-        if write_rc < rc:
-            _logger.error(f"Short file write: {rc}")
-            ret = -1
-            break
-        total_bytes += rc
-        if rc < xfer_size or total_bytes >= upload_limit:
-            # Last block, return successfully
-            ret = total_bytes
-            break
-        print("#")
-        transaction += 1
+    try:
+        with Progress() as progress:
+            progress.start_task(
+                description="Starting upload",
+                total=total_bytes
+            )
+            while True:
+                xfer_size = min(xfer_size, upload_limit - total_bytes)
+                rc = upload(dif, buf, transaction)
+                if rc < 0:
+                    _logger.error("Error during upload")
+                    ret = rc
+                    break
+                write_rc = file.file_p.write(buf[:rc])
+                if write_rc < rc:
+                    _logger.error(f"Short file write: {rc}")
+                    ret = -1
+                    break
+                total_bytes += rc
+                if rc < xfer_size or total_bytes >= upload_limit:
+                    # Last block, return successfully
+                    ret = total_bytes
+                    break
 
-    print("] finished!")
-    return ret
+                progress.update(description="Uploading...", advance=xfer_size)
+                transaction += 1
+
+            progress.update(description="Upload finished!")
+            return ret
+    except Exception as e:
+        logger.error(e)
+        return -1
 
 
 def dnload_chunk(dif: dfu.DfuIf, data: bytes, size: int, transaction: int) -> int:
     """
     Download a chunk of data during DFU download operation.
 
     :param dif: DfuIf object representing the DFU interface
@@ -533,15 +542,15 @@
             if not opts.force:
                 raise PermissionError("The mass erase command can only be used with force")
             _logger.info("Performing mass erase, this can take a moment")
             special_command(dif, 0, Command.MASS_ERASE)
 
     except (ValueError, PermissionError, IOError) as err:
         _logger.error(err)
-        sys.exit(1)
+        raise GeneralError
 
     if opts.address:
         if file.bcdDFU == 0x11a:
             _logger.error("This is a DfuSe file, not meant for raw download")
             return -1
         ret = do_bin_dnload(dif, xfer_size, file, opts.address)
     else:
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil/dfuse_mem.py` & `pydfuutil-0.0.3/pydfuutil/dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/pydfuutil/lmdfu.py` & `pydfuutil-0.0.3/pydfuutil/lmdfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/pydfuutil/progress.py` & `pydfuutil-0.0.3/pydfuutil/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Progress bar utilities"""
 
 
 import sys
 from abc import ABC, abstractmethod
 
+
+
 try:
     from rich import progress as RICH_PROGRESS
 except ImportError:
     try:
         from pip._vendor.rich import progress as RICH_PROGRESS
     except ImportError:
         RICH_PROGRESS = None
 
 try:
     from tqdm import tqdm as TQDM_PROGRESS
 except ImportError:
     TQDM_PROGRESS = None
 
+
 import logging
 
+
 _logger = logging.getLogger('progress')
 _logger.setLevel(logging.INFO)
 
 
 class AbstractProgressBackend(ABC):
     """Abstract class for progress bar backends"""
 
@@ -87,106 +91,143 @@
     REDIRECT_STD = True
 
     def __init__(self):
         super().__init__()
         self._value = None
         self._total = None
         self._rate = None
+        self._fail = None
 
     def _print(self, symbol: str):
         if self.REDIRECT_STD:
             sys.stdout.write(symbol)
             sys.stdout.flush()
         else:
             print(symbol, end="", flush=True)
 
     def start(self):
         pass
 
     def start_task(self, *, description: str = None, total: int = None):
         self._value = 0
         self._total = total
-        self._rate = self._total / self.BAR_WIDTH
+        self._fail = False
+        if self._total:
+            self._rate = self._total / self.BAR_WIDTH
         self._print(f"{description} [")
 
     def update(self, *, description: str = None, advance: int = None, completed: int = None):
-        if advance:
-            self._value += advance
-            if self._rate != 0 and self._value % self._rate != 0:
-                # self._print("#")
-                self._print("━")
-        if completed:
-            if completed < self._value:
-                raise ValueError(f"The progress can't run backward! "
-                                 f"{completed} < {self._value}")
-            self._value = completed
-            self._print("#" * (completed - self._value) // self._rate)
-        if self._total == self._value and (advance or completed):
-            self._print("] Complete!\n")
+        if self._total:
+
+            if advance:
+                self._value += advance
+                if self._rate != 0 and advance % self._rate != 0:
+                    self._print("━" * int(advance / self._rate))
+            if completed:
+                if completed < self._value:
+                    raise ValueError(f"The progress can't run backward! "
+                                     f"{completed} < {self._value}")
+                prev_value = self._value
+                self._value = completed
+                if (delta := self._value - prev_value) > 0:
+                    if delta % self._rate != 0:
+                        self._print("━" * int(delta / self._rate))
+            if self._total <= self._value and (advance or completed):
+                self._print("] Complete!\n")
+        else:
+            self._print("━")
 
     def fail(self):
         self._print("] Failed!\n")
 
     def stop(self):
-        pass
+        if not self._total and not self._fail:
+            self._print("] Complete!\n")
 
 
 class TqdmBackend(AbstractProgressBackend):
     """tqdm based progress bar backend"""
 
     BAR_FORMAT = ("{desc} {bar:20} {percentage:3.0f}% "
                   "{remaining} {n_fmt}/{total_fmt} bytes {rate_fmt}")
+    BAR_FORMAT_INF = "{desc} {postfix} {n_fmt}/{total_fmt} bytes {rate_fmt}"
 
     def __init__(self):
         super().__init__()
         self._progress = None
         self._value = None
+        self._spinner_state = None
 
     def start(self):
         pass
 
     def start_task(self, *, description: str = None, total: int = None):
         self._value = 0
-        self._progress = TQDM_PROGRESS(
-            total=total,
-            unit=' bytes',
-            desc=description,
-            bar_format=TqdmBackend.BAR_FORMAT,
-            colour="magenta",
-            ascii=' ━',
-        )
+        if total:
+            self._progress = TQDM_PROGRESS(
+                total=total,
+                unit=' bytes',
+                desc=description,
+                bar_format=TqdmBackend.BAR_FORMAT,
+                ascii=' ━',
+            )
+        else:
+            self._progress = TQDM_PROGRESS(
+                total=float('inf'),
+                unit=' bytes',
+                desc=description,
+                bar_format=TqdmBackend.BAR_FORMAT_INF,
+                postfix=""
+            )
+            self._spinner_state = 0
+
+    def _spin(self, complete=False):
+        if complete:
+            self._progress.postfix = "━" * 20
+            return
+
+        symbol = "=▶" if self._spinner_state % 2 == 1 else "▶="
+        self._progress.postfix = symbol * 10
+        self._spinner_state += 1
 
     def update(self, *, description: str = None, advance: int = None, completed: int = None):
         if description:
-            self._progress.description = description
+            self._progress.desc = description
+
         if advance:
             self._progress.update(advance)
         if completed:
             self._progress.n = completed
-        # if self._progress.total == self._value and (advance or completed):
-        #     self._progress.colour = "green"
-        #     self._progress.description = description
+
+        if self._progress.total:
+            if self._progress.total == self._value and (advance or completed):
+                self._progress.desc = description
+        else:
+            self._spin()
         self._progress.refresh()
 
     def fail(self):
         # self._progress.colour = "red"
         # self._progress.refresh()
         pass
 
     def stop(self):
+        if not self._progress.total:
+            self._spin(complete=True)
         self._progress = None
 
 
 class RichBackend(AbstractProgressBackend):
     """Rich.progress based progress bar backend"""
 
     def __init__(self):
         super().__init__()
         self._progress: [RICH_PROGRESS.Progress, None] = None
         self._task_id = None
+        self._fail = None
 
     def start(self):
         pass
 
     def _prepare(self):
         self._progress = RICH_PROGRESS.Progress(
             RICH_PROGRESS.TextColumn(
@@ -197,44 +238,51 @@
             RICH_PROGRESS.DownloadColumn(),
             RICH_PROGRESS.TransferSpeedColumn(),
         )
         self._progress.start()
 
     def start_task(self, *, description: str = None, total: int = None):
         self._prepare()
+        self._fail = False
         kwargs = {}
         if description is not None:
             kwargs["description"] = f"[#F92672]{description}"
-        if total is not None:
-            kwargs["total"] = total
+        kwargs["total"] = total
         self._task_id = self._progress.add_task(start=True, **kwargs)
 
     def update(self, *, description: str = None, advance: int = None, completed: int = None):
         kwargs = {}
         if description is not None:
             # kwargs["description"] = f"[rgb(249,38,114)]{description}"
             kwargs["description"] = f"[#F92672]{description}"
         if advance is not None:
             kwargs["advance"] = advance
         if completed is not None:
             kwargs["completed"] = completed
         self._progress.update(self._task_id, **kwargs)
         t = self._progress.tasks[self._task_id]
-        if t.completed == t.total:
+        if t.total is not None and t.completed >= t.total:
             desc = t.description.split(']')[-1]
             self._progress.update(self._task_id,
                                   description=f"[#729C1F]{desc}")
 
     def fail(self):
+        self._fail = True
         t = self._progress.tasks[self._task_id]
         desc = t.description.split(']')[-1]
         self._progress.update(self._task_id,
                               description=f"[red]{desc}")
 
     def stop(self):
+        if not self._fail:
+            t = self._progress.tasks[self._task_id]
+            desc = t.description.split(']')[-1]
+            self._progress.update(self._task_id,
+                                  description=f"[#729C1F]{desc}",
+                                  total=t.completed)
         # # uncomment to hide bar after complete
         # self._progress.remove_task(self._task_id)
         self._progress.stop()
         self._progress = None
 
 
 def find_backend():
@@ -307,16 +355,14 @@
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         if exc_type:
             self.fail()
             raise exc_type(exc_value)
-            # print(exc_type, exc_value, traceback.tb_lineno)
-            # raise Exception(exc_type, exc_value, traceback)
         self.stop()
         return True
 
 
 __all__ = (
     'Progress',
     'AsciiBackend',
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil/quirks.py` & `pydfuutil-0.0.3/pydfuutil/quirks.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/pydfuutil/suffix.py` & `pydfuutil-0.0.3/pydfuutil/suffix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
 import argparse
+import importlib.metadata
 import os
 import sys
 from enum import IntEnum
-import importlib.metadata
 
 from pydfuutil import __copyright__
 from pydfuutil import lmdfu
 from pydfuutil.dfu_file import DFUFile, parse_dfu_suffix
+from pydfuutil.exceptions import GeneralWarning, GeneralError, MisuseError
 from pydfuutil.logger import logger
 
 try:
     __version__ = importlib.metadata.version("pydfuutil")
 except importlib.metadata.PackageNotFoundError:
     __version__ = 'UNKNOWN'
 
@@ -33,35 +34,16 @@
     """LMDFU suffix operate mode"""
     NONE = 0x1
     ADD = 0x2
     DEL = 0x3
     CHECK = 0x4
 
 
-def print_version() -> None:
-    """
-    Prints dfu-suffix version to console
-    """
-    print(f'pydfuutil-suffix " {__version__} "\n')
-    print(f'{__copyright__[0]}\n'
-          'This program is Free Software and has ABSOLUTELY NO WARRANTY\n\n')
-
-
-OPTS = (
-    ("help", 0, 0, 'h'),
-    ("version", 0, 0, 'V'),
-    ("delete", 1, 0, 'D'),
-    ("pid", 1, 0, 'p'),
-    ("vid", 1, 0, 'v'),
-    ("did", 1, 0, 'd'),
-    ("check", 1, 0, 'c'),
-    ("add", 1, 0, 'a'),
-    ("stellaris-address", 1, 0, 's'),
-    ("stellaris", 0, 0, 'T'),
-)
+VERSION = (f'pydfuutil-suffix " {__version__} "\n {__copyright__[0]}\n'
+           f'This program is Free Software and has ABSOLUTELY NO WARRANTY\n\n')
 
 
 def check_suffix(file: DFUFile) -> int:
     """check dfu suffix for valid and prints it"""
     ret: int
 
     ret = parse_dfu_suffix(file)
@@ -86,16 +68,15 @@
 
     if hasattr(os, 'ftruncate'):
         try:
             with open(file.name, 'r+', encoding='utf-8') as f:
                 f.truncate(file.size - file.suffix_len)
             _logger.info("DFU suffix removed")
         except OSError as e:
-            _logger.error(f"Error truncating file: {e}")
-            sys.exit(1)
+            raise GeneralError(f"Error truncating file: {e}")
     else:
         _logger.error("Suffix removal not implemented on this platform")
     return 1
 
 
 def add_suffix(file: DFUFile, pid: int, vid: int, did: int) -> None:
     """Add suffix to DFU file"""
@@ -106,42 +87,22 @@
     file.bcdDevice = did
 
     ret = lmdfu.generate_dfu_suffix(file)
     if ret < 0:
         try:
             raise OSError("generate")
         except OSError as e:
-            _logger.error(e)
-            sys.exit(1)
+            raise GeneralError(e)
     _logger.info("New DFU suffix added.")
 
 
-def _get_arg_parser():
-    """Get custom argument parser"""
-
-    class CustomHelpFormatter(argparse.HelpFormatter):
-        """Custom argument parser formatter"""
-
-        def add_argument(self, action):
-            if action.dest == 'help':
-                action.help = 'Print this help message'
-            super().add_argument(action)
-
-    parser = argparse.ArgumentParser(
-        prog='dfu-suffix',
-        # description="",
-        # epilog='Text at the bottom of help',
-        # conflict_handler='resolve',
-        exit_on_error=False,
-        # add_help=True,
-        formatter_class=CustomHelpFormatter
-    )
-
+def add_cli_options(parser: argparse.ArgumentParser) -> None:
+    """Add cli options"""
     parser.add_argument('-V', '--version', action='version',
-                        version=f'{parser.prog} " v{__version__} "',
+                        version=VERSION,
                         help='Print the version number')
 
     group = parser.add_mutually_exclusive_group(required=True)
 
     group.add_argument('-c', '--check',
                        const=Mode.CHECK, dest='mode', action='store_const',
                        help='Check DFU suffix of <file>')
@@ -166,36 +127,29 @@
                         required=False,
                         type=lambda x: int(x, 16), help='Add device ID into DFU suffix in <file>')
     parser.add_argument('-s', '--stellaris-address', dest='lmdfu_flash_address',
                         metavar="<address>", type=int, help='Specify lmdfu address for LMDFU_ADD')
     parser.add_argument('-T', '--stellaris', dest='lmdfu_mode', action='store_const',
                         const=LmdfuMode.CHECK, help='Set lmdfu mode to LMDFU_CHECK')
 
-    return parser
 
+def main() -> None:
+    """cli entry point for suffix"""
 
-def get_args(parser, argv):
-    """parse command line arguments"""
-    print_version()
+    parser = argparse.ArgumentParser(
+        prog='pydfuutil-suffix',
+        exit_on_error=False,
+    )
+    add_cli_options(parser)
+    print(f"v{__version__}")
     try:
-        args = parser.parse_args(argv)
+        args = parser.parse_args()
     except argparse.ArgumentError as err:
         parser.print_help()
-        _logger.error(err)
-        sys.exit(1)
-    return args
-
-
-def main(argv) -> None:
-    """main executable"""
-    if argv[0] == __file__:
-        argv.pop(0)
-
-    parser = _get_arg_parser()
-    args = get_args(parser, argv)
+        raise GeneralError(err)
 
     lmdfu_mode = LmdfuMode.NONE
     lmdfu_flash_address: int = 0
     lmdfu_prefix: int = 0
 
     empty = 0xffff
 
@@ -218,16 +172,15 @@
     if mode != Mode.NONE:
         try:
             if mode == Mode.ADD:
 
                 if check_suffix(file):
                     if lmdfu_prefix:
                         lmdfu.check_prefix(file)
-                    _logger.warning("Please remove existing DFU suffix before adding a new one.")
-                    sys.exit(1)
+                    raise GeneralWarning("Please remove existing DFU suffix before adding a new one.")
 
                 if lmdfu_mode == LmdfuMode.ADD:
                     if lmdfu.check_prefix(file):
                         _logger.info("Adding new anyway")
                     lmdfu.add_prefix(file, lmdfu_flash_address)
 
                 add_suffix(file, pid, vid, did)
@@ -239,31 +192,39 @@
                     lmdfu.check_prefix(file)
 
             elif mode == Mode.DEL:
                 if (not remove_suffix(file)
                         and lmdfu_mode == LmdfuMode.DEL
                         and lmdfu.check_prefix(file)):
                     lmdfu.remove_prefix(file)
-                    sys.exit(1)
+                    raise GeneralWarning
 
             else:
                 parser.print_help()
-                sys.exit(2)
+                raise MisuseError
 
             if lmdfu_mode == LmdfuMode.DEL and check_suffix(file):
-                _logger.warning(
+                raise GeneralWarning(
                     "DFU suffix exist. "
                     "Remove suffix before using -T or use it with -D to delete suffix")
-                sys.exit(1)
 
             if lmdfu_mode == LmdfuMode.DEL and lmdfu.check_prefix(file):
                 lmdfu.remove_prefix(file)
 
         except Exception as error:
-            _logger.error(error)
-            sys.exit(1)
-
-    sys.exit(0)
+            raise GeneralError(error)
 
 
 if __name__ == '__main__':
-    main(sys.argv)
+    try:
+        main()
+    except GeneralWarning as warn:
+        if warn.__str__():
+            _logger.warning(warn)
+    except GeneralError as err:
+        if err.__str__():
+            _logger.error(err)
+        sys.exit(err.exit_code)
+    except Exception as err:
+        logger.error(err)
+        sys.exit(1)
+    sys.exit(0)
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.0.3/pydfuutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b3
+Version: 0.0.3
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -320,16 +320,22 @@
 - [x] dfu_load
 - [x] portable
 - [x] quirks
 - [x] suffix + cli entry point
 - [x] usb_dfu
 - [x] lmdfu
 - [x] dfuse_mem
-- [ ] dfuse (not fully supported yet)
-- [ ] dfu-util cli entry point (not fully supported yet)
+- [x] dfuse
+- [x] dfu-util cli entry point (not fully supported yet)
+
+#### Todo
+- [ ] Update sources to latest original version "dfu-util-0.11"
+
+[//]: # (https://dfu-util.sourceforge.net/)
+[//]: # (- https://sourceforge.net/p/dfu-util/dfu-util/ci/master/tree/)
 
 
 ## Getting help
 * To report a bug or propose a new feature, use our issue tracker. But please search the database before opening a new issue.
 
 ## About
 Dfu-util - Device Firmware Upgrade Utilities
```

### Comparing `pydfuutil-0.0.2b3/pydfuutil.egg-info/SOURCES.txt` & `pydfuutil-0.0.3/pydfuutil.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pydfuutil/__init__.py
 pydfuutil/__main__.py
 pydfuutil/dfu.py
 pydfuutil/dfu_file.py
 pydfuutil/dfu_load.py
 pydfuutil/dfuse.py
 pydfuutil/dfuse_mem.py
+pydfuutil/exceptions.py
 pydfuutil/lmdfu.py
 pydfuutil/logger.py
 pydfuutil/portable.py
 pydfuutil/progress.py
 pydfuutil/quirks.py
 pydfuutil/suffix.py
 pydfuutil/usb_dfu.py
@@ -26,9 +27,10 @@
 pydfuutil.egg-info/top_level.txt
 tests/test_dfu.py
 tests/test_dfu_file.py
 tests/test_dfu_load.py
 tests/test_dfuse.py
 tests/test_dfuse_mem.py
 tests/test_lmdfu.py
+tests/test_main.py
 tests/test_progress.py
 tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.2b3/pyproject.toml` & `pydfuutil-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydfuutil"
-version = "0.0.2b3"
+version = "0.0.3"
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
 ]
 description = "PyDfuUtil - Pure python fork of dfu-util wrappers to libusb"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfu_util", "dfu-util", "pydfu", "libusb", "python", "python3"]
```

### Comparing `pydfuutil-0.0.2b3/tests/test_dfu.py` & `pydfuutil-0.0.3/tests/test_dfu.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 
     def test_str(self):
         self.assertEqual(dfu.status_to_string(dfu.Status.OK), "No error condition is present")
         self.assertEqual(dfu.Status.OK.to_string(), "No error condition is present")
         self.assertEqual(dfu.state_to_string(dfu.State.APP_IDLE), "appIDLE")
         self.assertEqual(dfu.State.APP_IDLE.to_string(), "appIDLE")
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_detach(self, mock_find, mock_verify_init):
+    def test_detach(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -32,28 +31,26 @@
 
         # Calling the function
         interface = 0
         timeout = 1000
         result = dfu.detach(mock_device, interface, timeout)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21 | 0x01,
             bRequest=dfu.Command.DETACH,  # Assuming Command.DETACH is 23
             wValue=timeout,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, 1)  # Assuming success returns 1
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_upload(self, mock_find, mock_verify_init):
+    def test_upload(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -62,28 +59,26 @@
         # Calling the function
         interface = 0
         transaction = 0
         data = bytes(10)
         result = dfu.upload(mock_device, interface, transaction, data)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0xa1,
             bRequest=dfu.Command.UPLOAD,  # Assuming Command.UPLOAD
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=data,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, data)  # Assuming success returns bytes(10)
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_dwnload(self, mock_find, mock_verify_init):
+    def test_dwnload(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -92,28 +87,26 @@
         # Calling the function
         interface = 0
         transaction = 0
         data = bytes(10)
         result = dfu.download(mock_device, interface, transaction, data)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
             bRequest=dfu.Command.DNLOAD,  # Assuming Command.DNLOAD
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=data,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, len(data))  # Assuming success returns 10
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_get_status(self, mock_find, mock_verify_init):
+    def test_get_status(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -122,28 +115,26 @@
         # Calling the function
         interface = 0
         transaction = 0
         length = 6
         status = dfu.get_status(mock_device, interface)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0xa1,
             bRequest=dfu.Command.GETSTATUS,  # Assuming Command.GETSTATUS
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=length,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(status.bState, 0)  # Assuming success returns 0
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_clear_status(self, mock_find, mock_verify_init):
+    def test_clear_status(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -151,28 +142,26 @@
 
         # Calling the function
         interface = 0
         transaction = 0
         result = dfu.clear_status(mock_device, interface)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
             bRequest=dfu.Command.CLRSTATUS,  # Assuming Command.CLRSTATUS
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
         )
         self.assertEqual(result, 0)  # Assuming success returns 0
 
-    @patch("pydfuutil.dfu.verify_init")
     @patch("usb.core.find")
-    def test_abort(self, mock_find, mock_verify_init):
+    def test_abort(self, mock_find):
         # Mocking the device
         mock_device = MagicMock()
 
         # Mocking the return value of usb.core.find
         mock_find.return_value = mock_device
 
         # Mocking the return value of ctrl_transfer method
@@ -180,15 +169,14 @@
 
         # Calling the function
         interface = 0
         transaction = 0
         result = dfu.abort(mock_device, interface)
 
         # Assertions
-        mock_verify_init.assert_called_once()
         mock_device.ctrl_transfer.assert_called_once_with(
             bmRequestType=0x21,
             bRequest=dfu.Command.ABORT,  # Assuming Command.ABORT
             wValue=transaction,
             wIndex=interface,
             data_or_wLength=None,
             timeout=1000,  # Assuming TIMEOUT is 1000
```

### Comparing `pydfuutil-0.0.2b3/tests/test_dfu_file.py` & `pydfuutil-0.0.3/tests/test_dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/tests/test_dfu_load.py` & `pydfuutil-0.0.3/tests/test_dfu_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,31 @@
         dif.get_status.return_value = total_size
 
         # Mock file_p.write to return the length of the data written
         with patch.object(file.file_p, 'write', return_value=xfer_size) as mock_write:
             result = do_upload(dif, xfer_size, file, total_size)
 
         # Assertions
-        self.assertEqual(result, total_size)  # Assuming total_size bytes are received
+        self.assertEqual(result, total_size)  # Assuming expected_size bytes are received
 
     def test_dfu_load_do_dnload(self):
 
         xfer_size = 1024
         result = dfu.StatusRetVal(dfu.Status.OK, 100, dfu.State.DFU_DOWNLOAD_IDLE, 0)
 
         dif = Mock()
         dif.download.return_value = xfer_size
         dif.get_status.return_value = result
 
         file = DFUFile(name='test_file', file_p=Mock(), size=xfer_size, suffix_len=0)
         quirks = 0
-        verbose = False
 
         # Mock file_p.readinto to return the length of the data read
         with patch.object(file.file_p, 'readinto', return_value=xfer_size) as mock_readinto:
-            result = do_dnload(dif, xfer_size, file, quirks, verbose)
+            result = do_dnload(dif, xfer_size, file, quirks)
 
         # Assertions
         self.assertEqual(result, xfer_size)  # Assuming xfer_size bytes are sent
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pydfuutil-0.0.2b3/tests/test_dfuse.py` & `pydfuutil-0.0.3/tests/test_dfuse.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/tests/test_dfuse_mem.py` & `pydfuutil-0.0.3/tests/test_dfuse_mem.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/tests/test_lmdfu.py` & `pydfuutil-0.0.3/tests/test_lmdfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b3/tests/test_progress.py` & `pydfuutil-0.0.3/tests/test_progress.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,45 +4,68 @@
 from pydfuutil.progress import *
 
 unittest.TestLoader.sortTestMethodsUsing = None
 
 
 class TestDfuProgress(unittest.TestCase):
 
-    def _loop(self, backend=None):
+    def _loop(self, backend=None, total=None):
         i = 10
 
         with Progress(backend) as prog:
             name = (backend.__name__
                     if backend
                     else f"Any")
 
             prog.start_task(description=f"{name}",
-                            total=i)
+                            total=total)
             while i >= 1:
                 sleep(0.1)
                 prog.update(advance=1)
                 i -= 1
             prog.update(description=f"{name} OK")
 
     @unittest.skipIf(not TQDM_PROGRESS,
                      "package not installed ImportError/UnboundLocalError/AttributeError")
     def test_tqdm(self):
-        self._loop(TqdmBackend)
+        self._loop(TqdmBackend, 10)
+
+        with self.subTest("indeterminate"):
+            self._loop(TqdmBackend, None)
 
     @unittest.skipIf(not RICH_PROGRESS,
                      "package not installed ImportError/UnboundLocalError/AttributeError")
     def test_rich(self):
-        self._loop(RichBackend)
+        self._loop(RichBackend, 10)
+
+        with self.subTest("indeterminate"):
+            self._loop(RichBackend, None)
 
     def test_no_progress(self):
         self._loop(NoProgressBarBackend)
 
     def test_ascii(self):
-        self._loop(AsciiBackend)
+        with self.subTest("by completed"):
+            i, j = 20, 1
+            n = AsciiBackend.__name__
+            with Progress(AsciiBackend) as prog:
+                prog.start_task(description=n,
+                                total=i)
+                while i >= 0:
+                    sleep(0.1)
+                    prog.update(completed=21-i)
+                    i -= 1 + j
+                    j += 1
+                prog.update(description=f"{n} OK")
+
+        with self.subTest("by advance"):
+            self._loop(AsciiBackend, 10)
+
+        with self.subTest("indeterminate"):
+            self._loop(AsciiBackend, None)
 
     @unittest.skip("rich.errors.LiveError: Only one live display may be active at once")
     def test_autodetect(self):
         self._loop(None)
 
     def test_exception(self):
         i = 10
```

### Comparing `pydfuutil-0.0.2b3/tests/test_quirks.py` & `pydfuutil-0.0.3/tests/test_quirks.py`

 * *Files identical despite different names*

