# Comparing `tmp/pn532pi-1.5.tar.gz` & `tmp/pn532pi-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pn532pi-1.5.tar", last modified: Sat Jan  6 21:15:40 2024, max compression
+gzip compressed data, was "pn532pi-1.6.tar", last modified: Mon May  6 00:20:29 2024, max compression
```

## Comparing `pn532pi-1.5.tar` & `pn532pi-1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.558419 pn532pi-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-01-06 21:15:40.558419 pn532pi-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-01-06 21:15:32.000000 pn532pi-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.550418 pn532pi-1.5/pn532pi/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.550418 pn532pi-1.5/pn532pi/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/interfaces/pn532Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/interfaces/pn532hsu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/interfaces/pn532i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/interfaces/pn532spi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.554419 pn532pi-1.5/pn532pi/nfc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/emulatetag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/llcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/macLink.py
--rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/pn532.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/pn532_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-01-06 21:15:32.000000 pn532pi-1.5/pn532pi/nfc/snep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.558419 pn532pi-1.5/pn532pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-01-06 21:15:40.000000 pn532pi-1.5/pn532pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-06 21:15:40.000000 pn532pi-1.5/pn532pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 21:15:40.000000 pn532pi-1.5/pn532pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-06 21:15:40.000000 pn532pi-1.5/pn532pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-06 21:15:40.000000 pn532pi-1.5/pn532pi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.554419 pn532pi-1.5/quick2wire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/asm_generic_ioctl.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/board_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/eventfd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/gpio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.554419 pn532pi-1.5/quick2wire/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/helpers/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/i2c_ctypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:40.558419 pn532pi-1.5/quick2wire/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/mcp23017.py
--rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/mcp23x17.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/pcf8591.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/test_mcp23017_interrupts_loopback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/test_mcp23017_loopback.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/test_mcp23x17.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/test_pcf8591.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/parts/test_pcf8591_loopback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/spi_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/syscall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_eventfd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_gpio_loopback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_spi_loopback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/test_timerfd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-01-06 21:15:32.000000 pn532pi-1.5/quick2wire/timerfd.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 21:15:40.558419 pn532pi-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-06 21:15:32.000000 pn532pi-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.796115 pn532pi-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-06 00:20:29.796115 pn532pi-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-06 00:20:25.000000 pn532pi-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.788115 pn532pi-1.6/pn532pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.788115 pn532pi-1.6/pn532pi/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/interfaces/pn532Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/interfaces/pn532hsu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/interfaces/pn532i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/interfaces/pn532spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.788115 pn532pi-1.6/pn532pi/nfc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/emulatetag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/llcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/macLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/pn532.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/pn532_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-06 00:20:25.000000 pn532pi-1.6/pn532pi/nfc/snep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.796115 pn532pi-1.6/pn532pi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-06 00:20:29.000000 pn532pi-1.6/pn532pi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 00:20:29.000000 pn532pi-1.6/pn532pi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 00:20:29.000000 pn532pi-1.6/pn532pi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 00:20:29.000000 pn532pi-1.6/pn532pi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 00:20:29.000000 pn532pi-1.6/pn532pi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.792115 pn532pi-1.6/quick2wire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/asm_generic_ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/board_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/eventfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/gpio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.792115 pn532pi-1.6/quick2wire/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/helpers/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/i2c_ctypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:29.796115 pn532pi-1.6/quick2wire/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/mcp23017.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/mcp23x17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/pcf8591.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/test_mcp23017_interrupts_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/test_mcp23017_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/test_mcp23x17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/test_pcf8591.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/parts/test_pcf8591_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/spi_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/syscall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_eventfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_gpio_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_spi_loopback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/test_timerfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-06 00:20:25.000000 pn532pi-1.6/quick2wire/timerfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 00:20:29.796115 pn532pi-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-06 00:20:25.000000 pn532pi-1.6/setup.py
```

### Comparing `pn532pi-1.5/PKG-INFO` & `pn532pi-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pn532pi
-Version: 1.5
+Version: 1.6
 Summary: PN532 library for Raspberry Pi
 Home-page: https://github.com/gassajor000/pn532pi
 Author: gassajor000
 Author-email: lgassjsg@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License 
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pn532pi-1.5/README.md` & `pn532pi-1.6/README.md`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/__init__.py` & `pn532pi-1.6/pn532pi/__init__.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/interfaces/pn532Interface.py` & `pn532pi-1.6/pn532pi/interfaces/pn532Interface.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/interfaces/pn532hsu.py` & `pn532pi-1.6/pn532pi/interfaces/pn532hsu.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/interfaces/pn532i2c.py` & `pn532pi-1.6/pn532pi/interfaces/pn532i2c.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/interfaces/pn532spi.py` & `pn532pi-1.6/pn532pi/interfaces/pn532spi.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,25 +41,28 @@
     def _xfer_bytes(self, data: bytearray) -> bytearray:
         return _reverse_bits(self._spi.xfer2(list(_reverse_bits(data))))
 
     def _check_status(self) -> int:
         data_out = list(_reverse_bits([STATUS_READ, 0]))
         return _reverse_bits(self._spi.xfer2(data_out))[1]
 
-    def __init__(self, ss: int):
+    def __init__(self, ss: int, speed_hz: int=4_000_000):
+        """Pass in slave select pin and optional speed (4MHz default, 5MHz max)"""
         self._command = 0
         self._ss = ss
         self._spi = SpiDev()
+        assert speed_hz <= 5_000_000, "SPI Bus speed must be <= 5MHz"
+        self._speed = speed_hz
         assert ss in [1, 0], 'Chip select must be 1 or 0'
 
     def begin(self):
         self._spi.open(RPI_BUS0, self._ss)
         self._spi.mode = SPI_MODE0  # PN532 only supports mode0
         self._spi.cshigh = False  # Active low
-        self._spi.max_speed_hz = 5000000 # 5 MHz
+        self._spi.max_speed_hz = self._speed
 
     def wakeup(self) -> None:
         # Chip select controlled by driver
         self._isReady()
 
     def writeCommand(self, header: bytearray, body: bytearray = bytearray()) -> int:
         self._command = header[0]
@@ -82,15 +85,15 @@
         PN532_NACK = [0, 0, 0xFF, 0xFF, 0, 0]
         timer = 0
 
         while (not self._isReady()):
             time.sleep(.001)    # sleep 1 ms
             timer+=1
             if ((0 != timeout) and (timer > timeout)):
-                return -1          
+                return -1  
 
 
         data = self._xfer_bytes([DATA_READ] + [0 for i in range(5)])
         data = data[1:]  # first byte is garbage
         DMSG('_getResponseLength length frame: {!r}'.format(data))
 
         if data[:-2] != bytearray([PN532_PREAMBLE, PN532_STARTCODE1, PN532_STARTCODE2]):
```

### Comparing `pn532pi-1.5/pn532pi/nfc/emulatetag.py` & `pn532pi-1.6/pn532pi/nfc/emulatetag.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/nfc/llcp.py` & `pn532pi-1.6/pn532pi/nfc/llcp.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/nfc/pn532.py` & `pn532pi-1.6/pn532pi/nfc/pn532.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/nfc/pn532_log.py` & `pn532pi-1.6/pn532pi/nfc/pn532_log.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi/nfc/snep.py` & `pn532pi-1.6/pn532pi/nfc/snep.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/pn532pi.egg-info/PKG-INFO` & `pn532pi-1.6/pn532pi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pn532pi
-Version: 1.5
+Version: 1.6
 Summary: PN532 library for Raspberry Pi
 Home-page: https://github.com/gassajor000/pn532pi
 Author: gassajor000
 Author-email: lgassjsg@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License 
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pn532pi-1.5/pn532pi.egg-info/SOURCES.txt` & `pn532pi-1.6/pn532pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/asm_generic_ioctl.py` & `pn532pi-1.6/quick2wire/asm_generic_ioctl.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/eventfd.py` & `pn532pi-1.6/quick2wire/eventfd.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/gpio.py` & `pn532pi-1.6/quick2wire/gpio.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/i2c.py` & `pn532pi-1.6/quick2wire/i2c.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/i2c_ctypes.py` & `pn532pi-1.6/quick2wire/i2c_ctypes.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/mcp23017.py` & `pn532pi-1.6/quick2wire/parts/mcp23017.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/mcp23x17.py` & `pn532pi-1.6/quick2wire/parts/mcp23x17.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/pcf8591.py` & `pn532pi-1.6/quick2wire/parts/pcf8591.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/test_mcp23017_interrupts_loopback.py` & `pn532pi-1.6/quick2wire/parts/test_mcp23017_interrupts_loopback.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/test_mcp23017_loopback.py` & `pn532pi-1.6/quick2wire/parts/test_mcp23017_loopback.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/test_mcp23x17.py` & `pn532pi-1.6/quick2wire/parts/test_mcp23x17.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/test_pcf8591.py` & `pn532pi-1.6/quick2wire/parts/test_pcf8591.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/parts/test_pcf8591_loopback.py` & `pn532pi-1.6/quick2wire/parts/test_pcf8591_loopback.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/selector.py` & `pn532pi-1.6/quick2wire/selector.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/spi.py` & `pn532pi-1.6/quick2wire/spi.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/spi_ctypes.py` & `pn532pi-1.6/quick2wire/spi_ctypes.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/syscall.py` & `pn532pi-1.6/quick2wire/syscall.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_eventfd.py` & `pn532pi-1.6/quick2wire/test_eventfd.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_gpio.py` & `pn532pi-1.6/quick2wire/test_gpio.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_gpio_loopback.py` & `pn532pi-1.6/quick2wire/test_gpio_loopback.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_selector.py` & `pn532pi-1.6/quick2wire/test_selector.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_spi_loopback.py` & `pn532pi-1.6/quick2wire/test_spi_loopback.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/test_timerfd.py` & `pn532pi-1.6/quick2wire/test_timerfd.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/quick2wire/timerfd.py` & `pn532pi-1.6/quick2wire/timerfd.py`

 * *Files identical despite different names*

### Comparing `pn532pi-1.5/setup.py` & `pn532pi-1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pn532pi",
-    version="1.5",
+    version="1.6",
     author="gassajor000",
     author_email="lgassjsg@example.com",
     description="PN532 library for Raspberry Pi",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gassajor000/pn532pi",
     packages=setuptools.find_packages(include=['quick2wire', 'quick2wire.*', 'pn532pi', 'pn532pi.*']),
```

