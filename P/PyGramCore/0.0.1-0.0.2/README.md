# Comparing `tmp/pygramcore-0.0.1.tar.gz` & `tmp/PyGramCore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygramcore-0.0.1.tar", last modified: Mon May  6 14:36:43 2024, max compression
+gzip compressed data, was "PyGramCore-0.0.2.tar", last modified: Mon May  6 17:10:27 2024, max compression
```

## Comparing `pygramcore-0.0.1.tar` & `PyGramCore-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 14:36:32.000000 pygramcore-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 14:36:43.281008 pygramcore-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/PyGramCore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 14:36:43.000000 pygramcore-0.0.1/PyGramCore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 14:36:43.000000 pygramcore-0.0.1/PyGramCore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:36:43.000000 pygramcore-0.0.1/PyGramCore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 14:36:43.000000 pygramcore-0.0.1/PyGramCore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 14:36:43.000000 pygramcore-0.0.1/PyGramCore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 14:36:32.000000 pygramcore-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:36:43.281008 pygramcore-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-06 14:36:32.000000 pygramcore-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/src/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/elements/Comment.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/elements/Post.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/elements/User.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/src/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/exceptions/Auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/exceptions/Format.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:43.281008 pygramcore-0.0.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-06 14:36:32.000000 pygramcore-0.0.1/src/utils/navigation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.045757 PyGramCore-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4062 2024-05-06 17:10:27.044757 PyGramCore-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.043757 PyGramCore-0.0.2/PyGramCore.egg-info/
+-rw-rw-rw-   0        0        0     4062 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3336 2024-05-06 16:49:49.000000 PyGramCore-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:10:27.045757 PyGramCore-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2024-05-06 16:54:23.000000 PyGramCore-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.033257 PyGramCore-0.0.2/src/
+-rw-rw-rw-   0        0        0        0 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     6036 2024-05-06 13:11:25.000000 PyGramCore-0.0.2/src/auth.py
+-rw-rw-rw-   0        0        0      240 2024-05-06 11:25:42.000000 PyGramCore-0.0.2/src/constants.py
+-rw-rw-rw-   0        0        0      992 2024-05-06 13:12:51.000000 PyGramCore-0.0.2/src/driver.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.037258 PyGramCore-0.0.2/src/elements/
+-rw-rw-rw-   0        0        0       71 2024-05-05 21:01:41.000000 PyGramCore-0.0.2/src/elements/Comment.py
+-rw-rw-rw-   0        0        0      386 2024-05-05 20:01:12.000000 PyGramCore-0.0.2/src/elements/Post.py
+-rw-rw-rw-   0        0        0      640 2024-05-05 20:01:24.000000 PyGramCore-0.0.2/src/elements/User.py
+-rw-rw-rw-   0        0        0        0 2024-05-05 19:37:24.000000 PyGramCore-0.0.2/src/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.039756 PyGramCore-0.0.2/src/exceptions/
+-rw-rw-rw-   0        0        0      222 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/exceptions/Auth.py
+-rw-rw-rw-   0        0        0      433 2024-05-06 11:27:24.000000 PyGramCore-0.0.2/src/exceptions/Format.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 13:12:23.000000 PyGramCore-0.0.2/src/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-05-06 14:18:40.000000 PyGramCore-0.0.2/src/test.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.042257 PyGramCore-0.0.2/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      292 2024-05-05 19:01:19.000000 PyGramCore-0.0.2/src/utils/auth.py
+-rw-rw-rw-   0        0        0     3592 2024-05-06 13:08:46.000000 PyGramCore-0.0.2/src/utils/navigation.py
```

### Comparing `pygramcore-0.0.1/LICENSE` & `PyGramCore-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Joel Taylor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Joel Taylor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pygramcore-0.0.1/setup.py` & `PyGramCore-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from setuptools import setup, find_packages
-from codecs import open
-from os import path
-
-NAME = "PyGramCore"
-VERSION = '0.0.1'
-DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
-
-# Get the long description from the README file
-here = path.abspath(path.dirname(__file__))
-with open(path.join(here, "README.md"), encoding="utf-8") as f:
-    LONG_DESCRIPTION = f.read()
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    author="Joel Taylor",
-    author_email="contact@joeltaylor.business",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.12",
-        "Programming Language :: Python :: Implementation :: CPython",
-    ],
-    keywords=["instagram", "instagram bot", "selenium", "automation", "bot"],
-    packages=find_packages(exclude=["docs", "tests"]),
-    install_requires=["selenium", "selenium-stealth"],
-    setup_requires=["setuptools>=38.6.0"],
-)
+from setuptools import setup, find_packages
+from codecs import open
+from os import path
+
+NAME = "PyGramCore"
+VERSION = '0.0.2'
+DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
+
+# Get the long description from the README file
+here = path.abspath(path.dirname(__file__))
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
+    LONG_DESCRIPTION = f.read()
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
+    author="Joel Taylor",
+    author_email="contact@joeltaylor.business",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: Implementation :: CPython",
+    ],
+    keywords=["instagram", "instagram bot", "selenium", "automation", "bot"],
+    packages=find_packages(exclude=["docs", "tests"]),
+    install_requires=["selenium", "selenium-stealth"],
+    setup_requires=["setuptools>=38.6.0"],
+)
```

### Comparing `pygramcore-0.0.1/src/auth.py` & `PyGramCore-0.0.2/src/auth.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from typing import List, Dict, Union
-import os
-import time
-import random
-
-from exceptions.Format import IncorrectFormat
-from utils.navigation import *
-from constants import *
-
-
-class Account:
-    """
-    Represents an instagram account.
-
-    Args:
-        email_or_cookies (Union[str, List[Dict[str, str]]]):
-            Either the email address of the account as a string or
-            a list of cookies as dictionaries. If email is provided,
-            the `password` argument can be optionally provided.
-        password (str, optional):
-            The password of the account. Required if `email_or_cookies`
-            is an email address. Defaults to None.
-
-    Raises:
-        RuntimeError:
-            If an attempt is made to instantiate more than one Account object.
-        ValueError:
-            If the `email_or_cookies` argument is neither a string nor a list.
-    """
-
-    _instance = None
-
-    def __init__(
-        self, email_or_cookies: Union[str, List[Dict[str, str]]], password: str = None
-    ):
-        if Account._instance is not None:
-            raise RuntimeError("Cannot instantiate more than one Account.")
-        Account._instance = self
-
-        if isinstance(email_or_cookies, str):
-            self._email = email_or_cookies
-            self._password = password
-            self._cookies = []
-        elif isinstance(email_or_cookies, list):
-            self._email = None
-            self._password = None
-            self._cookies = email_or_cookies
-        else:
-            raise ValueError("Invalid argument type for email_or_cookies.")
-
-        self._logged_in = bool(self._cookies)
-        self.driver: webdriver.Chrome = None
-
-    @classmethod
-    def get_instance(cls):
-        """
-        Returns the current instance of the account.
-        """
-        return cls._instance
-
-    def get_cookies(self):
-        return self._cookies
-
-    def set_cookies(self, cookies):
-        self._cookies = cookies
-
-    def is_logged_in(self):
-        return self._logged_in
-
-    @get_webdriver(INSTAGRAM_LOGIN_URL)
-    @handle_cookies_dialog
-    def login(self):
-        """
-        Uses the Instagram UI to log in. It will require user interaction to get past CAPTCHAs and the sort.
-        Returns:
-            list[dict]: list of cookies.
-        """
-        # Write email
-        email_input = self.driver.find_element(
-            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(1) > div > label > input"
-        )
-        self.write(email_input, self._email)
-
-        # Write password
-        password_input = self.driver.find_element(
-            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(2) > div > label > input"
-        )
-        self.write(password_input, self._password)
-
-        # Login
-        login_btn = self.driver.find_element(
-            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(3) > button"
-        )
-        login_btn.click()
-
-        # Wait till fully logged in
-        time.sleep(5)
-
-        # Update value
-        self._logged_in = True
-
-        # Return cookies after logging in
-        self._cookies = self.driver.get_cookies()
-        return self._cookies
-
-    @get_webdriver(INSTAGRAM_URL)
-    def post(self, image_path: str, caption: str = None):
-        """
-        Posts a specific image to the account.
-        Args:
-            image_path (str): absolute path to the image
-        """
-        # Check if image is the correct format
-        _, extension = os.path.splitext(image_path)
-        if extension[1:] not in MEDIA_FORMATS:
-            raise IncorrectFormat()
-
-        # Open create dialog
-        create_button = self.driver.find_element(
-            By.CSS_SELECTOR,
-            "svg[aria-label='New post']",
-        )
-        create_button.click()
-
-        # Add file to the input
-        file_input = self.driver.find_element(By.CSS_SELECTOR, "input[type='file']")
-        file_input.send_keys(image_path)
-
-        # Click 'Next' next button twice
-        for _ in range(2):
-            # It requires to be found each iteration due to the "StaleElementReferenceException"
-            next_btn = self.driver.find_element(
-                By.CSS_SELECTOR,
-                "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div > div > div > div._ap97 > div > div > div > div._ac7b._ac7d > div",
-            )
-            next_btn.click()
-            time.sleep(random.random())
-
-        # Write caption if specified
-        if caption:
-            caption_input = self.driver.find_element(
-                By.CSS_SELECTOR, "div[aria-label='Write a caption...']"
-            )
-            self.write(caption_input, caption)
-
-        # Click 'Share' button
-        share_btn = self.driver.find_element(
-            By.CSS_SELECTOR,
-            "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div > div > div > div._ap97 > div > div > div > div._ac7b._ac7d > div",
-        )
-        # next_btn.click()
-
-    def write(self, input, text, speed=3):
-        """
-        Types some text letter by letter at random intervals in an input field. This is done so the interaction feels more "human-like".
-
-        Args:
-            input (WebElement): The input to write in.
-            text (str): Text being written.
-            speed (int): Divides the random float (from 0 to 1). The higher the number the faster it writes.
-        """
-        for letter in text:
-            input.send_keys(letter)
-            time.sleep(random.random() / speed)
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from typing import List, Dict, Union
+import os
+import time
+import random
+
+from exceptions.Format import IncorrectFormat
+from utils.navigation import *
+from constants import *
+
+
+class Account:
+    """
+    Represents an instagram account.
+
+    Args:
+        email_or_cookies (Union[str, List[Dict[str, str]]]):
+            Either the email address of the account as a string or
+            a list of cookies as dictionaries. If email is provided,
+            the `password` argument can be optionally provided.
+        password (str, optional):
+            The password of the account. Required if `email_or_cookies`
+            is an email address. Defaults to None.
+
+    Raises:
+        RuntimeError:
+            If an attempt is made to instantiate more than one Account object.
+        ValueError:
+            If the `email_or_cookies` argument is neither a string nor a list.
+    """
+
+    _instance = None
+
+    def __init__(
+        self, email_or_cookies: Union[str, List[Dict[str, str]]], password: str = None
+    ):
+        if Account._instance is not None:
+            raise RuntimeError("Cannot instantiate more than one Account.")
+        Account._instance = self
+
+        if isinstance(email_or_cookies, str):
+            self._email = email_or_cookies
+            self._password = password
+            self._cookies = []
+        elif isinstance(email_or_cookies, list):
+            self._email = None
+            self._password = None
+            self._cookies = email_or_cookies
+        else:
+            raise ValueError("Invalid argument type for email_or_cookies.")
+
+        self._logged_in = bool(self._cookies)
+        self.driver: webdriver.Chrome = None
+
+    @classmethod
+    def get_instance(cls):
+        """
+        Returns the current instance of the account.
+        """
+        return cls._instance
+
+    def get_cookies(self):
+        return self._cookies
+
+    def set_cookies(self, cookies):
+        self._cookies = cookies
+
+    def is_logged_in(self):
+        return self._logged_in
+
+    @get_webdriver(INSTAGRAM_LOGIN_URL)
+    @handle_cookies_dialog
+    def login(self):
+        """
+        Uses the Instagram UI to log in. It will require user interaction to get past CAPTCHAs and the sort.
+        Returns:
+            list[dict]: list of cookies.
+        """
+        # Write email
+        email_input = self.driver.find_element(
+            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(1) > div > label > input"
+        )
+        self.write(email_input, self._email)
+
+        # Write password
+        password_input = self.driver.find_element(
+            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(2) > div > label > input"
+        )
+        self.write(password_input, self._password)
+
+        # Login
+        login_btn = self.driver.find_element(
+            By.CSS_SELECTOR, "#loginForm > div > div:nth-child(3) > button"
+        )
+        login_btn.click()
+
+        # Wait till fully logged in
+        time.sleep(5)
+
+        # Update value
+        self._logged_in = True
+
+        # Return cookies after logging in
+        self._cookies = self.driver.get_cookies()
+        return self._cookies
+
+    @get_webdriver(INSTAGRAM_URL)
+    def post(self, image_path: str, caption: str = None):
+        """
+        Posts a specific image to the account.
+        Args:
+            image_path (str): absolute path to the image
+        """
+        # Check if image is the correct format
+        _, extension = os.path.splitext(image_path)
+        if extension[1:] not in MEDIA_FORMATS:
+            raise IncorrectFormat()
+
+        # Open create dialog
+        create_button = self.driver.find_element(
+            By.CSS_SELECTOR,
+            "svg[aria-label='New post']",
+        )
+        create_button.click()
+
+        # Add file to the input
+        file_input = self.driver.find_element(By.CSS_SELECTOR, "input[type='file']")
+        file_input.send_keys(image_path)
+
+        # Click 'Next' next button twice
+        for _ in range(2):
+            # It requires to be found each iteration due to the "StaleElementReferenceException"
+            next_btn = self.driver.find_element(
+                By.CSS_SELECTOR,
+                "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div > div > div > div._ap97 > div > div > div > div._ac7b._ac7d > div",
+            )
+            next_btn.click()
+            time.sleep(random.random())
+
+        # Write caption if specified
+        if caption:
+            caption_input = self.driver.find_element(
+                By.CSS_SELECTOR, "div[aria-label='Write a caption...']"
+            )
+            self.write(caption_input, caption)
+
+        # Click 'Share' button
+        share_btn = self.driver.find_element(
+            By.CSS_SELECTOR,
+            "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div > div > div > div._ap97 > div > div > div > div._ac7b._ac7d > div",
+        )
+        # next_btn.click()
+
+    def write(self, input, text, speed=3):
+        """
+        Types some text letter by letter at random intervals in an input field. This is done so the interaction feels more "human-like".
+
+        Args:
+            input (WebElement): The input to write in.
+            text (str): Text being written.
+            speed (int): Divides the random float (from 0 to 1). The higher the number the faster it writes.
+        """
+        for letter in text:
+            input.send_keys(letter)
+            time.sleep(random.random() / speed)
```

### Comparing `pygramcore-0.0.1/src/elements/User.py` & `PyGramCore-0.0.2/src/elements/User.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from dataclasses import dataclass
-
-from utils.auth import check_auth
-from elements.Post import Post
-
-
-@dataclass
-class User:
-    """
-    Represents an Instagram user.
-
-    Args:
-        name (str): Username of the user.
-    """
-
-    name: str
-
-    def is_private(self) -> bool:
-        pass
-
-    def follow(self) -> None:
-        pass
-
-    def unfollow(self) -> None:
-        pass
-
-    def get_followers(self) -> int:
-        pass
-
-    def get_following(self) -> int:
-        pass
-
-    def send_dm(self, message: str) -> None:
-        pass
-
-    def get_posts(self, limit=10) -> list[Post]:
-        pass
+from dataclasses import dataclass
+
+from utils.auth import check_auth
+from elements.Post import Post
+
+
+@dataclass
+class User:
+    """
+    Represents an Instagram user.
+
+    Args:
+        name (str): Username of the user.
+    """
+
+    name: str
+
+    def is_private(self) -> bool:
+        pass
+
+    def follow(self) -> None:
+        pass
+
+    def unfollow(self) -> None:
+        pass
+
+    def get_followers(self) -> int:
+        pass
+
+    def get_following(self) -> int:
+        pass
+
+    def send_dm(self, message: str) -> None:
+        pass
+
+    def get_posts(self, limit=10) -> list[Post]:
+        pass
```

### Comparing `pygramcore-0.0.1/src/utils/navigation.py` & `PyGramCore-0.0.2/src/utils/navigation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support.ui import WebDriverWait
-from selenium.webdriver.support import expected_conditions as EC
-
-
-from driver import WebDriver
-from constants import IMPLICIT_WAIT
-
-
-def get_webdriver(url: str = None):
-    """
-    Inserts the current instance of the webdriver in the class instance.
-
-    Args:
-        url (str): Initial URL to go to.
-
-    Usage:
-    ```
-    @get_webdriver("https://google.com")
-    def your_function(driver):
-        ...
-
-    your_function()
-    ```
-    """
-
-    def decorator(func):
-        def wrapper(account, *args, **kwargs):
-            # Get current instance of the driver
-            instance = WebDriver()
-
-            # Navigate to url if specified
-            if url:
-                instance.get(url)
-
-            account.driver = instance
-
-            # Add cookies to the driver if any
-            account_cookies = account.get_cookies()
-            if account_cookies:
-                current_cookies = instance.get_cookies()
-
-                for cookie in account_cookies:
-                    # Check if they have been added already
-                    if cookie not in current_cookies:
-                        instance.add_cookie(cookie)
-
-                # Refresh page to effectuate cookies
-                instance.refresh()
-
-                # Close notification dialog
-                disallow_notifications()
-
-            value = func(account, *args, **kwargs)
-            return value
-
-        return wrapper
-
-    return decorator
-
-
-def handle_cookies_dialog(func):
-    def wrapper(*args, **kwargs):
-        # Get current instance of the driver
-        driver = WebDriver()
-
-        # Attempt to click the cookies dialog if found
-        # If not, it shall pass
-        try:
-            btn = WebDriverWait(driver, 3).until(
-                EC.element_to_be_clickable(
-                    (
-                        By.CSS_SELECTOR,
-                        "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe.x5yr21d.x19onx9a > div > button._a9--._ap36._a9_1",
-                    )
-                )
-            )
-            btn.click()
-        except:
-            print("Not found")
-
-        # Run function being decorated
-        value = func(*args, **kwargs)
-        return value
-
-    return wrapper
-
-
-def disallow_notifications():
-    """
-    Clicks "Not Now" when Instagram asks for notification access. This decorator should be placed on functions that login the account.
-    """
-    # Get current instance of the driver
-    driver = WebDriver()
-
-    # Attempt to disallow notifications
-    try:
-        btn = WebDriverWait(driver, 3).until(
-            EC.element_to_be_clickable(
-                (
-                    By.CSS_SELECTOR,
-                    "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div._a9-z > button._a9--._ap36._a9_1",
-                )
-            )
-        )
-        btn.click()
-    except:
-        print("not found")
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+
+
+from driver import WebDriver
+from constants import IMPLICIT_WAIT
+
+
+def get_webdriver(url: str = None):
+    """
+    Inserts the current instance of the webdriver in the class instance.
+
+    Args:
+        url (str): Initial URL to go to.
+
+    Usage:
+    ```
+    @get_webdriver("https://google.com")
+    def your_function(driver):
+        ...
+
+    your_function()
+    ```
+    """
+
+    def decorator(func):
+        def wrapper(account, *args, **kwargs):
+            # Get current instance of the driver
+            instance = WebDriver()
+
+            # Navigate to url if specified
+            if url:
+                instance.get(url)
+
+            account.driver = instance
+
+            # Add cookies to the driver if any
+            account_cookies = account.get_cookies()
+            if account_cookies:
+                current_cookies = instance.get_cookies()
+
+                for cookie in account_cookies:
+                    # Check if they have been added already
+                    if cookie not in current_cookies:
+                        instance.add_cookie(cookie)
+
+                # Refresh page to effectuate cookies
+                instance.refresh()
+
+                # Close notification dialog
+                disallow_notifications()
+
+            value = func(account, *args, **kwargs)
+            return value
+
+        return wrapper
+
+    return decorator
+
+
+def handle_cookies_dialog(func):
+    def wrapper(*args, **kwargs):
+        # Get current instance of the driver
+        driver = WebDriver()
+
+        # Attempt to click the cookies dialog if found
+        # If not, it shall pass
+        try:
+            btn = WebDriverWait(driver, 3).until(
+                EC.element_to_be_clickable(
+                    (
+                        By.CSS_SELECTOR,
+                        "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe.x5yr21d.x19onx9a > div > button._a9--._ap36._a9_1",
+                    )
+                )
+            )
+            btn.click()
+        except:
+            print("Not found")
+
+        # Run function being decorated
+        value = func(*args, **kwargs)
+        return value
+
+    return wrapper
+
+
+def disallow_notifications():
+    """
+    Clicks "Not Now" when Instagram asks for notification access. This decorator should be placed on functions that login the account.
+    """
+    # Get current instance of the driver
+    driver = WebDriver()
+
+    # Attempt to disallow notifications
+    try:
+        btn = WebDriverWait(driver, 3).until(
+            EC.element_to_be_clickable(
+                (
+                    By.CSS_SELECTOR,
+                    "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div._a9-z > button._a9--._ap36._a9_1",
+                )
+            )
+        )
+        btn.click()
+    except:
+        print("not found")
```

