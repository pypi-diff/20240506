# Comparing `tmp/vnpy_evo-0.2.0.tar.gz` & `tmp/vnpy_evo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_evo-0.2.0.tar", last modified: Sat Apr 13 06:10:07 2024, max compression
+gzip compressed data, was "vnpy_evo-0.2.1.tar", last modified: Mon May  6 14:07:00 2024, max compression
```

## Comparing `vnpy_evo-0.2.0.tar` & `vnpy_evo-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.070781 vnpy_evo-0.2.0/
--rw-rw-rw-   0        0        0     1109 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       30 2024-03-10 12:14:20.000000 vnpy_evo-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11325 2024-04-13 06:10:07.070781 vnpy_evo-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10247 2024-04-13 06:07:39.000000 vnpy_evo-0.2.0/README.md
--rw-rw-rw-   0        0        0     1251 2024-04-13 06:10:07.072789 vnpy_evo-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-03-05 02:02:42.000000 vnpy_evo-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.009396 vnpy_evo-0.2.0/vnpy_evo/
--rw-rw-rw-   0        0        0     1241 2024-04-13 06:06:30.000000 vnpy_evo-0.2.0/vnpy_evo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.026934 vnpy_evo-0.2.0/vnpy_evo/chart/
--rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/chart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.027943 vnpy_evo-0.2.0/vnpy_evo/event/
--rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/event/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.046401 vnpy_evo-0.2.0/vnpy_evo/rpc/
--rw-rw-rw-   0        0        0       22 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/rpc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.061091 vnpy_evo-0.2.0/vnpy_evo/trader/
--rw-rw-rw-   0        0        0        0 2024-03-18 09:46:57.000000 vnpy_evo-0.2.0/vnpy_evo/trader/__init__.py
--rw-rw-rw-   0        0        0       31 2024-03-08 07:51:09.000000 vnpy_evo-0.2.0/vnpy_evo/trader/app.py
--rw-rw-rw-   0        0        0      459 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/constant.py
--rw-rw-rw-   0        0        0       37 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/converter.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/database.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/datafeed.py
--rw-rw-rw-   0        0        0       34 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/engine.py
--rw-rw-rw-   0        0        0       33 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/event.py
--rw-rw-rw-   0        0        0       35 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/gateway.py
--rw-rw-rw-   0        0        0       34 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/object.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/optimize.py
--rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.065788 vnpy_evo-0.2.0/vnpy_evo/trader/ui/
--rw-rw-rw-   0        0        0       95 2024-03-18 09:46:51.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.069785 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/
--rw-rw-rw-   0        0        0        0 2024-03-11 11:13:46.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/__init__.py
--rw-rw-rw-   0        0        0    35149 2022-05-31 14:57:28.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/veighna.ico
--rw-rw-rw-   0        0        0     7951 2024-03-18 09:40:05.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/mainwindow.py
--rw-rw-rw-   0        0        0    22875 2024-04-05 09:48:27.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/monitor.py
--rw-rw-rw-   0        0        0     3960 2024-03-18 09:49:02.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/qt.py
--rw-rw-rw-   0        0        0    23194 2024-03-18 09:48:54.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/widget.py
--rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/utility.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.025938 vnpy_evo-0.2.0/vnpy_evo.egg-info/
--rw-rw-rw-   0        0        0    11325 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.532358 vnpy_evo-0.2.1/
+-rw-rw-rw-   0        0        0     1109 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-03-10 12:14:20.000000 vnpy_evo-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11325 2024-05-06 14:07:00.532509 vnpy_evo-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10247 2024-05-06 14:06:07.000000 vnpy_evo-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1251 2024-05-06 14:07:00.534510 vnpy_evo-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-03-05 02:02:42.000000 vnpy_evo-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.467263 vnpy_evo-0.2.1/vnpy_evo/
+-rw-rw-rw-   0        0        0     1241 2024-05-06 14:06:14.000000 vnpy_evo-0.2.1/vnpy_evo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.510722 vnpy_evo-0.2.1/vnpy_evo/chart/
+-rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/chart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.511721 vnpy_evo-0.2.1/vnpy_evo/event/
+-rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/event/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.513724 vnpy_evo-0.2.1/vnpy_evo/rpc/
+-rw-rw-rw-   0        0        0       22 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/rpc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.525856 vnpy_evo-0.2.1/vnpy_evo/trader/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:57.000000 vnpy_evo-0.2.1/vnpy_evo/trader/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-03-08 07:51:09.000000 vnpy_evo-0.2.1/vnpy_evo/trader/app.py
+-rw-rw-rw-   0        0        0      478 2024-04-26 08:33:17.000000 vnpy_evo-0.2.1/vnpy_evo/trader/constant.py
+-rw-rw-rw-   0        0        0       37 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/converter.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/database.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/datafeed.py
+-rw-rw-rw-   0        0        0       34 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/engine.py
+-rw-rw-rw-   0        0        0       33 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/event.py
+-rw-rw-rw-   0        0        0       35 2024-04-06 05:51:44.000000 vnpy_evo-0.2.1/vnpy_evo/trader/gateway.py
+-rw-rw-rw-   0        0        0       34 2024-04-06 05:51:44.000000 vnpy_evo-0.2.1/vnpy_evo/trader/object.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/optimize.py
+-rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/setting.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.529854 vnpy_evo-0.2.1/vnpy_evo/trader/ui/
+-rw-rw-rw-   0        0        0       95 2024-03-18 09:46:51.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.530854 vnpy_evo-0.2.1/vnpy_evo/trader/ui/ico/
+-rw-rw-rw-   0        0        0        0 2024-03-11 11:13:46.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/ico/__init__.py
+-rw-rw-rw-   0        0        0    35149 2022-05-31 14:57:28.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/ico/veighna.ico
+-rw-rw-rw-   0        0        0     7951 2024-03-18 09:40:05.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/mainwindow.py
+-rw-rw-rw-   0        0        0    22875 2024-04-05 09:48:27.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/monitor.py
+-rw-rw-rw-   0        0        0     3960 2024-03-18 09:49:02.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/qt.py
+-rw-rw-rw-   0        0        0    23194 2024-03-18 09:48:54.000000 vnpy_evo-0.2.1/vnpy_evo/trader/ui/widget.py
+-rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.1/vnpy_evo/trader/utility.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:07:00.509734 vnpy_evo-0.2.1/vnpy_evo.egg-info/
+-rw-rw-rw-   0        0        0    11325 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 14:07:00.000000 vnpy_evo-0.2.1/vnpy_evo.egg-info/top_level.txt
```

### Comparing `vnpy_evo-0.2.0/LICENSE` & `vnpy_evo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/PKG-INFO` & `vnpy_evo-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_evo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core module for using VeighNa project on crypto markets.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/veighna-global/vnpy_evo
 Keywords: quant,quantitative,investment,trading,algotrading,crypto,btc
@@ -26,15 +26,15 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market.
```

### Comparing `vnpy_evo-0.2.0/README.md` & `vnpy_evo-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market.
```

### Comparing `vnpy_evo-0.2.0/setup.cfg` & `vnpy_evo-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo/__init__.py` & `vnpy_evo-0.2.1/vnpy_evo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 os.environ["LANG"] = "en"       # Only support English
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/veighna.ico` & `vnpy_evo-0.2.1/vnpy_evo/trader/ui/ico/veighna.ico`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo/trader/ui/mainwindow.py` & `vnpy_evo-0.2.1/vnpy_evo/trader/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo/trader/ui/monitor.py` & `vnpy_evo-0.2.1/vnpy_evo/trader/ui/monitor.py`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo/trader/ui/qt.py` & `vnpy_evo-0.2.1/vnpy_evo/trader/ui/qt.py`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo/trader/ui/widget.py` & `vnpy_evo-0.2.1/vnpy_evo/trader/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.2.0/vnpy_evo.egg-info/PKG-INFO` & `vnpy_evo-0.2.1/vnpy_evo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-evo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core module for using VeighNa project on crypto markets.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/veighna-global/vnpy_evo
 Keywords: quant,quantitative,investment,trading,algotrading,crypto,btc
@@ -26,15 +26,15 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.1-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market.
```

### Comparing `vnpy_evo-0.2.0/vnpy_evo.egg-info/SOURCES.txt` & `vnpy_evo-0.2.1/vnpy_evo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

