# Comparing `tmp/anicli_api-0.6.4.tar.gz` & `tmp/anicli_api-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anicli_api-0.6.4.tar", max compression
+gzip compressed data, was "anicli_api-0.6.5.tar", max compression
```

## Comparing `anicli_api-0.6.4.tar` & `anicli_api-0.6.5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    18450 2024-03-13 06:53:31.234216 anicli_api-0.6.4/README.MD
--rw-r--r--   0        0        0     5658 2024-03-13 06:53:31.234216 anicli_api-0.6.4/anicli_api/_http.py
--rw-r--r--   0        0        0      278 2023-12-11 18:34:31.718016 anicli_api-0.6.4/anicli_api/_logger.py
--rw-r--r--   0        0        0     6414 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/base.py
--rw-r--r--   0        0        0      618 2024-03-13 06:53:31.234216 anicli_api-0.6.4/anicli_api/player/__init__.py
--rw-r--r--   0        0        0      870 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/player/__template__.py
--rw-r--r--   0        0        0     3900 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/player/aniboom.py
--rw-r--r--   0        0        0      827 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/player/animejoy.py
--rw-r--r--   0        0        0     3891 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/player/base.py
--rw-r--r--   0        0        0     1153 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/player/csst.py
--rw-r--r--   0        0        0     1550 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/player/dzen.py
--rw-r--r--   0        0        0     9304 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/player/kodik.py
--rw-r--r--   0        0        0     1639 2024-02-09 17:41:36.435301 anicli_api-0.6.4/anicli_api/player/mailru.py
--rw-r--r--   0        0        0     1447 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/player/nuum.py
--rw-r--r--   0        0        0     1588 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/player/okru.py
--rw-r--r--   0        0        0     1060 2024-01-11 19:00:37.648276 anicli_api-0.6.4/anicli_api/player/sibnet.py
--rw-r--r--   0        0        0      727 2024-02-09 17:41:36.475298 anicli_api-0.6.4/anicli_api/player/sovetromantica.py
--rw-r--r--   0        0        0     1257 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/player/vkcom.py
--rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.6.4/anicli_api/source/__init__.py
--rw-r--r--   0        0        0     2538 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/__template__.py
--rw-r--r--   0        0        0     8242 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/anilibria.py
--rw-r--r--   0        0        0     4341 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/animania.py
--rw-r--r--   0        0        0     7500 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/source/animego.py
--rw-r--r--   0        0        0     8407 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/animejoy.py
--rw-r--r--   0        0        0     9131 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/source/animevost.py
--rw-r--r--   0        0        0     5918 2024-03-27 12:34:29.951966 anicli_api-0.6.4/anicli_api/source/jutsu.py
--rw-r--r--   0        0        0        0 2023-12-07 17:43:53.340574 anicli_api-0.6.4/anicli_api/source/parsers/__init__.py
--rw-r--r--   0        0        0     8506 2024-03-13 06:53:49.113499 anicli_api-0.6.4/anicli_api/source/parsers/animania_parser.py
--rw-r--r--   0        0        0    12813 2024-03-13 06:53:45.953778 anicli_api-0.6.4/anicli_api/source/parsers/animego_parser.py
--rw-r--r--   0        0        0    10525 2024-03-13 06:53:51.029356 anicli_api-0.6.4/anicli_api/source/parsers/animejoy_parser.py
--rw-r--r--   0        0        0    10959 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/parsers/jutsu_parser.py
--rw-r--r--   0        0        0     7962 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/parsers/sameband_parser.py
--rw-r--r--   0        0        0    10546 2024-03-13 06:53:51.313336 anicli_api-0.6.4/anicli_api/source/parsers/sovetromantica_parser.py
--rw-r--r--   0        0        0     4853 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/sameband.py
--rw-r--r--   0        0        0     3646 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/source/sovetromantica.py
--rw-r--r--   0        0        0      121 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/tools/__init__.py
--rw-r--r--   0        0        0     3071 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/tools/dummy_cli.py
--rw-r--r--   0        0        0     5048 2024-03-13 06:53:31.238216 anicli_api-0.6.4/anicli_api/tools/m3u.py
--rw-r--r--   0        0        0     2565 2024-03-27 12:34:29.951966 anicli_api-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    19636 1970-01-01 00:00:00.000000 anicli_api-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    18723 2024-05-06 08:56:39.988944 anicli_api-0.6.5/README.MD
+-rw-r--r--   0        0        0     5798 2024-05-06 08:42:40.266424 anicli_api-0.6.5/anicli_api/_http.py
+-rw-r--r--   0        0        0      278 2023-12-11 18:34:31.718016 anicli_api-0.6.5/anicli_api/_logger.py
+-rw-r--r--   0        0        0     6414 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/base.py
+-rw-r--r--   0        0        0      618 2024-03-13 06:53:31.234216 anicli_api-0.6.5/anicli_api/player/__init__.py
+-rw-r--r--   0        0        0      870 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/player/__template__.py
+-rw-r--r--   0        0        0     3900 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/player/aniboom.py
+-rw-r--r--   0        0        0      827 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/player/animejoy.py
+-rw-r--r--   0        0        0     3891 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/player/base.py
+-rw-r--r--   0        0        0     1153 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/player/csst.py
+-rw-r--r--   0        0        0     1550 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/player/dzen.py
+-rw-r--r--   0        0        0     9304 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/player/kodik.py
+-rw-r--r--   0        0        0     1639 2024-02-09 17:41:36.435301 anicli_api-0.6.5/anicli_api/player/mailru.py
+-rw-r--r--   0        0        0     1447 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/player/nuum.py
+-rw-r--r--   0        0        0     1588 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/player/okru.py
+-rw-r--r--   0        0        0     1060 2024-01-11 19:00:37.648276 anicli_api-0.6.5/anicli_api/player/sibnet.py
+-rw-r--r--   0        0        0      727 2024-02-09 17:41:36.475298 anicli_api-0.6.5/anicli_api/player/sovetromantica.py
+-rw-r--r--   0        0        0     1257 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/player/vkcom.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:38:52.517152 anicli_api-0.6.5/anicli_api/source/__init__.py
+-rw-r--r--   0        0        0     2538 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/__template__.py
+-rw-r--r--   0        0        0     8242 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/anilibria.py
+-rw-r--r--   0        0        0     4341 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/animania.py
+-rw-r--r--   0        0        0     7500 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/source/animego.py
+-rw-r--r--   0        0        0     6073 2024-05-06 08:34:43.845004 anicli_api-0.6.5/anicli_api/source/animego_pro.py
+-rw-r--r--   0        0        0     8407 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/animejoy.py
+-rw-r--r--   0        0        0     9131 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/source/animevost.py
+-rw-r--r--   0        0        0     5918 2024-03-27 12:34:29.951966 anicli_api-0.6.5/anicli_api/source/jutsu.py
+-rw-r--r--   0        0        0        0 2023-12-07 17:43:53.340574 anicli_api-0.6.5/anicli_api/source/parsers/__init__.py
+-rw-r--r--   0        0        0     8834 2024-05-06 08:13:27.995792 anicli_api-0.6.5/anicli_api/source/parsers/animania_parser.py
+-rw-r--r--   0        0        0    12827 2024-05-06 08:13:26.919860 anicli_api-0.6.5/anicli_api/source/parsers/animego_parser.py
+-rw-r--r--   0        0        0    13099 2024-05-06 08:13:27.471825 anicli_api-0.6.5/anicli_api/source/parsers/animego_pro_parser.py
+-rw-r--r--   0        0        0    10688 2024-05-06 08:13:28.571755 anicli_api-0.6.5/anicli_api/source/parsers/animejoy_parser.py
+-rw-r--r--   0        0        0    11048 2024-05-06 08:13:29.555692 anicli_api-0.6.5/anicli_api/source/parsers/jutsu_parser.py
+-rw-r--r--   0        0        0     8682 2024-05-06 08:13:29.999663 anicli_api-0.6.5/anicli_api/source/parsers/sameband_parser.py
+-rw-r--r--   0        0        0     9178 2024-05-06 08:13:29.063723 anicli_api-0.6.5/anicli_api/source/parsers/sovetromantica_parser.py
+-rw-r--r--   0        0        0     4853 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/sameband.py
+-rw-r--r--   0        0        0     3646 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/source/sovetromantica.py
+-rw-r--r--   0        0        0      121 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/tools/__init__.py
+-rw-r--r--   0        0        0     3071 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/tools/dummy_cli.py
+-rw-r--r--   0        0        0     5048 2024-03-13 06:53:31.238216 anicli_api-0.6.5/anicli_api/tools/m3u.py
+-rw-r--r--   0        0        0     2614 2024-05-06 08:57:31.389880 anicli_api-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    19909 1970-01-01 00:00:00.000000 anicli_api-0.6.5/PKG-INFO
```

### Comparing `anicli_api-0.6.4/README.MD` & `anicli_api-0.6.5/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,16 @@
 | animego        | https://animego.org        | NO           | many              | источники kodik, animego, не работает на IP отличных от СНГ                                                                                      |
 | animania       | https://animania.online    | NO           | many              | источник kodik, не работает на IP отличных от СНГ                                                                                                |
 | animejoy       | https://animejoy.ru        | NO           | subtitles         | **имеет cloudflare**, требуется реализация обхода или предварительное получения cookies и headers, много источников                              |
 | sovetromantica | https://sovetromantica.com | NO           | subtitles, author | не на все тайтлы есть видео, у себя хостят                                                                                                       |
 | anilibria      | https://anilibria.tv       | YES          | author            |                                                                                                                                                  |
 | animevost      | https://animevost.org      | YES          | author            |                                                                                                                                                  |
 | jutsu          | https://jut.su             | NO           | once              | Запуск видео в сторонних плеерах зависим от используемого user-agent заголовка в API интерфейсе. Некоторые тайтлы заблокированы на территории РФ |
-| sameband       | https://jut.su             | NO           | author            |                                                                                                                                                  |
+| sameband       | https://sameband.studio    | NO           | author            |                                                                                                                                                  |
+| animego.pro    | https://animego.pro        | NO           | many              | Нестабильный uptime сайта (могут быть проблемы с доступом)                                                                                       |
 
 
 # players description
 
 > Требует дополнения и дополнительные тесты
 
 - name - имя плеера
```

### Comparing `anicli_api-0.6.4/anicli_api/_http.py` & `anicli_api-0.6.5/anicli_api/_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     AsyncClient,
     AsyncHTTPTransport,
     Client,
     HTTPTransport,
     NetworkError,
     Request,
     Response,
-    TimeoutException,
+    TimeoutException, ReadTimeout,
 )
 
 from anicli_api._logger import logger
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Linux; Android 10.0; Nexus 5 Build/MRA58N) "
     "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Mobile Safari/537.36",
@@ -87,18 +87,22 @@
                 resp = super().handle_request(request)
                 if have_ddos_protect(resp):
                     msg = f"'{resp.headers.get('Server')}' detected"
                     raise DDOSServerDetectError(msg)
                 logger.debug("%s -> %s", repr(request), repr(resp))
                 return resp
 
-            except (NetworkError, TimeoutException) as exc:
+            except (NetworkError, TimeoutException, ReadTimeout) as exc:
                 exc_name = exc.__class__.__name__
                 exc_msg = getattr(exc, "message", exc.args[0])
                 sleep(delay)
+                # stub response
+                if exc.__class__ == ReadTimeout:
+                    resp = None
+
                 logger.warning(
                     "[%s] %s: %s, %s -> %s try again", i + 1, exc_name, exc_msg, repr(request), repr(resp)
                 )  # type: ignore
                 if isinstance(exc, DDOSServerDetectError) and i == self.ATTEMPTS_CONNECT - 1:
                     raise exc
                 delay += self.DELAY_INCREASE_STEP
         return super().handle_request(request)
```

### Comparing `anicli_api-0.6.4/anicli_api/base.py` & `anicli_api-0.6.5/anicli_api/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/__init__.py` & `anicli_api-0.6.5/anicli_api/player/__init__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/__template__.py` & `anicli_api-0.6.5/anicli_api/player/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/aniboom.py` & `anicli_api-0.6.5/anicli_api/player/aniboom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/animejoy.py` & `anicli_api-0.6.5/anicli_api/player/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/base.py` & `anicli_api-0.6.5/anicli_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/csst.py` & `anicli_api-0.6.5/anicli_api/player/csst.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/dzen.py` & `anicli_api-0.6.5/anicli_api/player/dzen.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/kodik.py` & `anicli_api-0.6.5/anicli_api/player/kodik.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/mailru.py` & `anicli_api-0.6.5/anicli_api/player/mailru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/nuum.py` & `anicli_api-0.6.5/anicli_api/player/nuum.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/okru.py` & `anicli_api-0.6.5/anicli_api/player/okru.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/sibnet.py` & `anicli_api-0.6.5/anicli_api/player/sibnet.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/sovetromantica.py` & `anicli_api-0.6.5/anicli_api/player/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/player/vkcom.py` & `anicli_api-0.6.5/anicli_api/player/vkcom.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/__template__.py` & `anicli_api-0.6.5/anicli_api/source/__template__.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/anilibria.py` & `anicli_api-0.6.5/anicli_api/source/anilibria.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/animania.py` & `anicli_api-0.6.5/anicli_api/source/animania.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/animego.py` & `anicli_api-0.6.5/anicli_api/source/animego.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/animejoy.py` & `anicli_api-0.6.5/anicli_api/source/animejoy.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/animevost.py` & `anicli_api-0.6.5/anicli_api/source/animevost.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/jutsu.py` & `anicli_api-0.6.5/anicli_api/source/jutsu.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/animania_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/animania_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Auto generated code by ssc_gen
 # WARNING: Any manual changes made to this file will be lost when this
 # is run again. Do not edit this file unless you know what you are doing.
 
 from __future__ import annotations  # python 3.7, 3.8 comp
-
 import re
 from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
 _T_DICT_ITEM = dict[str, Union[str, list[str]]]
 _T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
@@ -37,15 +36,18 @@
         """parse logic entrypoint"""
         pass
 
 
 class AnimeView(_BaseStructParser):
     """send request to anime page
 
-        GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
+        GET https://animania.online/<ANIME_PAGE_PATH>
+
+        EXAMPLE:
+            GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
 
         AnimeView view() item signature:
 
     {
         "title": "String",
         "description": "String",
         "thumbnail": "String"
@@ -142,15 +144,17 @@
         var_3 = "https://animania.online{}".format(var_2)
         return var_3
 
 
 class VideoView(_BaseStructParser):
     """send request to anime page
 
-        GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
+            GET https://animania.online/<ANIME PATH>
+        EXAMPLE:
+            GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
 
         VideoView view() item signature:
 
     {
         "id": "String",
         "names": "Array['String']",
         "urls": "Array['String']"
@@ -209,14 +213,19 @@
 
 class SearchView(_BaseStructParser):
     """Send search request
 
         GET https://animania.online/index.php
         story={QUERY}&do=search&subaction=search
 
+
+        EXAMPLE:
+
+            GET https://animania.online/index.php?do=search&subaction=search&story=LAIN
+
         SearchView view() item signature:
 
     {
         "title": "String",
         "thumbnail": "String",
         "url": "String"
     }
@@ -265,15 +274,18 @@
         var_2 = var_1.attrib["href"]
         return var_2
 
 
 class DubbersView(_BaseStructParser):
     """send to anime page request
 
-        GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
+        GET https://animania.online/<ANIME PATH>
+
+        EXAMPLE:
+            GET https://animania.online/9403-jeksperimenty-ljejn-serial-experiments-lain-1998-smotret-onlajn.html
 
         DubbersView view() item signature:
 
     {
         "key": "String",
         "value": "String"
     }
```

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/animego_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/animego_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Auto generated code by ssc_gen
 # WARNING: Any manual changes made to this file will be lost when this
 # is run again. Do not edit this file unless you know what you are doing.
 
 from __future__ import annotations  # python 3.7, 3.8 comp
-
 import re
 from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
 _T_DICT_ITEM = dict[str, Union[str, list[str]]]
 _T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
@@ -54,21 +53,14 @@
     }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
         self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, doc: Selector) -> None:
-        var_0 = doc
-        var_1 = var_0.css("title")
-        var_2 = var_1.css("::text").get()
-        assert re.search(r"Смотреть Аниме онлайн", var_2)
-        return
-
     def _part_document(self) -> SelectorList:
         doc = self.__selector__
         var_0 = doc
         var_1 = var_0.css(".border-bottom-0.cursor-pointer")
         return var_1
 
     def _start_parse(self):
@@ -129,14 +121,18 @@
 
 class SearchView(_BaseStructParser):
     """Get all search results by query
 
         GET https://animego.org/search/anime
         q={QUERY}
 
+        EXAMPLE:
+
+            GET https://animego.org/search/anime?q=LAIN
+
         SearchView view() item signature:
 
     {
         "title": "String",
         "thumbnail": "String",
         "url": "String"
     }
@@ -182,17 +178,21 @@
         var_0 = doc
         var_1 = var_0.css(".text-truncate a")
         var_2 = var_1.attrib["href"]
         return var_2
 
 
 class AnimeView(_BaseStructParser):
-    """Anime page information
+    """Anime page information. anime path contains in SearchView.url or Ongoing.urk
+
+        GET https://animego.org/anime/<ANIME_PATH>
+
+        EXAMPLE:
 
-        GET https://animego.org/anime/eksperimenty-leyn-1114
+            GET https://animego.org/anime/eksperimenty-leyn-1114
 
         AnimeView view() item signature:
 
     {
         "title": "String",
         "description": "Array['String']",
         "thumbnail": "String",
@@ -201,21 +201,14 @@
     }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
         self._cached_result: _T_DICT_ITEM = {}
 
-    def _pre_validate(self, doc: Selector) -> None:
-        var_0 = doc
-        var_1 = var_0.css("title")
-        var_2 = var_1.css("::text").get()
-        assert re.search(r".* смотреть онлайн .*", var_2)
-        return
-
     def _start_parse(self):
         self._cached_result.clear()
         self._cached_result["title"] = self._parse_title(self.__selector__)
         self._cached_result["description"] = self._parse_description(self.__selector__)
         self._cached_result["thumbnail"] = self._parse_thumbnail(self.__selector__)
         self._cached_result["id"] = self._parse_id(self.__selector__)
         self._cached_result["raw_json"] = self._parse_raw_json(self.__selector__)
@@ -265,14 +258,17 @@
 
         Prepare:
           1. get id from Anime object
           2. GET 'https://animego.org/anime/{Anime.id}/player?_allow=true'
           3. extract html from json by ['content'] key
           4. OPTIONAL: unescape HTML
 
+        EXAMPLE:
+            GET https://animego.org/anime/anime/1114//player?_allow=true
+
         DubbersView view() item signature:
 
     {
         "key": "String",
         "value": "String"
     }
     """
@@ -322,14 +318,17 @@
 
         Prepare:
           1. get id from Anime object
           2. GET 'https://animego.org/anime/{Anime.id}/player?_allow=true'
           3. extract html from json by ['content'] key
           4. OPTIONAL: unescape HTML
 
+        EXAMPLE:
+            GET https://animego.org/anime/anime/1114//player?_allow=true
+
         EpisodeView view() item signature:
 
     {
         "num": "String",
         "title": "String",
         "id": "String"
     }
@@ -391,14 +390,18 @@
           GET https://animego.org/anime/series
           dubbing=2&provider=24&episode={Episode.num}id={Episode.id}
 
           3. extract html from json by ["content"] key
 
           4. OPTIONAL: unescape document
 
+        EXAMPLE:
+
+            GET https://animego.org/anime/series?dubbing=2&provider=24&episode=2&id=15837
+
         SourceView view() item signature:
 
     {
         "title": "String",
         "url": "String",
         "data_provider": "String",
         "data_provide_dubbing": "String"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/animejoy_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/animejoy_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Auto generated code by ssc_gen
 # WARNING: Any manual changes made to this file will be lost when this
 # is run again. Do not edit this file unless you know what you are doing.
 
 from __future__ import annotations  # python 3.7, 3.8 comp
-
 import re
 from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
 _T_DICT_ITEM = dict[str, Union[str, list[str]]]
 _T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
@@ -52,21 +51,14 @@
     }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
         self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, doc: Selector) -> None:
-        var_0 = doc
-        var_1 = var_0.css("title")
-        var_2 = var_1.css("::text").get()
-        assert re.search(r"AnimeJoy.Ru аниме с субтитрами", var_2)
-        return
-
     def _part_document(self) -> SelectorList:
         doc = self.__selector__
         var_0 = doc
         var_1 = var_0.css(".shortstory")
         return var_1
 
     def _start_parse(self):
@@ -111,14 +103,18 @@
 
 
 class SearchView(_BaseStructParser):
     """
         POST https://animejoy.ru/
         story=<QUERY>&do=search&subaction=search
 
+        EXAMPLE:
+            POST https://animejoy.ru
+            story=LAIN&do=search&subaction=search
+
         SearchView view() item signature:
 
     {
         "title": "String",
         "alt_title": "String",
         "thumbnail": "String",
         "url": "String"
@@ -181,15 +177,18 @@
         var_2 = var_1.attrib["href"]
         var_3 = "https://animejoy.ru{}".format(var_2)
         return var_3
 
 
 class AnimeView(_BaseStructParser):
     """
-        GET https://animejoy.ru/tv-serialy/2654-van-pis-1001-.html
+        GET https://animejoy.ru/<ANIME PATH>
+
+        EXAMPLE:
+            GET https://animejoy.ru/tv-serialy/2654-van-pis-1001-.html
 
         AnimeView view() item signature:
 
     {
         "title": "String",
         "alt_title": "String",
         "description": "String",
@@ -263,18 +262,22 @@
         Prepare:
           1. get news_id from Anime class
 
           2.
             GET https://animejoy.ru/engine/ajax/playlists.php
             news_id={Anime.news_id}&xfield=playlist
 
-          3. get json, get HTML by "response" key
+          3. get json, get HTML by ["response"] key
 
           4. OPTIONAL: Unescape document
 
+        EXAMPLE:
+            GET https://animejoy.ru/engine/ajax/playlists.php
+            news_id=2789&xfield=playlist
+
         PlayerView view() item signature:
 
     {
         "key": "String",
         "value": "String"
     }
     """
@@ -323,14 +326,18 @@
           GET https://animejoy.ru/engine/ajax/playlists.php
           news_id={Anime.news_id}&xfield=playlist
 
           3. get json, get HTML by "response" key
 
           4. OPTIONAL: Unescape document
 
+        EXAMPLE:
+            https://animejoy.ru/engine/ajax/playlists.php
+            news_id=2789&xfield=playlist
+
         PlayerUrlsView view() item signature:
 
     {
         "player_id": "String",
         "url": "String"
     }
     """
```

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/jutsu_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/jutsu_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Auto generated code by ssc_gen
 # WARNING: Any manual changes made to this file will be lost when this
 # is run again. Do not edit this file unless you know what you are doing.
 
 from __future__ import annotations  # python 3.7, 3.8 comp
-
 import re
 from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
 _T_DICT_ITEM = dict[str, Union[str, list[str]]]
 _T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
@@ -55,19 +54,14 @@
     }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
         self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, doc: Selector) -> None:
-        var_0 = doc
-        assert var_0.css(".all_anime_global").get()
-        return
-
     def _part_document(self) -> SelectorList:
         doc = self.__selector__
         var_0 = doc
         var_1 = var_0.css(".all_anime_global")
         return var_1
 
     def _start_parse(self):
@@ -131,33 +125,32 @@
 
 
 class SearchView(_BaseStructParser):
     """
         POST https://jut.su/anime/
         ajax_load=yes&start_from_page=1&show_search=<QUERY>&anime_of_user=
 
+        EXAMPLE:
+            POST https://jut.su/anime/
+            ajax_load=yes&start_from_page=1&show_search=LA&anime_of_user=
+
         SearchView view() item signature:
 
     {
         "url": "String",
         "title": "String",
         "thumbnail": "String",
         "counts": "Array['String']"
     }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
         self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, doc: Selector) -> None:
-        var_0 = doc
-        assert var_0.css(".all_anime_global").get()
-        return
-
     def _part_document(self) -> SelectorList:
         doc = self.__selector__
         var_0 = doc
         var_1 = var_0.css(".all_anime_global")
         return var_1
 
     def _start_parse(self):
@@ -218,15 +211,15 @@
         var_3 = [s.strip("\r\n") for s in var_2]
         var_4 = " ".join(var_3)
         return var_4
 
 
 class SourceView(_BaseStructParser):
     """
-        GET https://jut.su/toradora/episode-1.html
+        GET https://jut.su/<ANIME PATH>/<SEASON?>/episode-<NUM>.html
 
         NOTE: VIDEO REQUEST SHOULD HAVE SAME USER-AGENT AS CLIENT
 
         need set user-agent same as send HTTP request in API
 
         eg:
 
@@ -236,14 +229,17 @@
 
         mpv s["url_1080"]  # 403, FORBIDDEN
 
         mpv s["url_1080"] --user-agent="Y"  # 403, FORBIDDEN
 
         mpv s["url_1080"] --user-agent="X"  # 200, OK
 
+        EXAMPLE:
+            GET https://jut.su/kime-no-yaiba/season-1/episode-1.html
+
         SourceView view() item signature:
 
     {
         "url_1080": "String",
         "url_720": "String",
         "url_480": "String",
         "url_360": "String"
@@ -299,15 +295,18 @@
             return var_3
         except Exception as e:
             return None
 
 
 class AnimeView(_BaseStructParser):
     """
-        GET https://jut.su/toradora/
+        GET https://jut.su/<ANIME PATH>
+
+        EXAMPLE:
+            GET https://jut.su/kime-no-yaiba/
 
         AnimeView view() item signature:
 
     {
         "title": "String",
         "description": "Array['String']",
         "thumbnail": "String"
@@ -347,15 +346,18 @@
         var_2 = var_1.attrib["style"]
         var_3 = re.search(r"'(https?://.*?)'", var_2)[1]
         return var_3
 
 
 class EpisodeView(_BaseStructParser):
     """
-        GET https://jut.su/toradora/
+        GET https://jut.su/<ANIME PATH>
+
+        EXAMPLE:
+            GET https://jut.su/kime-no-yaiba/
 
         EpisodeView view() item signature:
 
     {
         "title": "String",
         "url": "String"
     }
```

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/sameband_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/sameband_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Auto generated code by ssc_gen
 # WARNING: Any manual changes made to this file will be lost when this
 # is run again. Do not edit this file unless you know what you are doing.
 
 from __future__ import annotations  # python 3.7, 3.8 comp
-
 import re
 from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
 _T_DICT_ITEM = dict[str, Union[str, list[str]]]
 _T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
@@ -36,16 +35,14 @@
     def _start_parse(self):
         """parse logic entrypoint"""
         pass
 
 
 class OngoingView(_BaseStructParser):
     """GET https://sameband.studio
-
-
         OngoingView view() item signature:
 
     {
         "url": "String",
         "title": "String",
         "thumbnail": "String"
     }
@@ -96,14 +93,21 @@
 
 
 class SearchView(_BaseStructParser):
     """
         POST https://sameband.studio/index.php?do=search
         do=search&subaction=search&search_start=0&full_search=0&result_from=1&story=<QUERY>
 
+        NOTE:
+            search query len should be 4 or more characters. And in manual tests, works only cyrillic queries
+
+        EXAMPLE:
+            POST https://sameband.studio/index.php?do=search
+        do=search&subaction=search&search_start=0&full_search=0&result_from=1&story=ВЕДЬ
+
         SearchView view() item signature:
 
     {
         "title": "String",
         "thumbnail": "String",
         "url": "String"
     }
@@ -151,14 +155,20 @@
         var_1 = var_0.css(".image")
         var_2 = var_1.attrib["href"]
         return var_2
 
 
 class AnimeView(_BaseStructParser):
     """
+        GET https://sameband.studio/anime/<ANIME PATH>.html
+
+        EXAMPLE:
+            # https://sameband.studio/anime/20-госпожа-кагуя-3.html
+            GET https://sameband.studio/anime/20-%D0%B3%D0%BE%D1%81%D0%BF%D0%BE%D0%B6%D0%B0-%D0%BA%D0%B0%D0%B3%D1%83%D1%8F-3.html
+
         AnimeView view() item signature:
 
     {
         "title": "String",
         "alt_title": "String",
         "description": "Array['String']",
         "thumbnail": "String",
@@ -224,34 +234,18 @@
         var_1 = var_0.css(".player > .player-content > iframe")
         var_2 = var_1.attrib["src"]
         var_3 = "https://sameband.studio{}".format(var_2)
         return var_3
 
 
 class PlaylistURLView(_BaseStructParser):
-    """GET https://sameband.studio/pl/a/Mashle_2nd_Season.html
-
-        NOTE: url contains in AnimeView.player_url key
+    """GET https://sameband.studio/pl/a/<PLAYLIST NAME>.html
 
-        playlist items signature (need manually provide json marshall logic):
-
-        [
-      {
-        "title": "<img src='/v/anime/...01 RUS_snapshot.jpg' class=playlist_poster><div class=playlist_duration>23:37</div>... 01",
-        ### delimiter - ','
-        "file": "[480p]/v/anime/... - 01 RUS_480p/... - 01 RUS_r480p.m3u8,[720p]/v/anime/.../... - 01 RUS_720p/... - 01 RUS_r720p.m3u8,[1080p]/v/anime/.../... -
-        01 RUS_1080p/... - 01 RUS_r1080p.m3u8",
-        ### thumbnails images for video
-        "thumbnails": "/v/anime/.../thumbnails/... - 01 RUS.txt"  # contains
-      },
-      {
-      ...
-      },
-      ...
-      ]
+        EXAMPLE:
+            GET https://sameband.studio/pl/a/Mashle_2nd_Season.html
 
         PlaylistURLView view() item signature:
 
     {
         "playlist_url": "String"
     }
     """
@@ -264,12 +258,34 @@
         self._cached_result.clear()
         self._cached_result["playlist_url"] = self._parse_playlist_url(self.__selector__)
 
     def view(self) -> _T_DICT_ITEM:
         return self._cached_result
 
     def _parse_playlist_url(self, doc: Selector):
+        """
+          url contains in AnimeView.player_url key
+
+          playlist items signature (need manually provide json inmarshall logic):
+
+          [
+        {
+          "title": "<img src='/v/anime/...01 RUS_snapshot.jpg' class=playlist_poster><div class=playlist_duration>23:37</div>... 01",
+          ### delimiter - ','
+          "file": "[480p]/v/anime/... - 01 RUS_480p/... - 01 RUS_r480p.m3u8,[720p]/v/anime/.../... - 01 RUS_720p/... - 01 RUS_r720p.m3u8,[1080p]/v/anime/.../... -
+          01 RUS_1080p/... - 01 RUS_r1080p.m3u8",
+          ### thumbnails images for video
+          "thumbnails": "/v/anime/.../thumbnails/... - 01 RUS.txt"  # contains
+        },
+        {
+        ...
+        },
+        ...
+        ]
+
+        """
+
         var_0 = doc
         var_1 = var_0.get()
         var_2 = re.search(r"var\s*player\s*=[^>]+file:[\"']([^>]+)[\"']", var_1)[1]
         var_3 = "https://sameband.studio{}".format(var_2)
         return var_3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `anicli_api-0.6.4/anicli_api/source/parsers/sovetromantica_parser.py` & `anicli_api-0.6.5/anicli_api/source/parsers/sovetromantica_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,383 +1,325 @@
-"""Auto generated code by selector_schema_codegen
+# Auto generated code by ssc_gen
+# WARNING: Any manual changes made to this file will be lost when this
+# is run again. Do not edit this file unless you know what you are doing.
 
-id: sovetromantica
-name: sovetromantica
-author: vypivshiy
-description:
-    sovetromantica parser
-source: https://sovetromantica.com
-tags:
-    any
-
-WARNING: Any manual changes made to this file will be lost when this
-is run again. Do not edit this file unless you know what you are doing.
-"""
-
-from __future__ import annotations  # python 3.7, 3.8 typing comp
-from typing import Any
+from __future__ import annotations  # python 3.7, 3.8 comp
 import re
+from typing import Any, Union
 
 from parsel import Selector, SelectorList
 
+_T_DICT_ITEM = dict[str, Union[str, list[str]]]
+_T_LIST_ITEMS = list[dict[str, Union[str, list[str]]]]
+
 
-class __BaseViewModel:
+class _BaseStructParser:
     def __init__(self, document: str):
         self.__raw__ = document
         self.__selector__ = Selector(document)
-        self._cached_result: list[dict[str, Any]] = []
-        self._aliases: dict[str, str] = {}
-        self._view_keys: list[str] = []
-
-    def _pre_validate(self, doc):
-        pass
-
-    def _start_parse(self):
-        pass
+        self._cached_result: Union[_T_DICT_ITEM, _T_LIST_ITEMS] = {}
 
-    def _part_document(self, part: Selector):
+    def _pre_validate(self, document: Selector) -> None:
+        # pre validate entrypoint, contain assert expressions
         pass
 
     def parse(self):
+        """run parser"""
         self._pre_validate(self.__selector__)
         self._start_parse()
         return self
 
-    def view(self) -> list[dict[str, list[str] | str]]:
-        def map_fields(result):
-            view_dict = {}
-            for k in self._view_keys:
-                v = result.get(k)
-                if v != None:
-                    k = self._aliases.get(k, k)
-                    view_dict[k] = v
-            return view_dict
-
-        if len(self._cached_result) == 1:
-            return [map_fields(self._cached_result[0])]
-        return [map_fields(result) for result in self._cached_result]
+    def view(self) -> Union[_T_DICT_ITEM, _T_LIST_ITEMS]:
+        """get parsed values"""
+        return self._cached_result
 
+    def _start_parse(self):
+        """parse logic entrypoint"""
+        pass
 
-class OngoingView(__BaseViewModel):
-    """
-      Prepare:
-    1. GET https://sovetromantica.com/anime
-
-      view() elements signature:
-
-          thumbnail <TEXT> -
-
-          title <TEXT> -
-
-          alt_title <TEXT> -
 
-          url <TEXT> -
+class OngoingView(_BaseStructParser):
+    """
+        GET https://sovetromantica.com/anime
 
+        OngoingView view() item signature:
 
+    {
+        "url": "String",
+        "title": "String",
+        "thumbnail": "String",
+        "alt_title": "String"
+    }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
-        self._aliases = {}
-        self._view_keys = ["thumbnail", "title", "alt_title", "url"]
+        self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, part: Selector):
-        val_0 = part.css("title")
-        val_1 = val_0.css("::text").get()
-        assert re.search(r"Аниме / SovetRomantica", val_1)
-
-    def _part_document(self, part: Selector):
-        val_0 = part.css(".anime--block__desu")
-        return val_0
-
-    def _parse_thumbnail(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--poster--loading > img"
-        # attr "src"
-        #
-        val_0 = part.css(".anime--poster--loading > img")
-        val_1 = val_0.attrib["src"]
-        return val_1
-
-    def _parse_title(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__name > span + span"
-        # text
-        #
-        val_0 = part.css(".anime--block__name > span + span")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_alt_title(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__name > span"
-        # text
-        #
-        val_0 = part.css(".anime--block__name > span")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_url(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__desu a"
-        # attr "href"
-        #
-        val_0 = part.css(".anime--block__desu a")
-        val_1 = val_0.attrib["href"]
-        return val_1
+    def _part_document(self) -> SelectorList:
+        doc = self.__selector__
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__desu")
+        return var_1
 
     def _start_parse(self):
-        # clear cache
         self._cached_result.clear()
-        for part in self._part_document(self.__selector__):
+        for part in self._part_document():
             self._cached_result.append(
                 {
-                    "thumbnail": self._parse_thumbnail(part),
+                    "url": self._parse_url(part),
                     "title": self._parse_title(part),
+                    "thumbnail": self._parse_thumbnail(part),
                     "alt_title": self._parse_alt_title(part),
-                    "url": self._parse_url(part),
                 }
             )
 
+    def view(self) -> _T_LIST_ITEMS:
+        return self._cached_result
 
-class SearchView(__BaseViewModel):
-    """
-      Prepare:
-    1. GET https://sovetromantica.com/anime?query=<QUERY>
-
-      view() elements signature:
-
-          thumbnail <TEXT> -
-
-          title <TEXT> -
-
-          alt_title <TEXT> -
-
-          url <TEXT> -
-
+    def _parse_url(self, doc: Selector):
+        """ongoing page"""
 
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__desu a")
+        var_2 = var_1.attrib["href"]
+        return var_2
+
+    def _parse_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__name > span + span")
+        var_2 = var_1.css("::text").get()
+        return var_2
+
+    def _parse_thumbnail(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--poster--loading > img")
+        var_2 = var_1.attrib["src"]
+        return var_2
+
+    def _parse_alt_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__name > span")
+        var_2 = var_1.css("::text").get()
+        return var_2
+
+
+class SearchView(_BaseStructParser):
+    """Get all search results by query
+
+        GET https://sovetromantica.com/anime
+        query=<QUERY>
+
+        EXAMPLE:
+            GET https://sovetromantica.com/anime
+            query=LAIN
+
+        SearchView view() item signature:
+
+    {
+        "title": "String",
+        "thumbnail": "String",
+        "alt_title": "String",
+        "url": "String"
+    }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
-        self._aliases = {}
-        self._view_keys = ["thumbnail", "title", "alt_title", "url"]
+        self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, part: Selector):
-        val_0 = part.css("title")
-        val_1 = val_0.css("::text").get()
-        assert re.search(r"\w+ / SovetRomantica", val_1)
-
-    def _part_document(self, part: Selector):
-        val_0 = part.css(".anime--block__desu")
-        return val_0
-
-    def _parse_thumbnail(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--poster--loading > img"
-        # attr "src"
-        #
-        val_0 = part.css(".anime--poster--loading > img")
-        val_1 = val_0.attrib["src"]
-        return val_1
-
-    def _parse_title(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__name > span + span"
-        # text
-        #
-        val_0 = part.css(".anime--block__name > span + span")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_alt_title(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__name > span"
-        # text
-        #
-        val_0 = part.css(".anime--block__name > span")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_url(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime--block__desu a"
-        # attr "href"
-        #
-        val_0 = part.css(".anime--block__desu a")
-        val_1 = val_0.attrib["href"]
-        return val_1
+    def _pre_validate(self, doc: Selector) -> None:
+        var_0 = doc
+        var_1 = var_0.css("title")
+        var_2 = var_1.css("::text").get()
+        assert re.search(r"Аниме / SovetRomantica", var_2)
+        return
+
+    def _part_document(self) -> SelectorList:
+        doc = self.__selector__
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__desu")
+        return var_1
 
     def _start_parse(self):
-        # clear cache
         self._cached_result.clear()
-        for part in self._part_document(self.__selector__):
+        for part in self._part_document():
             self._cached_result.append(
                 {
-                    "thumbnail": self._parse_thumbnail(part),
                     "title": self._parse_title(part),
+                    "thumbnail": self._parse_thumbnail(part),
                     "alt_title": self._parse_alt_title(part),
                     "url": self._parse_url(part),
                 }
             )
 
+    def view(self) -> _T_LIST_ITEMS:
+        return self._cached_result
 
-class AnimeView(__BaseViewModel):
+    def _parse_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__name > span + span")
+        var_2 = var_1.css("::text").get()
+        return var_2
+
+    def _parse_thumbnail(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--poster--loading > img")
+        var_2 = var_1.attrib["src"]
+        return var_2
+
+    def _parse_alt_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__name > span")
+        var_2 = var_1.css("::text").get()
+        return var_2
+
+    def _parse_url(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime--block__desu a")
+        var_2 = var_1.attrib["href"]
+        return var_2
+
+
+class AnimeView(_BaseStructParser):
+    """Anime page information
+
+        GET https://sovetromantica.com/anime/<ANIME PATH>
+
+        EXAMPLE:
+            GET https://sovetromantica.com/anime/1459-sousou-no-frieren
+
+        AnimeView view() item signature:
+
+    {
+        "title": "String",
+        "description": "String",
+        "thumbnail": "String",
+        "video": "String"
+    }
     """
-      Prepare:
-    1. GET to anime URL page
 
-      view() elements signature:
-
-          thumbnail <TEXT> -
+    def __init__(self, document: str):
+        super().__init__(document)
+        self._cached_result: _T_DICT_ITEM = {}
 
-          title <TEXT> -
+    def _start_parse(self):
+        self._cached_result.clear()
+        self._cached_result["title"] = self._parse_title(self.__selector__)
+        self._cached_result["description"] = self._parse_description(self.__selector__)
+        self._cached_result["thumbnail"] = self._parse_thumbnail(self.__selector__)
+        self._cached_result["video"] = self._parse_video(self.__selector__)
+
+    def view(self) -> _T_DICT_ITEM:
+        return self._cached_result
+
+    def _parse_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css(".anime-name .block--container")
+        var_2 = var_1.css("::text").get()
+        return var_2
 
-          description <TEXT> -
+    def _parse_description(self, doc: Selector):
+        var_0 = doc
+        try:
+            var_2 = var_0.css("#js-description_open-full")
+            var_3 = var_2.css("::text").get()
+            return var_3
+        except Exception as e:
+            return ""
 
-          video <TEXT> -
+    def _parse_thumbnail(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css("#poster")
+        var_2 = var_1.attrib["src"]
+        var_3 = "https://sovetromantica.com{}".format(var_2)
+        return var_3
 
+    def _parse_video(self, doc: Selector):
+        """WARNING!
 
-    """
+        in main page give first episode video contains in <meta> tag and maybe does not exist
 
-    def __init__(self, document: str):
-        super().__init__(document)
-        self._aliases = {}
-        self._view_keys = ["thumbnail", "title", "description", "video"]
+        EG:
 
-    def _pre_validate(self, part: Selector):
-        val_0 = part.css("title")
-        val_1 = val_0.css("::text").get()
-        assert re.search(r"/ SovetRomantica", val_1)
-
-    def _part_document(self, part: Selector):
-        return [part]
-
-    def _parse_thumbnail(self, part: Selector) -> str:
-        # script signature:
-        # css "#poster"
-        # attr "src"
-        # format "https://sovetromantica.com{{}}"
-        #
-        val_0 = part.css("#poster")
-        val_1 = val_0.attrib["src"]
-        val_2 = "https://sovetromantica.com{}".format(val_1)
-        return val_2
-
-    def _parse_title(self, part: Selector) -> str:
-        # script signature:
-        # css ".anime-name .block--container"
-        # text
-        #
-        val_0 = part.css(".anime-name .block--container")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_description(self, part: Selector) -> str:
-        # script signature:
-        # css ".block--full .anime-description"
-        # text
-        #
-        val_0 = part.css(".block--full .anime-description")
-        val_1 = val_0.css("::text").get()
-        return val_1
-
-    def _parse_video(self, part: Selector) -> str:
-        # script signature:
-        # default ""
-        # raw
-        # re "<meta property=\".*\" content=\"(https://.*?\.m3u8)\""
-        #
-        try:
-            val_1 = part.get()
-            val_2 = re.search(r"<meta property=\".*\" content=\"(https://.*?\.m3u8)\"", val_1)[1]
-            return val_2
+          https://sovetromantica.com/anime/1398-tsundere-akuyaku-reijou-liselotte-to-jikkyou-no-endou-kun-to-kaisetsu-no-kobayashi-san
 
-        except Exception:
-            return ""
+        """
 
-    def _start_parse(self):
-        # clear cache
-        self._cached_result.clear()
-        for part in self._part_document(self.__selector__):
-            self._cached_result.append(
-                {
-                    "thumbnail": self._parse_thumbnail(part),
-                    "title": self._parse_title(part),
-                    "description": self._parse_description(part),
-                    "video": self._parse_video(part),
-                }
-            )
+        var_0 = doc
+        try:
+            var_2 = var_0.get()
+            var_3 = re.search(r"\"file\":\"([^>]+\.m3u8)\"\s*}", var_2)[1]
+            return var_3
+        except Exception as e:
+            return None
 
 
-class EpisodeView(__BaseViewModel):
-    """
-        WARNING! target page maybe does not contains video!
-    Prepare:
-      1. GET to anime page
+class EpisodeView(_BaseStructParser):
+    """WARNING!
 
-        view() elements signature:
+        target page maybe does not contain video!
 
-            url <TEXT> -
+        GET https://sovetromantica.com/anime/<ANIME PATH>
 
-            thumbnail <TEXT> -
+        EXAMPLE:
+            GET https://sovetromantica.com/anime/1459-sousou-no-frieren
 
-            title <TEXT> -
 
+        EpisodeView view() item signature:
 
+    {
+        "url": "String",
+        "thumbnail": "String",
+        "title": "String"
+    }
     """
 
     def __init__(self, document: str):
         super().__init__(document)
-        self._aliases = {}
-        self._view_keys = ["url", "thumbnail", "title"]
+        self._cached_result: _T_LIST_ITEMS = []
 
-    def _pre_validate(self, part: Selector):
-        val_0 = part.css("title")
-        val_1 = val_0.css("::text").get()
-        assert re.search(r"/ SovetRomantica", val_1)
-
-    def _part_document(self, part: Selector):
-        val_0 = part.css(".episodes-slick_item")
-        return val_0
-
-    def _parse_url(self, part: Selector) -> str:
-        # script signature:
-        # css "a"
-        # attr "href"
-        # format "https://sovetromantica.com{{}}"
-        #
-        val_0 = part.css("a")
-        val_1 = val_0.attrib["href"]
-        val_2 = "https://sovetromantica.com{}".format(val_1)
-        return val_2
-
-    def _parse_thumbnail(self, part: Selector) -> str:
-        # script signature:
-        # css "img"
-        # attr "src"
-        # format "https://sovetromantica.com{{}}"
-        #
-        val_0 = part.css("img")
-        val_1 = val_0.attrib["src"]
-        val_2 = "https://sovetromantica.com{}".format(val_1)
-        return val_2
-
-    def _parse_title(self, part: Selector) -> str:
-        # script signature:
-        # css "img"
-        # attr "alt"
-        val_0 = part.css("img")
-        val_1 = val_0.attrib["alt"]
-        return val_1
+    def _pre_validate(self, doc: Selector) -> None:
+        var_0 = doc
+        var_1 = var_0.css("title")
+        var_2 = var_1.css("::text").get()
+        assert re.search(r"/ SovetRomantica", var_2)
+        return
+
+    def _part_document(self) -> SelectorList:
+        doc = self.__selector__
+        var_0 = doc
+        var_1 = var_0.css(".episodes-slick_item")
+        return var_1
 
     def _start_parse(self):
-        # clear cache
         self._cached_result.clear()
-        for part in self._part_document(self.__selector__):
+        for part in self._part_document():
             self._cached_result.append(
                 {
                     "url": self._parse_url(part),
                     "thumbnail": self._parse_thumbnail(part),
                     "title": self._parse_title(part),
                 }
             )
+
+    def view(self) -> _T_LIST_ITEMS:
+        return self._cached_result
+
+    def _parse_url(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css("a")
+        var_2 = var_1.attrib["href"]
+        var_3 = "https://sovetromantica.com{}".format(var_2)
+        return var_3
+
+    def _parse_thumbnail(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css("img")
+        var_2 = var_1.attrib["src"]
+        return var_2
+
+    def _parse_title(self, doc: Selector):
+        var_0 = doc
+        var_1 = var_0.css("img")
+        var_2 = var_1.attrib["alt"]
+        return var_2
```

### Comparing `anicli_api-0.6.4/anicli_api/source/sameband.py` & `anicli_api-0.6.5/anicli_api/source/sameband.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/source/sovetromantica.py` & `anicli_api-0.6.5/anicli_api/source/sovetromantica.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/tools/dummy_cli.py` & `anicli_api-0.6.5/anicli_api/tools/dummy_cli.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/anicli_api/tools/m3u.py` & `anicli_api-0.6.5/anicli_api/tools/m3u.py`

 * *Files identical despite different names*

### Comparing `anicli_api-0.6.4/pyproject.toml` & `anicli_api-0.6.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anicli_api"
-version = "0.6.4"
+version = "0.6.5"
 description = "Anime extractors api implementation"
 authors = ["vypivshiy"]
 license = "MIT"
 readme = "README.MD"
 packages = [{include = "anicli_api"}]
 exclude = ["tests/", 'scripts/', 'libanime_schema/', 'dev/']
 keywords = [
@@ -109,7 +109,10 @@
 [tool.black]
 line-length = 120
 target-version = ['py38']
 
 [tool.isort]
 profile = "black"
 line_length = 120
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `anicli_api-0.6.4/PKG-INFO` & `anicli_api-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli_api
-Version: 0.6.4
+Version: 0.6.5
 Summary: Anime extractors api implementation
 License: MIT
 Keywords: anime,api,ru,russia,asyncio,parser,httpx,dev
 Author: vypivshiy
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -193,15 +193,16 @@
 | animego        | https://animego.org        | NO           | many              | источники kodik, animego, не работает на IP отличных от СНГ                                                                                      |
 | animania       | https://animania.online    | NO           | many              | источник kodik, не работает на IP отличных от СНГ                                                                                                |
 | animejoy       | https://animejoy.ru        | NO           | subtitles         | **имеет cloudflare**, требуется реализация обхода или предварительное получения cookies и headers, много источников                              |
 | sovetromantica | https://sovetromantica.com | NO           | subtitles, author | не на все тайтлы есть видео, у себя хостят                                                                                                       |
 | anilibria      | https://anilibria.tv       | YES          | author            |                                                                                                                                                  |
 | animevost      | https://animevost.org      | YES          | author            |                                                                                                                                                  |
 | jutsu          | https://jut.su             | NO           | once              | Запуск видео в сторонних плеерах зависим от используемого user-agent заголовка в API интерфейсе. Некоторые тайтлы заблокированы на территории РФ |
-| sameband       | https://jut.su             | NO           | author            |                                                                                                                                                  |
+| sameband       | https://sameband.studio    | NO           | author            |                                                                                                                                                  |
+| animego.pro    | https://animego.pro        | NO           | many              | Нестабильный uptime сайта (могут быть проблемы с доступом)                                                                                       |
 
 
 # players description
 
 > Требует дополнения и дополнительные тесты
 
 - name - имя плеера
```

