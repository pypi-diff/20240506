# Comparing `tmp/pyxbox-0.1.4.tar.gz` & `tmp/pyxbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxbox-0.1.4.tar", last modified: Thu Aug 17 14:10:14 2023, max compression
+gzip compressed data, was "dist\pyxbox-0.1.5.tar", last modified: Mon May  6 15:32:41 2024, max compression
```

## Comparing `pyxbox-0.1.4.tar` & `pyxbox-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-17 14:10:14.003959 pyxbox-0.1.4/
--rw-rw-rw-   0        0        0     1087 2023-05-28 05:11:25.000000 pyxbox-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1510 2023-08-17 14:10:14.002961 pyxbox-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1254 2023-08-17 14:02:30.000000 pyxbox-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-17 14:10:13.983621 pyxbox-0.1.4/pyxbox/
--rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-17 14:10:14.000967 pyxbox-0.1.4/pyxbox/bilibili_utils/
--rw-rw-rw-   0        0        0      344 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/ApiException.py
--rw-rw-rw-   0        0        0     5113 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/BytesReader.py
--rw-rw-rw-   0        0        0     2218 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/Color.py
--rw-rw-rw-   0        0        0     3382 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/Danmaku.py
--rw-rw-rw-   0        0        0      337 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/DanmakuClosedException.py
--rw-rw-rw-   0        0        0      378 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/ResponseException.py
--rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/__init__.py
--rw-rw-rw-   0        0        0     3667 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/utils.py
--rw-rw-rw-   0        0        0      598 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/bilibili_utils/varint.py
--rw-rw-rw-   0        0        0     2963 2023-05-29 13:28:13.000000 pyxbox-0.1.4/pyxbox/mail.py
--rw-rw-rw-   0        0        0     4127 2023-08-17 13:56:36.000000 pyxbox-0.1.4/pyxbox/media.py
--rw-rw-rw-   0        0        0    10266 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/proxies.py
--rw-rw-rw-   0        0        0    79745 2023-05-28 07:23:35.000000 pyxbox-0.1.4/pyxbox/tools.py
--rw-rw-rw-   0        0        0    42825 2023-05-28 05:11:25.000000 pyxbox-0.1.4/pyxbox/user_agent.py
--rw-rw-rw-   0        0        0     1857 2023-08-17 14:02:30.000000 pyxbox-0.1.4/pyxbox/weibo_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-17 14:10:13.990678 pyxbox-0.1.4/pyxbox.egg-info/
--rw-rw-rw-   0        0        0     1510 2023-08-17 14:10:13.000000 pyxbox-0.1.4/pyxbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-08-17 14:10:13.000000 pyxbox-0.1.4/pyxbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-17 14:10:13.000000 pyxbox-0.1.4/pyxbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-08-17 14:10:13.000000 pyxbox-0.1.4/pyxbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-17 14:10:13.000000 pyxbox-0.1.4/pyxbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-17 14:10:14.003959 pyxbox-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-08-17 14:02:30.000000 pyxbox-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:32:41.000000 pyxbox-0.1.5/
+-rw-rw-rw-   0        0        0     1087 2024-05-06 15:27:51.000000 pyxbox-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1510 2024-05-06 15:32:41.000000 pyxbox-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1254 2024-05-06 15:27:51.000000 pyxbox-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox/
+-rw-rw-rw-   0        0        0      232 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/
+-rw-rw-rw-   0        0        0      344 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/ApiException.py
+-rw-rw-rw-   0        0        0     5113 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/BytesReader.py
+-rw-rw-rw-   0        0        0     2218 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/Color.py
+-rw-rw-rw-   0        0        0     3382 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/Danmaku.py
+-rw-rw-rw-   0        0        0      337 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/DanmakuClosedException.py
+-rw-rw-rw-   0        0        0      378 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/ResponseException.py
+-rw-rw-rw-   0        0        0      232 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/__init__.py
+-rw-rw-rw-   0        0        0     3667 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/utils.py
+-rw-rw-rw-   0        0        0      598 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/bilibili_utils/varint.py
+-rw-rw-rw-   0        0        0     2963 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/mail.py
+-rw-rw-rw-   0        0        0     4127 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/media.py
+-rw-rw-rw-   0        0        0    10266 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/proxies.py
+-rw-rw-rw-   0        0        0    79967 2024-05-06 15:29:43.000000 pyxbox-0.1.5/pyxbox/tools.py
+-rw-rw-rw-   0        0        0    42825 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/user_agent.py
+-rw-rw-rw-   0        0        0     1857 2024-05-06 15:27:51.000000 pyxbox-0.1.5/pyxbox/weibo_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/
+-rw-rw-rw-   0        0        0     1510 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 15:32:41.000000 pyxbox-0.1.5/pyxbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:32:41.000000 pyxbox-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-06 15:29:43.000000 pyxbox-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyxbox-0.1.4/LICENSE` & `pyxbox-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/PKG-INFO` & `pyxbox-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbox
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitee.com/spider-x/pyxbox
 Author: BruceLong
 Author-email: 18656170559@163.com
 License: MIT Licence
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyxbox-0.1.4/README.md` & `pyxbox-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/bilibili_utils/BytesReader.py` & `pyxbox-0.1.5/pyxbox/bilibili_utils/BytesReader.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/bilibili_utils/Color.py` & `pyxbox-0.1.5/pyxbox/bilibili_utils/Color.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/bilibili_utils/Danmaku.py` & `pyxbox-0.1.5/pyxbox/bilibili_utils/Danmaku.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/bilibili_utils/utils.py` & `pyxbox-0.1.5/pyxbox/bilibili_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/bilibili_utils/varint.py` & `pyxbox-0.1.5/pyxbox/bilibili_utils/varint.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/mail.py` & `pyxbox-0.1.5/pyxbox/mail.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/media.py` & `pyxbox-0.1.5/pyxbox/media.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/proxies.py` & `pyxbox-0.1.5/pyxbox/proxies.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/tools.py` & `pyxbox-0.1.5/pyxbox/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1985,44 +1985,42 @@
 
 
 # ************************************************ SQL数据库相关 --end ************************************************
 
 # ************************************************ b站转码相关模块 --start ************************************************
 class Bilibili:
     def __init__(self):
-        self.table = 'fZodR9XQDSUm21yCkr6zBqiveYah8bt4xsWpHnJE7jL5VG3guMTKNPAwcF'
-        self.tr = {}
-        for i in range(58):
-            self.tr[self.table[i]] = i
-        self.s = [11, 10, 3, 8, 4, 6]
-        self.xor = 177451812
-        self.add = 8728348608
+        self.XOR_CODE = 23442827791579
+        self.MASK_CODE = 2251799813685247
+        self.MAX_AID = 1 << 51
+        self.ALPHABET = "FcwAPNKTMug3GV5Lj7EJnHpWsx4tb8haYeviqBz6rkCy12mUSDQX9RdoZf"
+        self.ENCODE_MAP = 8, 7, 0, 5, 1, 3, 2, 4, 6
+        self.DECODE_MAP = tuple(reversed(self.ENCODE_MAP))
+        self.BASE = len(self.ALPHABET)
+        self.PREFIX = "BV1"
+        self.PREFIX_LEN = len(self.PREFIX)
+        self.CODE_LEN = len(self.ENCODE_MAP)
 
     def bv_to_av(self, bvd: str) -> int:
-        '''
-        bv转av
-        :param bvd: eg:BV1UY411p7jc
-        :return: av
-        '''
-        r = 0
-        for i in range(6):
-            r += self.tr[bvd[self.s[i]]] * 58 ** i
-        return (r - self.add) ^ self.xor
+        assert bvd[:3] == self.PREFIX
+
+        bvd = bvd[3:]
+        tmp = 0
+        for i in range(self.CODE_LEN):
+            idx = self.ALPHABET.index(bvd[self.DECODE_MAP[i]])
+            tmp = tmp * self.BASE + idx
+        return (tmp & self.MASK_CODE) ^ self.XOR_CODE
 
     def av_to_bv(self, avd: int) -> str:
-        '''
-        av转bv
-        :param avd: eg:252242806
-        :return:
-        '''
-        x = (avd ^ self.xor) + self.add
-        r = list('BV1  4 1 7  ')
-        for i in range(6):
-            r[self.s[i]] = self.table[x // 58 ** i % 58]
-        return ''.join(r)
+        bvid = [""] * 9
+        tmp = (self.MAX_AID | avd) ^ self.XOR_CODE
+        for i in range(self.CODE_LEN):
+            bvid[self.ENCODE_MAP[i]] = self.ALPHABET[tmp % self.BASE]
+            tmp //= self.BASE
+        return self.PREFIX + "".join(bvid)
 
     def decode_view(self, stream: bytes):
         '''
         获取弹幕的视图函数
         :param stream: 请求的二进制流
         :return:
         '''
```

### Comparing `pyxbox-0.1.4/pyxbox/user_agent.py` & `pyxbox-0.1.5/pyxbox/user_agent.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox/weibo_utils.py` & `pyxbox-0.1.5/pyxbox/weibo_utils.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/pyxbox.egg-info/PKG-INFO` & `pyxbox-0.1.5/pyxbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbox
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitee.com/spider-x/pyxbox
 Author: BruceLong
 Author-email: 18656170559@163.com
 License: MIT Licence
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyxbox-0.1.4/pyxbox.egg-info/SOURCES.txt` & `pyxbox-0.1.5/pyxbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.4/setup.py` & `pyxbox-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     README = readme.read()
 
 # 允许setup.py在任何路径下执行
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="pyxbox",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     long_description=README,  # 详细描述（一般会写在README.md中）
     long_description_content_type="text/markdown",  # README.md中描述的语法（一般为markdown）
     url="https://gitee.com/spider-x/pyxbox",
     author="BruceLong",
     license="MIT Licence",
     author_email="18656170559@163.com",
```

