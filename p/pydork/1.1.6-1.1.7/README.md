# Comparing `tmp/pydork-1.1.6.tar.gz` & `tmp/pydork-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydork-1.1.6.tar", last modified: Sun Sep  3 14:28:25 2023, max compression
+gzip compressed data, was "pydork-1.1.7.tar", last modified: Mon May  6 07:15:38 2024, max compression
```

## Comparing `pydork-1.1.6.tar` & `pydork-1.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-09-03 14:28:25.571790 pydork-1.1.6/
--rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.6/LICENSE
--rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-09-03 14:28:25.571881 pydork-1.1.6/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)     7974 2023-09-03 14:20:35.000000 pydork-1.1.6/README.md
--rw-r--r--   0 uesugi     (501) staff       (20)     8179 2022-02-13 15:58:36.000000 pydork-1.1.6/README.rst
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-09-03 14:28:25.565747 pydork-1.1.6/completion/
--rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.6/completion/_pydork
--rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.6/completion/pydork-completion.bash
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-09-03 14:28:25.570513 pydork-1.1.6/pydork/
--rwxr-xr-x   0 uesugi     (501) staff       (20)     9192 2023-07-17 07:42:24.000000 pydork-1.1.6/pydork/__init__.py
--rw-r--r--   0 uesugi     (501) staff       (20)     7668 2023-02-17 02:51:20.000000 pydork-1.1.6/pydork/common.py
--rw-r--r--   0 uesugi     (501) staff       (20)    19059 2023-08-29 01:22:28.000000 pydork-1.1.6/pydork/engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    11393 2023-07-17 06:44:12.000000 pydork-1.1.6/pydork/engine_baidu.py
--rw-r--r--   0 uesugi     (501) staff       (20)    11282 2023-07-27 10:54:27.000000 pydork-1.1.6/pydork/engine_bing.py
--rw-r--r--   0 uesugi     (501) staff       (20)    31520 2023-08-29 01:21:47.000000 pydork-1.1.6/pydork/engine_common.py
--rw-r--r--   0 uesugi     (501) staff       (20)     8749 2023-07-27 10:22:34.000000 pydork-1.1.6/pydork/engine_duckduckgo.py
--rw-r--r--   0 uesugi     (501) staff       (20)    18020 2023-08-28 14:51:53.000000 pydork-1.1.6/pydork/engine_google.py
--rw-r--r--   0 uesugi     (501) staff       (20)    10255 2023-07-17 07:37:47.000000 pydork-1.1.6/pydork/engine_yahoo.py
--rw-r--r--   0 uesugi     (501) staff       (20)      556 2023-09-03 14:27:30.000000 pydork-1.1.6/pydork/engine_yandex.py
--rw-r--r--   0 uesugi     (501) staff       (20)     5563 2023-07-10 14:22:02.000000 pydork-1.1.6/pydork/messages.py
--rw-r--r--   0 uesugi     (501) staff       (20)     9743 2023-02-13 22:53:01.000000 pydork-1.1.6/pydork/recaptcha.py
--rw-r--r--   0 uesugi     (501) staff       (20)    12800 2023-07-27 10:58:20.000000 pydork-1.1.6/pydork/sub_commands.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14791 2023-02-13 22:52:45.000000 pydork-1.1.6/pydork/test_engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14893 2023-02-13 22:52:49.000000 pydork-1.1.6/pydork/test_engine_selenium.py
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-09-03 14:28:25.571664 pydork-1.1.6/pydork.egg-info/
--rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)      618 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/SOURCES.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        1 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/dependency_links.txt
--rw-r--r--   0 uesugi     (501) staff       (20)       39 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/entry_points.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      216 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/requires.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        7 2023-09-03 14:28:25.000000 pydork-1.1.6/pydork.egg-info/top_level.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      111 2023-09-03 14:28:25.572208 pydork-1.1.6/setup.cfg
--rwxr-xr-x   0 uesugi     (501) staff       (20)     4301 2023-09-03 14:28:03.000000 pydork-1.1.6/setup.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2024-05-06 07:15:38.618452 pydork-1.1.7/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.7/LICENSE
+-rw-r--r--   0 uesugi     (501) staff       (20)     9448 2024-05-06 07:15:38.618313 pydork-1.1.7/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)     7974 2024-05-06 06:08:13.000000 pydork-1.1.7/README.md
+-rw-r--r--   0 uesugi     (501) staff       (20)     8314 2024-05-06 07:15:38.000000 pydork-1.1.7/README.rst
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2024-05-06 07:15:38.611961 pydork-1.1.7/completion/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.7/completion/_pydork
+-rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.7/completion/pydork-completion.bash
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2024-05-06 07:15:38.616802 pydork-1.1.7/pydork/
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     9192 2023-11-19 07:45:05.000000 pydork-1.1.7/pydork/__init__.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     7668 2023-02-17 02:51:20.000000 pydork-1.1.7/pydork/common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    19059 2023-08-29 01:22:28.000000 pydork-1.1.7/pydork/engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    11393 2023-07-17 06:44:12.000000 pydork-1.1.7/pydork/engine_baidu.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    11282 2023-07-27 10:54:27.000000 pydork-1.1.7/pydork/engine_bing.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    32518 2024-05-06 07:09:15.000000 pydork-1.1.7/pydork/engine_common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     8749 2023-07-27 10:22:34.000000 pydork-1.1.7/pydork/engine_duckduckgo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    18055 2024-05-06 07:05:38.000000 pydork-1.1.7/pydork/engine_google.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    10255 2023-07-17 07:37:47.000000 pydork-1.1.7/pydork/engine_yahoo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)      556 2023-09-05 06:00:44.000000 pydork-1.1.7/pydork/engine_yandex.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     5563 2023-07-10 14:22:02.000000 pydork-1.1.7/pydork/messages.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     9743 2023-02-13 22:53:01.000000 pydork-1.1.7/pydork/recaptcha.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    12800 2023-07-27 10:58:20.000000 pydork-1.1.7/pydork/sub_commands.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14791 2023-02-13 22:52:45.000000 pydork-1.1.7/pydork/test_engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14893 2023-02-13 22:52:49.000000 pydork-1.1.7/pydork/test_engine_selenium.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2024-05-06 07:15:38.617969 pydork-1.1.7/pydork.egg-info/
+-rw-r--r--   0 uesugi     (501) staff       (20)     9448 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)      618 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/SOURCES.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        1 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/dependency_links.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)       39 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/entry_points.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      216 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/requires.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        7 2024-05-06 07:15:38.000000 pydork-1.1.7/pydork.egg-info/top_level.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      111 2024-05-06 07:15:38.618689 pydork-1.1.7/setup.cfg
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     4355 2024-03-23 03:03:43.000000 pydork-1.1.7/setup.py
```

### Comparing `pydork-1.1.6/LICENSE` & `pydork-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/PKG-INFO` & `pydork-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,72 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.6
+Version: 1.1.7
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
+Requires-Dist: bs4
+Requires-Dist: get-chrome-driver
+Requires-Dist: get-gecko-driver
+Requires-Dist: chromedriver_autoinstaller
+Requires-Dist: geckodriver_autoinstaller
+Requires-Dist: fake_useragent
+Requires-Dist: lxml
+Requires-Dist: requests[socks]
+Requires-Dist: selenium==4.7.2
+Requires-Dist: selenium_requests
+Requires-Dist: pickle-mixin
+Requires-Dist: sphinx
+Requires-Dist: sphinx-rtd-theme
+Requires-Dist: sphinx-autobuild
 
 PyDork
 ======
 
 Description
 -----------
 
-Scraping and listing text and image searches on Google, Bing,
-DuckDuckGo, Baidu, Yahoo japan.
+Scraping and listing text and image searches on **Google**, **Bing**,
+**DuckDuckGo**, **Baidu**, **Yahoo japan**.
 
 Install
 -------
 
 .. code:: bash
 
-   git clone https://github.com/blacknon/pydork
-   cd pydork
-   pip install ./
+   pip install pydork
+
+Build
+-----
+
+Documents
+~~~~~~~~~
+
+.. code:: bash
+
+   python setup.py build_sphinx
+
+Dockerimage
+~~~~~~~~~~~
+
+.. code:: bash
+
+   docker build -t "pydork" --progress=plain .
 
 How to use
 ----------
 
 commandline tool
 ~~~~~~~~~~~~~~~~
```

### Comparing `pydork-1.1.6/README.md` & `pydork-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/README.rst` & `pydork-1.1.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 PyDork
 ======
 
 Description
 -----------
 
-Scraping and listing text and image searches on Google, Bing,
-DuckDuckGo, Baidu, Yahoo japan.
+Scraping and listing text and image searches on **Google**, **Bing**,
+**DuckDuckGo**, **Baidu**, **Yahoo japan**.
 
 Install
 -------
 
 .. code:: bash
 
-   git clone https://github.com/blacknon/pydork
-   cd pydork
-   pip install ./
+   pip install pydork
+
+Build
+-----
+
+Documents
+~~~~~~~~~
+
+.. code:: bash
+
+   python setup.py build_sphinx
+
+Dockerimage
+~~~~~~~~~~~
+
+.. code:: bash
+
+   docker build -t "pydork" --progress=plain .
 
 How to use
 ----------
 
 commandline tool
 ~~~~~~~~~~~~~~~~
```

### Comparing `pydork-1.1.6/completion/_pydork` & `pydork-1.1.7/completion/_pydork`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/__init__.py` & `pydork-1.1.7/pydork/__init__.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/common.py` & `pydork-1.1.7/pydork/common.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine.py` & `pydork-1.1.7/pydork/engine.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine_baidu.py` & `pydork-1.1.7/pydork/engine_baidu.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine_bing.py` & `pydork-1.1.7/pydork/engine_bing.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine_common.py` & `pydork-1.1.7/pydork/engine_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """engine_common
     * SearchEngine Classから呼び出す、各検索エンジンで共通の処理を保持させる継承用Classである `CommonEngine` を持つモジュール.
 """
 
 import requests
 import os
 import pickle
-import time
 
 # selenium driver auto install packages
 import chromedriver_autoinstaller
 import geckodriver_autoinstaller
 
 # seleniumrequests
 from seleniumrequests import Chrome, Firefox
@@ -571,19 +570,20 @@
             str: htmlの文字列.
         """
 
         # 優先度1: Selenium経由でのアクセス
         if self.USE_SELENIUM:
             result = self.request_selenium(url, method=method, data=data)
 
-            for i in range(0, 10):
-                self.driver.execute_script(
-                    "window.scrollTo(0,document.body.scrollHeight)"
-                )
-                time.sleep(3)
+            # NOTE: seleniumでのブラウザスクロール. googleでの処理で不要になったため、ただ遅くなるだけで不便なので一旦コメントアウト.
+            # for i in range(0, 10):
+            #     self.driver.execute_script(
+            #         "window.scrollTo(0,document.body.scrollHeight)"
+            #     )
+            #     time.sleep(0.5)
 
         # 優先度2: Splash経由でのアクセス(Seleniumが有効になってない場合はこちら)
         elif self.USE_SPLASH:
             # create splash url
             result = self.request_splash(url, method=method, data=data)
 
         # 優先度3: request.sessionからのリクエスト(SeleniumもSplashも有効でない場合)
@@ -701,22 +701,43 @@
 
         Returns:
             list: linkの検索結果([xxx,xxx,xxx...])
             list: titleの検索結果([xxx,xxx,xxx...])
             list: textの検索結果([xxx,xxx,xxx...])
         """
         # linkのurlを取得する
+        self.MESSAGE.print_text(
+            self.SOUP_SELECT_URL,  # type: ignore
+            header=self.MESSAGE.HEADER + ': ' + \
+            Color.GREEN + '[get_text_link.SOUP_SELECT_URL]' + Color.END,
+            separator=" :",
+            mode="debug",
+        )
         elements = soup.select(self.SOUP_SELECT_URL)
         elinks = [e['href'] for e in elements]
 
         # linkのtitleを取得する
+        self.MESSAGE.print_text(
+            self.SOUP_SELECT_TITLE,  # type: ignore
+            header=self.MESSAGE.HEADER + ': ' + \
+            Color.GREEN + '[get_text_link.SOUP_SELECT_TITLE]' + Color.END,
+            separator=" :",
+            mode="debug",
+        )
         elements = soup.select(self.SOUP_SELECT_TITLE)
         etitles = [e.text for e in elements]
 
         # linkのtextを取得する
+        self.MESSAGE.print_text(
+            self.SOUP_SELECT_TEXT,  # type: ignore
+            header=self.MESSAGE.HEADER + ': ' + \
+            Color.GREEN + '[get_text_link.SOUP_SELECT_TEXT]' + Color.END,
+            separator=" :",
+            mode="debug",
+        )
         elements = soup.select(self.SOUP_SELECT_TEXT)
         etext = [e.text for e in elements]
 
         return elinks, etitles, etext
 
     # 画像検索ページの検索結果(links(list()))を生成するfunction
     def get_image_links(self, soup: BeautifulSoup):
```

### Comparing `pydork-1.1.6/pydork/engine_duckduckgo.py` & `pydork-1.1.7/pydork/engine_duckduckgo.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine_google.py` & `pydork-1.1.7/pydork/engine_google.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,24 +198,24 @@
             self.SOUP_SELECT_URL = '#main > div > div > .kCrYT > a'
             self.SOUP_SELECT_TITLE = '#main > div > div > .kCrYT > a > h3 > div'
             self.SOUP_SELECT_TEXT = '#main > div > div > .kCrYT > div > div > div > div > div'
             self.SOUP_SELECT_NEXT_URL = ''
 
             # Selenium経由、かつFirefoxを使っている場合
             if self.USE_SELENIUM:
-                self.SOUP_SELECT_URL = '.yuRUbf > div > a'
-                self.SOUP_SELECT_TITLE = '.yuRUbf > div > a > .LC20lb'
-                self.SOUP_SELECT_TEXT = '.lEBKkf'
+                self.SOUP_SELECT_URL = '.yuRUbf > div > span > a'
+                self.SOUP_SELECT_TITLE = '.yuRUbf > div > span > a > h3'
+                self.SOUP_SELECT_TEXT = '.yXK7lf'
                 self.SOUP_SELECT_NEXT_URL = '.AaVjTc > tbody > tr > td > a'
 
             # Splash経由で通信している場合
             elif self.USE_SPLASH:
-                self.SOUP_SELECT_URL = '.yuRUbf > a'
-                self.SOUP_SELECT_TITLE = '.yuRUbf > a > .LC20lb'
-                self.SOUP_SELECT_TEXT = '.lEBKkf'
+                self.SOUP_SELECT_URL = '.yuRUbf > div > span > a.href'
+                self.SOUP_SELECT_TITLE = '.yuRUbf > div > span > a > h3'
+                self.SOUP_SELECT_TEXT = '.yXK7lf'
                 self.SOUP_SELECT_NEXT_URL = '.AaVjTc > tbody > tr > td > a'
 
             # TODO: SEARCH_NEXT_URLを書き換える
             # self.get_nextpage_url(html)
 
             # CommonEngineの処理を呼び出す
             links = super().get_links(url, html, type)
```

### Comparing `pydork-1.1.6/pydork/engine_yahoo.py` & `pydork-1.1.7/pydork/engine_yahoo.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/engine_yandex.py` & `pydork-1.1.7/pydork/engine_yandex.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/messages.py` & `pydork-1.1.7/pydork/messages.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/recaptcha.py` & `pydork-1.1.7/pydork/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/sub_commands.py` & `pydork-1.1.7/pydork/sub_commands.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/test_engine.py` & `pydork-1.1.7/pydork/test_engine.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork/test_engine_selenium.py` & `pydork-1.1.7/pydork/test_engine_selenium.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/pydork.egg-info/PKG-INFO` & `pydork-1.1.7/pydork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,72 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.6
+Version: 1.1.7
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
+Requires-Dist: bs4
+Requires-Dist: get-chrome-driver
+Requires-Dist: get-gecko-driver
+Requires-Dist: chromedriver_autoinstaller
+Requires-Dist: geckodriver_autoinstaller
+Requires-Dist: fake_useragent
+Requires-Dist: lxml
+Requires-Dist: requests[socks]
+Requires-Dist: selenium==4.7.2
+Requires-Dist: selenium_requests
+Requires-Dist: pickle-mixin
+Requires-Dist: sphinx
+Requires-Dist: sphinx-rtd-theme
+Requires-Dist: sphinx-autobuild
 
 PyDork
 ======
 
 Description
 -----------
 
-Scraping and listing text and image searches on Google, Bing,
-DuckDuckGo, Baidu, Yahoo japan.
+Scraping and listing text and image searches on **Google**, **Bing**,
+**DuckDuckGo**, **Baidu**, **Yahoo japan**.
 
 Install
 -------
 
 .. code:: bash
 
-   git clone https://github.com/blacknon/pydork
-   cd pydork
-   pip install ./
+   pip install pydork
+
+Build
+-----
+
+Documents
+~~~~~~~~~
+
+.. code:: bash
+
+   python setup.py build_sphinx
+
+Dockerimage
+~~~~~~~~~~~
+
+.. code:: bash
+
+   docker build -t "pydork" --progress=plain .
 
 How to use
 ----------
 
 commandline tool
 ~~~~~~~~~~~~~~~~
```

### Comparing `pydork-1.1.6/pydork.egg-info/SOURCES.txt` & `pydork-1.1.7/pydork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydork-1.1.6/setup.py` & `pydork-1.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         readme = f.read()
 except IOError:
     readme = ''
 
 
 # 補完ファイルインストール用関数
 def get_data_files():
-
     # 補完ファイルのインストール先を取得する関数
     def get_completefile_install_location(shell):
         # pathのprefixを定義
         prefix = ''
 
         # osの種類を取得
         uname = platform.uname()[0]
@@ -74,20 +73,21 @@
         ]
     )
 
     # data_files形式でreturn
     data_files = []
     data_files.append((loc['bash'], files['bash']))
     data_files.append((loc['zsh'], files['zsh']))
+
     return data_files
 
 
 name = 'pydork'
-version = '1.1.6'
-release = '1.1.6'
+version = '1.1.7'
+release = '1.1.7'
 
 if __name__ == "__main__":
     setuptools.setup(
         name=name,
         version=version,
         author='blacknon',
         author_email='blacknon@orebibou.com',
@@ -122,14 +122,15 @@
         },
         classifiers=[
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'License :: OSI Approved :: MIT License',
         ],
         data_files=get_data_files(),
         cmdclass=cmdclass,
         command_options={
             'build_sphinx': {
                 'project': ('setup.py', name),
```

