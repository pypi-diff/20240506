# Comparing `tmp/SMSCallBomber-0.1.tar.gz` & `tmp/SMSCallBomber-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMSCallBomber-0.1.tar", last modified: Mon May  6 17:10:48 2024, max compression
+gzip compressed data, was "SMSCallBomber-1.1.tar", last modified: Mon May  6 16:35:09 2024, max compression
```

## Comparing `SMSCallBomber-0.1.tar` & `SMSCallBomber-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:10:48.273088 SMSCallBomber-0.1/
--rw-r--r--   0 root         (0) root         (0)     1055 2024-05-05 16:24:34.000000 SMSCallBomber-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3153 2024-05-06 17:10:48.273088 SMSCallBomber-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2635 2024-05-06 16:42:18.000000 SMSCallBomber-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:10:48.269088 SMSCallBomber-0.1/SMSCallBomber.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3153 2024-05-06 17:10:48.000000 SMSCallBomber-0.1/SMSCallBomber.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-06 17:10:48.000000 SMSCallBomber-0.1/SMSCallBomber.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 17:10:48.000000 SMSCallBomber-0.1/SMSCallBomber.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-05-06 17:10:48.000000 SMSCallBomber-0.1/SMSCallBomber.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-06 17:10:48.000000 SMSCallBomber-0.1/SMSCallBomber.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 17:10:48.269088 SMSCallBomber-0.1/SMSСallBomber/
--rw-r--r--   0 root         (0) root         (0)     2811 2024-05-06 16:00:57.000000 SMSCallBomber-0.1/SMSСallBomber/SMSCallBomber.py
--rw-r--r--   0 root         (0) root         (0)   580121 2024-05-04 14:02:20.000000 SMSCallBomber-0.1/SMSСallBomber/Services.py
--rw-r--r--   0 root         (0) root         (0)  1335628 2024-05-03 17:22:00.000000 SMSCallBomber-0.1/SMSСallBomber/User_Agent.py
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-06 17:08:47.000000 SMSCallBomber-0.1/SMSСallBomber/__init__.py
--rw-r--r--   0 root         (0) root         (0)      530 2024-05-01 13:34:45.000000 SMSCallBomber-0.1/SMSСallBomber/config.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-05-06 15:56:10.000000 SMSCallBomber-0.1/SMSСallBomber/service.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 17:10:48.273088 SMSCallBomber-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-06 17:10:25.000000 SMSCallBomber-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:35:09.252418 SMSCallBomber-1.1/
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-05-05 16:24:34.000000 SMSCallBomber-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-05-06 16:35:09.252418 SMSCallBomber-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-05-06 15:28:17.000000 SMSCallBomber-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:35:09.252418 SMSCallBomber-1.1/SMSCallBomber.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-05-06 16:35:09.000000 SMSCallBomber-1.1/SMSCallBomber.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-06 16:35:09.000000 SMSCallBomber-1.1/SMSCallBomber.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 16:35:09.000000 SMSCallBomber-1.1/SMSCallBomber.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-06 16:35:09.000000 SMSCallBomber-1.1/SMSCallBomber.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-06 16:35:09.000000 SMSCallBomber-1.1/SMSCallBomber.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:35:09.252418 SMSCallBomber-1.1/SMSСallBomber/
+-rw-r--r--   0 root         (0) root         (0)   580121 2024-05-04 14:02:20.000000 SMSCallBomber-1.1/SMSСallBomber/Services.py
+-rw-r--r--   0 root         (0) root         (0)  1335628 2024-05-03 17:22:00.000000 SMSCallBomber-1.1/SMSСallBomber/User_Agent.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 15:41:53.000000 SMSCallBomber-1.1/SMSСallBomber/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-01 13:34:45.000000 SMSCallBomber-1.1/SMSСallBomber/config.py
+-rw-r--r--   0 root         (0) root         (0)     2811 2024-05-06 16:00:57.000000 SMSCallBomber-1.1/SMSСallBomber/main.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-05-06 15:56:10.000000 SMSCallBomber-1.1/SMSСallBomber/service.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 16:35:09.252418 SMSCallBomber-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      819 2024-05-06 15:57:53.000000 SMSCallBomber-1.1/setup.py
```

### Comparing `SMSCallBomber-0.1/LICENSE` & `SMSCallBomber-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/PKG-INFO` & `SMSCallBomber-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SMSCallBomber
-Version: 0.1
-Summary: A library for SMS and call bomber / Библиотека для SMS бомбера со звонками
+Version: 1.1
+Summary: {'A library for SMS and call bomber / Библиотека для SMS бомбера со звонками'}
 Home-page: https://github.com/BabayVadimovich/SMSCallBomber
 Author: BabayVadimovich
 Author-email: hmatvej49@gmail.com
 Keywords: bomber,sms,call,smsbomber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,18 @@
 
 This library provides functionality for SMS and call bombing.
 
 ### Usage
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Creating an instance of SMSCallBomber
-args = Namespace(country=Country Code by number without + (Specify ALL for all countries), phone=Phone number for attack (without +)", time="Attack time in seconds, threads=Number of threads, timeout=Request timeout)
+args = Namespace(country="Country Code by number (Specify ALL for all countries)", phone="Phone number for attack (without +)", time="Attack time in seconds", threads="Number of threads", timeout="Request timeout")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Starting the attack
 t.start()
 
 # Stopping the attack
@@ -66,19 +65,18 @@
 
 Эта библиотека предоставляет функционал для SMS бомбера со звонками.
 
 ### Использование
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Создание экземпляра SMSCallBomber
-args = Namespace(country=Код страны числом без + (Укажите ALL для всех стран), phone=Номер телефона для атаки (без +), time=Время атаки в секундах, threads=Количество потоков, timeout=Время ожидания запроса)
+args = Namespace(country="Код страны числом (Укажите ALL для всех стран)", phone="Номер телефона для атаки (без +)", time="Время атаки в секундах", threads="Количество потоков", timeout="Время ожидания запроса")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Запуск атаки
 t.start()
 
 # Остановка атаки
```

### Comparing `SMSCallBomber-0.1/README.md` & `SMSCallBomber-1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 
 This library provides functionality for SMS and call bombing.
 
 ### Usage
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Creating an instance of SMSCallBomber
-args = Namespace(country=Country Code by number without + (Specify ALL for all countries), phone=Phone number for attack (without +)", time="Attack time in seconds, threads=Number of threads, timeout=Request timeout)
+args = Namespace(country="Country Code by number (Specify ALL for all countries)", phone="Phone number for attack (without +)", time="Attack time in seconds", threads="Number of threads", timeout="Request timeout")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Starting the attack
 t.start()
 
 # Stopping the attack
@@ -49,19 +48,18 @@
 
 Эта библиотека предоставляет функционал для SMS бомбера со звонками.
 
 ### Использование
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Создание экземпляра SMSCallBomber
-args = Namespace(country=Код страны числом без + (Укажите ALL для всех стран), phone=Номер телефона для атаки (без +), time=Время атаки в секундах, threads=Количество потоков, timeout=Время ожидания запроса)
+args = Namespace(country="Код страны числом (Укажите ALL для всех стран)", phone="Номер телефона для атаки (без +)", time="Время атаки в секундах", threads="Количество потоков", timeout="Время ожидания запроса")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Запуск атаки
 t.start()
 
 # Остановка атаки
```

### Comparing `SMSCallBomber-0.1/SMSCallBomber.egg-info/PKG-INFO` & `SMSCallBomber-1.1/SMSCallBomber.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SMSCallBomber
-Version: 0.1
-Summary: A library for SMS and call bomber / Библиотека для SMS бомбера со звонками
+Version: 1.1
+Summary: {'A library for SMS and call bomber / Библиотека для SMS бомбера со звонками'}
 Home-page: https://github.com/BabayVadimovich/SMSCallBomber
 Author: BabayVadimovich
 Author-email: hmatvej49@gmail.com
 Keywords: bomber,sms,call,smsbomber
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,18 @@
 
 This library provides functionality for SMS and call bombing.
 
 ### Usage
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Creating an instance of SMSCallBomber
-args = Namespace(country=Country Code by number without + (Specify ALL for all countries), phone=Phone number for attack (without +)", time="Attack time in seconds, threads=Number of threads, timeout=Request timeout)
+args = Namespace(country="Country Code by number (Specify ALL for all countries)", phone="Phone number for attack (without +)", time="Attack time in seconds", threads="Number of threads", timeout="Request timeout")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Starting the attack
 t.start()
 
 # Stopping the attack
@@ -66,19 +65,18 @@
 
 Эта библиотека предоставляет функционал для SMS бомбера со звонками.
 
 ### Использование
 
 ```python
 import SMSCallBomber
-import time
 from argparse import Namespace
 
 # Создание экземпляра SMSCallBomber
-args = Namespace(country=Код страны числом без + (Укажите ALL для всех стран), phone=Номер телефона для атаки (без +), time=Время атаки в секундах, threads=Количество потоков, timeout=Время ожидания запроса)
+args = Namespace(country="Код страны числом (Укажите ALL для всех стран)", phone="Номер телефона для атаки (без +)", time="Время атаки в секундах", threads="Количество потоков", timeout="Время ожидания запроса")
 args.time += time.time()
 t = SMSCallBomber(args)
 
 # Запуск атаки
 t.start()
 
 # Остановка атаки
```

### Comparing `SMSCallBomber-0.1/SMSСallBomber/SMSCallBomber.py` & `SMSCallBomber-1.1/SMSСallBomber/main.py`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/SMSСallBomber/Services.py` & `SMSCallBomber-1.1/SMSСallBomber/Services.py`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/SMSСallBomber/User_Agent.py` & `SMSCallBomber-1.1/SMSСallBomber/User_Agent.py`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/SMSСallBomber/config.py` & `SMSCallBomber-1.1/SMSСallBomber/config.py`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/SMSСallBomber/service.py` & `SMSCallBomber-1.1/SMSСallBomber/service.py`

 * *Files identical despite different names*

### Comparing `SMSCallBomber-0.1/setup.py` & `SMSCallBomber-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SMSCallBomber',
+    version='1.1',
     packages=find_packages(),
-    version='0.1',
     author='BabayVadimovich',
     author_email='hmatvej49@gmail.com',
-    description='A library for SMS and call bomber / Библиотека для SMS бомбера со звонками',
+    description={
+    'A library for SMS and call bomber / Библиотека для SMS бомбера со звонками',
+    },
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BabayVadimovich/SMSCallBomber',
     install_requires=[
         'requests',
         'argparse',
         'urllib3'
```

