# Comparing `tmp/shuangchentools-0.0.3.tar.gz` & `tmp/shuangchentools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuangchentools-0.0.3.tar", last modified: Wed Apr 24 06:28:17 2024, max compression
+gzip compressed data, was "shuangchentools-0.0.4.tar", last modified: Sun May  5 13:14:43 2024, max compression
```

## Comparing `shuangchentools-0.0.3.tar` & `shuangchentools-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.936745 shuangchentools-0.0.3/
--rw-rw-rw-   0        0        0      842 2024-04-24 06:28:17.935733 shuangchentools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      573 2024-03-25 02:02:16.000000 shuangchentools-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 06:28:17.936745 shuangchentools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      590 2024-04-24 05:31:40.000000 shuangchentools-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.922572 shuangchentools-0.0.3/shuangchentools/
--rw-rw-rw-   0        0        0       64 2024-03-13 10:53:27.000000 shuangchentools-0.0.3/shuangchentools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.929601 shuangchentools-0.0.3/shuangchentools/doc_segment/
--rw-rw-rw-   0        0        0       51 2024-03-12 12:56:11.000000 shuangchentools-0.0.3/shuangchentools/doc_segment/__init__.py
--rw-rw-rw-   0        0        0     7036 2024-04-19 11:18:34.000000 shuangchentools-0.0.3/shuangchentools/doc_segment/doc_segment_by_rule.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.932119 shuangchentools-0.0.3/shuangchentools/spider/
--rw-rw-rw-   0        0        0       38 2024-03-12 11:09:07.000000 shuangchentools-0.0.3/shuangchentools/spider/__init__.py
--rw-rw-rw-   0        0        0     3119 2024-04-24 06:26:59.000000 shuangchentools-0.0.3/shuangchentools/spider/selenium.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.935733 shuangchentools-0.0.3/shuangchentools/utils/
--rw-rw-rw-   0        0        0       47 2024-03-25 02:48:24.000000 shuangchentools-0.0.3/shuangchentools/utils/__init__.py
--rw-rw-rw-   0        0        0     1569 2024-04-19 11:18:23.000000 shuangchentools-0.0.3/shuangchentools/utils/decorators.py
--rw-rw-rw-   0        0        0     3405 2024-04-19 11:24:59.000000 shuangchentools-0.0.3/shuangchentools/utils/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-24 06:28:17.927496 shuangchentools-0.0.3/shuangchentools.egg-info/
--rw-rw-rw-   0        0        0      842 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 06:28:17.000000 shuangchentools-0.0.3/shuangchentools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.500096 shuangchentools-0.0.4/
+-rw-rw-rw-   0        0        0     1208 2024-05-05 13:14:43.500096 shuangchentools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2024-05-05 13:12:02.000000 shuangchentools-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 13:14:43.501110 shuangchentools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      590 2024-05-05 13:08:59.000000 shuangchentools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.436567 shuangchentools-0.0.4/shuangchentools/
+-rw-rw-rw-   0        0        0       64 2024-03-13 10:53:27.000000 shuangchentools-0.0.4/shuangchentools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.443586 shuangchentools-0.0.4/shuangchentools/doc_segment/
+-rw-rw-rw-   0        0        0       51 2024-03-12 12:56:11.000000 shuangchentools-0.0.4/shuangchentools/doc_segment/__init__.py
+-rw-rw-rw-   0        0        0     7036 2024-04-19 11:18:34.000000 shuangchentools-0.0.4/shuangchentools/doc_segment/doc_segment_by_rule.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.477130 shuangchentools-0.0.4/shuangchentools/spider/
+-rw-rw-rw-   0        0        0       38 2024-03-12 11:09:07.000000 shuangchentools-0.0.4/shuangchentools/spider/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-04-24 06:38:21.000000 shuangchentools-0.0.4/shuangchentools/spider/selenium.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.486094 shuangchentools-0.0.4/shuangchentools/utils/
+-rw-rw-rw-   0        0        0       66 2024-05-05 13:04:52.000000 shuangchentools-0.0.4/shuangchentools/utils/__init__.py
+-rw-rw-rw-   0        0        0     1226 2024-05-05 13:09:56.000000 shuangchentools-0.0.4/shuangchentools/utils/command.py
+-rw-rw-rw-   0        0        0     1569 2024-04-19 11:18:23.000000 shuangchentools-0.0.4/shuangchentools/utils/decorators.py
+-rw-rw-rw-   0        0        0      658 2024-05-05 13:07:49.000000 shuangchentools-0.0.4/shuangchentools/utils/file.py
+-rw-rw-rw-   0        0        0     3405 2024-04-19 11:24:59.000000 shuangchentools-0.0.4/shuangchentools/utils/transform.py
+drwxrwxrwx   0        0        0        0 2024-05-05 13:14:43.440580 shuangchentools-0.0.4/shuangchentools.egg-info/
+-rw-rw-rw-   0        0        0     1208 2024-05-05 13:14:43.000000 shuangchentools-0.0.4/shuangchentools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2024-05-05 13:14:43.000000 shuangchentools-0.0.4/shuangchentools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 13:14:43.000000 shuangchentools-0.0.4/shuangchentools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-05 13:14:43.000000 shuangchentools-0.0.4/shuangchentools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 13:14:43.000000 shuangchentools-0.0.4/shuangchentools.egg-info/top_level.txt
```

### Comparing `shuangchentools-0.0.3/setup.py` & `shuangchentools-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='shuangchentools',
-    version='0.0.3',
+    version='0.0.4',
     author='shuangchen',
     author_email='wangtao.cpu@gmail.com',
     description='encapsulated some commonly used tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/wangtao2001/shuangchentools',
     packages=setuptools.find_packages(),
```

### Comparing `shuangchentools-0.0.3/shuangchentools/doc_segment/doc_segment_by_rule.py` & `shuangchentools-0.0.4/shuangchentools/doc_segment/doc_segment_by_rule.py`

 * *Files identical despite different names*

### Comparing `shuangchentools-0.0.3/shuangchentools/spider/selenium.py` & `shuangchentools-0.0.4/shuangchentools/spider/selenium.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         try:
             r = requests.get(url, headers=self.headers)
         except requests.exceptions.ConnectTimeout:
             raise PageNotFound('网页不存在: ' + url)
         else:
             if r.status_code == 412 or r.status_code == 202:
                 self._get_client_cookies()
-                raise
+                self.get_html(url)
             elif r.status_code == 404 or r.status_code == 500:
                 raise PageNotFound('网页不存在: ' + url)
             r.encoding = 'utf-8'
             return r.text
 
     def get_content(self, url=None) -> bytes:
         """
```

### Comparing `shuangchentools-0.0.3/shuangchentools/utils/decorators.py` & `shuangchentools-0.0.4/shuangchentools/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `shuangchentools-0.0.3/shuangchentools/utils/transform.py` & `shuangchentools-0.0.4/shuangchentools/utils/transform.py`

 * *Files identical despite different names*

