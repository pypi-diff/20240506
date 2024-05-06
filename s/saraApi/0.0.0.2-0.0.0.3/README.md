# Comparing `tmp/saraapi-0.0.0.2.tar.gz` & `tmp/saraapi-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saraapi-0.0.0.2.tar", last modified: Mon May  6 02:05:52 2024, max compression
+gzip compressed data, was "saraapi-0.0.0.3.tar", last modified: Mon May  6 03:53:16 2024, max compression
```

## Comparing `saraapi-0.0.0.2.tar` & `saraapi-0.0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.787742 saraapi-0.0.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4799 2024-05-06 02:05:52.785210 saraapi-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4066 2024-05-06 01:36:18.000000 saraapi-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.759827 saraapi-0.0.0.2/sara/
--rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.2/sara/__init__.py
--rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.2/sara/ext.py
--rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.2/sara/nsfw.py
--rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.2/sara/req.py
--rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.2/sara/sfw.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:05:52.784207 saraapi-0.0.0.2/saraApi.egg-info/
--rw-rw-rw-   0        0        0     4799 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 02:05:52.000000 saraapi-0.0.0.2/saraApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 02:05:52.787742 saraapi-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-05-06 01:59:13.000000 saraapi-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:53:16.609302 saraapi-0.0.0.3/
+-rw-rw-rw-   0        0        0        0 2024-05-05 23:25:57.000000 saraapi-0.0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4823 2024-05-06 03:53:16.607442 saraapi-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4090 2024-05-06 03:49:10.000000 saraapi-0.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 03:53:16.580486 saraapi-0.0.0.3/sara/
+-rw-rw-rw-   0        0        0       81 2024-04-29 01:35:10.000000 saraapi-0.0.0.3/sara/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-04-29 01:33:03.000000 saraapi-0.0.0.3/sara/ext.py
+-rw-rw-rw-   0        0        0     1937 2024-04-29 01:33:40.000000 saraapi-0.0.0.3/sara/nsfw.py
+-rw-rw-rw-   0        0        0      626 2024-05-06 01:28:07.000000 saraapi-0.0.0.3/sara/req.py
+-rw-rw-rw-   0        0        0      219 2024-04-29 01:34:39.000000 saraapi-0.0.0.3/sara/sfw.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:53:16.604972 saraapi-0.0.0.3/saraApi.egg-info/
+-rw-rw-rw-   0        0        0     4823 2024-05-06 03:53:16.000000 saraapi-0.0.0.3/saraApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-06 03:53:16.000000 saraapi-0.0.0.3/saraApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:53:16.000000 saraapi-0.0.0.3/saraApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 03:53:16.000000 saraapi-0.0.0.3/saraApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 03:53:16.000000 saraapi-0.0.0.3/saraApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:53:16.610079 saraapi-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2024-05-06 03:52:56.000000 saraapi-0.0.0.3/setup.py
```

### Comparing `saraapi-0.0.0.2/PKG-INFO` & `saraapi-0.0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://media.discordapp.net/attachments/682872468322648119/682872516259217418/sara.png" width="546" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="546" alt="Cute As Fubuki" /></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.2 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.3 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `saraapi-0.0.0.2/README.md` & `saraapi-0.0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://media.discordapp.net/attachments/682872468322648119/682872516259217418/sara.png" width="546" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="546" alt="Cute As Fubuki" /></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

### Comparing `saraapi-0.0.0.2/sara/ext.py` & `saraapi-0.0.0.3/sara/ext.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.2/sara/nsfw.py` & `saraapi-0.0.0.3/sara/nsfw.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.2/sara/req.py` & `saraapi-0.0.0.3/sara/req.py`

 * *Files identical despite different names*

### Comparing `saraapi-0.0.0.2/saraApi.egg-info/PKG-INFO` & `saraapi-0.0.0.3/saraApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saraApi
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: sara api public based akanekopy
 Home-page: https://github.com/EverGasterXd/sara_api
 Author: evergaster
 License: MIT license
 Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 <div align="center">
   <br />
   <p>
-    <a href="https://discord.gg/DxHvWwC"><img src="https://media.discordapp.net/attachments/682872468322648119/682872516259217418/sara.png" width="546" alt="Cute As Fubuki" /></a>
+    <a href="https://discord.gg/DxHvWwC"><img src="https://cdn.donmai.us/original/65/bd/__modeus_helltaker_drawn_by_kiyovero__65bd0b99d080bceb39fff3f4de7cc586.png" width="546" alt="Cute As Fubuki" /></a>
   </p>
   <br />
 </div>
 sara is both a SFW and NSFW Wrapper, there's hentais for you perverts to use, however do understand that I'm the only one working on this, and I hand pick images to add, so you may get repeated images! Use it for your Discord Bot, your Self Made Console Waifu, or whatever it is :3
 
 ## NOTE: This Readme.md is from the [Offical Repository](https://gitlab.com/weeb-squad/akaneko/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.2 Summary: sara api public
+Metadata-Version: 2.1 Name: saraApi Version: 0.0.0.3 Summary: sara api public
 based akanekopy Home-page: https://github.com/EverGasterXd/sara_api Author:
 evergaster License: MIT license Keywords: sara anime wallpaper hentai
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Development Status :: 4 - Beta Classifier:
 Natural Language :: English Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
```

### Comparing `saraapi-0.0.0.2/setup.py` & `saraapi-0.0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md','r', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 install_requires = [
 	'requests'
 ]
 
-version = '0.0.0.2'
+version = '0.0.0.3'
 
 setup(
     author='evergaster',
     version=version,
     description='sara api public based akanekopy',
     install_package_data=True,
     install_requires=install_requires,
```

