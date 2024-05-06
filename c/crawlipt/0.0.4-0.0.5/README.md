# Comparing `tmp/crawlipt-0.0.4.tar.gz` & `tmp/crawlipt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.4.tar", last modified: Sun May  5 08:52:18 2024, max compression
+gzip compressed data, was "crawlipt-0.0.5.tar", last modified: Mon May  6 12:27:43 2024, max compression
```

## Comparing `crawlipt-0.0.4.tar` & `crawlipt-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 08:52:14.000000 crawlipt-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-05 08:52:14.000000 crawlipt-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 08:52:18.430924 crawlipt-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-05 08:52:14.000000 crawlipt-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.426924 crawlipt-0.0.4/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:52:18.430924 crawlipt-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-05 08:52:14.000000 crawlipt-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:43.546126 crawlipt-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-06 12:27:39.000000 crawlipt-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 12:27:39.000000 crawlipt-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-06 12:27:43.546126 crawlipt-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-06 12:27:39.000000 crawlipt-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:43.542126 crawlipt-0.0.5/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:43.542126 crawlipt-0.0.5/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:43.546126 crawlipt-0.0.5/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-05-06 12:27:39.000000 crawlipt-0.0.5/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:43.546126 crawlipt-0.0.5/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-06 12:27:43.000000 crawlipt-0.0.5/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-06 12:27:43.000000 crawlipt-0.0.5/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:27:43.000000 crawlipt-0.0.5/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 12:27:43.000000 crawlipt-0.0.5/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 12:27:43.000000 crawlipt-0.0.5/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:27:43.546126 crawlipt-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-06 12:27:39.000000 crawlipt-0.0.5/setup.py
```

### Comparing `crawlipt-0.0.4/LICENSE` & `crawlipt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/PKG-INFO` & `crawlipt-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.4
+Version: 0.0.5
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -45,17 +45,22 @@
 
 
 ## introduction
 
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlipt
+
 `pip install crawlipt` or `pip3 install crawlipt`
 
+If you have already installed crawlelip, you may need to update to the latest version
+
+`pip install --upgrade crawlipt`
+
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
 from selenium.webdriver.chrome.service import Service
 import crawlipt as cpt
 option = wd.ChromeOptions()
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.4 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.5 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
-physical storage. ## installing You can use pip or pip3 to install the
-crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
-```python from webdriver_manager.chrome import ChromeDriverManager from
-selenium import webdriver as wd from selenium.webdriver.chrome.service import
-Service import crawlipt as cpt option = wd.ChromeOptions() option.add_argument
-("start-maximized") option.add_argument("window-size=1920x3000") agent = 'user-
-agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36
-(KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"' option.add_argument
-(agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
-options=option) # Define scripts # You can also deserialize JSON strings into a
-dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
-"next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
-"åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
-Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
-you are interested and would like to see more detailed documentation, please
-click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
-"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
-Document") ## Contributing Please submit pull requests to the develop branch
+physical storage. ## installing You can use pip or pip3 to install the crawlipt
+`pip install crawlipt` or `pip3 install crawlipt` If you have already installed
+crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt` ## quickly start ```python from webdriver_manager.chrome import
+ChromeDriverManager from selenium import webdriver as wd from
+selenium.webdriver.chrome.service import Service import crawlipt as cpt option
+= wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
+("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
+Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
+Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
+(service=Service(ChromeDriverManager().install()), options=option) # Define
+scripts # You can also deserialize JSON strings into a dictionary script =
+{ "method": "redirect", "url": "https://www.baidu.com/", "next": { "method":
+"input", "xpath": "//*[@id=\"kw\"]", "keyword": "åæ³é¾çº±", "next":
+{ "method": "click", "xpath": "//*[@id=\"su\"]" } } } # Execute script
+cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If you are
+interested and would like to see more detailed documentation, please click on
+the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh "ä¸­æææ¡£")|
+[English](https://wwydev.gitbook.io/crawlipt "English Document") ##
+Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.4/README.md` & `crawlipt-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,22 @@
 
 
 ## introduction
 
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlipt
+
 `pip install crawlipt` or `pip3 install crawlipt`
 
+If you have already installed crawlelip, you may need to update to the latest version
+
+`pip install --upgrade crawlipt`
+
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
 from selenium.webdriver.chrome.service import Service
 import crawlipt as cpt
 option = wd.ChromeOptions()
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
-physical storage. ## installing You can use pip or pip3 to install the
-crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
-```python from webdriver_manager.chrome import ChromeDriverManager from
-selenium import webdriver as wd from selenium.webdriver.chrome.service import
-Service import crawlipt as cpt option = wd.ChromeOptions() option.add_argument
-("start-maximized") option.add_argument("window-size=1920x3000") agent = 'user-
-agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36
-(KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"' option.add_argument
-(agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
-options=option) # Define scripts # You can also deserialize JSON strings into a
-dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
-"next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
-"åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
-Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
-you are interested and would like to see more detailed documentation, please
-click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
-"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
-Document") ## Contributing Please submit pull requests to the develop branch
+physical storage. ## installing You can use pip or pip3 to install the crawlipt
+`pip install crawlipt` or `pip3 install crawlipt` If you have already installed
+crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt` ## quickly start ```python from webdriver_manager.chrome import
+ChromeDriverManager from selenium import webdriver as wd from
+selenium.webdriver.chrome.service import Service import crawlipt as cpt option
+= wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
+("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
+Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
+Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
+(service=Service(ChromeDriverManager().install()), options=option) # Define
+scripts # You can also deserialize JSON strings into a dictionary script =
+{ "method": "redirect", "url": "https://www.baidu.com/", "next": { "method":
+"input", "xpath": "//*[@id=\"kw\"]", "keyword": "åæ³é¾çº±", "next":
+{ "method": "click", "xpath": "//*[@id=\"su\"]" } } } # Execute script
+cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If you are
+interested and would like to see more detailed documentation, please click on
+the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh "ä¸­æææ¡£")|
+[English](https://wwydev.gitbook.io/crawlipt "English Document") ##
+Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.4/crawlipt/actions/click.py` & `crawlipt-0.0.5/crawlipt/actions/click.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/get.py` & `crawlipt-0.0.5/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/input.py` & `crawlipt-0.0.5/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/redirect.py` & `crawlipt-0.0.5/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/select.py` & `crawlipt-0.0.5/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/slide.py` & `crawlipt-0.0.5/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/actions/switch.py` & `crawlipt-0.0.5/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/annotation.py` & `crawlipt-0.0.5/crawlipt/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
                     raise ParamTypeError(f"Parameter {name} must be indicated the type.")
                 if name not in all_kwargs:
                     raise ParamTypeError(f"Parameter {name} is not in the defined parameter list.")
                 if all_kwargs[name] is None and type_.default is not type_.empty:
                     continue
                 if all_kwargs[name] == "__PRE_RETURN__":
                     continue
+                if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__v-") and all_kwargs[name].endswith("__"):
+                    continue
                 if isinstance(all_kwargs[name], int) and type_.annotation is float:
                     all_kwargs[name] = float(all_kwargs.get(name))
                 if not isinstance(all_kwargs[name], type_.annotation):
                     raise ParamTypeError(f"Parameter {name} must be {type_.annotation}.")
             return func(*args, **kwargs)
 
         return inner_wrapper
```

### Comparing `crawlipt-0.0.4/crawlipt/conditions/element.py` & `crawlipt-0.0.5/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/conditions/frame.py` & `crawlipt-0.0.5/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/conditions/presence.py` & `crawlipt-0.0.5/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/conditions/text.py` & `crawlipt-0.0.5/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/conditions/visibility.py` & `crawlipt-0.0.5/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.4/crawlipt/script.py` & `crawlipt-0.0.5/crawlipt/script.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from crawlipt.action import Action
 from crawlipt.condition import Condition
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.wait import WebDriverWait
 import copy
 
+from crawlipt.pojo import VariableError, VariableBase
+
 
 class ScriptError(Exception):
     def __init__(self, e: Exception, method: str, deep: str):
         self.e = e
         self.method = method
         self.deep = deep
 
@@ -30,15 +32,14 @@
         elif self.method and self.method in ScriptProcess.CONDITIONS.keys():
             params = "\ndef " + self.method + " " + signature(Script.CONDITIONS[self.method]).__str__()
             doc = ScriptProcess.CONDITIONS[self.method].__doc__
             info = "----------------------condition info--------------------------"
         error = "[" + self.e.__class__.__name__ + "] " + self.e.__str__() + "\n"
         return "(Deep:%s method:%s) arguments is wrong\n" % (self.deep, self.method) + error + info + params + doc
 
-
 def dfs_search(obj):
     for parent in obj.__bases__:
         if parent == object:
             continue
         dfs_search(parent)
         yield parent.__dict__
 
@@ -57,15 +58,15 @@
     all_dict.update(alias_dict)
     return all_dict
 
 
 class ScriptProcess:
     ACTIONS = get_dict(Action)
     CONDITIONS = get_dict(Condition)
-    __POP_KEY = {"method", "next", "if", "check", "condition"}
+    __POP_KEY = {"method", "next", "if", "check", "condition", "loop"}
 
     @staticmethod
     @check
     def __condition_check(temp_condition: dict, name: str, pre_deep: str, current_deep: int) -> None:
         condition = temp_condition.get("condition")
         temp_args = {"driver": None}
         if not condition:
@@ -109,14 +110,17 @@
                     raise ScriptError(ParamTypeError(msg), "", pre_deep + str(current_deep))
                 if while_condition:
                     ScriptProcess.__condition_check(temp_condition=while_condition,
                                                     name="while",
                                                     pre_deep=pre_deep,
                                                     current_deep=current_deep)
                 loop_script = loop_temp.get("script")
+                if not loop_script:
+                    msg = "(Deep %s) loop must set the param of script" % (pre_deep + str(current_deep))
+                    raise ScriptError(ParamTypeError(msg), "", pre_deep + str(current_deep))
                 ScriptProcess.syntax_check(loop_script, pre_deep=pre_deep + str(current_deep) + "->")
                 script = script.get("next")
                 continue
             check_condition = script.get("check")
             if check_condition:
                 ScriptProcess.__condition_check(temp_condition=check_condition,
                                                 name="check",
@@ -181,15 +185,16 @@
         while script:
             loop_temp: dict = script.get("loop")
             if loop_temp:
                 cnt = loop_temp.get("cnt")
                 while_condition = loop_temp.get("while")
                 loop_script = loop_temp.get("script")
                 if while_condition and cnt:
-                    while ScriptProcess.__process_condition(temp_condition=while_condition, webdriver=webdriver) and cnt:
+                    while ScriptProcess.__process_condition(temp_condition=while_condition,
+                                                            webdriver=webdriver) and cnt:
                         ScriptProcess._process_script(script=loop_script,
                                                       global_script=global_script,
                                                       webdriver=webdriver,
                                                       interval=interval,
                                                       wait=wait)
                         cnt -= 1
                     script = script.get("next")
@@ -248,14 +253,30 @@
                 pre_return = current_return
             script = script.get("next")
             time.sleep(random.uniform(interval / 2, interval))
         return pre_return
 
     @staticmethod
     @check
+    def _replace_variable(script: dict, variable: VariableBase) -> None:
+        while script:
+            for key in script.keys():
+                if key not in ScriptProcess.__POP_KEY and isinstance(script[key], str) and script[key].startswith("__v-") and script[key].endswith("__"):
+                    variable_name = script[key][4:-2]
+                    if variable_name not in variable:
+                        msg = f"The {variable_name} is not defined."
+                        raise VariableError(msg)
+                    script[key] = variable.get(variable_name)
+            for key in script.keys():
+                if isinstance(script[key], dict):
+                    ScriptProcess._replace_variable(script=script[key], variable=variable)
+            script = script.get("next")
+
+    @staticmethod
+    @check
     def generate(scripts: list | dict | str) -> dict:
         """
         generate the scripts(dict) from list
         """
         if isinstance(scripts, dict):
             return scripts
         if isinstance(scripts, str):
@@ -319,23 +340,25 @@
             func = func.__func__
         except Exception:
             pass
         if "__crawlipt_func_name__" in func.__dict__:
             ScriptProcess.CONDITIONS[func.__crawlipt_func_name__] = func_bak
 
 
+
+
 class Script(ScriptProcess):
 
     @check
     def __init__(self, script: dict | str | list, global_script: dict | str | list = None, interval: float = 0.5,
                  wait: float = 10, is_need_syntax_check: bool = True):
         """
         Script Parser
         :param script: Need a str of json or dict or list steps that conforms to syntax conventions
-        :param b: This script will be executed before every actions
+        :param global_script: This script will be executed before every actions
         :param interval: The direct interval between two consecutive scripts
         :param wait: The longest wait time before presence of element located
         :param is_need_syntax_check: Whether the script need a syntax check
         """
         self.script = ScriptProcess.generate(script)
         if global_script is None:
             self.global_script = {}
@@ -347,22 +370,30 @@
             ScriptProcess.syntax_check(self.global_script)
         assert interval >= 0
         assert wait >= 0
         self.interval = interval
         self.wait = wait
 
     @check
-    def process(self, webdriver: WebDriver) -> Any:
+    def process(self, webdriver: WebDriver, variable: VariableBase = None) -> Any:
         """
         process the script
         """
         if self.is_need_syntax_check:
             ScriptProcess.syntax_check(self.script)
             ScriptProcess.syntax_check(self.global_script)
-        return ScriptProcess._process_script(script=self.script,
-                                             global_script=self.global_script,
+        script = copy.deepcopy(self.script)
+        global_script = copy.deepcopy(self.global_script)
+        if variable:
+            ScriptProcess._replace_variable(script, variable)
+            ScriptProcess._replace_variable(global_script, variable)
+            if self.is_need_syntax_check:
+                ScriptProcess.syntax_check(script)
+                ScriptProcess.syntax_check(global_script)
+        return ScriptProcess._process_script(script=script,
+                                             global_script=global_script,
                                              webdriver=webdriver,
                                              interval=self.interval,
                                              wait=self.wait)
 
     def __call__(self, webdriver: WebDriver):
         return self.process(webdriver)
```

### Comparing `crawlipt-0.0.4/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.5/crawlipt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.4
+Version: 0.0.5
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -45,17 +45,22 @@
 
 
 ## introduction
 
 You can use Crawlipt to driver the selenium by script in python.The script adopts JSON format for better cross language operations and physical storage.
 
 ## installing
-You can use pip or pip3 to install the crawlist\
+You can use pip or pip3 to install the crawlipt
+
 `pip install crawlipt` or `pip3 install crawlipt`
 
+If you have already installed crawlelip, you may need to update to the latest version
+
+`pip install --upgrade crawlipt`
+
 ## quickly start
 ```python
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium import webdriver as wd
 from selenium.webdriver.chrome.service import Service
 import crawlipt as cpt
 option = wd.ChromeOptions()
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.4 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.5 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: selenium>=4.0.0
                                   _[_c_r_a_w_l_i_s_t_]
                  # crawlipt The script for selenium in python
                          _[_p_y_p_i_][python]_[_G_i_t_H_u_b_ _s_t_a_r_s_]
 ## introduction You can use Crawlipt to driver the selenium by script in
 python.The script adopts JSON format for better cross language operations and
-physical storage. ## installing You can use pip or pip3 to install the
-crawlist\ `pip install crawlipt` or `pip3 install crawlipt` ## quickly start
-```python from webdriver_manager.chrome import ChromeDriverManager from
-selenium import webdriver as wd from selenium.webdriver.chrome.service import
-Service import crawlipt as cpt option = wd.ChromeOptions() option.add_argument
-("start-maximized") option.add_argument("window-size=1920x3000") agent = 'user-
-agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36
-(KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"' option.add_argument
-(agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
-options=option) # Define scripts # You can also deserialize JSON strings into a
-dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
-"next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
-"åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
-Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
-you are interested and would like to see more detailed documentation, please
-click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
-"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
-Document") ## Contributing Please submit pull requests to the develop branch
+physical storage. ## installing You can use pip or pip3 to install the crawlipt
+`pip install crawlipt` or `pip3 install crawlipt` If you have already installed
+crawlelip, you may need to update to the latest version `pip install --upgrade
+crawlipt` ## quickly start ```python from webdriver_manager.chrome import
+ChromeDriverManager from selenium import webdriver as wd from
+selenium.webdriver.chrome.service import Service import crawlipt as cpt option
+= wd.ChromeOptions() option.add_argument("start-maximized") option.add_argument
+("window-size=1920x3000") agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel
+Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77
+Safari/537.36"' option.add_argument(agent) webdriver = wd.Chrome
+(service=Service(ChromeDriverManager().install()), options=option) # Define
+scripts # You can also deserialize JSON strings into a dictionary script =
+{ "method": "redirect", "url": "https://www.baidu.com/", "next": { "method":
+"input", "xpath": "//*[@id=\"kw\"]", "keyword": "åæ³é¾çº±", "next":
+{ "method": "click", "xpath": "//*[@id=\"su\"]" } } } # Execute script
+cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If you are
+interested and would like to see more detailed documentation, please click on
+the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh "ä¸­æææ¡£")|
+[English](https://wwydev.gitbook.io/crawlipt "English Document") ##
+Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.4/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.0.5/crawlipt.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 README.md
 setup.py
 crawlipt/__init__.py
 crawlipt/__version__.py
 crawlipt/action.py
 crawlipt/annotation.py
 crawlipt/condition.py
+crawlipt/pojo.py
 crawlipt/script.py
 crawlipt.egg-info/PKG-INFO
 crawlipt.egg-info/SOURCES.txt
 crawlipt.egg-info/dependency_links.txt
 crawlipt.egg-info/requires.txt
 crawlipt.egg-info/top_level.txt
 crawlipt/actions/__init__.py
 crawlipt/actions/click.py
 crawlipt/actions/get.py
 crawlipt/actions/input.py
 crawlipt/actions/redirect.py
 crawlipt/actions/select.py
 crawlipt/actions/slide.py
 crawlipt/actions/switch.py
+crawlipt/actions/window.py
 crawlipt/conditions/__init__.py
 crawlipt/conditions/element.py
 crawlipt/conditions/frame.py
 crawlipt/conditions/presence.py
 crawlipt/conditions/text.py
 crawlipt/conditions/visibility.py
```

### Comparing `crawlipt-0.0.4/setup.py` & `crawlipt-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

