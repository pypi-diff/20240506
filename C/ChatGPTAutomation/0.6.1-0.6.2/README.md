# Comparing `tmp/chatgptautomation-0.6.1.tar.gz` & `tmp/chatgptautomation-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgptautomation-0.6.1.tar", last modified: Mon Apr 29 07:49:31 2024, max compression
+gzip compressed data, was "chatgptautomation-0.6.2.tar", last modified: Mon May  6 06:33:01 2024, max compression
```

## Comparing `chatgptautomation-0.6.1.tar` & `chatgptautomation-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.454935 chatgptautomation-0.6.1/
-drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.451560 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/
--rw-rw-rw-   0        0        0     9679 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      827 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/LICENCE.md
--rw-rw-rw-   0        0        0     9679 2024-04-29 07:49:31.453810 chatgptautomation-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     6925 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.446225 chatgptautomation-0.6.1/chatgpt_automation/
--rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/chatgpt_automation/__init__.py
--rw-rw-rw-   0        0        0    39539 2024-04-29 07:29:15.000000 chatgptautomation-0.6.1/chatgpt_automation/chatgpt_automation.py
--rw-rw-rw-   0        0        0     5956 2024-04-29 07:35:24.000000 chatgptautomation-0.6.1/chatgpt_automation/chromedriver_manager.py
--rw-rw-rw-   0        0        0       42 2024-04-29 07:49:31.454935 chatgptautomation-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1504 2024-04-29 07:39:58.000000 chatgptautomation-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.449880 chatgptautomation-0.6.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2762 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/tests/test_chatgpt_automation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:33:01.864690 chatgptautomation-0.6.2/
+drwxrwxrwx   0        0        0        0 2024-05-06 06:33:01.862655 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/
+-rw-rw-rw-   0        0        0     9679 2024-05-06 06:33:01.000000 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2024-05-06 06:33:01.000000 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:33:01.000000 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      827 2024-05-06 06:33:01.000000 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-06 06:33:01.000000 chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-04-28 19:36:18.000000 chatgptautomation-0.6.2/LICENCE.md
+-rw-rw-rw-   0        0        0     9679 2024-05-06 06:33:01.863655 chatgptautomation-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6925 2024-04-28 19:36:18.000000 chatgptautomation-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 06:33:01.861606 chatgptautomation-0.6.2/chatgpt_automation/
+-rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.2/chatgpt_automation/__init__.py
+-rw-rw-rw-   0        0        0    39582 2024-05-06 06:26:52.000000 chatgptautomation-0.6.2/chatgpt_automation/chatgpt_automation.py
+-rw-rw-rw-   0        0        0     5956 2024-04-29 07:35:24.000000 chatgptautomation-0.6.2/chatgpt_automation/chromedriver_manager.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:33:01.864690 chatgptautomation-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1504 2024-05-06 06:29:26.000000 chatgptautomation-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:33:01.862655 chatgptautomation-0.6.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2762 2024-04-28 19:36:18.000000 chatgptautomation-0.6.2/tests/test_chatgpt_automation.py
```

### Comparing `chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/PKG-INFO` & `chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/requires.txt` & `chatgptautomation-0.6.2/ChatGPTAutomation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.1/LICENCE.md` & `chatgptautomation-0.6.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.1/PKG-INFO` & `chatgptautomation-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chatgptautomation-0.6.1/README.md` & `chatgptautomation-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.1/chatgpt_automation/chatgpt_automation.py` & `chatgptautomation-0.6.2/chatgpt_automation/chatgpt_automation.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
     GMAIL_INPUT = (By.CSS_SELECTOR, 'input[type="email"][id="identifierId"]')
     GMAIL_NEXT_BTN = (By.ID, 'identifierNext')
     GMAIL_PASSWORD_INPUT = (By.CSS_SELECTOR, 'input[type="password"][name="password"]')
     GMAIL_PASSWORD_NEXT_BTN = (By.ID, 'passwordNext')
     ADD_NEW_GMAIL_BTN = (By.XPATH, '//li[contains(.,"Use another account")]')
 
+    RESPONSE_DIV = (By.CLASS_NAME, "markdown")
+
 class ChatGPTAutomation:
     class DelayTimes:
         CONSTRUCTOR_DELAY = 6
         SEND_PROMPT_DELAY = 20
         UPLOAD_FILE_DELAY = 10
         RETURN_LAST_RESPONSE_DELAY = 2
         OPEN_NEW_CHAT_DELAY = 10
@@ -420,15 +422,15 @@
         The text is retrieved from the clipboard and returned. Error handling and logging are implemented
         to capture any issues during the execution of the function.
 
         :return: The text of the last ChatGPT response as a string, or an error message if an exception occurs.
         """
 
         try:
-            response = self.driver.find_elements(*ChatGPTLocators.CHAT_GPT_CONVERSION)[-1]
+            response = self.driver.find_elements(*ChatGPTLocators.RESPONSE_DIV)[-1]
 
             return response.text
 
         except NoSuchElementException:
             # Handle the case where the element is not found
             logging.error('Element not found in return_last_response')
             return "Element not found."
```

### Comparing `chatgptautomation-0.6.1/chatgpt_automation/chromedriver_manager.py` & `chatgptautomation-0.6.2/chatgpt_automation/chromedriver_manager.py`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.1/setup.py` & `chatgptautomation-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements from the requirements.txt file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='ChatGPTAutomation',
-    version='0.6.1',
+    version='0.6.2',
     author='Seyed Ali Hosseini',
     author_email='iamseyedalipro@gmail.com',
     description='A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation',
     long_description=open('README.md', encoding="utf8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/iamseyedalipro/ChatGPTAutomation',
     packages=find_packages(),
```

### Comparing `chatgptautomation-0.6.1/tests/test_chatgpt_automation.py` & `chatgptautomation-0.6.2/tests/test_chatgpt_automation.py`

 * *Files identical despite different names*

