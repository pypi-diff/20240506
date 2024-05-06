# Comparing `tmp/web-ui-helper-0.0.7.tar.gz` & `tmp/web-ui-helper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.0.7.tar", last modified: Sun May  5 18:44:17 2024, max compression
+gzip compressed data, was "web-ui-helper-0.0.8.tar", last modified: Sun May  5 18:55:14 2024, max compression
```

## Comparing `web-ui-helper-0.0.7.tar` & `web-ui-helper-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.913647 web-ui-helper-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-05 18:44:17.911652 web-ui-helper-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 18:44:17.913647 web-ui-helper-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-05 18:44:14.000000 web-ui-helper-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.868801 web-ui-helper-0.0.7/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.7/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.888715 web-ui-helper-0.0.7/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.7/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.894697 web-ui-helper-0.0.7/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.7/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.895695 web-ui-helper-0.0.7/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.898711 web-ui-helper-0.0.7/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    27313 2024-05-05 18:44:03.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.902678 web-ui-helper-0.0.7/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     5206 2024-05-05 18:18:39.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.905694 web-ui-helper-0.0.7/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.7/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.908686 web-ui-helper-0.0.7/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.7/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:44:17.910656 web-ui-helper-0.0.7/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-05 18:44:17.000000 web-ui-helper-0.0.7/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-05 18:44:17.000000 web-ui-helper-0.0.7/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:44:17.000000 web-ui-helper-0.0.7/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-05 18:44:17.000000 web-ui-helper-0.0.7/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 18:44:17.000000 web-ui-helper-0.0.7/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.273050 web-ui-helper-0.0.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-05 18:55:14.271060 web-ui-helper-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:55:14.273050 web-ui-helper-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-05 18:55:06.000000 web-ui-helper-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.216210 web-ui-helper-0.0.8/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.8/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.242136 web-ui-helper-0.0.8/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.8/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.247122 web-ui-helper-0.0.8/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.8/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.250093 web-ui-helper-0.0.8/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.254107 web-ui-helper-0.0.8/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    27737 2024-05-05 18:55:00.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.258094 web-ui-helper-0.0.8/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     5206 2024-05-05 18:18:39.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.263085 web-ui-helper-0.0.8/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.8/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.267069 web-ui-helper-0.0.8/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.8/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:55:14.270039 web-ui-helper-0.0.8/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-05 18:55:14.000000 web-ui-helper-0.0.8/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-05 18:55:14.000000 web-ui-helper-0.0.8/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:55:14.000000 web-ui-helper-0.0.8/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-05 18:55:14.000000 web-ui-helper-0.0.8/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 18:55:14.000000 web-ui-helper-0.0.8/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.0.7/LICENSE` & `web-ui-helper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/PKG-INFO` & `web-ui-helper-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.7/setup.py` & `web-ui-helper-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.0.7',
+    version='0.0.8',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.0.8/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/dir.py` & `web-ui-helper-0.0.8/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/log.py` & `web-ui-helper-0.0.8/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.0.8/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/platforms.py` & `web-ui-helper-0.0.8/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.0.8/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.0.8/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.0.8/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.0.8/web_ui_helper/selenium/frame/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,14 +562,27 @@
         # 使用 JavaScript 获取网络请求的 Cookie 头部信息
         cookies = self.browser.execute_script("return document.cookie")
         return cookies or ''
 
     def get_cookies(self) -> list:
         return self.browser.get_cookies() or list()
 
+    def get_cookie(self, name: str) -> dict:
+        """
+        {'domain': '.ctrip.com',
+         'expiry': 1717525670,
+         'httpOnly': True,
+         'name': 'cticket',
+         'path': '/',
+         'sameSite': 'None',
+         'secure': True,
+         'value': '275F2106E6E6CAAA34E1A32FE2452F42450E99443E2B22A31360D38C0BB2DEB3'}
+        """
+        return self.browser.get_cookie(name=name) or dict()
+
     def refresh(self) -> None:
         # 刷新当前页面
         self.browser.refresh()
 
 
 @element_find_exception
 def scroll_to_bottom(driver: webdriver) -> None:
```

### Comparing `web-ui-helper-0.0.7/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.0.8/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.0.8/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper/terminal/device.py` & `web-ui-helper-0.0.8/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.7/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.0.8/web_ui_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.7/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.0.8/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

