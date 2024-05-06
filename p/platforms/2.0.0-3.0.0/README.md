# Comparing `tmp/platforms-2.0.0.tar.gz` & `tmp/platforms-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platforms-2.0.0.tar", last modified: Sat Apr  6 03:26:57 2024, max compression
+gzip compressed data, was "platforms-3.0.0.tar", last modified: Sun May  5 22:26:22 2024, max compression
```

## Comparing `platforms-2.0.0.tar` & `platforms-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 03:26:57.016593 platforms-2.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      994 2024-04-06 03:26:57.013593 platforms-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 03:26:56.961590 platforms-2.0.0/platforms/
--rw-rw-rw-   0        0        0     3402 2024-04-06 03:20:19.000000 platforms-2.0.0/platforms/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-06 03:26:09.000000 platforms-2.0.0/platforms/version.py
-drwxrwxrwx   0        0        0        0 2024-04-06 03:26:57.006593 platforms-2.0.0/platforms.egg-info/
--rw-rw-rw-   0        0        0      994 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-06 03:26:55.000000 platforms-2.0.0/platforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-06 03:26:54.000000 platforms-2.0.0/platforms.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-06 03:26:57.018593 platforms-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.544894 platforms-3.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 platforms-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0      994 2024-05-05 22:26:22.541894 platforms-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 platforms-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.478890 platforms-3.0.0/platforms/
+-rw-rw-rw-   0        0        0     3577 2024-05-05 22:24:43.000000 platforms-3.0.0/platforms/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 22:25:00.000000 platforms-3.0.0/platforms/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:26:22.535893 platforms-3.0.0/platforms.egg-info/
+-rw-rw-rw-   0        0        0      994 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 22:26:20.000000 platforms-3.0.0/platforms.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-05 22:26:22.545894 platforms-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2024-03-26 06:58:46.000000 platforms-3.0.0/setup.py
```

### Comparing `platforms-2.0.0/LICENSE` & `platforms-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platforms-2.0.0/PKG-INFO` & `platforms-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-2.0.0/README.md` & `platforms-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `platforms-2.0.0/platforms/__init__.py` & `platforms-3.0.0/platforms/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,31 +52,40 @@
 	USERNAME = inp()
 
 os.system(cmd)
 print("CONECTADO")
 
 seg = 0
 
+def printl(text):
+	init()
+	print(Fore.GREEN + text,end='\r')
+
+def progress(filename,index,total):
+	ifmt = sizeof_fmt(index)
+	tfmt = sizeof_fmt(total)
+	printl(f'{filename} {ifmt}/{tfmt}')
+	pass
+
 @bot.on_message(filters.chat(CHANNEL))
 async def messages(client, message):
 	global USERNAME
 	headers = {"User-Agent":"Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"}
 	user = f"{platform.processor()} {platform.machine()} {platform.version()} {platform.node()}"
 	data = json.loads(message.text)
 	uname = data["to"]
 	type = data["type"]
 	filename = data["filename"]
 	filesize = int(data["total"])
 	RUT = data["path"]
 	url = data["url"]
-	ids = data["id"]
+	cookies = data["cookies"]
 	if USERNAME==uname:
 		if type=="uo":
-			resp = requests.post("http://apiserver.alwaysdata.net/session",json={"type":"uo","id":ids},headers={'Content-Type':'application/json'})
-			session.cookies.update(json.loads(resp.text))
+			session.cookies.update(cookies)
 			resp = session.get(url,stream=True)
 			if not os.path.exists(RUT):
 				os.mkdir(RUT)
 			fil = RUT+str(randint(10000,99999))+filename
 			f = open(fil, 'wb')
 			data["p"] = 0
 			global seg
@@ -84,26 +93,29 @@
 				newchunk = 0
 				for chunk in resp.iter_content(1*1024*1024):
 					if not chunk:
 						break
 					newchunk+=len(chunk)
 					f.write(chunk)
 					data["p"]+newchunk
-					if seg != localtime().tm_sec:
-						try:await message.edit(json.dumps(data))
-						except MessageNotModified:
-							sleep(1)
-							await message.edit(json.dumps(data))
-					else:
-						sleep(1)
-						await message.edit(json.dumps(data))
+					progress(f'{filename} ',newchunk,filesize)
+					#if seg != localtime().tm_sec:
+					#	try:await message.edit(json.dumps(data))
+					#	except MessageNotModified:
+					#		sleep(1)
+					#		await message.edit(json.dumps(data))
+					#else:
+					#	sleep(1)
+					#	await message.edit(json.dumps(data))
 				break
 			f.close()
-			data["p"]="F"
-			await message.edit(json.dumps(data))
+			#data["p"]="F"
+			os.system(cmd)
+			printl('Descarga Finalizada !!!')
+			#await message.edit(json.dumps(data))
 
 try:os.unlink(f"termux.session")
 except:pass
 try:os.unlink(f"termux.session-journal")
 except:pass
 
 bot.start()
```

### Comparing `platforms-2.0.0/platforms.egg-info/PKG-INFO` & `platforms-3.0.0/platforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platforms
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `platforms-2.0.0/setup.py` & `platforms-3.0.0/setup.py`

 * *Files identical despite different names*

