# Comparing `tmp/vnpy_rest-1.0.7.tar.gz` & `tmp/vnpy_rest-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_rest-1.0.7.tar", last modified: Sun Sep  3 13:46:58 2023, max compression
+gzip compressed data, was "vnpy_rest-1.0.8.tar", last modified: Mon May  6 14:00:29 2024, max compression
```

## Comparing `vnpy_rest-1.0.7.tar` & `vnpy_rest-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 13:46:58.674812 vnpy_rest-1.0.7/
--rw-rw-rw-   0        0        0     1083 2022-11-14 08:31:48.000000 vnpy_rest-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1784 2023-09-03 13:46:58.675833 vnpy_rest-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-09-03 13:45:50.000000 vnpy_rest-1.0.7/README.md
--rw-rw-rw-   0        0        0      985 2023-09-03 13:46:58.677393 vnpy_rest-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0       43 2022-11-14 08:31:48.000000 vnpy_rest-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-03 13:46:58.639702 vnpy_rest-1.0.7/vnpy_rest/
--rw-rw-rw-   0        0        0     1377 2022-12-13 08:13:01.000000 vnpy_rest-1.0.7/vnpy_rest/__init__.py
--rw-rw-rw-   0        0        0     9659 2023-08-24 08:47:32.000000 vnpy_rest-1.0.7/vnpy_rest/rest_client.py
-drwxrwxrwx   0        0        0        0 2023-09-03 13:46:58.673792 vnpy_rest-1.0.7/vnpy_rest.egg-info/
--rw-rw-rw-   0        0        0     1784 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-09-03 13:46:58.000000 vnpy_rest-1.0.7/vnpy_rest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.834289 vnpy_rest-1.0.8/
+-rw-rw-rw-   0        0        0     1099 2024-05-06 13:59:09.000000 vnpy_rest-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1789 2024-05-06 14:00:29.835366 vnpy_rest-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      855 2024-05-06 13:59:26.000000 vnpy_rest-1.0.8/README.md
+-rw-rw-rw-   0        0        0      988 2024-05-06 14:00:29.859688 vnpy_rest-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-11-14 08:31:48.000000 vnpy_rest-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.758672 vnpy_rest-1.0.8/vnpy_rest/
+-rw-rw-rw-   0        0        0     1377 2022-12-13 08:13:01.000000 vnpy_rest-1.0.8/vnpy_rest/__init__.py
+-rw-rw-rw-   0        0        0     9687 2024-05-06 13:58:07.000000 vnpy_rest-1.0.8/vnpy_rest/rest_client.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:00:29.831504 vnpy_rest-1.0.8/vnpy_rest.egg-info/
+-rw-rw-rw-   0        0        0     1789 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 14:00:29.000000 vnpy_rest-1.0.8/vnpy_rest.egg-info/top_level.txt
```

### Comparing `vnpy_rest-1.0.7/LICENSE` & `vnpy_rest-1.0.8/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 vn.py
+Copyright (c) 2015-present, Xiaoyou Chen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `vnpy_rest-1.0.7/PKG-INFO` & `vnpy_rest-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: vnpy_rest
-Version: 1.0.7
+Version: 1.0.8
 Summary: REST API client for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于asyncio和aiohttp开发的协程异步REST API客户端，用于开发高性能的REST交易接口。
```

### Comparing `vnpy_rest-1.0.7/README.md` & `vnpy_rest-1.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于asyncio和aiohttp开发的协程异步REST API客户端，用于开发高性能的REST交易接口。
```

### Comparing `vnpy_rest-1.0.7/setup.cfg` & `vnpy_rest-1.0.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 7265 7374 0d0a 7665   = vnpy_rest..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 370d 0a75  rsion = 1.0.7..u
+00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a75  rsion = 1.0.8..u
 00000030: 726c 203d 2068 7474 7073 3a2f 2f77 7777  rl = https://www
 00000040: 2e76 6e70 792e 636f 6d0d 0a6c 6963 656e  .vnpy.com..licen
 00000050: 7365 203d 204d 4954 0d0a 6175 7468 6f72  se = MIT..author
 00000060: 203d 2058 6961 6f79 6f75 2043 6865 6e0d   = Xiaoyou Chen.
 00000070: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000080: 7869 616f 796f 752e 6368 656e 406d 6169  xiaoyou.chen@mai
 00000090: 6c2e 766e 7079 2e63 6f6d 0d0a 6465 7363  l.vnpy.com..desc
@@ -28,35 +28,35 @@
 000001b0: 5374 6162 6c65 0d0a 094f 7065 7261 7469  Stable...Operati
 000001c0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 000001d0: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
 000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000200: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
 00000210: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000220: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000230: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000240: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000250: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000270: 6f6e 203a 3a20 332e 3130 0d0a 0954 6f70  on :: 3.10...Top
-00000280: 6963 203a 3a20 4f66 6669 6365 2f42 7573  ic :: Office/Bus
-00000290: 696e 6573 7320 3a3a 2046 696e 616e 6369  iness :: Financi
-000002a0: 616c 203a 3a20 496e 7665 7374 6d65 6e74  al :: Investment
-000002b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002d0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
-000002e0: 696f 6e20 3a3a 2043 5079 7468 6f6e 0d0a  ion :: CPython..
-000002f0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000300: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000310: 4c69 6365 6e73 650d 0a09 4e61 7475 7261  License...Natura
-00000320: 6c20 4c61 6e67 7561 6765 203a 3a20 4368  l Language :: Ch
-00000330: 696e 6573 6520 2853 696d 706c 6966 6965  inese (Simplifie
-00000340: 6429 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  d)....[options].
-00000350: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000360: 3a0d 0a7a 6970 5f73 6166 6520 3d20 4661  :..zip_safe = Fa
-00000370: 6c73 650d 0a70 7974 686f 6e5f 7265 7175  lse..python_requ
-00000380: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
-00000390: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000003a0: 200d 0a09 6169 6f68 7474 700d 0a0d 0a5b   ...aiohttp....[
-000003b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000003c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000003d0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000220: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000250: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000260: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000270: 7468 6f6e 203a 3a20 332e 3132 0d0a 0954  thon :: 3.12...T
+00000280: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
+00000290: 7573 696e 6573 7320 3a3a 2046 696e 616e  usiness :: Finan
+000002a0: 6369 616c 203a 3a20 496e 7665 7374 6d65  cial :: Investme
+000002b0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+000002c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002d0: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+000002e0: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
+000002f0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+00000300: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000310: 5420 4c69 6365 6e73 650d 0a09 4e61 7475  T License...Natu
+00000320: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+00000330: 4368 696e 6573 6520 2853 696d 706c 6966  Chinese (Simplif
+00000340: 6965 6429 0d0a 0d0a 5b6f 7074 696f 6e73  ied)....[options
+00000350: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
+00000360: 6e64 3a0d 0a7a 6970 5f73 6166 6520 3d20  nd:..zip_safe = 
+00000370: 4661 6c73 650d 0a70 7974 686f 6e5f 7265  False..python_re
+00000380: 7175 6972 6573 203d 203e 3d33 2e31 300d  quires = >=3.10.
+00000390: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000003a0: 7320 3d20 0d0a 0961 696f 6874 7470 0d0a  s = ...aiohttp..
+000003b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000003c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000003d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `vnpy_rest-1.0.7/vnpy_rest/__init__.py` & `vnpy_rest-1.0.8/vnpy_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_rest-1.0.7/vnpy_rest/rest_client.py` & `vnpy_rest-1.0.8/vnpy_rest/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,28 @@
 
     def __init__(
         self,
         method: str,
         path: str,
         params: dict,
         data: Union[dict, str, bytes],
+        json: dict,
         headers: dict,
         callback: CALLBACK_TYPE = None,
         on_failed: ON_FAILED_TYPE = None,
         on_error: ON_ERROR_TYPE = None,
         extra: Any = None,
     ):
         """"""
         self.method: str = method
         self.path: str = path
         self.callback: CALLBACK_TYPE = callback
         self.params: dict = params
         self.data: Union[dict, str, bytes] = data
+        self.json: dict = json
         self.headers: dict = headers
 
         self.on_failed: ON_FAILED_TYPE = on_failed
         self.on_error: ON_ERROR_TYPE = on_error
         self.extra: Any = extra
 
         self.response: "Response" = None
@@ -79,22 +81,24 @@
             status_code = self.response.status_code
 
         return (
             "request : {} {} because {}: \n"
             "headers: {}\n"
             "params: {}\n"
             "data: {}\n"
+            "json: {}\n"
             "response:"
             "{}\n".format(
                 self.method,
                 self.path,
                 status_code,
                 self.headers,
                 self.params,
                 self.data,
+                self.json,
                 "" if self.response is None else self.response.text,
             )
         )
 
 
 class Response:
     """结果对象"""
@@ -135,54 +139,52 @@
     ) -> None:
         """传入REST API的根地址，初始化客户端"""
         self.url_base = url_base
 
         if proxy_host and proxy_port:
             self.proxy = f"http://{proxy_host}:{proxy_port}"
 
-    def start(self, session_number: int = 3) -> None:
+    def start(self) -> None:
         """启动客户端的事件循环"""
         try:
             self.loop = get_running_loop()
         except RuntimeError:
             self.loop = new_event_loop()
 
         start_event_loop(self.loop)
 
     def stop(self) -> None:
         """停止客户端的事件循环"""
-        if self.session:
-            coro = self.session.close()
-            run_coroutine_threadsafe(coro, self.loop).result()
-
         if self.loop and self.loop.is_running():
             self.loop.stop()
 
     def join(self) -> None:
         """等待子线程退出"""
         pass
 
     def add_request(
         self,
         method: str,
         path: str,
         callback: CALLBACK_TYPE,
         params: dict = None,
         data: Union[dict, str, bytes] = None,
+        json: dict = None,
         headers: dict = None,
         on_failed: ON_FAILED_TYPE = None,
         on_error: ON_ERROR_TYPE = None,
         extra: Any = None,
     ) -> Request:
         """添加新的请求任务"""
         request: Request = Request(
             method,
             path,
             params,
             data,
+            json,
             headers,
             callback,
             on_failed,
             on_error,
             extra,
         )
 
@@ -255,14 +257,15 @@
 
         cr: ClientResponse = await self.session.request(
             request.method,
             url,
             headers=request.headers,
             params=request.params,
             data=request.data,
+            json=request.json,
             proxy=self.proxy
         )
 
         text: str = await cr.text()
         status_code = cr.status
 
         request.response = Response(status_code, text)
```

### Comparing `vnpy_rest-1.0.7/vnpy_rest.egg-info/PKG-INFO` & `vnpy_rest-1.0.8/vnpy_rest.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: vnpy-rest
-Version: 1.0.7
+Version: 1.0.8
 Summary: REST API client for vn.py quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeighNa框架的REST API客户端
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.0.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.0.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 基于asyncio和aiohttp开发的协程异步REST API客户端，用于开发高性能的REST交易接口。
```

