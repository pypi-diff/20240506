# Comparing `tmp/2captcha-python-1.2.4.tar.gz` & `tmp/2captcha_python-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2captcha-python-1.2.4.tar", last modified: Tue Apr  2 10:44:39 2024, max compression
+gzip compressed data, was "2captcha_python-1.2.5.tar", last modified: Mon May  6 09:10:26 2024, max compression
```

## Comparing `2captcha-python-1.2.4.tar` & `2captcha_python-1.2.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/2captcha_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-04-02 10:44:39.000000 2captcha-python-1.2.4/2captcha_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 10:44:39.000000 2captcha-python-1.2.4/2captcha_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:44:39.000000 2captcha-python-1.2.4/2captcha_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 10:44:39.000000 2captcha-python-1.2.4/2captcha_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 10:44:39.000000 2captcha-python-1.2.4/2captcha_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15371 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2634 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_amazon_waf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_atb_captcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1774 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_capy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1630 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_cutcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_friendly_captcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1329 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_funcaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1034 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_geetest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_geetest_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      727 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_hcaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_keycaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      985 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_lemin.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_mtcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_normal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_recaptcha.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_rotate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_text.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      847 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/tests/test_turnstile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:44:39.099055 2captcha-python-1.2.4/twocaptcha/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/twocaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/twocaptcha/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20111 2024-04-02 10:44:33.000000 2captcha-python-1.2.4/twocaptcha/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:10:26.809093 2captcha_python-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:10:26.809093 2captcha_python-1.2.5/2captcha_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-05-06 09:10:26.000000 2captcha_python-1.2.5/2captcha_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 09:10:26.000000 2captcha_python-1.2.5/2captcha_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:10:26.000000 2captcha_python-1.2.5/2captcha_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 09:10:26.000000 2captcha_python-1.2.5/2captcha_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 09:10:26.000000 2captcha_python-1.2.5/2captcha_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-05-06 09:10:26.809093 2captcha_python-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:10:26.809093 2captcha_python-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:10:26.805093 2captcha_python-1.2.5/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2634 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_amazon_waf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_atb_captcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1774 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_capy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1630 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_cutcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_friendly_captcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1329 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_funcaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1034 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_geetest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_geetest_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      727 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_hcaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1254 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_keycaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      985 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_lemin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_mtcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_normal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1882 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_recaptcha.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2164 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_tencent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      835 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      847 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/tests/test_turnstile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:10:26.805093 2captcha_python-1.2.5/twocaptcha/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/twocaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/twocaptcha/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40399 2024-05-06 09:10:19.000000 2captcha_python-1.2.5/twocaptcha/solver.py
```

### Comparing `2captcha-python-1.2.4/2captcha_python.egg-info/PKG-INFO` & `2captcha_python-1.2.5/2captcha_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2captcha-python
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python module for easy integration with 2Captcha API
 Home-page: https://github.com/2captcha/2captcha-python/
 Author: 2Captcha
 Author-email: info@2captcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
     - [MTCaptcha](#mtcaptcha)
     - [Friendly Captcha](#friendly-captcha)
     - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
-    - [send / getResult](#send--getresult)
+    - [send / get_result](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
 
 ## Installation
@@ -91,15 +91,15 @@
 | softId           | -              | your software ID obtained after publishing in [2captcha sofware catalog]                                                                           |
 | callback         | -              | URL of your web-sever that receives the captcha recognition result. The URl should be first registered in [pingback settings] of your account      |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except reCAPTCHA. Defines how long the module tries to get the answer from `res.php` API endpoint |
 | recaptchaTimeout | 600            | Polling timeout for reCAPTCHA in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
 >  **IMPORTANT:** once `callback` is defined for `TwoCaptcha` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
-To get the answer manually use [getResult method](#send--getresult)
+To get the answer manually use [get_result method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help 2captcha workers to solve it properly.
 
 ### Captcha options
 | Option        | Default Value | Description                                                                                        |
 | ------------- | ------------- | -------------------------------------------------------------------------------------------------- |
@@ -173,28 +173,29 @@
                         challenge='12345678abc90123d45678ef90123a456b',
                         url='https://www.site.com/page/',
                         param1=..., ...)
 
 ```
 
 
-### hCaptcha
-Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
+### GeeTest v4
+Use this method to solve GeeTest v4. Returns the response in JSON.
 ```python
-result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
-                            url='https://www.site.com/page/', 
+result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
+                            url='https://www.site.com/page/',  
                             param1=..., ...)
 
 ```
 
-### GeeTest v4
-Use this method to solve GeeTest v4. Returns the response in JSON.
+
+### hCaptcha
+Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
 ```python
-result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
-                            url='https://www.site.com/page/',  
+result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
+                            url='https://www.site.com/page/', 
                             param1=..., ...)
 
 ```
 
 
 ### Lemin Cropped Captcha
 Use this method to solve hCaptcha challenge. Returns JSON with an answer containing the following values: answer, challenge_id.
@@ -310,15 +311,15 @@
                            url='https://mysite.com/page/with/cutcaptcha',
                            param1=..., ...)
 ```
 
 
 ## Other methods
 
-### send / getResult
+### send / get_result
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . . 
 
 
 id = solver.send(file='path/to/captcha.jpg')
@@ -358,15 +359,19 @@
     # captcha is not solved so far
 	print(e)
 ```
 
 
 ### Proxies
 
-You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha and geetest. The proxy will be forwarded to the API to solve the captcha.
+You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha, geetest, geetest v4, hcaptcha, 
+keycaptcha, capy pazzle, grid, rotate, lemin, atbcaptcha, turnstile, amazon waf, mtcaptcha, friendly captcha, cutcaptcha. 
+The proxy will be forwarded to the API to solve the captcha.
+
+We have our own proxies that we can offer you. [Buy residential proxies] for avoid restrictions and blocks. [Quick start].
 
 ```python
 proxy={
     'type': 'HTTPS',
     'uri': 'login:password@IP_address:PORT'
 }
 ```
@@ -388,11 +393,13 @@
         return result
 ```
 
 
 [2Captcha]: https://2captcha.com/
 [2captcha sofware catalog]: https://2captcha.com/software
 [pingback settings]: https://2captcha.com/setting/pingback
-[post options]: https://2captcha.com/2captcha-api#normal_post
+[post options]: https://2captcha.com/2captcha-api#solving_normal_captcha
 [list of supported languages]: https://2captcha.com/2captcha-api#language
 [examples directory]: /examples
 [asyncio]: https://docs.python.org/3/library/asyncio.html
+[Buy residential proxies]: https://2captcha.com/proxy/residential-proxies
+[Quick start]: https://2captcha.com/proxy?openAddTrafficModal=true
```

### Comparing `2captcha-python-1.2.4/2captcha_python.egg-info/SOURCES.txt` & `2captcha_python-1.2.5/2captcha_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 tests/test_hcaptcha.py
 tests/test_keycaptcha.py
 tests/test_lemin.py
 tests/test_mtcaptcha.py
 tests/test_normal.py
 tests/test_recaptcha.py
 tests/test_rotate.py
+tests/test_tencent.py
 tests/test_text.py
 tests/test_turnstile.py
 twocaptcha/__init__.py
 twocaptcha/api.py
 twocaptcha/solver.py
```

### Comparing `2captcha-python-1.2.4/LICENSE` & `2captcha_python-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/PKG-INFO` & `2captcha_python-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2captcha-python
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python module for easy integration with 2Captcha API
 Home-page: https://github.com/2captcha/2captcha-python/
 Author: 2Captcha
 Author-email: info@2captcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
     - [MTCaptcha](#mtcaptcha)
     - [Friendly Captcha](#friendly-captcha)
     - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
-    - [send / getResult](#send--getresult)
+    - [send / get_result](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
 
 ## Installation
@@ -91,15 +91,15 @@
 | softId           | -              | your software ID obtained after publishing in [2captcha sofware catalog]                                                                           |
 | callback         | -              | URL of your web-sever that receives the captcha recognition result. The URl should be first registered in [pingback settings] of your account      |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except reCAPTCHA. Defines how long the module tries to get the answer from `res.php` API endpoint |
 | recaptchaTimeout | 600            | Polling timeout for reCAPTCHA in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
 >  **IMPORTANT:** once `callback` is defined for `TwoCaptcha` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
-To get the answer manually use [getResult method](#send--getresult)
+To get the answer manually use [get_result method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help 2captcha workers to solve it properly.
 
 ### Captcha options
 | Option        | Default Value | Description                                                                                        |
 | ------------- | ------------- | -------------------------------------------------------------------------------------------------- |
@@ -173,28 +173,29 @@
                         challenge='12345678abc90123d45678ef90123a456b',
                         url='https://www.site.com/page/',
                         param1=..., ...)
 
 ```
 
 
-### hCaptcha
-Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
+### GeeTest v4
+Use this method to solve GeeTest v4. Returns the response in JSON.
 ```python
-result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
-                            url='https://www.site.com/page/', 
+result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
+                            url='https://www.site.com/page/',  
                             param1=..., ...)
 
 ```
 
-### GeeTest v4
-Use this method to solve GeeTest v4. Returns the response in JSON.
+
+### hCaptcha
+Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
 ```python
-result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
-                            url='https://www.site.com/page/',  
+result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
+                            url='https://www.site.com/page/', 
                             param1=..., ...)
 
 ```
 
 
 ### Lemin Cropped Captcha
 Use this method to solve hCaptcha challenge. Returns JSON with an answer containing the following values: answer, challenge_id.
@@ -310,15 +311,15 @@
                            url='https://mysite.com/page/with/cutcaptcha',
                            param1=..., ...)
 ```
 
 
 ## Other methods
 
-### send / getResult
+### send / get_result
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . . 
 
 
 id = solver.send(file='path/to/captcha.jpg')
@@ -358,15 +359,19 @@
     # captcha is not solved so far
 	print(e)
 ```
 
 
 ### Proxies
 
-You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha and geetest. The proxy will be forwarded to the API to solve the captcha.
+You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha, geetest, geetest v4, hcaptcha, 
+keycaptcha, capy pazzle, grid, rotate, lemin, atbcaptcha, turnstile, amazon waf, mtcaptcha, friendly captcha, cutcaptcha. 
+The proxy will be forwarded to the API to solve the captcha.
+
+We have our own proxies that we can offer you. [Buy residential proxies] for avoid restrictions and blocks. [Quick start].
 
 ```python
 proxy={
     'type': 'HTTPS',
     'uri': 'login:password@IP_address:PORT'
 }
 ```
@@ -388,11 +393,13 @@
         return result
 ```
 
 
 [2Captcha]: https://2captcha.com/
 [2captcha sofware catalog]: https://2captcha.com/software
 [pingback settings]: https://2captcha.com/setting/pingback
-[post options]: https://2captcha.com/2captcha-api#normal_post
+[post options]: https://2captcha.com/2captcha-api#solving_normal_captcha
 [list of supported languages]: https://2captcha.com/2captcha-api#language
 [examples directory]: /examples
 [asyncio]: https://docs.python.org/3/library/asyncio.html
+[Buy residential proxies]: https://2captcha.com/proxy/residential-proxies
+[Quick start]: https://2captcha.com/proxy?openAddTrafficModal=true
```

### Comparing `2captcha-python-1.2.4/README.md` & `2captcha_python-1.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     - [Canvas](#canvas)
     - [ClickCaptcha](#clickcaptcha)
     - [Rotate](#rotate)
     - [MTCaptcha](#mtcaptcha)
     - [Friendly Captcha](#friendly-captcha)
     - [Cutcaptcha](#cutcaptcha)
   - [Other methods](#other-methods)
-    - [send / getResult](#send--getresult)
+    - [send / get_result](#send--getresult)
     - [balance](#balance)
     - [report](#report)
     - [Error handling](#error-handling)
     - [Proxies](#proxies)
     - [Async calls](#async-calls)
 
 ## Installation
@@ -76,15 +76,15 @@
 | softId           | -              | your software ID obtained after publishing in [2captcha sofware catalog]                                                                           |
 | callback         | -              | URL of your web-sever that receives the captcha recognition result. The URl should be first registered in [pingback settings] of your account      |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except reCAPTCHA. Defines how long the module tries to get the answer from `res.php` API endpoint |
 | recaptchaTimeout | 600            | Polling timeout for reCAPTCHA in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
 >  **IMPORTANT:** once `callback` is defined for `TwoCaptcha` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
-To get the answer manually use [getResult method](#send--getresult)
+To get the answer manually use [get_result method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help 2captcha workers to solve it properly.
 
 ### Captcha options
 | Option        | Default Value | Description                                                                                        |
 | ------------- | ------------- | -------------------------------------------------------------------------------------------------- |
@@ -158,28 +158,29 @@
                         challenge='12345678abc90123d45678ef90123a456b',
                         url='https://www.site.com/page/',
                         param1=..., ...)
 
 ```
 
 
-### hCaptcha
-Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
+### GeeTest v4
+Use this method to solve GeeTest v4. Returns the response in JSON.
 ```python
-result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
-                            url='https://www.site.com/page/', 
+result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
+                            url='https://www.site.com/page/',  
                             param1=..., ...)
 
 ```
 
-### GeeTest v4
-Use this method to solve GeeTest v4. Returns the response in JSON.
+
+### hCaptcha
+Use this method to solve the hCaptcha challenge. Returns a token to bypass the captcha.
 ```python
-result = solver.geetest_v4(captcha_id='e392e1d7fd421dc63325744d5a2b9c73',
-                            url='https://www.site.com/page/',  
+result = solver.hcaptcha(sitekey='10000000-ffff-ffff-ffff-000000000001',
+                            url='https://www.site.com/page/', 
                             param1=..., ...)
 
 ```
 
 
 ### Lemin Cropped Captcha
 Use this method to solve hCaptcha challenge. Returns JSON with an answer containing the following values: answer, challenge_id.
@@ -295,15 +296,15 @@
                            url='https://mysite.com/page/with/cutcaptcha',
                            param1=..., ...)
 ```
 
 
 ## Other methods
 
-### send / getResult
+### send / get_result
 These methods can be used for manual captcha submission and answer polling.
 ```python
 import time
 . . . . . 
 
 
 id = solver.send(file='path/to/captcha.jpg')
@@ -343,15 +344,19 @@
     # captcha is not solved so far
 	print(e)
 ```
 
 
 ### Proxies
 
-You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha and geetest. The proxy will be forwarded to the API to solve the captcha.
+You can pass your proxy as an additional argument for methods: recaptcha, funcaptcha, geetest, geetest v4, hcaptcha, 
+keycaptcha, capy pazzle, grid, rotate, lemin, atbcaptcha, turnstile, amazon waf, mtcaptcha, friendly captcha, cutcaptcha. 
+The proxy will be forwarded to the API to solve the captcha.
+
+We have our own proxies that we can offer you. [Buy residential proxies] for avoid restrictions and blocks. [Quick start].
 
 ```python
 proxy={
     'type': 'HTTPS',
     'uri': 'login:password@IP_address:PORT'
 }
 ```
@@ -373,11 +378,13 @@
         return result
 ```
 
 
 [2Captcha]: https://2captcha.com/
 [2captcha sofware catalog]: https://2captcha.com/software
 [pingback settings]: https://2captcha.com/setting/pingback
-[post options]: https://2captcha.com/2captcha-api#normal_post
+[post options]: https://2captcha.com/2captcha-api#solving_normal_captcha
 [list of supported languages]: https://2captcha.com/2captcha-api#language
 [examples directory]: /examples
 [asyncio]: https://docs.python.org/3/library/asyncio.html
+[Buy residential proxies]: https://2captcha.com/proxy/residential-proxies
+[Quick start]: https://2captcha.com/proxy?openAddTrafficModal=true
```

### Comparing `2captcha-python-1.2.4/setup.py` & `2captcha_python-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_amazon_waf.py` & `2captcha_python-1.2.5/tests/test_amazon_waf.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_atb_captcha.py` & `2captcha_python-1.2.5/tests/test_atb_captcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_canvas.py` & `2captcha_python-1.2.5/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_capy.py` & `2captcha_python-1.2.5/tests/test_capy.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_coordinates.py` & `2captcha_python-1.2.5/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_cutcaptcha.py` & `2captcha_python-1.2.5/tests/test_cutcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_friendly_captcha.py` & `2captcha_python-1.2.5/tests/test_friendly_captcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_funcaptcha.py` & `2captcha_python-1.2.5/tests/test_funcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_geetest.py` & `2captcha_python-1.2.5/tests/test_geetest.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_geetest_v4.py` & `2captcha_python-1.2.5/tests/test_geetest_v4.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_grid.py` & `2captcha_python-1.2.5/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_hcaptcha.py` & `2captcha_python-1.2.5/tests/test_hcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_keycaptcha.py` & `2captcha_python-1.2.5/tests/test_keycaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_lemin.py` & `2captcha_python-1.2.5/tests/test_lemin.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_mtcaptcha.py` & `2captcha_python-1.2.5/tests/test_mtcaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_normal.py` & `2captcha_python-1.2.5/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_recaptcha.py` & `2captcha_python-1.2.5/tests/test_recaptcha.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_rotate.py` & `2captcha_python-1.2.5/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_text.py` & `2captcha_python-1.2.5/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/tests/test_turnstile.py` & `2captcha_python-1.2.5/tests/test_turnstile.py`

 * *Files identical despite different names*

### Comparing `2captcha-python-1.2.4/twocaptcha/api.py` & `2captcha_python-1.2.5/twocaptcha/api.py`

 * *Files identical despite different names*

