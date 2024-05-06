# Comparing `tmp/translate_util-1.0.9.tar.gz` & `tmp/translate_util-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/translate_util-1.0.9.tar", last modified: Wed Aug 24 03:21:53 2022, max compression
+gzip compressed data, was "dist/translate_util-1.1.0.tar", last modified: Mon May  6 04:14:28 2024, max compression
```

## Comparing `translate_util-1.0.9.tar` & `translate_util-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-24 03:21:53.000000 translate_util-1.0.9/
--rw-r--r--   0 admin      (501) staff       (20)     2206 2022-08-24 03:21:53.000000 translate_util-1.0.9/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1126 2022-03-25 06:09:58.000000 translate_util-1.0.9/README.md
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-08-24 03:21:53.000000 translate_util-1.0.9/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1177 2022-08-24 03:20:35.000000 translate_util-1.0.9/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util/
--rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.0.9/translate_util/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      641 2022-08-24 03:09:36.000000 translate_util-1.0.9/translate_util/base_translate.py
--rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.0.9/translate_util/common_request.py
--rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.0.9/translate_util/translate_baidu.py
--rw-r--r--   0 admin      (501) staff       (20)     1386 2022-08-24 03:13:27.000000 translate_util-1.0.9/translate_util/translate_google.py
--rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.0.9/translate_util/translate_iciba.py
--rw-r--r--   0 admin      (501) staff       (20)     3996 2022-08-24 03:21:15.000000 translate_util-1.0.9/translate_util/translate_tool.py
--rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.0.9/translate_util/translate_youdao.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2206 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      471 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       63 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       15 2022-08-24 03:21:53.000000 translate_util-1.0.9/translate_util.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 04:14:28.000000 translate_util-1.1.0/
+-rw-r--r--   0 admin      (501) staff       (20)     1790 2024-05-06 04:14:28.000000 translate_util-1.1.0/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      774 2024-05-06 04:12:29.000000 translate_util-1.1.0/README.md
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-06 04:14:28.000000 translate_util-1.1.0/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1177 2024-05-06 03:32:25.000000 translate_util-1.1.0/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util/
+-rw-r--r--   0 admin      (501) staff       (20)       60 2020-06-12 15:15:27.000000 translate_util-1.1.0/translate_util/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      713 2024-05-06 03:30:42.000000 translate_util-1.1.0/translate_util/base_translate.py
+-rw-r--r--   0 admin      (501) staff       (20)      756 2020-06-13 13:57:02.000000 translate_util-1.1.0/translate_util/common_request.py
+-rw-r--r--   0 admin      (501) staff       (20)     5817 2022-08-24 03:09:35.000000 translate_util-1.1.0/translate_util/translate_baidu.py
+-rw-r--r--   0 admin      (501) staff       (20)     2937 2024-05-06 04:03:54.000000 translate_util-1.1.0/translate_util/translate_google.py
+-rw-r--r--   0 admin      (501) staff       (20)     1608 2022-08-24 03:14:57.000000 translate_util-1.1.0/translate_util/translate_iciba.py
+-rw-r--r--   0 admin      (501) staff       (20)     4178 2024-05-06 03:55:52.000000 translate_util-1.1.0/translate_util/translate_tool.py
+-rw-r--r--   0 admin      (501) staff       (20)     1801 2022-08-24 03:16:53.000000 translate_util-1.1.0/translate_util/translate_youdao.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     1790 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      471 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       15 2024-05-06 04:14:28.000000 translate_util-1.1.0/translate_util.egg-info/top_level.txt
```

### Comparing `translate_util-1.0.9/PKG-INFO` & `translate_util-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate_util
-Version: 1.0.9
+Version: 1.1.0
 Summary: translate tool support(google,baidu,iciba,youdao)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -20,34 +20,26 @@
         ```shell
         pip install translate-util
         ```
         
         ### DEMO
         
         ```python
-            from translate_util.translate_tool import translate_other2cn,translate_other2en
+            from translate_util.translate_tool import translate_other2cn,translate_other2en,translate_text
             
             # translate other language to chinese (default use google)
             print(translate_other2cn('china'))
             
             # translate other language to english (default use google)
             print(translate_other2en('中国'))
             
-            # other plat translate demo
-            content = 'china'
-            for plat in ['google', 'baidu', 'youdao']:
-                print(f'{plat}:{translate_other2cn(content, plat)}')
-        
-            content = '中国'
-            for plat in ['google', 'baidu', 'youdao']:
-                print(f'{plat}:{translate_other2en(content, plat)}')
+            # translate other language to de ,support any language
+            print(translate_text('china', tl='de'))
+            
             
-            # if your request is limit by google,please use proxies ip
-            tran_rs = translate_other2cn(content='chinese', platform='google', proxies='5.34.178.48:8080')
-            print(tran_rs)
         ```
         
         ### OTHER SUPPORT
         any customization demand,contact me with email
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `translate_util-1.0.9/setup.py` & `translate_util-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @TIME 2020/04/29 23:26
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='translate_util',
-    version='1.0.9',
+    version='1.1.0',
     description=(
         'translate tool support(google,baidu,iciba,youdao)'
     ),
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     author='cc',
     author_email='abcdef123456chen@sohu.com',
```

### Comparing `translate_util-1.0.9/translate_util/base_translate.py` & `translate_util-1.1.0/translate_util/base_translate.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,7 +21,10 @@
         pass
 
     def trans_text_other2cn(self):
         pass
 
     def trans_text_other2en(self):
         pass
+
+    def trans_text(self, st: str, sl='auto', tl='zh-CN'):
+        pass
```

### Comparing `translate_util-1.0.9/translate_util/common_request.py` & `translate_util-1.1.0/translate_util/common_request.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.0.9/translate_util/translate_baidu.py` & `translate_util-1.1.0/translate_util/translate_baidu.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.0.9/translate_util/translate_iciba.py` & `translate_util-1.1.0/translate_util/translate_iciba.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.0.9/translate_util/translate_tool.py` & `translate_util-1.1.0/translate_util/translate_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 # -*- coding:utf-8 -*-
 # @Author cc
 # @TIME 2020/5/25 16:46
 import traceback
 
 from retrying import retry
-from translate_util.translate_baidu import BaiduTranslate
 from translate_util.translate_google import GoogleTranslate
-# from translate_util.translate_iciba import IcibaTranslate
-from translate_util.translate_youdao import YoudaoTranslate
 
 
 @retry(stop_max_attempt_number=3)
 def translate_en2cn(content: str, platform: str = 'google', proxies: str = None):
     """
     根据翻译平台将中文翻译成英文
     :param content: 带翻译的平台
     :param platform: 使用的翻译平台 google,baidu,iciba,youdao
     :param proxies: 代理IP(5.34.178.48:8080)
     :return: 翻译后的内容 string
     """
     try:
         if platform == 'google':
             return GoogleTranslate(content=content, proxies=proxies).trans_text_en2cn()
-        elif platform == 'baidu':
-            return BaiduTranslate(content=content, proxies=proxies).trans_text_en2cn()
-        elif platform == 'iciba':
-            return BaiduTranslate(content=content, proxies=proxies).trans_text_en2cn()
-        elif platform == 'youdao':
-            return YoudaoTranslate(content=content, proxies=proxies).trans_text_en2cn()
+        # elif platform == 'baidu':
+        #     return BaiduTranslate(content=content, proxies=proxies).trans_text_en2cn()
+        # elif platform == 'iciba':
+        #     return BaiduTranslate(content=content, proxies=proxies).trans_text_en2cn()
+        # elif platform == 'youdao':
+        #    return YoudaoTranslate(content=content, proxies=proxies).trans_text_en2cn()
         else:
             return GoogleTranslate(content=content, proxies=proxies).trans_text_en2cn()
     except(Exception,):
         raise Exception(traceback.format_exc())
 
+@retry(stop_max_attempt_number=3)
+def translate_text(content: str, sl='auto', tl='zh-CN'):
+    try:
+        return GoogleTranslate(content=content).trans_text(content, sl, tl)
+    except(Exception,):
+        raise Exception(traceback.format_exc())
+
 
 @retry(stop_max_attempt_number=3)
 def translate_other2cn(content: str, platform='google', proxies: str = None):
     """
     根据翻译平台将其它语言翻译成中文
     :param content: 带翻译的平台
     :param platform: 使用的翻译平台 google,baidu,iciba,youdao
     :param proxies: 代理IP(5.34.178.48:8080)
     :return: 翻译后的内容 string
     """
     try:
         if platform == 'google':
             return GoogleTranslate(content=content, proxies=proxies).trans_text_other2cn()
-        elif platform == 'baidu':
-            return BaiduTranslate(content=content, proxies=proxies).trans_text_other2cn()
-        elif platform == 'iciba':
-            return BaiduTranslate(content=content, proxies=proxies).trans_text_other2cn()
-        elif platform == 'youdao':
-            return YoudaoTranslate(content=content, proxies=proxies).trans_text_other2cn()
+        # elif platform == 'baidu':
+        #     return BaiduTranslate(content=content, proxies=proxies).trans_text_other2cn()
+        # elif platform == 'iciba':
+        #     return BaiduTranslate(content=content, proxies=proxies).trans_text_other2cn()
+        # elif platform == 'youdao':
+        #     return YoudaoTranslate(content=content, proxies=proxies).trans_text_other2cn()
         else:
             return GoogleTranslate(content=content).trans_text_other2cn()
     except(Exception,):
         raise Exception(traceback.format_exc())
 
 
 @retry(stop_max_attempt_number=3)
-def translate_other2en(content: str, platform='google', proxies: str = None, sl:str='auto'):
+def translate_other2en(content: str, platform='google', proxies: str = None, sl: str = 'auto'):
     """
     根据翻译平台将其它语言翻译成英文
     :param content: 带翻译的平台
     :param platform: 使用的翻译平台 google,baidu,iciba,youdao
     :param proxies: 代理IP(5.34.178.48:8080)
     :param sl: 源语言的编码
     :return: 翻译后的内容 string
     """
     try:
         if platform == 'google':
             return GoogleTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
-        elif platform == 'baidu':
-            return BaiduTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
-        elif platform == 'iciba':
-            return BaiduTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
-        elif platform == 'youdao':
-            return YoudaoTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
-        else:
-            return GoogleTranslate(content=content, proxies=proxies).trans_text_other2en()
+        # elif platform == 'baidu':
+        #     return BaiduTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
+        # elif platform == 'iciba':
+        #     return BaiduTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
+        # elif platform == 'youdao':
+        #     return YoudaoTranslate(content=content, proxies=proxies, sl=sl).trans_text_other2en()
+        # else:
+        #     return GoogleTranslate(content=content, proxies=proxies).trans_text_other2en()
     except(Exception,):
         raise Exception(traceback.format_exc())
 
 
 if __name__ == '__main__':
     # _content = 'china'
     # for plat in ['google', 'baidu', 'iciba', 'youdao']:
@@ -90,7 +94,10 @@
 
     _content = '31 maggio 2021'
     for plat in ['google']:
         print(f'{plat}:{translate_other2en(_content, plat, sl="it")}')
 
     tran_rs = translate_other2cn(content='chinese', platform='google', proxies='5.34.178.48:8080')
     print(tran_rs)
+
+    res = translate_text('我是中国人', tl='fr')
+    print(res)
```

### Comparing `translate_util-1.0.9/translate_util/translate_youdao.py` & `translate_util-1.1.0/translate_util/translate_youdao.py`

 * *Files identical despite different names*

### Comparing `translate_util-1.0.9/translate_util.egg-info/PKG-INFO` & `translate_util-1.1.0/translate_util.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-util
-Version: 1.0.9
+Version: 1.1.0
 Summary: translate tool support(google,baidu,iciba,youdao)
 Home-page: https://github.com/abo123456789/translate_util
 Author: cc
 Author-email: abcdef123456chen@sohu.com
 Maintainer: cc
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
@@ -20,34 +20,26 @@
         ```shell
         pip install translate-util
         ```
         
         ### DEMO
         
         ```python
-            from translate_util.translate_tool import translate_other2cn,translate_other2en
+            from translate_util.translate_tool import translate_other2cn,translate_other2en,translate_text
             
             # translate other language to chinese (default use google)
             print(translate_other2cn('china'))
             
             # translate other language to english (default use google)
             print(translate_other2en('中国'))
             
-            # other plat translate demo
-            content = 'china'
-            for plat in ['google', 'baidu', 'youdao']:
-                print(f'{plat}:{translate_other2cn(content, plat)}')
-        
-            content = '中国'
-            for plat in ['google', 'baidu', 'youdao']:
-                print(f'{plat}:{translate_other2en(content, plat)}')
+            # translate other language to de ,support any language
+            print(translate_text('china', tl='de'))
+            
             
-            # if your request is limit by google,please use proxies ip
-            tran_rs = translate_other2cn(content='chinese', platform='google', proxies='5.34.178.48:8080')
-            print(tran_rs)
         ```
         
         ### OTHER SUPPORT
         any customization demand,contact me with email
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

